# Comparing `tmp/ValiotWorker-5.3.0.tar.gz` & `tmp/ValiotWorker-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValiotWorker-5.3.0.tar", last modified: Mon Mar 27 19:36:31 2023, max compression
+gzip compressed data, was "ValiotWorker-5.3.1.tar", last modified: Fri Apr 21 16:45:19 2023, max compression
```

## Comparing `ValiotWorker-5.3.0.tar` & `ValiotWorker-5.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.238664 ValiotWorker-5.3.0/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.0/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.0/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-03-27 19:36:31.238442 ValiotWorker-5.3.0/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.0/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.234682 ValiotWorker-5.3.0/ValiotWorker/
--rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-02-21 21:42:45.000000 ValiotWorker-5.3.0/ValiotWorker/Logging.py
--rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.0/ValiotWorker/Notifications.py
--rw-r--r--   0 baruc      (501) staff       (20)      294 2023-03-27 19:36:21.000000 ValiotWorker-5.3.0/ValiotWorker/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-03-27 19:36:21.000000 ValiotWorker-5.3.0/ValiotWorker/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-03-27 19:36:21.000000 ValiotWorker-5.3.0/ValiotWorker/__version__.py
--rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.0/ValiotWorker/croniterHelpers.py
--rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.0/ValiotWorker/dateHelpers.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.237319 ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/
--rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/__main__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.237650 ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/modules/
--rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/modules/http_server.py
--rw-r--r--   0 baruc      (501) staff       (20)     7003 2023-03-07 22:03:01.000000 ValiotWorker-5.3.0/ValiotWorker/mutations.py
--rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.0/ValiotWorker/queries.py
--rw-r--r--   0 baruc      (501) staff       (20)     5258 2023-02-21 21:42:45.000000 ValiotWorker-5.3.0/ValiotWorker/redis.py
--rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-03-27 19:36:21.000000 ValiotWorker-5.3.0/ValiotWorker/subscriptions.py
--rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.0/ValiotWorker/uploaders.py
--rw-r--r--   0 baruc      (501) staff       (20)    69757 2023-03-27 19:36:21.000000 ValiotWorker-5.3.0/ValiotWorker/worker.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.236690 ValiotWorker-5.3.0/ValiotWorker.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      791 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       60 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)      237 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)       13 2023-03-27 19:36:31.000000 ValiotWorker-5.3.0/ValiotWorker.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-03-27 19:36:31.238861 ValiotWorker-5.3.0/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     2289 2023-02-22 19:57:08.000000 ValiotWorker-5.3.0/setup.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-03-27 19:36:31.238077 ValiotWorker-5.3.0/tests/
--rw-r--r--   0 baruc      (501) staff       (20)      106 2023-03-27 19:29:07.000000 ValiotWorker-5.3.0/tests/test_dummy.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.957589 ValiotWorker-5.3.1/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.1/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.1/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-04-21 16:45:19.957387 ValiotWorker-5.3.1/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.1/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.954006 ValiotWorker-5.3.1/ValiotWorker/
+-rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.1/ValiotWorker/Logging.py
+-rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.1/ValiotWorker/Notifications.py
+-rw-r--r--   0 baruc      (501) staff       (20)      294 2023-03-27 19:36:21.000000 ValiotWorker-5.3.1/ValiotWorker/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-04-21 16:31:49.000000 ValiotWorker-5.3.1/ValiotWorker/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-04-21 16:44:47.000000 ValiotWorker-5.3.1/ValiotWorker/__version__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.1/ValiotWorker/croniterHelpers.py
+-rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.1/ValiotWorker/dateHelpers.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.956463 ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/
+-rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/__main__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.956771 ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/modules/
+-rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/modules/http_server.py
+-rw-r--r--   0 baruc      (501) staff       (20)     7003 2023-03-07 22:03:01.000000 ValiotWorker-5.3.1/ValiotWorker/mutations.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.1/ValiotWorker/queries.py
+-rw-r--r--   0 baruc      (501) staff       (20)     5258 2023-04-14 18:00:15.000000 ValiotWorker-5.3.1/ValiotWorker/redis.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-03-27 19:36:21.000000 ValiotWorker-5.3.1/ValiotWorker/subscriptions.py
+-rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.1/ValiotWorker/uploaders.py
+-rw-r--r--   0 baruc      (501) staff       (20)    69745 2023-04-21 16:44:47.000000 ValiotWorker-5.3.1/ValiotWorker/worker.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.955991 ValiotWorker-5.3.1/ValiotWorker.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      791 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       60 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)      237 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       13 2023-04-21 16:45:19.000000 ValiotWorker-5.3.1/ValiotWorker.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-04-21 16:45:19.957645 ValiotWorker-5.3.1/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     2289 2023-02-22 19:57:08.000000 ValiotWorker-5.3.1/setup.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:45:19.957051 ValiotWorker-5.3.1/tests/
+-rw-r--r--   0 baruc      (501) staff       (20)      106 2023-04-21 16:31:49.000000 ValiotWorker-5.3.1/tests/test_dummy.py
```

### Comparing `ValiotWorker-5.3.0/LICENCE` & `ValiotWorker-5.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/PKG-INFO` & `ValiotWorker-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.0
+Version: 5.3.1
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.0/README.md` & `ValiotWorker-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/Logging.py` & `ValiotWorker-5.3.1/ValiotWorker/Logging.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/Notifications.py` & `ValiotWorker-5.3.1/ValiotWorker/Notifications.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/__main__.py` & `ValiotWorker-5.3.1/ValiotWorker/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/__main__.py` & `ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/healthCheckProbe/modules/http_server.py` & `ValiotWorker-5.3.1/ValiotWorker/healthCheckProbe/modules/http_server.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/mutations.py` & `ValiotWorker-5.3.1/ValiotWorker/mutations.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/queries.py` & `ValiotWorker-5.3.1/ValiotWorker/queries.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/redis.py` & `ValiotWorker-5.3.1/ValiotWorker/redis.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/subscriptions.py` & `ValiotWorker-5.3.1/ValiotWorker/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/ValiotWorker/worker.py` & `ValiotWorker-5.3.1/ValiotWorker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
           unsubJobCreated (GraphQLClient.sub): GraphQLClient subscriptions. Defaults
             to None.
           useRedis (boolean): Determine to use Redis. Defaults to False.
           redis (WorkerRedis): Instance of a WorkerRedis.
           continuousJobs (list): List of a running job. Defaults to list.
           logginStyle (LogStyle.PREFIX_FIRST_LINE) = LogStyle.PREFIX_FIRST_LINE
           stopLogging (boolean): Set to stop logs.
