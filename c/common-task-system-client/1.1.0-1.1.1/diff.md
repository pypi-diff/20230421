# Comparing `tmp/common-task-system-client-1.1.0.tar.gz` & `tmp/common-task-system-client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-task-system-client-1.1.0.tar", last modified: Tue Apr 18 05:45:45 2023, max compression
+gzip compressed data, was "common-task-system-client-1.1.1.tar", last modified: Fri Apr 21 05:43:09 2023, max compression
```

## Comparing `common-task-system-client-1.1.0.tar` & `common-task-system-client-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/
--rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.280985 common-task-system-client-1.1.0/common_task_system_client.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-18 05:45:30.000000 common-task-system-client-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.282990 common-task-system-client-1.1.0/task_system_client/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.0/task_system_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.285413 common-task-system-client-1.1.0/task_system_client/callback/
--rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.0/task_system_client/callback/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.0/task_system_client/callback/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.286670 common-task-system-client-1.1.0/task_system_client/callback/callbacks/
--rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.0/task_system_client/callback/callbacks/__init__.py
--rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.0/task_system_client/callback/callbacks/upload_log.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.287676 common-task-system-client-1.1.0/task_system_client/executor/
--rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.0/task_system_client/executor/__init__.py
--rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.1.0/task_system_client/executor/base.py
--rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.1.0/task_system_client/executor/executor.py
--rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.0/task_system_client/main.py
--rw-rw-rw-   0        0        0     1711 2023-03-17 05:50:08.000000 common-task-system-client-1.1.0/task_system_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.289689 common-task-system-client-1.1.0/task_system_client/subscriber/
--rw-rw-rw-   0        0        0      514 2023-03-16 03:25:28.000000 common-task-system-client-1.1.0/task_system_client/subscriber/__init__.py
--rw-rw-rw-   0        0        0     2777 2023-04-18 05:44:26.000000 common-task-system-client-1.1.0/task_system_client/subscriber/base.py
--rw-rw-rw-   0        0        0     3578 2023-03-17 09:31:53.000000 common-task-system-client-1.1.0/task_system_client/subscriber/threaded.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.290688 common-task-system-client-1.1.0/task_system_client/task_center/
--rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.0/task_system_client/task_center/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.291685 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/
--rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.293683 common-task-system-client-1.1.0/task_system_client/task_center/subscription/
--rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/__init__.py
--rw-rw-rw-   0        0        0      934 2023-03-23 02:33:23.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/base.py
--rw-rw-rw-   0        0        0     1382 2023-04-18 05:41:46.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/http.py
--rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/redis.py
--rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/sql.py
--rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.1.0/task_system_client/task_center/task.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.295620 common-task-system-client-1.1.0/task_system_client/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.0/task_system_client/utils/__init__.py
--rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.0/task_system_client/utils/class_loader.py
--rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.0/task_system_client/utils/db_utils.py
--rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.0/task_system_client/utils/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.925353 common-task-system-client-1.1.1/common_task_system_client.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-04-21 03:23:50.000000 common-task-system-client-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.927354 common-task-system-client-1.1.1/task_system_client/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.1/task_system_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.929866 common-task-system-client-1.1.1/task_system_client/callback/
+-rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.1/task_system_client/callback/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.1/task_system_client/callback/base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.931126 common-task-system-client-1.1.1/task_system_client/callback/callbacks/
+-rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.1/task_system_client/callback/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.1/task_system_client/callback/callbacks/upload_log.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.932641 common-task-system-client-1.1.1/task_system_client/executor/
+-rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.1/task_system_client/executor/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.1.1/task_system_client/executor/base.py
+-rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.1.1/task_system_client/executor/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.934638 common-task-system-client-1.1.1/task_system_client/handler/
+-rw-rw-rw-   0        0        0      277 2023-04-21 03:33:18.000000 common-task-system-client-1.1.1/task_system_client/handler/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 03:13:13.000000 common-task-system-client-1.1.1/task_system_client/handler/base.py
+-rw-rw-rw-   0        0        0      694 2023-04-21 03:22:51.000000 common-task-system-client-1.1.1/task_system_client/handler/exception.py
+-rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.1/task_system_client/main.py
+-rw-rw-rw-   0        0        0     1888 2023-04-21 05:42:56.000000 common-task-system-client-1.1.1/task_system_client/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.936639 common-task-system-client-1.1.1/task_system_client/subscriber/
+-rw-rw-rw-   0        0        0      541 2023-04-21 03:36:06.000000 common-task-system-client-1.1.1/task_system_client/subscriber/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-04-21 03:13:46.000000 common-task-system-client-1.1.1/task_system_client/subscriber/base.py
+-rw-rw-rw-   0        0        0     4530 2023-04-21 03:28:45.000000 common-task-system-client-1.1.1/task_system_client/subscriber/threaded.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.938641 common-task-system-client-1.1.1/task_system_client/task_center/
+-rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.1/task_system_client/task_center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.939638 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/
+-rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/__init__.py
+-rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.943639 common-task-system-client-1.1.1/task_system_client/task_center/subscription/
+-rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-04-21 05:30:08.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/base.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 05:13:58.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/http.py
+-rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/redis.py
+-rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/sql.py
+-rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.1.1/task_system_client/task_center/task.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.945639 common-task-system-client-1.1.1/task_system_client/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.1/task_system_client/utils/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.1/task_system_client/utils/class_loader.py
+-rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.1/task_system_client/utils/db_utils.py
+-rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.1/task_system_client/utils/module_loading.py
```

### Comparing `common-task-system-client-1.1.0/LICENSE` & `common-task-system-client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/common_task_system_client.egg-info/SOURCES.txt` & `common-task-system-client-1.1.1/common_task_system_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 task_system_client/callback/__init__.py
 task_system_client/callback/base.py
 task_system_client/callback/callbacks/__init__.py
 task_system_client/callback/callbacks/upload_log.py
 task_system_client/executor/__init__.py
 task_system_client/executor/base.py
 task_system_client/executor/executor.py
