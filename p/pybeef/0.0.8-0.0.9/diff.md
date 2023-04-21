# Comparing `tmp/pybeef-0.0.8-py3-none-any.whl.zip` & `tmp/pybeef-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6888 bytes, number of entries: 7
+Zip file size: 7020 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      350 b- defN 20-Feb-02 00:00 beef/__init__.py
--rw-r--r--  2.0 unx    12117 b- defN 20-Feb-02 00:00 beef/beef.py
+-rw-r--r--  2.0 unx    12557 b- defN 20-Feb-02 00:00 beef/beef.py
 -rw-r--r--  2.0 unx     1825 b- defN 20-Feb-02 00:00 beef/pool.py
-?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 pybeef-0.0.8.dist-info/RECORD
-7 files, 18474 bytes uncompressed, 6000 bytes compressed:  67.5%
+?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 pybeef-0.0.9.dist-info/RECORD
+7 files, 18914 bytes uncompressed, 6132 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: beef/beef.py
 Comment: 
 
 Filename: beef/pool.py
 Comment: 
 
-Filename: pybeef-0.0.8.dist-info/METADATA
+Filename: pybeef-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pybeef-0.0.8.dist-info/WHEEL
+Filename: pybeef-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pybeef-0.0.8.dist-info/licenses/LICENSE
+Filename: pybeef-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pybeef-0.0.8.dist-info/RECORD
+Filename: pybeef-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beef/beef.py

```diff
@@ -4,14 +4,15 @@
 import uuid
 from enum import Enum
 import inspect
 import json
 from typing import Callable, Awaitable, Any, Optional, NoReturn, Tuple, List, Dict
 import aio_pika
 import aiormq
+import sys
 from .pool import Pool
 
 AsyncFunction = Callable[..., Awaitable[Any]]
 TaskID = str
 
 class TaskNotFoundError(RuntimeError):
     pass
@@ -126,15 +127,14 @@
 
         :return: task id
         '''
         async with self._acquire_channel() as channel:
             await channel.declare_queue(self.name, durable=True)
             task_id = str(uuid.uuid4())
             await channel.declare_queue(task_id, durable=True, arguments={'x-expires': self._reply_expiration_millis})
-            print(f'Declared reply queue {task_id} with idle exporation of {self._reply_expiration_millis}')
             await self._set_status(channel, Status.progress(task_id=task_id, steps=0, progress=-1))
             await channel.default_exchange.publish(
                 _work_request_to_message(task_id, *av, **kw),
                 routing_key=self.name,
             )
             return task_id
 
@@ -223,33 +223,39 @@
 
     async def serve(self) -> NoReturn:
         '''
         Worker that executes the task.
 
         This call block forever, waiting for incoming requests.
         '''
-        async with self._acquire_channel() as channel:
-            await channel.set_qos(prefetch_count=1)
-            queue = await channel.declare_queue(self.name, durable=True)
-            async with queue.iterator(no_ack=False) as queue_iter:
-                async for msg in queue_iter:
-                    try:
-                        task_id, av, kw = _message_to_work_request(msg)
-                        self._task_id.set(task_id)
-                        result = await self.fn(*av, **kw)
-                        status = Status.success(task_id=task_id, result=result)
-                    except Exception as e:
-                        import traceback
-                        traceback.print_exc()
-                        status = Status.failure(task_id=task_id, error=repr(e))
-                    finally:
-                        self._task_id.set(None)
+        while True:
+            with contextlib.suppress(TimeoutError):
+                # need this loop with timeout and suppressed TimeoutError, because
+                # queue iterator does not exit on connection/channel close
+                # we want this loop to break if connection to AMQP server is lost, hence
+                # the looping with timeout hack
+                async with self._acquire_channel() as channel:
+                    await channel.set_qos(prefetch_count=1)
+                    queue = await channel.declare_queue(self.name, durable=True)
+                    async with queue.iterator(no_ack=False, timeout=10) as queue_iter:
+                        async for msg in queue_iter:
+                            try:
+                                task_id, av, kw = _message_to_work_request(msg)
+                                self._task_id.set(task_id)
+                                result = await self.fn(*av, **kw)
+                                status = Status.success(task_id=task_id, result=result)
+                            except Exception as e:
+                                import traceback
+                                traceback.print_exc(file=sys.stderr)
+                                status = Status.failure(task_id=task_id, error=repr(e))
+                            finally:
+                                self._task_id.set(None)
 
-                    await self._set_status(channel, status)
-                    await msg.ack()
+                            await self._set_status(channel, status)
+                            await msg.ack()
 
     @contextlib.asynccontextmanager
     async def connect(self, url: str, max_channels=10) -> Pool:
         '''
         Opens a (single) connection to AMQP server at :url: and creates a pool of channels
         '''
         connection = await aio_pika.connect(url)
```

## Comparing `pybeef-0.0.8.dist-info/METADATA` & `pybeef-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Opinionated distributed RPC using AMQP workers
 Project-URL: Homepage, https://github.com/innodatalabs/beef
 Project-URL: Bug Tracker, https://github.com/pypa/innodatalabs/beef
 Author-email: Mike Kroutikov <mkroutikov@innodata.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pybeef-0.0.8.dist-info/licenses/LICENSE` & `pybeef-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

