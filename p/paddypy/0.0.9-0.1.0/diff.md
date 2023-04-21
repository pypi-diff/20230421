# Comparing `tmp/paddypy-0.0.9.tar.gz` & `tmp/paddypy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.0.9.tar", last modified: Mon Apr 17 11:00:01 2023, max compression
+gzip compressed data, was "paddypy-0.1.0.tar", last modified: Fri Apr 21 08:32:52 2023, max compression
```

## Comparing `paddypy-0.0.9.tar` & `paddypy-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.333416 paddypy-0.0.9/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-04-17 11:00:01.332916 paddypy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.321414 paddypy-0.0.9/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 10:59:11.000000 paddypy-0.0.9/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.9/paddypy/access.py
--rw-rw-rw-   0        0        0     2912 2023-04-17 10:59:27.000000 paddypy-0.0.9/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.331915 paddypy-0.0.9/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 11:00:01.333416 paddypy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1449 2023-04-17 10:59:57.000000 paddypy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.235098 paddypy-0.1.0/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-04-21 08:32:52.234597 paddypy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.218596 paddypy-0.1.0/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.0/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.0/paddypy/access.py
+-rw-rw-rw-   0        0        0     2847 2023-04-21 08:31:43.000000 paddypy-0.1.0/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.233599 paddypy-0.1.0/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-21 08:32:52.000000 paddypy-0.1.0/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:32:52.235098 paddypy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-04-21 08:32:10.000000 paddypy-0.1.0/setup.py
```

### Comparing `paddypy-0.0.9/LICENSE` & `paddypy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.9/PKG-INFO` & `paddypy-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.9/README.md` & `paddypy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.9/paddypy/access.py` & `paddypy-0.1.0/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.9/paddypy/log.py` & `paddypy-0.1.0/paddypy/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 import time
 import logging
 import datetime
 from . import access
 
 class CloudLogger():
-    def __init__(self, app_logger_name, module_name, logger_level=int(access.getValue(key="loggging-level", deactivate_kv_access=False))):
+    def __init__(self, app_logger_name, module_name, logger_level=10):
         self.LOGGER_LEVEL = logger_level
         self.logger = self._get_logger(app_logger_name=app_logger_name, module_name=module_name)
 
         
     def _get_logger(self, app_logger_name, module_name):
         FMT = "[{levelname:^9}] {name}: {message}"
         FORMATS = {
@@ -45,15 +45,15 @@
     def timeit(self, func):
         @wraps(func)
         def timeit_wrapper(*args, **kwargs):
             start_time = time.perf_counter()
             result = func(*args, **kwargs)
             end_time = time.perf_counter()
             total_time = end_time - start_time
-            self.logger.log(msg=f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.DEBUG)
+            self.logger.log(msg=f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.INFO)
             #logging.log(f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.DEBUG)
             return result
         return timeit_wrapper
 
 
 
 
@@ -63,8 +63,9 @@
         exceptionType = str(type(inst))
         exceptionArgument = str(inst.args)
         exceptionInstance = str(inst)
         self.logger.log(msg="Exception message: {message}".format(message=exceptionMessage), level=logging.ERROR)
         self.logger.log(msg="Exception occured at: {message}".format(message=exceptionTimne), level=logging.ERROR)
         self.logger.log(msg="Exception instance type: {message}".format(message=exceptionType), level=logging.ERROR)
         self.logger.log(msg="Exception argument: {message}".format(message=exceptionArgument), level=logging.ERROR)
-        self.logger.log(msg="Exception instance: {message}".format(message=exceptionInstance), level=logging.ERROR)
+        self.logger.log(msg="Exception instance: {message}".format(message=exceptionInstance), level=logging.ERROR)
+
```

### Comparing `paddypy-0.0.9/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.0/paddypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.9/setup.py` & `paddypy-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