-          loggingThread (Thread): Gets the logs of a process. Defaults to None.
+          loggingProcess (Process): Gets the logs of a process. Defaults to None.
           log (Log): Log message. Defaults to None.
           logQueues (dict): A dictionry with all queues logs.
 
       Examples:
           >>> <With> clause:
             '''
             import os
@@ -199,15 +199,15 @@
         # logging attributes
         current_env = os.environ.get('ENV')
         if current_env == 'dev':
             self.setLoggingStyle(LogStyle.PREFIX_FIRST_LINE)
         else:
             self.setLoggingStyle(LogStyle.JSON)
         self.stopLogging = False
-        self.loggingThread = None
+        self.loggingProcess = None
         self.log = None
         self.logQueues = {
             'main': SimpleQueue()  # queue for the main thread (Orchestator)
         }
 
     def setClient(self, client):
         """Set a GraphQLClient instance.
@@ -1541,20 +1541,24 @@
             except KeyboardInterrupt:
                 log(LogLevel.WARNING, 'Logging stopped due to keyboard interrupt')
             log(LogLevel.WARNING, 'Logging loop stopped')
         # END FN DEFINITION --------------------------
         # Create Queues for each queue:
         for queue_name, _ in self.queues.items():
             self.logQueues[queue_name] = SimpleQueue()
-        # ! Start logging loop as a Daemon thread, so it can be stopped by the main Process on termination
-        # ! this way, we don't need to worry about the logging loop being stopped elsewhere
-        self.loggingThread = Thread(target=loggingLoop, daemon=True, name="logging-loop")
-        self.loggingThread.start()
+        self.loggingProcess = self.context.Process(target=loggingLoop)
+        self.loggingProcess.start()
         self.log(LogLevel.SUCCESS, 'Logging loop started')
 
+    def stopLoggingLoop(self):
+         """This function stops de logging loop.
+         """
+         self.stopLogging = True
+         self.loggingProcess.join()
+
     def eventLoop(self, interval=1.0):
         """This function manages all generic worker activities.
 
         Args:
             interval (float, optional): Interval time of each loop. Defaults to 1.0.
         """
         try:
@@ -1652,10 +1656,11 @@
             self.redis.initializeRedis()
         self.registerContinuousJobs()
         while 1:
             try:
                 self.eventLoop(interval=interval)
             except KeyboardInterrupt:
                 log(LogLevel.WARNING, "\nuser's stop signal, exiting...")
+                self.stopLoggingLoop()
                 self.unlockFinishedJobs(force=True)
                 self.gql.close()
                 break
```

### Comparing `ValiotWorker-5.3.0/ValiotWorker.egg-info/PKG-INFO` & `ValiotWorker-5.3.1/ValiotWorker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.0
+Version: 5.3.1
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.0/ValiotWorker.egg-info/SOURCES.txt` & `ValiotWorker-5.3.1/ValiotWorker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.0/setup.py` & `ValiotWorker-5.3.1/setup.py`

 * *Files identical despite different names*

