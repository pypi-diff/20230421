# Comparing `tmp/prq-0.0.20.tar.gz` & `tmp/prq-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prq-0.0.20.tar", last modified: Wed Nov 16 09:34:57 2022, max compression
+gzip compressed data, was "prq-0.0.21.tar", last modified: Fri Apr 21 14:51:35 2023, max compression
```

## Comparing `prq-0.0.20.tar` & `prq-0.0.21.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 09:34:57.906884 prq-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2022-11-16 09:34:57.906884 prq-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      647 2022-11-16 09:34:27.000000 prq-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 09:34:57.902884 prq-0.0.20/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 09:34:27.000000 prq-0.0.20/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      230 2022-11-16 09:34:27.000000 prq-0.0.20/examples/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2022-11-16 09:34:27.000000 prq-0.0.20/examples/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 09:34:57.906884 prq-0.0.20/prq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2022-11-16 09:34:56.000000 prq-0.0.20/prq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      360 2022-11-16 09:34:57.000000 prq-0.0.20/prq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 09:34:56.000000 prq-0.0.20/prq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-11-16 09:34:56.000000 prq-0.0.20/prq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-11-16 09:34:56.000000 prq-0.0.20/prq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-16 09:34:56.000000 prq-0.0.20/prq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10637 2022-11-16 09:34:27.000000 prq-0.0.20/prq.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 09:34:57.906884 prq-0.0.20/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     3036 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42535 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1856 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/rqgenload.py
--rw-r--r--   0 runner    (1001) docker     (122)     6307 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/rqinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2022-11-16 09:34:27.000000 prq-0.0.20/scripts/rqworker.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 09:34:57.906884 prq-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      728 2022-11-16 09:34:27.000000 prq-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:51:35.708064 prq-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-21 14:51:35.708064 prq-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-21 14:51:21.000000 prq-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:51:35.704064 prq-0.0.21/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:51:21.000000 prq-0.0.21/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-21 14:51:21.000000 prq-0.0.21/examples/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 14:51:21.000000 prq-0.0.21/examples/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:51:35.704064 prq-0.0.21/prq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 14:51:35.000000 prq-0.0.21/prq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-21 14:51:21.000000 prq-0.0.21/prq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:51:35.708064 prq-0.0.21/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43056 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/redis_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/rqgenload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/rqinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-21 14:51:21.000000 prq-0.0.21/scripts/rqworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:51:35.708064 prq-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 14:51:21.000000 prq-0.0.21/setup.py
```

### Comparing `prq-0.0.20/PKG-INFO` & `prq-0.0.21/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prq
-Version: 0.0.20
+Version: 0.0.21
 Summary: UNKNOWN
 Home-page: https://github.com/StepanGavrilov/PRQ
 Author-email: gavrilovstepan78@gmail.com
 License: UNKNOWN
 Description: # Stats
         <img src="https://img.shields.io/pypi/dm/PRQ?style=for-the-badge" alt="pypi">
```

### Comparing `prq-0.0.20/README.md` & `prq-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `prq-0.0.20/examples/tasks.py` & `prq-0.0.21/examples/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import subprocess
 
 from scripts.job import Job
 from runnner import Runner
 
 
 def greeting():
-    subprocess.Popen("python examples/work_with_files/hello_world.py", shell=True).wait()
-    return {
-        "detail": {"response": {"data": [2, 4, 6]}}
-    }
+    subprocess.Popen(
+        "python examples/work_with_files/hello_world.py", shell=True
+    ).wait()
+    return {"detail": {"response": {"data": [2, 4, 6]}}}
 
 
 def entrypoint(job_id: str):
     prev_job = Job.fetch(job_id)
     print(f"get prev result: {job_id} result: {prev_job.result}")
-    subprocess.Popen("python examples/work_with_files/hello_world2.py", shell=True).wait()
+    subprocess.Popen(
+        "python examples/work_with_files/hello_world2.py", shell=True
+    ).wait()
 
 
 def foo():
     Runner(
         entrypoint_path="python examples/work_with_files/hello_world3.py",
-        wait_result=True
+        wait_result=True,
     ).run()
```

### Comparing `prq-0.0.20/prq.egg-info/PKG-INFO` & `prq-0.0.21/prq.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prq
-Version: 0.0.20
+Version: 0.0.21
 Summary: UNKNOWN
 Home-page: https://github.com/StepanGavrilov/PRQ
 Author-email: gavrilovstepan78@gmail.com
 License: UNKNOWN
 Description: # Stats
         <img src="https://img.shields.io/pypi/dm/PRQ?style=for-the-badge" alt="pypi">
```

### Comparing `prq-0.0.20/prq.py` & `prq-0.0.21/prq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import (
-    absolute_import, division,
-    print_function, unicode_literals
-)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import asyncio
 import signal
 import sys
 import traceback
 
 import gevent
@@ -18,79 +15,86 @@
 from rq.compat import as_text, text_type
 from rq.exceptions import DequeueTimeout
 from rq.logutils import setup_loghandlers
 from rq.timeouts import BaseDeathPenalty, JobTimeoutException
 from rq.utils import utcnow
 from rq.version import VERSION
 from rq.worker import StopRequested, green, blue, yellow
+
+from scripts.redis_interactor import flush_job_pids
 from scripts.log import lloger
 from scripts.job import Job
+
+
 monkey.patch_all()
 
 
 class GeventDeathPenalty(BaseDeathPenalty):
     def __init__(self, timeout, exception=JobTimeoutException, **kwargs):
         super().__init__(timeout, exception, **kwargs)
         self.gevent_timeout = None
 
     def setup_death_penalty(self):