+task_system_client/handler/__init__.py
+task_system_client/handler/base.py
+task_system_client/handler/exception.py
 task_system_client/subscriber/__init__.py
 task_system_client/subscriber/base.py
 task_system_client/subscriber/threaded.py
 task_system_client/task_center/__init__.py
 task_system_client/task_center/task.py
 task_system_client/task_center/dispatch/__init__.py
 task_system_client/task_center/dispatch/dispatcher.py
```

### Comparing `common-task-system-client-1.1.0/task_system_client/callback/callbacks/upload_log.py` & `common-task-system-client-1.1.1/task_system_client/callback/callbacks/upload_log.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/executor/executor.py` & `common-task-system-client-1.1.1/task_system_client/executor/executor.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/settings.py` & `common-task-system-client-1.1.1/task_system_client/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 THREAD_SUBSCRIBER = {
     "THREAD_NUM": 2,
     "MAX_QUEUE_SIZE": 1000,
     "THREAD_CLASS": "task_system_client.subscriber.threaded.ThreadExecutor",
     "QUEUE": "task_system_client.subscriber.threaded.PriorityQueue",
 }
 
+# 异常处理
+EXCEPTION_HANDLER = "task_system_client.handler.exception.ExceptionHandler"
+EXCEPTION_REPORT_URL = None
+
+# 并发控制， 为None则不限制
+SEMAPHORE = 10
 
 logger = logging.getLogger(__name__)
 BASIC_FORMAT = "[%(asctime)s][%(levelname)s]%(message)s"
 DATE_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 formatter = logging.Formatter(BASIC_FORMAT, DATE_FORMAT)
 
@@ -55,8 +61,7 @@
 import os
 env_settings = os.environ.get('TASK_CLIENT_SETTINGS_MODULE', None)
 if env_settings:
     settings = importlib.import_module(env_settings)
     for key in dir(settings):
         if key.isupper():
             globals()[key] = getattr(settings, key)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `common-task-system-client-1.1.0/task_system_client/subscriber/__init__.py` & `common-task-system-client-1.1.1/task_system_client/subscriber/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import BaseSubscriber
-from .threaded import ThreadSubscriber
+from .threaded import ThreadPoolSubscriber, FixedThreadSubscriber
 from ..utils.class_loader import load_class
 
 
 def get_subscriber_cls(subscriber=None):
     if subscriber is None:
         from ..settings import SUBSCRIBER
         subscriber = SUBSCRIBER
```

### Comparing `common-task-system-client-1.1.0/task_system_client/subscriber/base.py` & `common-task-system-client-1.1.1/task_system_client/subscriber/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from threading import Event
 from ..task_center.subscription import create_subscription
 from ..task_center.dispatch import create_dispatcher
 from ..settings import SUBSCRIPTION, DISPATCHER, logger
