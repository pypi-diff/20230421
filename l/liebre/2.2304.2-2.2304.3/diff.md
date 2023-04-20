# Comparing `tmp/liebre-2.2304.2-py3-none-any.whl.zip` & `tmp/liebre-2.2304.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19977 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      222 b- defN 23-Apr-20 10:18 liebre/__init__.py
--rw-rw-r--  2.0 unx     8079 b- defN 23-Apr-19 20:41 liebre/consumer.py
+Zip file size: 20013 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      222 b- defN 23-Apr-20 23:06 liebre/__init__.py
+-rw-rw-r--  2.0 unx     8039 b- defN 23-Apr-20 11:36 liebre/consumer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Dec-07 11:43 liebre/liebre.py
 -rw-rw-r--  2.0 unx       69 b- defN 22-Dec-07 11:44 liebre/logger.py
 -rw-rw-r--  2.0 unx      490 b- defN 23-Apr-19 20:41 liebre/message.py
 -rw-rw-r--  2.0 unx     2535 b- defN 23-Jan-17 11:16 liebre/producer.py
--rw-rw-r--  2.0 unx     7439 b- defN 23-Apr-20 10:16 liebre/rabbit_store.py
--rw-rw-r--  2.0 unx     1254 b- defN 23-Apr-19 21:05 liebre/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      985 b- defN 23-Apr-20 10:18 liebre-2.2304.2.dist-info/RECORD
-13 files, 57097 bytes uncompressed, 18349 bytes compressed:  67.9%
+-rw-rw-r--  2.0 unx     7800 b- defN 23-Apr-20 23:01 liebre/rabbit_store.py
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Apr-20 21:23 liebre/utils.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      730 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/RECORD
+13 files, 57182 bytes uncompressed, 18385 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: liebre/rabbit_store.py
 Comment: 
 
 Filename: liebre/utils.py
 Comment: 
 
-Filename: liebre-2.2304.2.dist-info/LICENSE
+Filename: liebre-2.2304.3.dist-info/LICENSE
 Comment: 
 
-Filename: liebre-2.2304.2.dist-info/METADATA
+Filename: liebre-2.2304.3.dist-info/METADATA
 Comment: 
 
-Filename: liebre-2.2304.2.dist-info/WHEEL
+Filename: liebre-2.2304.3.dist-info/WHEEL
 Comment: 
 
-Filename: liebre-2.2304.2.dist-info/top_level.txt
+Filename: liebre-2.2304.3.dist-info/top_level.txt
 Comment: 
 
-Filename: liebre-2.2304.2.dist-info/RECORD
+Filename: liebre-2.2304.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liebre/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 
 from .consumer import Consumer  # noqa F401
 from .producer import Producer  # noqa F401
 
 import logging
 
-__version__ = '2.2304.2'
+__version__ = '2.2304.3'
 
 logging.getLogger('pika').propagate = False
```

## liebre/consumer.py

```diff
@@ -41,34 +41,32 @@
                 'queue': queue,
                 'callback': callback,
                 'queue_options': queue_options,
                 'backup': backup,
             },
         )
         self._threads.append(thread)
+        thread.start()
 
     def commit(self, message: Message):
         message_queue = (message.properties.message_id, message.queue)
         if message_queue not in self._channel_by_message_queue:
             raise ValueError('Committing unknown message.')
 
         channel = self._channel_by_message_queue[message_queue]
         channel.basic_ack(delivery_tag=message.method.delivery_tag)
         del self._channel_by_message_queue[message_queue]
 
-    def status(self):
+    def is_alive(self):
         for thread in self._threads:
             if not thread.is_alive():
                 return False
         return True
 