-        exception = JobTimeoutException('Gevent Job exceeded maximum timeout value (%d seconds).' % self._timeout)
-        self.gevent_timeout = gevent.Timeout(
-            seconds=None,
-            exception=exception
+        exception = JobTimeoutException(
+            "Gevent Job exceeded maximum timeout value (%d seconds)." % self._timeout
         )
+        self.gevent_timeout = gevent.Timeout(seconds=None, exception=exception)
         self.gevent_timeout.start()
 
     def cancel_death_penalty(self):
         self.gevent_timeout.cancel()
 
 
 class GeventWorker(Worker):
     _name = "GEVENT"
     death_penalty_class = GeventDeathPenalty
     log = lloger
 
     def __init__(self, *args, **kwargs):
+        flushed = flush_job_pids(url=kwargs.pop("redis_url"))
         self.gevent_pool = gevent.pool.Pool(kwargs.get("pool_size", 20))
         super(GeventWorker, self).__init__(*args, **kwargs)
+        self.log.info(f"Flushed jobs: {flushed}")
 
     def register_birth(self):
         self.log.info(
             msg=f"Info on Birth\n"
-                f"=======\n"
-                f"pool size: {self.gevent_pool.size}\n"
-                f"timeout: {self.default_worker_ttl}\n"
-                f"pid: {self.pid}\n"
-                f"state: {self.state}\n"
-                f"queues: {self.queues}\n"
-                f"job class: {self.job_class}\n"
-                f"worker: {self._name}\n"
-                f"=======\n"
+            f"=======\n"
+            f"pool size: {self.gevent_pool.size}\n"
+            f"timeout: {self.default_worker_ttl}\n"
+            f"pid: {self.pid}\n"
+            f"state: {self.state}\n"
+            f"queues: {self.queues}\n"
+            f"job class: {self.job_class}\n"
+            f"worker: {self._name}\n"
+            f"=======\n"
         )
         super(GeventWorker, self).register_birth()
-        self.connection.hset(self.key, 'pool_size', self.gevent_pool.size)
+        self.connection.hset(self.key, "pool_size", self.gevent_pool.size)
 
     def heartbeat(self, timeout=0, pipeline=None):
         connection = pipeline if pipeline is not None else self.connection
         super(GeventWorker, self).heartbeat(timeout)
-        connection.hset(self.key, 'curr_pool_len', len(self.gevent_pool))
+        connection.hset(self.key, "curr_pool_len", len(self.gevent_pool))
 
     def _install_signal_handlers(self):
         def request_force_stop():
-            self.log.warning('Cold shut down.')
+            self.log.warning("Cold shut down.")
             self.gevent_pool.kill()
             raise SystemExit()
 
         def request_stop():
             gevent.signal_handler(signal.SIGINT, request_force_stop)
             gevent.signal_handler(signal.SIGTERM, request_force_stop)
 
-            self.log.warning('Warm shut down requested.')
-            self.log.warning('Stopping after all greenlets are finished. '
-                             'Press Ctrl+C again for a cold shutdown.')
+            self.log.warning("Warm shut down requested.")
+            self.log.warning(
+                "Stopping after all greenlets are finished. "
+                "Press Ctrl+C again for a cold shutdown."
+            )
 
             self._stopped = True
             self.gevent_pool.join()
 
             # import gc
             # from greenlet import greenlet
             # print('=====>', [obj for obj in gc.get_objects() if isinstance(obj, gevent.Greenlet)])
@@ -117,26 +121,24 @@
         The return value indicates whether any jobs were processed.
         """
         self.log.info("Lloger start")
         setup_loghandlers()
         self._install_signal_handlers()
         self.did_perform_work = False
         self.register_birth()
-        self.log.info('RQ worker started, version %s' % VERSION)
-        self.set_state('starting')
+        self.log.info("RQ worker started, version %s" % VERSION)
+        self.set_state("starting")
 
         try:
             while True:
-
                 if self._stop_requested:
-                    self.log.info('Stopping on request.')
+                    self.log.info("Stopping on request.")
                     break
 
-                timeout = None \
-                    if burst else max(1, self.default_worker_ttl - 60)
+                timeout = None if burst else max(1, self.default_worker_ttl - 60)
 
                 try:
                     result = self.dequeue_job_and_maintain_ttl(timeout)
                     self.log.info(f"Get job from queue: {result}")
 
                     # TODO add tree in future
                     # import gtools.tree
@@ -161,28 +163,27 @@
 
         finally:
             if not self.is_horse:
                 self.register_death()
         return self.did_perform_work
 
     def _execute(self):
-
         result = self.func(*self.args, **self.kwargs)
         if asyncio.iscoroutine(result):
             loop = asyncio.new_event_loop()
             coro_result = loop.run_until_complete(result)
             return coro_result
         return result
 
     def execute_job(self, job: Job, queue):
         self.log.info(
             msg=f"Start executing a job - "
-                f"id: {job.id} "
-                f"ttl: {'infinity' if not job.ttl else job.ttl} "
-                f"result ttl: {job.result_ttl}"
+            f"id: {job.id} "
+            f"ttl: {'infinity' if not job.ttl else job.ttl} "
+            f"result ttl: {job.result_ttl}"
         )
         self.gevent_pool.spawn(self.perform_job, job, queue)
 
     def perform_job(self, job, queue):
         """Performs the actual work of a job.  Will/should only be called
         inside the work horse's process.
         """
@@ -198,71 +199,78 @@
 
             job.started_at = utcnow()
             timeout = job.timeout or self.queue_class.DEFAULT_TIMEOUT
             job.result_ttl = 7200
             job.ttl = -1
 
             try:
-                with self.death_penalty_class(timeout, JobTimeoutException, job_id=job.id):
+                with self.death_penalty_class(
+                    timeout, JobTimeoutException, job_id=job.id
+                ):
                     rv = job.perform()
             except Exception:
-                with self.death_penalty_class(timeout, JobTimeoutException, job_id=job.id):
+                with self.death_penalty_class(
+                    timeout, JobTimeoutException, job_id=job.id
+                ):
                     rv = job.perform()
 
             job.ended_at = utcnow()
 
             # Pickle the result in the same try-except block since we need
             # to use the same exc handling when pickling fails
             job._result = rv
 
             if job.success_callback:
                 self.execute_success_callback(job, rv)
 
             self.handle_job_success(
-                job=job,
-                queue=queue,
-                started_job_registry=started_job_registry
+                job=job, queue=queue, started_job_registry=started_job_registry
             )
         except:  # NOQA
             job.ended_at = utcnow()
             exc_info = sys.exc_info()
-            exc_string = ''.join(traceback.format_exception(*exc_info))
+            exc_string = "".join(traceback.format_exception(*exc_info))
 
             if job.failure_callback:
                 try:
                     self.execute_failure_callback(job)
                 except:  # noqa
                     self.log.error(
-                        'Worker %s: error while executing failure callback',
-                        self.key, exc_info=True
+                        "Worker %s: error while executing failure callback",
+                        self.key,
+                        exc_info=True,
                     )
                     exc_info = sys.exc_info()
-                    exc_string = ''.join(traceback.format_exception(*exc_info))
+                    exc_string = "".join(traceback.format_exception(*exc_info))
 
-            self.handle_job_failure(job=job, exc_string=exc_string, queue=queue,
-                                    started_job_registry=started_job_registry)
+            self.handle_job_failure(
+                job=job,
+                exc_string=exc_string,
+                queue=queue,
+                started_job_registry=started_job_registry,
+            )
             self.handle_exception(job, *exc_info)
             return False
 
         finally:
             pop_connection()
 
-        self.log.info('%s: %s (%s)', green(job.origin), blue('Job OK'), job.id)
+        self.log.info("%s: %s (%s)", green(job.origin), blue("Job OK"), job.id)
         if rv is not None:
             log_result = "{0!r}".format(as_text(text_type(rv)))
-            self.log.debug('Result: %s', yellow(log_result))
+            self.log.debug("Result: %s", yellow(log_result))
 
         if self.log_result_lifespan:
             result_ttl = 10000
             if result_ttl == 0:
-                self.log.info('Result discarded immediately')
+                self.log.info("Result discarded immediately")
             elif result_ttl > 0:
-                self.log.info('Result is kept for %s seconds', result_ttl)
+                self.log.info("Result is kept for %s seconds", result_ttl)
             else:
-                self.log.info('Result will never expire, clean up result key manually')
+                self.log.info("Result will never expire, clean up result key manually")
 
         return True
 
     def dequeue_job_and_maintain_ttl(self, timeout):
         """ping queues for jobs"""
 
         if self._stop_requested:
@@ -277,22 +285,22 @@
             self.heartbeat()
             while self.gevent_pool.full():
                 gevent.sleep(0.1)
                 if self._stop_requested:
                     raise StopRequested()
             try:
                 result = self.queue_class.dequeue_any(
-                    self.queues,
-                    timeout,
-                    connection=self.connection
+                    self.queues, timeout, connection=self.connection
                 )
                 if result is not None:
                     job, queue = result
-                    self.log.info('%s: %s (%s)' % (green(queue.name),
-                                                   blue(job.description), job.id))
+                    self.log.info(
+                        "%s: %s (%s)"
+                        % (green(queue.name), blue(job.description), job.id)
+                    )
                 break
             except DequeueTimeout:
                 pass
 
         self.heartbeat()
         return result
 
@@ -301,18 +309,20 @@
     """
     Start worker
     """
 
     import sys
     from scripts.rqworker import main as rq_main
 
-    if '-w' in sys.argv or '--worker-class' in sys.argv:
-        print("You cannot specify worker class when using this script,"
-              "use the official rqworker instead")
+    if "-w" in sys.argv or "--worker-class" in sys.argv:
+        print(
+            "You cannot specify worker class when using this script,"
+            "use the official rqworker instead"
+        )
         sys.exit(1)
 
-    sys.argv.extend(['-w', 'prq.GeventWorker'])
+    sys.argv.extend(["-w", "prq.GeventWorker"])
     rq_main()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     worker()
```

### Comparing `prq-0.0.20/scripts/__init__.py` & `prq-0.0.21/scripts/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # -*- coding: utf-8 -*-
-from __future__ import (
-    absolute_import, division,
-    print_function, unicode_literals
-)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import os
 import importlib
 
 from functools import partial
 from warnings import warn
 
@@ -14,62 +11,104 @@
 
 from rq import use_connection
 from rq.utils import first
 from scripts.job import Job  # type: ignore # noqa F401
 
 
 def add_standard_arguments(parser):
-    parser.add_argument('--config', '-c', default=None,
-                        help='Module containing RQ settings.')
-    parser.add_argument('--url', '-u', default=None,
-                        help='URL describing Redis connection details. '
-                             'Overrides other connection arguments if supplied.')
-    parser.add_argument('--host', '-H', default=None,
-                        help='The Redis hostname (default: localhost)')
-    parser.add_argument('--port', '-p', default=None,
-                        help='The Redis portnumber (default: 6379)')
-    parser.add_argument('--db', '-d', type=int, default=None,
-                        help='The Redis database (default: 0)')
-    parser.add_argument('--password', '-a', default=None,
-                        help='The Redis password (default: None)')
-    parser.add_argument('--socket', '-s', default=None,
-                        help='The Redis Unix socket')
+    parser.add_argument(
+        "--config", "-c", default=None, help="Module containing RQ settings."
+    )
+    parser.add_argument(
+        "--url",
+        "-u",
+        default=None,
+        help="URL describing Redis connection details. "
+        "Overrides other connection arguments if supplied.",
+    )
+    parser.add_argument(
+        "--host", "-H", default=None, help="The Redis hostname (default: localhost)"
+    )
+    parser.add_argument(
+        "--port", "-p", default=None, help="The Redis portnumber (default: 6379)"
+    )
+    parser.add_argument(
+        "--db", "-d", type=int, default=None, help="The Redis database (default: 0)"
+    )
+    parser.add_argument(
+        "--password", "-a", default=None, help="The Redis password (default: None)"
+    )
+    parser.add_argument("--socket", "-s", default=None, help="The Redis Unix socket")
 
 
 def read_config_file(module):
     """Reads all UPPERCASE variables defined in the given module file."""
     settings = importlib.import_module(module)
-    return dict([(k, v)
-                 for k, v in settings.__dict__.items()
-                 if k.upper() == k])
+    return dict([(k, v) for k, v in settings.__dict__.items() if k.upper() == k])
 
 
 def setup_default_arguments(args, settings):
-    """ Sets up args from settings or defaults """
-    args.url = first([args.url, settings.get('REDIS_URL'), os.environ.get('RQ_REDIS_URL')])
+    """Sets up args from settings or defaults"""
+    args.url = first(
+        [args.url, settings.get("REDIS_URL"), os.environ.get("RQ_REDIS_URL")]
+    )
 
     if args.host or args.port or args.socket or args.db or args.password:
-        warn('Host, port, db, password options for Redis will not be '
-             'supported in future versions of RQ. '
-             'Please use `REDIS_URL` or `--url` instead.', DeprecationWarning)
+        warn(
+            "Host, port, db, password options for Redis will not be "
+            "supported in future versions of RQ. "
+            "Please use `REDIS_URL` or `--url` instead.",
+            DeprecationWarning,
+        )
 
     strict_first = partial(first, key=lambda obj: obj is not None)
 
-    args.host = strict_first([args.host, settings.get('REDIS_HOST'), os.environ.get('RQ_REDIS_HOST'), 'localhost'])
-    args.port = int(strict_first([args.port, settings.get('REDIS_PORT'), os.environ.get('RQ_REDIS_PORT'), 6379]))
-    args.socket = strict_first([args.socket, settings.get('REDIS_SOCKET'), os.environ.get('RQ_REDIS_SOCKET'), None])
-    args.db = strict_first([args.db, settings.get('REDIS_DB'), os.environ.get('RQ_REDIS_DB'), 0])
-    args.password = strict_first([args.password, settings.get('REDIS_PASSWORD'), os.environ.get('RQ_REDIS_PASSWORD')])
+    args.host = strict_first(
+        [
+            args.host,
+            settings.get("REDIS_HOST"),
+            os.environ.get("RQ_REDIS_HOST"),
+            "localhost",
+        ]
+    )
+    args.port = int(
+        strict_first(
+            [
+                args.port,
+                settings.get("REDIS_PORT"),
+                os.environ.get("RQ_REDIS_PORT"),
+                6379,
+            ]
+        )
+    )
+    args.socket = strict_first(
+        [
+            args.socket,
+            settings.get("REDIS_SOCKET"),
+            os.environ.get("RQ_REDIS_SOCKET"),
+            None,
+        ]
+    )
+    args.db = strict_first(
+        [args.db, settings.get("REDIS_DB"), os.environ.get("RQ_REDIS_DB"), 0]
+    )
+    args.password = strict_first(
+        [
+            args.password,
+            settings.get("REDIS_PASSWORD"),
+            os.environ.get("RQ_REDIS_PASSWORD"),
+        ]
+    )
 
 
 def setup_redis(args):
     if args.url is not None:
         redis_conn = redis.StrictRedis.from_url(args.url)
     else:
         redis_conn = redis.StrictRedis(
             host=args.host,
             port=args.port,
             db=args.db,
             password=args.password,
-            unix_socket_path=args.socket
+            unix_socket_path=args.socket,
         )
     use_connection(redis_conn)
```

### Comparing `prq-0.0.20/scripts/job.py` & `prq-0.0.21/scripts/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,35 @@
 from scripts.log import lloger
 from rq.local import LocalStack
 from collections.abc import Iterable
 from rq.serializers import resolve_serializer
 from rq.connections import resolve_connection
 from datetime import datetime, timedelta, timezone
 from rq.exceptions import (
-    DeserializationError, InvalidJobOperation,
+    DeserializationError,
+    InvalidJobOperation,
     NoSuchJobError,
 )
 from rq.registry import (
-    CanceledJobRegistry, FinishedJobRegistry,
-    DeferredJobRegistry, StartedJobRegistry,
-    ScheduledJobRegistry, FailedJobRegistry
+    CanceledJobRegistry,
+    FinishedJobRegistry,
+    DeferredJobRegistry,
+    StartedJobRegistry,
+    ScheduledJobRegistry,
+    FailedJobRegistry,
 )
 from rq.utils import (
-    ensure_list, parse_timeout,
-    import_attribute, utcnow,
-    utcformat, str_to_date,
-    get_version, get_call_string
+    ensure_list,
+    parse_timeout,
+    import_attribute,
+    utcnow,
+    utcformat,
+    str_to_date,
+    get_version,
+    get_call_string,
 )
 
 if t.TYPE_CHECKING:
     from rq.queue import Queue
     from redis import Redis
     from redis.client import Pipeline
 
@@ -42,151 +50,181 @@
 # Serialize pickle dumps using the highest pickle protocol (binary, default
 # uses ascii)
 dumps = partial(pickle.dumps, protocol=pickle.HIGHEST_PROTOCOL)
 loads = pickle.loads
 
 
 class JobStatus(str, Enum):
-    QUEUED = 'queued'
-    FINISHED = 'finished'
-    FAILED = 'failed'
-    STARTED = 'started'
-    DEFERRED = 'deferred'
-    SCHEDULED = 'scheduled'
-    STOPPED = 'stopped'
-    CANCELED = 'canceled'
+    QUEUED = "queued"
+    FINISHED = "finished"
+    FAILED = "failed"
+    STARTED = "started"
+    DEFERRED = "deferred"
+    SCHEDULED = "scheduled"
+    STOPPED = "stopped"
+    CANCELED = "canceled"
 
 
 class Dependency:
-    def __init__(self, jobs: t.List[t.Union['Job', str]], allow_failure: bool = False, enqueue_at_front: bool = False):
+    def __init__(
+        self,
+        jobs: t.List[t.Union["Job", str]],
+        allow_failure: bool = False,
+        enqueue_at_front: bool = False,
+    ):
         dependent_jobs = ensure_list(jobs)
         if not all(
-                isinstance(job, Job) or isinstance(job, str)
-                for job in dependent_jobs
-                if job
+            isinstance(job, Job) or isinstance(job, str)
+            for job in dependent_jobs
+            if job
         ):
-            raise ValueError("jobs: must contain objects of type Job and/or strings representing Job ids")
+            raise ValueError(
+                "jobs: must contain objects of type Job and/or strings representing Job ids"
+            )
         elif len(dependent_jobs) < 1:
             raise ValueError("jobs: cannot be empty.")
 
         self.dependencies = dependent_jobs
         self.allow_failure = allow_failure
         self.enqueue_at_front = enqueue_at_front
 
 
 # Sentinel value to mark that some of our lazily evaluated properties have not
 # yet been evaluated.
 UNEVALUATED = object()
 
 
-def cancel_job(job_id: str, connection: t.Optional['Redis'] = None, serializer=None, enqueue_dependents: bool = False):
+def cancel_job(
+    job_id: str,
+    connection: t.Optional["Redis"] = None,
+    serializer=None,
+    enqueue_dependents: bool = False,
+):
     """Cancels the job with the given job ID, preventing execution.  Discards
     any job info (i.e. it can't be requeued later).
     """
-    Job.fetch(job_id, connection=connection, serializer=serializer).cancel(enqueue_dependents=enqueue_dependents)
+    Job.fetch(job_id, connection=connection, serializer=serializer).cancel(
+        enqueue_dependents=enqueue_dependents
+    )
 
 
-def get_current_job(connection: t.Optional['Redis'] = None, job_class: t.Optional['Job'] = None):
+def get_current_job(
+    connection: t.Optional["Redis"] = None, job_class: t.Optional["Job"] = None
+):
     """Returns the Job instance that is currently being executed.  If this
     function is invoked from outside a job context, None is returned.
     """
     if job_class:
-        warnings.warn("job_class argument for get_current_job is deprecated.",
-                      DeprecationWarning)
+        warnings.warn(
+            "job_class argument for get_current_job is deprecated.", DeprecationWarning
+        )
     return _job_stack.top
 
 
-def requeue_job(job_id: str, connection: 'Redis', serializer=None):
+def requeue_job(job_id: str, connection: "Redis", serializer=None):
     job = Job.fetch(job_id, connection=connection, serializer=serializer)
     return job.requeue()
 
 
 class Job:
     """
     A Job is just a convenient datastructure to pass around job (meta) data.
     """
-    redis_job_namespace_prefix = 'rq:job:'
+
+    redis_job_namespace_prefix = "rq:job:"
     log = lloger
 
     # Job construction
     @classmethod
     def create(  # NOSONAR
-            cls,
-            func: t.Callable[..., t.Any],
-            args=None,
-            kwargs=None,
-            connection: t.Optional['Redis'] = None,
-            result_ttl=None,
-            ttl=None,
-            status=None,
-            description=None,
-            depends_on=None,
-            timeout=None,
-            id=None,
-            origin=None,
-            meta=None,
-            failure_ttl=None,
-            serializer=None,
-            *,
-            on_success=None,
-            on_failure=None,
-    ) -> 'Job':
+        cls,
+        func: t.Callable[..., t.Any],
+        args=None,
+        kwargs=None,
+        connection: t.Optional["Redis"] = None,
+        result_ttl=None,
+        ttl=None,
+        status=None,
+        description=None,
+        depends_on=None,
+        timeout=None,
+        id=None,
+        origin=None,
+        meta=None,
+        failure_ttl=None,
+        serializer=None,
+        *,
+        on_success=None,
+        on_failure=None,
+    ) -> "Job":
         """Creates a new Job instance for the given function, arguments, and
         keyword arguments.
         """
 
         if args is None:
             args = ()
         if kwargs is None:
             kwargs = {}
 
         if not isinstance(args, (tuple, list)):
-            raise TypeError('{0!r} is not a valid args list'.format(args))
+            raise TypeError("{0!r} is not a valid args list".format(args))
         if not isinstance(kwargs, dict):
-            raise TypeError('{0!r} is not a valid kwargs dict'.format(kwargs))
+            raise TypeError("{0!r} is not a valid kwargs dict".format(kwargs))
 
         job = cls(connection=connection, serializer=serializer)
 
         if id is not None:
             job.set_id(id)
         if origin is not None:
             job.origin = origin
 
         # Set the core job tuple properties
         job._instance = None
         if inspect.ismethod(func):
             job._instance = func.__self__
             job._func_name = func.__name__
         elif inspect.isfunction(func) or inspect.isbuiltin(func):
-            job._func_name = '{0}.{1}'.format(func.__module__, func.__qualname__)
+            job._func_name = "{0}.{1}".format(func.__module__, func.__qualname__)
         elif isinstance(func, string_types):
             job._func_name = as_text(func)
-        elif not inspect.isclass(func) and hasattr(func, '__call__'):  # a callable class instance
+        elif not inspect.isclass(func) and hasattr(
+            func, "__call__"
+        ):  # a callable class instance
             job._instance = func
-            job._func_name = '__call__'
+            job._func_name = "__call__"
         else:
-            raise TypeError('Expected a callable or a string, but got: {0}'.format(func))
+            raise TypeError(
+                "Expected a callable or a string, but got: {0}".format(func)
+            )
         job._args = args
         job._kwargs = kwargs
 
         if on_success:
             if isinstance(on_success, string_types):
                 job._success_callback_name = as_text(on_success)
-            elif not inspect.isfunction(on_success) and not inspect.isbuiltin(on_success):
-                raise ValueError('on_success callback must be a function')
+            elif not inspect.isfunction(on_success) and not inspect.isbuiltin(
+                on_success
+            ):
+                raise ValueError("on_success callback must be a function")
             else:
-                job._success_callback_name = '{0}.{1}'.format(on_success.__module__, on_success.__qualname__)
+                job._success_callback_name = "{0}.{1}".format(
+                    on_success.__module__, on_success.__qualname__
+                )
 
         if on_failure:
             if isinstance(on_failure, string_types):
                 job._failure_callback_name = as_text(on_failure)
-            elif not inspect.isfunction(on_failure) and not inspect.isbuiltin(on_failure):
-                raise ValueError('on_failure callback must be a function')
+            elif not inspect.isfunction(on_failure) and not inspect.isbuiltin(
+                on_failure
+            ):
+                raise ValueError("on_failure callback must be a function")
             else:
-                job._failure_callback_name = '{0}.{1}'.format(on_failure.__module__, on_failure.__qualname__)
+                job._failure_callback_name = "{0}.{1}".format(
+                    on_failure.__module__, on_failure.__qualname__
+                )
 
         # Extra meta data
         job.description = description or job.get_call_string()
         job.result_ttl = parse_timeout(result_ttl)
         job.failure_ttl = parse_timeout(failure_ttl)
         job.ttl = None
         job.timeout = parse_timeout(timeout)
@@ -198,39 +236,38 @@
             if isinstance(depends_on, Dependency):
                 job.enqueue_at_front = depends_on.enqueue_at_front
                 job.allow_dependency_failures = depends_on.allow_failure
                 depends_on_list = depends_on.dependencies
             else:
                 depends_on_list = ensure_list(depends_on)
             job._dependency_ids = [
-                dep.id if isinstance(dep, Job) else dep
-                for dep in depends_on_list
+                dep.id if isinstance(dep, Job) else dep for dep in depends_on_list
             ]
         return job
 
     def get_position(self):
         if self.origin:
             q = Queue(name=self.origin, connection=self.connection)
             return q.get_job_position(self._id)
         return None
 
     def get_status(self, refresh: bool = True) -> str:
         if refresh:
-            self._status = as_text(self.connection.hget(self.key, 'status'))
+            self._status = as_text(self.connection.hget(self.key, "status"))
 
         return self._status
 
-    def set_status(self, status: str, pipeline: t.Optional['Pipeline'] = None):
+    def set_status(self, status: str, pipeline: t.Optional["Pipeline"] = None):
         self._status = status
-        connection: 'Redis' = pipeline if pipeline is not None else self.connection
-        connection.hset(self.key, 'status', self._status)
+        connection: "Redis" = pipeline if pipeline is not None else self.connection
+        connection.hset(self.key, "status", self._status)
 
     def get_meta(self, refresh: bool = True):
         if refresh:
-            meta = self.connection.hget(self.key, 'meta')
+            meta = self.connection.hget(self.key, "meta")
             self.meta = self.serializer.loads(meta) if meta else {}  # type: ignore
 
         return self.meta
 
     @property
     def is_finished(self) -> bool:
         return self.get_status() == JobStatus.FINISHED
@@ -268,26 +305,26 @@
         """Returns the first item in self._dependency_ids. Present to
         preserve compatibility with third party packages..
         """
         if self._dependency_ids:
             return self._dependency_ids[0]
 
     @property
-    def dependency(self) -> t.Optional['Job']:
+    def dependency(self) -> t.Optional["Job"]:
         """Returns a job's first dependency. To avoid repeated Redis fetches, we cache
         job.dependency as job._dependency.
         """
         if not self._dependency_ids:
             return None
-        if hasattr(self, '_dependency'):
+        if hasattr(self, "_dependency"):
             return self._dependency  # type: ignore
         job = self.fetch(
             self._dependency_ids[0],
             connection=self.connection,
-            serializer=self.serializer  # type: ignore
+            serializer=self.serializer,  # type: ignore
         )
         # type: ignore
         self._dependency = job
         return job
 
     @property
     def dependent_ids(self) -> t.List[str]:
@@ -324,24 +361,29 @@
             else:
                 self._failure_callback = None
 
         return self._failure_callback
 
     def _deserialize_data(self):
         try:
-            self._func_name, self._instance, self._args, self._kwargs = self.serializer.loads(self.data)
+            (
+                self._func_name,
+                self._instance,
+                self._args,
+                self._kwargs,
+            ) = self.serializer.loads(self.data)
         except Exception as e:
             # catch anything because serializers are generic
             raise DeserializationError() from e
 
     @property
     def data(self):
         if self._data is UNEVALUATED:
             if self._func_name is UNEVALUATED:
-                raise ValueError('Cannot build the job data')
+                raise ValueError("Cannot build the job data")
 
             if self._instance is UNEVALUATED:
                 self._instance = None
 
             if self._args is UNEVALUATED:
                 self._args = ()
 
@@ -401,53 +443,55 @@
 
     @kwargs.setter
     def kwargs(self, value):
         self._kwargs = value
         self._data = UNEVALUATED
 
     @classmethod
-    def exists(cls, job_id: str, connection: t.Optional['Redis'] = None) -> int:
+    def exists(cls, job_id: str, connection: t.Optional["Redis"] = None) -> int:
         """Returns whether a job hash exists for the given job ID."""
         conn = resolve_connection(connection)
         return conn.exists(cls.key_for(job_id))
 
     @classmethod
-    def fetch(cls, id: str, connection: t.Optional['Redis'] = None, serializer=None) -> 'Job':
+    def fetch(
+        cls, id: str, connection: t.Optional["Redis"] = None, serializer=None
+    ) -> "Job":
         """Fetches a persisted job from its corresponding Redis key and
         instantiates it.
         """
         job = cls(id, connection=connection, serializer=serializer)
         job.refresh()
         return job
 
     @classmethod
-    def fetch_many(cls, job_ids: t.List[str], connection: 'Redis', serializer=None):
+    def fetch_many(cls, job_ids: t.List[str], connection: "Redis", serializer=None):
         """
         Bulk version of Job.fetch
 
         For any job_ids which a job does not exist, the corresponding item in
         the returned list will be None.
         """
         with connection.pipeline() as pipeline:
             for job_id in job_ids:
                 pipeline.hgetall(cls.key_for(job_id))
             results = pipeline.execute()
 
-        jobs: t.List[t.Optional['Job']] = []
+        jobs: t.List[t.Optional["Job"]] = []
         for i, job_id in enumerate(job_ids):
             if results[i]:
                 job = cls(job_id, connection=connection, serializer=serializer)
                 job.restore(results[i])
                 jobs.append(job)
             else:
                 jobs.append(None)  # type: ignore
 
         return jobs
 
-    def __init__(self, id: str = None, connection: t.Optional['Redis'] = None, serializer=None):  # type: ignore
+    def __init__(self, id: str = None, connection: t.Optional["Redis"] = None, serializer=None):  # type: ignore
         self.connection = resolve_connection(connection)
         self._id = id
         self.created_at = utcnow()
         self._data = UNEVALUATED
         self._func_name = UNEVALUATED
         self._instance = UNEVALUATED
         self._args = UNEVALUATED
@@ -476,22 +520,22 @@
         self.retry_intervals: t.Optional[t.List[int]] = None
         self.redis_server_version = None
         self.last_heartbeat: t.Optional[datetime] = None
         self.allow_dependency_failures: t.Optional[bool] = None
         self.enqueue_at_front: t.Optional[bool] = None
 
     def __repr__(self):  # noqa  # pragma: no cover
-        return '{0}({1!r}, enqueued_at={2!r})'.format(self.__class__.__name__,
-                                                      self._id,
-                                                      self.enqueued_at)
+        return "{0}({1!r}, enqueued_at={2!r})".format(
+            self.__class__.__name__, self._id, self.enqueued_at
+        )
 
     def __str__(self):
-        return '<{0} {1}: {2}>'.format(self.__class__.__name__,
-                                       self.id,
-                                       self.description)
+        return "<{0} {1}: {2}>".format(
+            self.__class__.__name__, self.id, self.description
+        )
 
     def __eq__(self, other):  # noqa
         return isinstance(other, self.__class__) and self.id == other.id
 
     def __hash__(self):  # pragma: no cover
         return hash(self.id)
 
@@ -503,67 +547,82 @@
         if self._id is None:
             self._id = str(uuid4())
         return self._id
 
     def set_id(self, value: str):
         """Sets a job ID for the given job."""
         if not isinstance(value, string_types):
-            raise TypeError('id must be a string, not {0}'.format(type(value)))
+            raise TypeError("id must be a string, not {0}".format(type(value)))
         self._id = value
 
-    def heartbeat(self, timestamp: datetime, ttl: int, pipeline: t.Optional['Pipeline'] = None, xx: bool = False):
+    def heartbeat(
+        self,
+        timestamp: datetime,
+        ttl: int,
+        pipeline: t.Optional["Pipeline"] = None,
+        xx: bool = False,
+    ):
         self.last_heartbeat = timestamp
         connection = pipeline if pipeline is not None else self.connection
-        connection.hset(self.key, 'last_heartbeat', utcformat(self.last_heartbeat))
+        connection.hset(self.key, "last_heartbeat", utcformat(self.last_heartbeat))
         self.started_job_registry.add(self, ttl, pipeline=pipeline, xx=xx)
 
     id = property(get_id, set_id)
 
     @classmethod
     def key_for(cls, job_id: str):
         """The Redis key that is used to store job hash under."""
-        return (cls.redis_job_namespace_prefix + job_id).encode('utf-8')
+        return (cls.redis_job_namespace_prefix + job_id).encode("utf-8")
 
     @classmethod
     def dependents_key_for(cls, job_id: str):
         """The Redis key that is used to store job dependents hash under."""
-        return '{0}{1}:dependents'.format(cls.redis_job_namespace_prefix, job_id)
+        return "{0}{1}:dependents".format(cls.redis_job_namespace_prefix, job_id)
 
     @property
     def key(self):
         """The Redis key that is used to store job hash under."""
         return self.key_for(self.id)
 
     @property
     def dependents_key(self):
         """The Redis key that is used to store job dependents hash under."""
         return self.dependents_key_for(self.id)
 
     @property
     def dependencies_key(self):
-        return '{0}:{1}:dependencies'.format(self.redis_job_namespace_prefix, self.id)
+        return "{0}:{1}:dependencies".format(self.redis_job_namespace_prefix, self.id)
 
-    def fetch_dependencies(self, watch: bool = False, pipeline: t.Optional['Pipeline'] = None):
+    def fetch_dependencies(
+        self, watch: bool = False, pipeline: t.Optional["Pipeline"] = None
+    ):
         """
         Fetch all of a job's dependencies. If a pipeline is supplied, and
         watch is true, then set WATCH on all the keys of all dependencies.
 
         Returned jobs will use self's connection, not the pipeline supplied.
 
         If a job has been deleted from redis, it is not returned.
         """
         connection = pipeline if pipeline is not None else self.connection
 
         if watch and self._dependency_ids:
-            connection.watch(*[self.key_for(dependency_id)
-                               for dependency_id in self._dependency_ids])
-
-        jobs = [job
-                for job in self.fetch_many(self._dependency_ids, connection=self.connection, serializer=self.serializer)
-                if job]
+            connection.watch(
+                *[self.key_for(dependency_id) for dependency_id in self._dependency_ids]
+            )
+
+        jobs = [
+            job
+            for job in self.fetch_many(
+                self._dependency_ids,
+                connection=self.connection,
+                serializer=self.serializer,
+            )
+            if job
+        ]
 
         return jobs
 
     @property
     def result(self):
         """Returns the return value of the job.
 
@@ -577,77 +636,93 @@
 
         Also note that you cannot draw the conclusion that a job has _not_
         been executed when its return value is None, since return values
         written back to Redis will expire after a given amount of time (500
         seconds by default).
         """
         if self._result is None:
-            rv = self.connection.hget(self.key, 'result')
+            rv = self.connection.hget(self.key, "result")
             if rv is not None:
                 # cache the result
                 self._result = self.serializer.loads(rv)
         return self._result
 
     """Backwards-compatibility accessor property `return_value`."""
     return_value = result
 
     def restore(self, raw_data):
         """Overwrite properties with the provided values stored in Redis"""
         obj = decode_redis_hash(raw_data)
         try:
-            raw_data = obj['data']
+            raw_data = obj["data"]
         except KeyError:
-            raise NoSuchJobError('Unexpected job format: {0}'.format(obj))
+            raise NoSuchJobError("Unexpected job format: {0}".format(obj))
 
         try:
             self.data = zlib.decompress(raw_data)
         except zlib.error:
             # Fallback to uncompressed string
             self.data = raw_data
 
-        self.created_at = str_to_date(obj.get('created_at'))
-        self.origin = as_text(obj.get('origin'))
-        self.worker_name = obj.get('worker_name').decode() if obj.get('worker_name') else None
-        self.description = as_text(obj.get('description'))
-        self.enqueued_at = str_to_date(obj.get('enqueued_at'))
-        self.started_at = str_to_date(obj.get('started_at'))
-        self.ended_at = str_to_date(obj.get('ended_at'))
-        self.last_heartbeat = str_to_date(obj.get('last_heartbeat'))
-        result = obj.get('result')
+        self.created_at = str_to_date(obj.get("created_at"))
+        self.origin = as_text(obj.get("origin"))
+        self.worker_name = (
+            obj.get("worker_name").decode() if obj.get("worker_name") else None
+        )
+        self.description = as_text(obj.get("description"))
+        self.enqueued_at = str_to_date(obj.get("enqueued_at"))
+        self.started_at = str_to_date(obj.get("started_at"))
+        self.ended_at = str_to_date(obj.get("ended_at"))
+        self.last_heartbeat = str_to_date(obj.get("last_heartbeat"))
+        result = obj.get("result")
         if result:
             try:
-                self._result = self.serializer.loads(obj.get('result'))
+                self._result = self.serializer.loads(obj.get("result"))
             except Exception:
                 self._result = "Unserializable return value"
-        self.timeout = parse_timeout(obj.get('timeout')) if obj.get('timeout') else None
-        self.result_ttl = int(obj.get('result_ttl')) if obj.get('result_ttl') else None
-        self.failure_ttl = int(obj.get('failure_ttl')) if obj.get('failure_ttl') else None
-        self._status = obj.get('status').decode() if obj.get('status') else None
-
-        if obj.get('success_callback_name'):
-            self._success_callback_name = obj.get('success_callback_name').decode()
-
-        if obj.get('failure_callback_name'):
-            self._failure_callback_name = obj.get('failure_callback_name').decode()
-
-        dep_ids = obj.get('dependency_ids')
-        dep_id = obj.get('dependency_id')  # for backwards compatibility
-        self._dependency_ids = (json.loads(dep_ids.decode()) if dep_ids
-                                else [dep_id.decode()] if dep_id else [])
-        self.allow_dependency_failures = bool(int(obj.get('allow_dependency_failures'))) if obj.get(
-            'allow_dependency_failures') else None
-        self.enqueue_at_front = bool(int(obj['enqueue_at_front'])) if 'enqueue_at_front' in obj else None
-        self.ttl = int(obj.get('ttl')) if obj.get('ttl') else None
-        self.meta = self.serializer.loads(obj.get('meta')) if obj.get('meta') else {}
-
-        self.retries_left = int(obj.get('retries_left')) if obj.get('retries_left') else None
-        if obj.get('retry_intervals'):
-            self.retry_intervals = json.loads(obj.get('retry_intervals').decode())
+        self.timeout = parse_timeout(obj.get("timeout")) if obj.get("timeout") else None
+        self.result_ttl = int(obj.get("result_ttl")) if obj.get("result_ttl") else None
+        self.failure_ttl = (
+            int(obj.get("failure_ttl")) if obj.get("failure_ttl") else None
+        )
+        self._status = obj.get("status").decode() if obj.get("status") else None
+
+        if obj.get("success_callback_name"):
+            self._success_callback_name = obj.get("success_callback_name").decode()
+
+        if obj.get("failure_callback_name"):
+            self._failure_callback_name = obj.get("failure_callback_name").decode()
 
-        raw_exc_info = obj.get('exc_info')
+        dep_ids = obj.get("dependency_ids")
+        dep_id = obj.get("dependency_id")  # for backwards compatibility
+        self._dependency_ids = (
+            json.loads(dep_ids.decode())
+            if dep_ids
+            else [dep_id.decode()]
+            if dep_id
+            else []
+        )
+        self.allow_dependency_failures = (
+            bool(int(obj.get("allow_dependency_failures")))
+            if obj.get("allow_dependency_failures")
+            else None
+        )
+        self.enqueue_at_front = (
+            bool(int(obj["enqueue_at_front"])) if "enqueue_at_front" in obj else None
+        )
+        self.ttl = int(obj.get("ttl")) if obj.get("ttl") else None
+        self.meta = self.serializer.loads(obj.get("meta")) if obj.get("meta") else {}
+
+        self.retries_left = (
+            int(obj.get("retries_left")) if obj.get("retries_left") else None
+        )
+        if obj.get("retry_intervals"):
+            self.retry_intervals = json.loads(obj.get("retry_intervals").decode())
+
+        raw_exc_info = obj.get("exc_info")
         if raw_exc_info:
             try:
                 self.exc_info = as_text(zlib.decompress(raw_exc_info))
             except zlib.error:
                 # Fallback to uncompressed string
                 self.exc_info = as_text(raw_exc_info)
 
@@ -656,79 +731,87 @@
         """Overwrite the current instance's properties with the values in the
         corresponding Redis key.
 
         Will raise a NoSuchJobError if no corresponding Redis key exists.
         """
         data = self.connection.hgetall(self.key)
         if not data:
-            raise NoSuchJobError('No such job: {0}'.format(self.key))
+            raise NoSuchJobError("No such job: {0}".format(self.key))
         self.restore(data)
 
     def to_dict(self, include_meta: bool = True) -> dict:
         """
         Returns a serialization of the current job instance
 
         You can exclude serializing the `meta` dictionary by setting
         `include_meta=False`.
         """
         obj = {
-            'created_at': utcformat(self.created_at or utcnow()),
-            'data': zlib.compress(self.data),
-            'success_callback_name': self._success_callback_name if self._success_callback_name else '',
-            'failure_callback_name': self._failure_callback_name if self._failure_callback_name else '',
-            'started_at': utcformat(self.started_at) if self.started_at else '',
-            'ended_at': utcformat(self.ended_at) if self.ended_at else '',
-            'last_heartbeat': utcformat(self.last_heartbeat) if self.last_heartbeat else '',
-            'worker_name': self.worker_name or ''
+            "created_at": utcformat(self.created_at or utcnow()),
+            "data": zlib.compress(self.data),
+            "success_callback_name": self._success_callback_name
+            if self._success_callback_name
+            else "",
+            "failure_callback_name": self._failure_callback_name
+            if self._failure_callback_name
+            else "",
+            "started_at": utcformat(self.started_at) if self.started_at else "",
+            "ended_at": utcformat(self.ended_at) if self.ended_at else "",
+            "last_heartbeat": utcformat(self.last_heartbeat)
+            if self.last_heartbeat
+            else "",
+            "worker_name": self.worker_name or "",
         }
 
         if self.retries_left is not None:
-            obj['retries_left'] = self.retries_left
+            obj["retries_left"] = self.retries_left
         if self.retry_intervals is not None:
-            obj['retry_intervals'] = json.dumps(self.retry_intervals)
+            obj["retry_intervals"] = json.dumps(self.retry_intervals)
         if self.origin is not None:
-            obj['origin'] = self.origin
+            obj["origin"] = self.origin
         if self.description is not None:
-            obj['description'] = self.description
+            obj["description"] = self.description
         if self.enqueued_at is not None:
-            obj['enqueued_at'] = utcformat(self.enqueued_at)
+            obj["enqueued_at"] = utcformat(self.enqueued_at)
 
         if self._result is not None:
             try:
-                obj['result'] = self.serializer.dumps(self._result)
+                obj["result"] = self.serializer.dumps(self._result)
             except:  # noqa
-                obj['result'] = "Unserializable return value"
+                obj["result"] = "Unserializable return value"
         if self.exc_info is not None:
-            obj['exc_info'] = zlib.compress(str(self.exc_info).encode('utf-8'))
+            obj["exc_info"] = zlib.compress(str(self.exc_info).encode("utf-8"))
         if self.timeout is not None:
-            obj['timeout'] = self.timeout
+            obj["timeout"] = self.timeout
         if self.result_ttl is not None:
-            obj['result_ttl'] = self.result_ttl
+            obj["result_ttl"] = self.result_ttl
         if self.failure_ttl is not None:
-            obj['failure_ttl'] = self.failure_ttl
+            obj["failure_ttl"] = self.failure_ttl
         if self._status is not None:
-            obj['status'] = self._status
+            obj["status"] = self._status
         if self._dependency_ids:
-            obj['dependency_id'] = self._dependency_ids[0]  # for backwards compatibility
-            obj['dependency_ids'] = json.dumps(self._dependency_ids)
+            obj["dependency_id"] = self._dependency_ids[
+                0
+            ]  # for backwards compatibility
+            obj["dependency_ids"] = json.dumps(self._dependency_ids)
         if self.meta and include_meta:
-            obj['meta'] = self.serializer.dumps(self.meta)
+            obj["meta"] = self.serializer.dumps(self.meta)
         if self.ttl:
-            obj['ttl'] = self.ttl
+            obj["ttl"] = self.ttl
 
         if self.allow_dependency_failures is not None:
             # convert boolean to integer to avoid redis.exception.DataError
             obj["allow_dependency_failures"] = int(self.allow_dependency_failures)
 
         if self.enqueue_at_front is not None:
             obj["enqueue_at_front"] = int(self.enqueue_at_front)
 
         return obj
 
-    def save(self, pipeline: t.Optional['Pipeline'] = None, include_meta: bool = True):
+    def save(self, pipeline: t.Optional["Pipeline"] = None, include_meta: bool = True):
         """
         Dumps the current job instance to its corresponding Redis key.
 
         Exclude saving the `meta` dictionary by setting
         `include_meta=False`. This is useful to prevent clobbering
         user metadata without an expensive `refresh()` call first.
 
@@ -749,56 +832,59 @@
             self.redis_server_version = get_version(self.connection)
 
         return self.redis_server_version
 
     def save_meta(self):
         """Stores job meta from the job instance to the corresponding Redis key."""
         meta = self.serializer.dumps(self.meta)
-        self.connection.hset(self.key, 'meta', meta)
+        self.connection.hset(self.key, "meta", meta)
 
-    def cancel(self, pipeline: t.Optional['Pipeline'] = None, enqueue_dependents: bool = False):
+    def cancel(
+        self, pipeline: t.Optional["Pipeline"] = None, enqueue_dependents: bool = False
+    ):
         """Cancels the given job, which will prevent the job from ever being
         ran (or inspected).
 
         This method merely exists as a high-level API call to cancel jobs
         without worrying about the internals required to implement job
         cancellation.
 
         You can enqueue the jobs dependents optionally,
         Same pipelining behavior as Queue.enqueue_dependents on whether or not a pipeline is passed in.
         """
         if self.is_canceled:
-            raise InvalidJobOperation("Cannot cancel already canceled job: {}".format(self.get_id()))
+            raise InvalidJobOperation(
+                "Cannot cancel already canceled job: {}".format(self.get_id())
+            )
         pipe = pipeline or self.connection.pipeline()
 
         while True:
             try:
                 q = Queue(
                     name=self.origin,
                     connection=self.connection,
                     job_class=self.__class__,
-                    serializer=self.serializer
+                    serializer=self.serializer,
                 )
 
                 self.set_status(JobStatus.CANCELED, pipeline=pipe)
                 if enqueue_dependents:
                     # Only WATCH if no pipeline passed, otherwise caller is responsible
                     if pipeline is None:
                         pipe.watch(self.dependents_key)
-                    q.enqueue_dependents(self, pipeline=pipeline, exclude_job_id=self.id)
-                self._remove_from_registries(
-                    pipeline=pipe,
-                    remove_from_queue=True
-                )
+                    q.enqueue_dependents(
+                        self, pipeline=pipeline, exclude_job_id=self.id
+                    )
+                self._remove_from_registries(pipeline=pipe, remove_from_queue=True)
 
                 registry = CanceledJobRegistry(
                     self.origin,
                     self.connection,
                     job_class=self.__class__,
-                    serializer=self.serializer
+                    serializer=self.serializer,
                 )
                 registry.add(self, pipeline=pipe)
                 if pipeline is None:
                     pipe.execute()
                 break
             except WatchError:
                 if pipeline is None:
@@ -809,78 +895,100 @@
                     # handle it
                     raise
 
     def requeue(self, at_front: bool = False):
         """Requeues job."""
         return self.failed_job_registry.requeue(self, at_front=at_front)
 
-    def _remove_from_registries(self, pipeline: t.Optional['Pipeline'] = None, remove_from_queue: bool = True):
+    def _remove_from_registries(
+        self, pipeline: t.Optional["Pipeline"] = None, remove_from_queue: bool = True
+    ):
         if remove_from_queue:
-            q = Queue(name=self.origin, connection=self.connection, serializer=self.serializer)
+            q = Queue(
+                name=self.origin, connection=self.connection, serializer=self.serializer
+            )
             q.remove(self, pipeline=pipeline)
 
         if self.is_finished:
-            registry = FinishedJobRegistry(self.origin,
-                                           connection=self.connection,
-                                           job_class=self.__class__,
-                                           serializer=self.serializer)
+            registry = FinishedJobRegistry(
+                self.origin,
+                connection=self.connection,
+                job_class=self.__class__,
+                serializer=self.serializer,
+            )
             registry.remove(self, pipeline=pipeline)
 
         elif self.is_deferred:
-            registry = DeferredJobRegistry(self.origin,
-                                           connection=self.connection,
-                                           job_class=self.__class__,
-                                           serializer=self.serializer)
+            registry = DeferredJobRegistry(
+                self.origin,
+                connection=self.connection,
+                job_class=self.__class__,
+                serializer=self.serializer,
+            )
             registry.remove(self, pipeline=pipeline)
 
         elif self.is_started:
-            registry = StartedJobRegistry(self.origin,
-                                          connection=self.connection,
-                                          job_class=self.__class__,
-                                          serializer=self.serializer)
+            registry = StartedJobRegistry(
+                self.origin,
+                connection=self.connection,
+                job_class=self.__class__,
+                serializer=self.serializer,
+            )
             registry.remove(self, pipeline=pipeline)
 
         elif self.is_scheduled:
-            registry = ScheduledJobRegistry(self.origin,
-                                            connection=self.connection,
-                                            job_class=self.__class__,
-                                            serializer=self.serializer)
+            registry = ScheduledJobRegistry(
+                self.origin,
+                connection=self.connection,
+                job_class=self.__class__,
+                serializer=self.serializer,
+            )
             registry.remove(self, pipeline=pipeline)
 
         elif self.is_failed or self.is_stopped:
             self.failed_job_registry.remove(self, pipeline=pipeline)
 
         elif self.is_canceled:
-            registry = CanceledJobRegistry(self.origin, connection=self.connection,
-                                           job_class=self.__class__,
-                                           serializer=self.serializer)
+            registry = CanceledJobRegistry(
+                self.origin,
+                connection=self.connection,
+                job_class=self.__class__,
+                serializer=self.serializer,
+            )
             registry.remove(self, pipeline=pipeline)
 
-    def delete(self, pipeline: t.Optional['Pipeline'] = None, remove_from_queue: bool = True,
-               delete_dependents=False):
+    def delete(
+        self,
+        pipeline: t.Optional["Pipeline"] = None,
+        remove_from_queue: bool = True,
+        delete_dependents=False,
+    ):
         """Cancels the job and deletes the job hash from Redis. Jobs depending
         on this job can optionally be deleted as well."""
 
         connection = pipeline if pipeline is not None else self.connection
 
-        self._remove_from_registries(pipeline=pipeline, remove_from_queue=remove_from_queue)
+        self._remove_from_registries(
+            pipeline=pipeline, remove_from_queue=remove_from_queue
+        )
 
         if delete_dependents:
             self.delete_dependents(pipeline=pipeline)
 
         connection.delete(self.key, self.dependents_key, self.dependencies_key)
 
-    def delete_dependents(self, pipeline: t.Optional['Pipeline'] = None):
+    def delete_dependents(self, pipeline: t.Optional["Pipeline"] = None):
         """Delete jobs depending on this job."""
         connection = pipeline if pipeline is not None else self.connection
         for dependent_id in self.dependent_ids:
             try:
-                job = Job.fetch(dependent_id, connection=self.connection, serializer=self.serializer)
-                job.delete(pipeline=pipeline,
-                           remove_from_queue=False)
+                job = Job.fetch(
+                    dependent_id, connection=self.connection, serializer=self.serializer
+                )
+                job.delete(pipeline=pipeline, remove_from_queue=False)
             except NoSuchJobError:
                 # It could be that the dependent job was never saved to redis
                 pass
         connection.delete(self.dependents_key)
 
     # Job execution
     def perform(self):  # noqa
@@ -890,25 +998,25 @@
         _job_stack.push(self)
         try:
             self._result = self._execute()
         finally:
             assert self is _job_stack.pop()
         return self._result
 
-    def prepare_for_execution(self, worker_name: str, pipeline: 'Pipeline'):
+    def prepare_for_execution(self, worker_name: str, pipeline: "Pipeline"):
         """Set job metadata before execution begins"""
         self.worker_name = worker_name
         self.last_heartbeat = utcnow()
         self.started_at = self.last_heartbeat
         self._status = JobStatus.STARTED
         mapping = {
-            'last_heartbeat': utcformat(self.last_heartbeat),
-            'status': self._status,
-            'started_at': utcformat(self.started_at),
-            'worker_name': worker_name
+            "last_heartbeat": utcformat(self.last_heartbeat),
+            "status": self._status,
+            "started_at": utcformat(self.started_at),
+            "worker_name": worker_name,
         }
         pipeline.hmset(self.key, mapping)
 
     def _execute(self):
         result = self.func(*self.args, **self.kwargs)
         if asyncio.iscoroutine(result):
             loop = asyncio.new_event_loop()
@@ -933,16 +1041,20 @@
     # Representation
     def get_call_string(self):  # noqa
         """Returns a string representation of the call, formatted as a regular
         Python function invocation statement.
         """
         return get_call_string(self.func_name, self.args, self.kwargs, max_length=75)
 
-    def cleanup(self, ttl: t.Optional[int] = None, pipeline: t.Optional['Pipeline'] = None,
-                remove_from_queue: bool = True):
+    def cleanup(
+        self,
+        ttl: t.Optional[int] = None,
+        pipeline: t.Optional["Pipeline"] = None,
+        remove_from_queue: bool = True,
+    ):
         """Prepare job for eventual deletion (if needed). This method is usually
         called after successful execution. How long we persist the job and its
         result depends on the value of ttl:
         - If ttl is 0, cleanup the job immediately.
         - If it's a positive number, set the job to expire in X seconds.
         - If ttl is negative, don't set an expiry to it (persist
           forever)
@@ -955,150 +1067,167 @@
             connection = pipeline if pipeline is not None else self.connection
             connection.expire(self.key, ttl)
             connection.expire(self.dependents_key, ttl)
             connection.expire(self.dependencies_key, ttl)
 
     @property
     def started_job_registry(self):
-        return StartedJobRegistry(self.origin, connection=self.connection,
-                                  job_class=self.__class__,
-                                  serializer=self.serializer)
+        return StartedJobRegistry(
+            self.origin,
+            connection=self.connection,
+            job_class=self.__class__,
+            serializer=self.serializer,
+        )
 
     @property
     def failed_job_registry(self):
-        return FailedJobRegistry(self.origin, connection=self.connection,
-                                 job_class=self.__class__,
-                                 serializer=self.serializer)
+        return FailedJobRegistry(
+            self.origin,
+            connection=self.connection,
+            job_class=self.__class__,
+            serializer=self.serializer,
+        )
 
     def get_retry_interval(self):
         """Returns the desired retry interval.
         If number of retries is bigger than length of intervals, the first
         value in the list will be used multiple times.
         """
         if self.retry_intervals is None:
             return 0
         number_of_intervals = len(self.retry_intervals)
         index = max(number_of_intervals - self.retries_left, 0)
         return self.retry_intervals[index]
 
-    def retry(self, queue: 'Queue', pipeline: 'Pipeline'):
+    def retry(self, queue: "Queue", pipeline: "Pipeline"):
         """Requeue or schedule this job for execution"""
         retry_interval = self.get_retry_interval()
         self.retries_left = self.retries_left - 1  # type: ignore
         if retry_interval:
-            scheduled_datetime = datetime.now(timezone.utc) + timedelta(seconds=retry_interval)
+            scheduled_datetime = datetime.now(timezone.utc) + timedelta(
+                seconds=retry_interval
+            )
             self.set_status(JobStatus.SCHEDULED)
             queue.schedule_job(self, scheduled_datetime, pipeline=pipeline)
         else:
             queue.enqueue_job(self, pipeline=pipeline)
 
-    def register_dependency(self, pipeline: t.Optional['Pipeline'] = None):
+    def register_dependency(self, pipeline: t.Optional["Pipeline"] = None):
         """Jobs may have dependencies. Jobs are enqueued only if the jobs they
         depend on are successfully performed. We record this relation as
         a reverse dependency (a Redis set), with a key that looks something
         like:
 
             rq:job:job_id:dependents = {'job_id_1', 'job_id_2'}
 
         This method adds the job in its dependencies' dependents sets,
         and adds the job to DeferredJobRegistry.
         """
 
-        registry = DeferredJobRegistry(self.origin,
-                                       connection=self.connection,
-                                       job_class=self.__class__,
-                                       serializer=self.serializer)
+        registry = DeferredJobRegistry(
+            self.origin,
+            connection=self.connection,
+            job_class=self.__class__,
+            serializer=self.serializer,
+        )
         registry.add(self, pipeline=pipeline)
 
         connection = pipeline if pipeline is not None else self.connection
 
         for dependency_id in self._dependency_ids:
             dependents_key = self.dependents_key_for(dependency_id)
             connection.sadd(dependents_key, self.id)
             connection.sadd(self.dependencies_key, dependency_id)
 
     @property
     def dependency_ids(self):
         dependencies = self.connection.smembers(self.dependencies_key)
-        return [Job.key_for(_id.decode())  # type: ignore
-                for _id in dependencies]
+        return [Job.key_for(_id.decode()) for _id in dependencies]  # type: ignore
 
-    def dependencies_are_met(self, parent_job: t.Optional['Job'] = None,
-                             pipeline: t.Optional['Pipeline'] = None, exclude_job_id: str = None):  # type: ignore
+    def dependencies_are_met(
+        self,
+        parent_job: t.Optional["Job"] = None,
+        pipeline: t.Optional["Pipeline"] = None,
+        exclude_job_id: str = None,
+    ):  # type: ignore
         """Returns a boolean indicating if all of this job's dependencies are _FINISHED_
 
         If a pipeline is passed, all dependencies are WATCHed.
 
         `parent_job` allows us to directly pass parent_job for the status check.
         This is useful when enqueueing the dependents of a _successful_ job -- that status of
         `FINISHED` may not be yet set in redis, but said job is indeed _done_ and this
         method is _called_ in the _stack_ of its dependents are being enqueued.
         """
         connection = pipeline if pipeline is not None else self.connection
 
         if pipeline is not None:
-            connection.watch(*[self.key_for(dependency_id)
-                               for dependency_id in self._dependency_ids])
+            connection.watch(
+                *[self.key_for(dependency_id) for dependency_id in self._dependency_ids]
+            )
 
-        dependencies_ids = {_id.decode()
-                            for _id in connection.smembers(self.dependencies_key)}
+        dependencies_ids = {
+            _id.decode() for _id in connection.smembers(self.dependencies_key)
+        }
 
         if exclude_job_id:
             dependencies_ids.discard(exclude_job_id)
             if parent_job.id == exclude_job_id:  # type: ignore
                 parent_job = None
 
         if parent_job:
             # If parent job is canceled, treat dependency as failed
             # If parent job is not finished, we should only continue
             # if this job allows parent job to fail
             dependencies_ids.discard(parent_job.id)
             if parent_job._status == JobStatus.CANCELED:
                 return False
-            elif parent_job._status == JobStatus.FAILED and not self.allow_dependency_failures:
+            elif (
+                parent_job._status == JobStatus.FAILED
+                and not self.allow_dependency_failures
+            ):
                 return False
 
             # If the only dependency is parent job, dependency has been met
             if not dependencies_ids:
                 return True
 
         with connection.pipeline() as pipeline:
             for key in dependencies_ids:
-                pipeline.hget(self.key_for(key), 'status')
+                pipeline.hget(self.key_for(key), "status")
 
             dependencies_statuses = pipeline.execute()
 
         if self.allow_dependency_failures:
             allowed_statuses = [JobStatus.FINISHED, JobStatus.FAILED]
         else:
             allowed_statuses = [JobStatus.FINISHED]
 
         return all(
             status.decode() in allowed_statuses
-            for status
-            in dependencies_statuses
+            for status in dependencies_statuses
             if status
         )
 
 
 _job_stack = LocalStack()
 
 
 class Retry:
     def __init__(self, max, interval: int = 0):
         """`interval` can be a positive number or a list of ints"""
         super().__init__()
         if max < 1:
-            raise ValueError('max: please enter a value greater than 0')
+            raise ValueError("max: please enter a value greater than 0")
 
         if isinstance(interval, int):
             if interval < 0:
-                raise ValueError('interval: negative numbers are not allowed')
+                raise ValueError("interval: negative numbers are not allowed")
             intervals = [interval]
         elif isinstance(interval, Iterable):
             for i in interval:
                 if i < 0:
-                    raise ValueError('interval: negative numbers are not allowed')
+                    raise ValueError("interval: negative numbers are not allowed")
             intervals = interval
 
         self.max = max
         self.intervals = intervals
```

### Comparing `prq-0.0.20/scripts/log.py` & `prq-0.0.21/scripts/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from typing import Union, Optional
 
 from pydantic import BaseModel
 
 
 def convert_bytes(b, to, bsize=1024):
-    a = {'k': 1, 'm': 2, 'g': 3, 't': 4, 'p': 5, 'e': 6}
+    a = {"k": 1, "m": 2, "g": 3, "t": 4, "p": 5, "e": 6}
     return b / (bsize ** a[to])
 
 
 LOGGER_FILE = Path(os.getenv("PRQ_LOGS", f"{os.curdir}/logs"))
 if LOGGER_FILE.exists() and convert_bytes(LOGGER_FILE.stat().st_size, to="m") > 512:
     os.system(f"rm {LOGGER_FILE.absolute()}")
 
@@ -30,33 +30,28 @@
 
 
 @lru_cache
 def get_logger_config():
     from rich.logging import RichHandler
 
     output_file_handler = logging.FileHandler(LOGGER_FILE)
-    handler_format = logging.Formatter(
-        LOGGER_FORMAT,
-        datefmt=DATE_FORMAT
-    )
+    handler_format = logging.Formatter(LOGGER_FORMAT, datefmt=DATE_FORMAT)
     output_file_handler.setFormatter(handler_format)
 
     return LoggerConfig(
         handlers=[
             RichHandler(
-                rich_tracebacks=True,
-                tracebacks_show_locals=True,
-                show_time=False
+                rich_tracebacks=True, tracebacks_show_locals=True, show_time=False
             ),
-            output_file_handler
+            output_file_handler,
         ],
         format=LOGGER_FORMAT,
         date_format=DATE_FORMAT,
         logger_file=LOGGER_FILE,
-        level=logging.CRITICAL
+        level=logging.CRITICAL,
     )
 
 
 def setup_rich_logger():
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
```

### Comparing `prq-0.0.20/scripts/rqgenload.py` & `prq-0.0.21/scripts/rqgenload.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import optparse
 
 from rq import dummy, Queue, use_connection
 
 
 def parse_args():
     parser = optparse.OptionParser()
-    parser.add_option('-n', '--count', type='int', dest='count', default=1)
+    parser.add_option("-n", "--count", type="int", dest="count", default=1)
     opts, args = parser.parse_args()
     return opts, args, parser
 
 
 def main():
     import sys
-    sys.path.insert(0, '.')
+
+    sys.path.insert(0, ".")
 
     opts, args, parser = parse_args()
 
     use_connection()
 
-    queues = ('default', 'high', 'low')
+    queues = ("default", "high", "low")
 
     sample_calls = [
         (dummy.do_nothing, [], {}),
         (dummy.sleep, [1], {}),
         (dummy.fib, [8], {}),  # normal result
         (dummy.fib, [24], {}),  # takes pretty long
         (dummy.div_by_zero, [], {}),  # 5 / 0 => div by zero exc
-        (dummy.random_failure, [], {}),  # simulate random failure (handy for requeue testing)
+        (
+            dummy.random_failure,
+            [],
+            {},
+        ),  # simulate random failure (handy for requeue testing)
     ]
 
     for _ in range(opts.count):
         import random
+
         f, args, kwargs = random.choice(sample_calls)
 
         q = Queue(random.choice(queues))
         q.enqueue(f, *args, **kwargs)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `prq-0.0.20/scripts/rqinfo.py` & `prq-0.0.21/scripts/rqinfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from __future__ import (
-    absolute_import, division,
-    print_function, unicode_literals
-)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import argparse
 import os
 import sys
 import time
 
 from redis.exceptions import ConnectionError
-from rq import get_failed_queue, Queue, Worker # type: ignore
+from rq import get_failed_queue, Queue, Worker  # type: ignore
 from prq.scripts import (  # type: ignore
-    add_standard_arguments, read_config_file,
-    setup_default_arguments, setup_redis
+    add_standard_arguments,
+    read_config_file,
+    setup_default_arguments,
+    setup_redis,
 )
 from rq.utils import gettermsize, make_colorizer  # type: ignore
 
-red = make_colorizer('darkred')
-green = make_colorizer('darkgreen')
-yellow = make_colorizer('darkyellow')
+red = make_colorizer("darkred")
+green = make_colorizer("darkgreen")
+yellow = make_colorizer("darkyellow")
 
 
 def pad(s, pad_to_length):
     """Pads the given string to the given length."""
-    return ('%-' + '%ds' % pad_to_length) % (s,)
+    return ("%-" + "%ds" % pad_to_length) % (s,)
 
 
 def get_scale(x):
     """Finds the lowest scale where x <= scale."""
     scales = [20, 50, 100, 200, 400, 600, 800, 1000]
     for scale in scales:
         if x <= scale:
             return scale
     return x
 
 
 def state_symbol(state):
     symbols = {
-        'busy': red('busy'),
-        'idle': green('idle'),
+        "busy": red("busy"),
+        "idle": green("idle"),
     }
     try:
         return symbols[state]
     except KeyError:
         return state
 
 
@@ -66,24 +65,24 @@
         max_count = max(max_count, count)
     scale = get_scale(max_count)
     ratio = chartwidth * 1.0 / scale
 
     for q in qs:
         count = counts[q]
         if not args.raw:
-            chart = green('|' + '█' * int(ratio * count))
-            line = '%-12s %s %d' % (q.name, chart, count)
+            chart = green("|" + "█" * int(ratio * count))
+            line = "%-12s %s %d" % (q.name, chart, count)
         else:
-            line = 'queue %s %d' % (q.name, count)
+            line = "queue %s %d" % (q.name, count)
 
         num_jobs += count
 
     # Print summary when not in raw mode
     if not args.raw:
-        print('%d queues, %d jobs total' % (len(qs), num_jobs))
+        print("%d queues, %d jobs total" % (len(qs), num_jobs))
 
 
 def show_workers(args):
     if len(args.queues):
         qs = list(map(Queue, args.queues))
 
         def any_matching_queue(worker):
@@ -103,99 +102,146 @@
         ws = Worker.all()
         filter_queues = lambda x: x  # noqa E731
 
     if not args.by_queue:
         for w in ws:
             worker_queues = filter_queues(w.queue_names())
             if not args.raw:
-                print('%s %s: %s' % (w.name, state_symbol(w.get_state()), ', '.join(worker_queues)))
+                print(
+                    "%s %s: %s"
+                    % (w.name, state_symbol(w.get_state()), ", ".join(worker_queues))
+                )
             else:
-                print('worker %s %s %s' % (w.name, w.get_state(), ','.join(worker_queues)))
+                print(
+                    "worker %s %s %s" % (w.name, w.get_state(), ",".join(worker_queues))
+                )
     else:
         # Create reverse lookup table
         queues = dict([(q, []) for q in qs])
         for w in ws:
             for q in w.queues:
                 if q not in queues:
                     continue
                 queues[q].append(w)
 
         max_qname = max(map(lambda q: len(q.name), queues.keys())) if queues else 0
         for q in queues:
             if queues[q]:
                 queues_str = ", ".join(
-                    sorted(map(lambda w: '%s (%s)' % (w.name, state_symbol(w.get_state())), queues[q])))  # noqa
+                    sorted(
+                        map(
+                            lambda w: "%s (%s)" % (w.name, state_symbol(w.get_state())),
+                            queues[q],
+                        )
+                    )
+                )  # noqa
             else:
-                queues_str = '–'
-            print('%s %s' % (pad(q.name + ':', max_qname + 1), queues_str))
+                queues_str = "–"
+            print("%s %s" % (pad(q.name + ":", max_qname + 1), queues_str))
 
     if not args.raw:
-        print('%d workers, %d queues' % (len(ws), len(qs)))
+        print("%d workers, %d queues" % (len(ws), len(qs)))
 
 
 def show_both(args):
     show_queues(args)
     if not args.raw:
-        print('')
+        print("")
     show_workers(args)
     if not args.raw:
-        print('')
+        print("")
         import datetime
-        print('Updated: %s' % datetime.datetime.now())
+
+        print("Updated: %s" % datetime.datetime.now())
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description='RQ command-line monitor.')
+    parser = argparse.ArgumentParser(description="RQ command-line monitor.")
     add_standard_arguments(parser)
-    parser.add_argument('--path', '-P', default='.', help='Specify the import path.')
-    parser.add_argument('--interval', '-i', metavar='N', type=float, default=2.5,
-                        help='Updates stats every N seconds (default: don\'t poll)')  # noqa
-    parser.add_argument('--raw', '-r', action='store_true', default=False,
-                        help='Print only the raw numbers, no bar charts')  # noqa
-    parser.add_argument('--only-queues', '-Q', dest='only_queues', default=False, action='store_true',
-                        help='Show only queue info')  # noqa
-    parser.add_argument('--only-workers', '-W', dest='only_workers', default=False, action='store_true',
-                        help='Show only worker info')  # noqa
-    parser.add_argument('--by-queue', '-R', dest='by_queue', default=False, action='store_true',
-                        help='Shows workers by queue')  # noqa
-    parser.add_argument('--empty-failed-queue', '-X', dest='empty_failed_queue', default=False, action='store_true',
-                        help='Empties the failed queue, then quits')  # noqa
-    parser.add_argument('queues', nargs='*', help='The queues to poll')
+    parser.add_argument("--path", "-P", default=".", help="Specify the import path.")
+    parser.add_argument(
+        "--interval",
+        "-i",
+        metavar="N",
+        type=float,
+        default=2.5,
+        help="Updates stats every N seconds (default: don't poll)",
+    )  # noqa
+    parser.add_argument(
+        "--raw",
+        "-r",
+        action="store_true",
+        default=False,
+        help="Print only the raw numbers, no bar charts",
+    )  # noqa
+    parser.add_argument(
+        "--only-queues",
+        "-Q",
+        dest="only_queues",
+        default=False,
+        action="store_true",
+        help="Show only queue info",
+    )  # noqa
+    parser.add_argument(
+        "--only-workers",
+        "-W",
+        dest="only_workers",
+        default=False,
+        action="store_true",
+        help="Show only worker info",
+    )  # noqa
+    parser.add_argument(
+        "--by-queue",
+        "-R",
+        dest="by_queue",
+        default=False,
+        action="store_true",
+        help="Shows workers by queue",
+    )  # noqa
+    parser.add_argument(
+        "--empty-failed-queue",
+        "-X",
+        dest="empty_failed_queue",
+        default=False,
+        action="store_true",
+        help="Empties the failed queue, then quits",
+    )  # noqa
+    parser.add_argument("queues", nargs="*", help="The queues to poll")
     return parser.parse_args()
 
 
 def interval(val, func, args):
     while True:
         if val and sys.stdout.isatty():
-            os.system('clear')
+            os.system("clear")
         func(args)
         if val and sys.stdout.isatty():
             time.sleep(val)
         else:
             break
 
 
 def main():
     args = parse_args()
 
     if args.path:
-        sys.path = args.path.split(':') + sys.path
+        sys.path = args.path.split(":") + sys.path
 
     settings = {}
     if args.config:
         settings = read_config_file(args.config)
 
     setup_default_arguments(args, settings)
 
     setup_redis(args)
 
     try:
         if args.empty_failed_queue:
             num_jobs = get_failed_queue().empty()
-            print('{} jobs removed from failed queue'.format(num_jobs))
+            print("{} jobs removed from failed queue".format(num_jobs))
         else:
             if args.only_queues:
                 func = show_queues
             elif args.only_workers:
                 func = show_workers
             else:
                 func = show_both
```

### Comparing `prq-0.0.20/setup.py` & `prq-0.0.21/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 setup(
     url="https://github.com/StepanGavrilov/PRQ",
     packages=find_packages(),
     author_email="gavrilovstepan78@gmail.com",
     name="prq",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    version="0.0.20",
+    long_description_content_type="text/markdown",
+    version="0.0.21",
     py_modules=["prq"],
     entry_points={
         "console_scripts": [
             "prq=prq:worker",
         ]
     },
     keywords=["python", "queue", "redis", "parallel", "workers", "tasks", "jobs"],
```