+from ..handler import ExceptionHandler, BaseHandler
 import time
 
 
 class BaseSubscriber(object):
     SUBSCRIPTION = None
     DISPATCHER = None
     block_on_subscription = False
 
     def __init__(self, name='BaseSubscribe'):
         self.name = name
         self._state = Event()
         self.start_time = time.time()
         self.dispatcher = create_dispatcher(self.DISPATCHER or DISPATCHER)
         self.subscription = create_subscription(self.SUBSCRIPTION or SUBSCRIPTION)
+        self.exception_handler = None
+        if ExceptionHandler is not None:
+            self.exception_handler: BaseHandler = ExceptionHandler()
 
-    def run_executor(self, executor):
+    def run_synchronous(self, executor):
         try:
             executor.run()
         except Exception as e:
             logger.exception("%s run error: %s", executor, e)
             on_error = getattr(executor, 'on_error', None)
             if on_error:
                 on_error(e)
@@ -29,27 +33,44 @@
             on_success = getattr(executor, 'on_success', None)
             if on_success:
                 on_success()
         on_done = getattr(executor, 'on_done', None)
         if on_done:
             on_done()
 
-    def on_succeed(self, schedule, executor):
+    def execute(self, executor):
+        try:
+            self.run_synchronous(executor)
+        except Exception as e:
+            self.on_execute_failed(executor.schedule, executor, e)
+        else:
+            self.on_execute_succeed(executor.schedule, executor)
+        self.on_execute_done(executor.schedule, executor)
+
+    def run_executor(self, executor):
+        self.execute(executor)
+
+    def on_execute_succeed(self, schedule, executor):
         pass
 
-    def on_failed(self, schedule, executor, e):
+    def on_execute_failed(self, schedule, executor, e):
         pass
 
-    def on_done(self, schedule, executor):
+    def on_execute_done(self, schedule, executor):
         pass
 
+    def on_exception(self, e):
+        logger.exception("Subscriber %s error: %s", self.name, e)
+        if self.exception_handler:
+            self.exception_handler.handle(e)
+
     def is_schedulable(self):
         return True
 
-    def is_executable(self, schedule):
+    def is_executable(self, executor):
         return True
 
     def run(self):
         get_schedule = self.subscription.get_one
         dispatch = self.dispatcher.dispatch
         block = self.block_on_subscription
 
@@ -62,23 +83,17 @@
                 schedule = get_schedule(block)
                 if not schedule:
                     time.sleep(1)
                     continue
                 executor = dispatch(schedule)
                 if not self.is_executable(executor):
                     continue
-                try:
-                    self.run_executor(executor)
-                except Exception as e:
-                    self.on_failed(schedule, executor, e)
-                else:
-                    self.on_succeed(schedule, executor)
-                self.on_done(schedule, executor)
+                self.run_executor(executor)
             except Exception as e:
-                logger.exception("Run error: %s", e)
+                self.on_exception(e)
 
     def start(self):
         self._state.set()
         self.run()
 
     def stop(self):
         self._state.clear()
```

### Comparing `common-task-system-client-1.1.0/task_system_client/subscriber/threaded.py` & `common-task-system-client-1.1.1/task_system_client/subscriber/threaded.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 logger = settings.logger
 
 
 class ThreadExecutor(Thread):
     SUBSCRIPTION = None
     DISPATCHER = None
 
-    def __init__(self, queue, on_succeed=None, on_failed=None, on_done=None, name='Subscribe'):
+    def __init__(self, queue, on_succeed=None, on_failed=None, on_done=None, on_exception=None, name='Subscribe'):
         self.queue = queue
         self.on_succeed = on_succeed
         self.on_failed = on_failed
         self.on_done = on_done
+        self.on_exception = on_exception
         super().__init__(name=name, daemon=True)
 
     @classmethod
     def run_executor(cls, executor: BaseExecutor):
         try:
             executor.run()
         except Exception as e:
@@ -35,64 +36,91 @@
             if on_success:
                 on_success()
         on_done = getattr(executor, 'on_done', None)
         if on_done:
             on_done()
 
     def run(self):
+        on_execute_succeed = self.on_succeed
+        on_execute_failed = self.on_failed
+        on_execute_done = self.on_done
+        on_exception = self.on_exception
         while True:
             executor: BaseExecutor = self.queue.get()
             time.sleep(0.1)
             try:
                 try:
                     self.run_executor(executor)
                 except Exception as e:
-                    self.on_failed(executor.schedule, executor, e)
+                    on_execute_failed(executor.schedule, executor, e)
                 else:
-                    self.on_succeed(executor.schedule, executor)
-                self.on_done(executor.schedule, executor)
+                    on_execute_succeed(executor.schedule, executor)
+                on_execute_done(executor.schedule, executor)
             except Exception as e:
-                logger.exception("Run error: %s", e)
+                if on_exception:
+                    on_exception(e)
 
 
-class ThreadSubscriber(BaseSubscriber):
+class FixedThreadSubscriber(BaseSubscriber):
 
     def __init__(self, name=None, queue=None, thread_num=None):
         super().__init__(name=name)
         thread_subscriber = settings.THREAD_SUBSCRIBER
         self.max_queue_size = thread_subscriber.get('MAX_QUEUE_SIZE', 100)
         self.queue = queue or Queue(maxsize=self.max_queue_size)
         self.thread_num = thread_num or thread_subscriber.get('THREAD_NUM', 2)
         thread_class = thread_subscriber.get('THREAD_CLASS', ThreadExecutor.__module__ + '.' + ThreadExecutor.__name__)
         self._threads = [self.create_thread(thread_class,
                                             name=f'{self.name}_{i}',
                                             queue=self.queue,
-                                            on_succeed=self.on_succeed,
-                                            on_failed=self.on_failed,
-                                            on_done=self.on_done)
+                                            on_succeed=self.on_execute_succeed,
+                                            on_failed=self.on_execute_failed,
+                                            on_done=self.on_execute_done)
                          for i in range(self.thread_num)]
 
     @classmethod
     def create_thread(cls, thread_class, **kwargs):
         return load_class(thread_class)(**kwargs)
 
     def run(self):
         get_schedule = self.subscription.get_one
         dispatch = self.dispatcher.dispatch
         while self._state.is_set():
             time.sleep(0.1)
             try:
-                if not self.is_runnable():
+                if not self.is_schedulable():
                     continue
                 schedule = get_schedule()
                 executor = dispatch(schedule)
                 self.run_executor(executor)
             except Exception as e:
                 logger.exception("Run error: %s", e)
 
     def run_executor(self, executor):
         self.queue.put(executor)
 
     def start(self):
         for t in self._threads:
             t.start()
-        super(ThreadSubscriber, self).start()
+        super(FixedThreadSubscriber, self).start()
+
+
+class ThreadPoolSubscriber(BaseSubscriber):
+
+    def __init__(self, name=None):
+        super(ThreadPoolSubscriber, self).__init__(name=name)
+        self._threads = []
+
+    def is_schedulable(self):
+        n = len(self._threads)
+        if n < settings.SEMAPHORE:
+            return True
+        for t in range(n)[::-1]:
+            if not self._threads[t].is_alive():
+                self._threads.pop(t)
+                return True
+        return False
+
+    def run_executor(self, executor):
+        thread = Thread(target=self.execute, args=(executor,), daemon=True)
+        thread.start()
+        self._threads.append(thread)
```

### Comparing `common-task-system-client-1.1.0/task_system_client/task_center/dispatch/dispatcher.py` & `common-task-system-client-1.1.1/task_system_client/task_center/dispatch/dispatcher.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/task_center/subscription/http.py` & `common-task-system-client-1.1.1/task_system_client/task_center/subscription/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         super(HttpSubscription, self).__init__()
 
     def get(self, block=True):
         try:
             response = requests.get(self.subscription_url)
             if response.status_code == 200:
                 return TaskSchedule(response.json())
-            elif response.status_code == 204:
+            elif response.status_code == 202:
                 stdout.write('[%s]no more schedule now, wait 1 second...\r' % time.strftime('%Y-%m-%d %H:%M:%S'))
                 stdout.flush()
             else:
                 # 有可能存在500情况是被nginx代理的，所以输出response.text不会错
                 stdout.write('[%s]get schedule error, status code: %s\n' % (
                     time.strftime('%Y-%m-%d %H:%M:%S'), response.text))
                 stdout.flush()
```

### Comparing `common-task-system-client-1.1.0/task_system_client/task_center/subscription/redis.py` & `common-task-system-client-1.1.1/task_system_client/task_center/subscription/redis.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/task_center/subscription/sql.py` & `common-task-system-client-1.1.1/task_system_client/task_center/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/task_center/task.py` & `common-task-system-client-1.1.1/task_system_client/task_center/task.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/utils/db_utils.py` & `common-task-system-client-1.1.1/task_system_client/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.0/task_system_client/utils/module_loading.py` & `common-task-system-client-1.1.1/task_system_client/utils/module_loading.py`

 * *Files identical despite different names*