-    def start(self):
-        for thread in self.threads:
-            thread.start()
-
+    def join(self):
         for thread in self.threads:
             thread.join()
 
     def _send_to_bottom(
         self,
         message,
         channel,
```

## liebre/rabbit_store.py

```diff
@@ -3,14 +3,15 @@
 import pika
 from .utils import (
     get_partition_queue_name,
     get_backup_queue_name,
     get_dead_letter_queue_name,
 )
 from threading import Lock
+import ssl
 
 
 class RabbitStore:
 
     EXCHANGE_OPTIONS = {
         'type': 'direct',
         'durable': True,
@@ -30,14 +31,15 @@
         self,
         user=None,
         password=None,
         host=None,
         port=None,
         vhost=None,
         exchange=None,
+        tls=None,
         max_retry_seconds=None,
         max_retries=None,
         sleep_seconds_on_retry=None,
         auto_ack=True,
         prefetch=None,
         partitions=None,
         exchange_options=None,
@@ -48,14 +50,15 @@
 
         self._user = user or 'guest'
         self._password = password or 'guest'
         self._host = host or 'localhost'
         self._port = port or 5672
         self._vhost = vhost or '/'
         self._exchange = exchange
+        self._tls = True if tls else False
         self._max_retry_seconds = (
             max_retry_seconds
             if max_retry_seconds and max_retry_seconds > 0 else 0
         )
 
         self._sleep_seconds_on_retry = (
             sleep_seconds_on_retry
@@ -116,74 +119,76 @@
                         logger.exception(
                             'Reconnecting... '
                             f'({retries}/{instance._max_retries})',
                         )
 
         return _
 
-    def connect(self, force=False):
-        if not force and self._initialized:
-            return
-
-        self._channel = self._get_channel()
-        self._declare_exchange()
-
-        self._initialized = True
-
     def thread_safe(function):
 
         def _(*args, **kwargs):
             instance = args[0]
             with instance._lock:
                 return function(*args, **kwargs)
 
         return _
 
+    def connect(self, force=False):
+        if not force and self._initialized:
+            return
+
+        self._channel = self._get_channel()
+        self._declare_exchange()
+
+        self._initialized = True
+
+    @reconnect
     @thread_safe
-    def _declare_exchange(self):
-        self._channel.exchange_declare(
-            exchange=self._exchange,
-            exchange_type=self._exchange_options['type'],
-            durable=self._exchange_options['durable'],
-            auto_delete=self._exchange_options['auto_delete'],
-        )
+    def get_info(self):
+        status = {}
+        for queue_name in self._declared_queues:
+            queue_data = self._channel.queue_declare(queue_name, passive=True)
+            status[queue_name] = {
+                'messages': queue_data.method.message_count,
+                'consumers': queue_data.method.consumer_count,
+            }
+        return status
 
-    def _get_channel(self, prefetch=None):
-        if prefetch is None:
-            prefetch = self._prefetch
+    @reconnect
+    @thread_safe
+    def declare_queue(
+        self,
+        queue,
+        options=None,
+    ):
+        if options is None:
+            options = {}
+        options = self._queue_options | options
 
-        # Pika's connection is not thread-safe, can't be reused.
-        # Thus, neither the channels belonging to it.
-        connection = pika.BlockingConnection(
-            pika.ConnectionParameters(
-                self._host,
-                self._port,
-                self._vhost,
-                pika.PlainCredentials(
-                    self._user,
-                    self._password,
-                ),
+        if options['dead_letters']:
+            self._declare_queue(
+                queue,
+                options,
+                dead_letter=True,
             )
-        )
 
-        channel = connection.channel()
-        channel.confirm_delivery()
-        channel.basic_qos(prefetch_count=prefetch)
-
-        return channel
+        for partition in range(self._partitions):
+            if options['backup']:
+                self._declare_queue(
+                    queue,
+                    options,
+                    partition=partition,
+                    backup=True,
+                )
 
-    # TODO same result as with liebre-js
-    def get_info(self):
-        try:
-            # Provide a connection object so it can be closed
-            channel = self._get_channel()
-            channel.connection.close()
-            return True
-        except Exception:
-            return False
+            self._declare_queue(
+                queue,
+                options,
+                partition=partition,
+            )
 
     def _declare_queue(
         self,
         queue,
         options,
         partition=None,
         dead_letter=False,
@@ -230,39 +235,44 @@
 
         self._channel.queue_bind(
             exchange=self._exchange,
             queue=queue_name,
             routing_key=queue_name,
         )
 
-    @reconnect
     @thread_safe
-    def declare_queue(
-        self,
-        queue,
-        options=None,
-    ):
-        if options is None:
-            options = {}
-        options = self._queue_options | options
+    def _declare_exchange(self):
+        self._channel.exchange_declare(
+            exchange=self._exchange,
+            exchange_type=self._exchange_options['type'],
+            durable=self._exchange_options['durable'],
+            auto_delete=self._exchange_options['auto_delete'],
+        )
 
-        if options['dead_letters']:
-            self._declare_queue(
-                queue,
-                options,
-                dead_letter=True,
-            )
+    def _get_channel(self, prefetch=None):
+        if prefetch is None:
+            prefetch = self._prefetch
 
-        for partition in range(self._partitions):
-            if options['backup']:
-                self._declare_queue(
-                    queue,
-                    options,
-                    partition=partition,
-                    backup=True,
-                )
+        ssl_options = None
+        if self._tls:
+            ssl_options = pika.SSLOptions(ssl.SSLContext())
 
-            self._declare_queue(
-                queue,
-                options,
-                partition=partition,
+        # Pika's connection is not thread-safe, can't be reused.
+        # Thus, neither the channels belonging to it.
+        connection = pika.BlockingConnection(
+            pika.ConnectionParameters(
+                host=self._host,
+                port=self._port,
+                virtual_host=self._vhost,
+                credentials=pika.PlainCredentials(
+                    self._user,
+                    self._password,
+                ),
+                ssl_options=ssl_options,
             )
+        )
+
+        channel = connection.channel()
+        channel.confirm_delivery()
+        channel.basic_qos(prefetch_count=prefetch)
+
+        return channel
```

## liebre/utils.py

```diff
@@ -1,34 +1,27 @@
 import json
 
 
 def serialize_content(content):
     if isinstance(content, bytes):
         return content
 
+    if isinstance(content, str):
+        return content
+
     return json.dumps(
         content,
         ensure_ascii=False,
         separators=(',', ':'),
     )
 
 
 def deserialize_content(content):
     try:
-        deserialized_content = json.loads(content)
-
-        # Fix double serialization
-        if isinstance(content, str):
-            try:
-                deserialized_content = json.loads(deserialized_content)
-            except Exception:
-                deserialized_content = content
-
-        return deserialized_content
-
+        return json.loads(content)
     except Exception:
         return content
 
 
 def get_suffixed_queue_name(queue, suffix):
     return f'{queue}.{suffix}'
```

## Comparing `liebre-2.2304.2.dist-info/LICENSE` & `liebre-2.2304.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `liebre-2.2304.2.dist-info/METADATA` & `liebre-2.2304.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liebre
-Version: 2.2304.2
+Version: 2.2304.3
 Home-page: https://github.com/councilbox/liebre-python
 Author: 
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

