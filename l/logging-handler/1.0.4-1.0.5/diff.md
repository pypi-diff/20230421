# Comparing `tmp/logging_handler-1.0.4.tar.gz` & `tmp/logging_handler-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_handler-1.0.4.tar", last modified: Fri Apr 21 04:51:33 2023, max compression
+gzip compressed data, was "logging_handler-1.0.5.tar", last modified: Fri Apr 21 04:54:53 2023, max compression
```

## Comparing `logging_handler-1.0.4.tar` & `logging_handler-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:51:33.051484 logging_handler-1.0.4/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-01-27 21:59:39.000000 logging_handler-1.0.4/LICENSE
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 04:51:33.051484 logging_handler-1.0.4/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3278 2023-01-27 21:59:39.000000 logging_handler-1.0.4/README.md
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      804 2023-04-21 04:50:20.000000 logging_handler-1.0.4/pyproject.toml
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-04-21 04:51:33.051484 logging_handler-1.0.4/setup.cfg
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:51:33.048151 logging_handler-1.0.4/src/
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:51:33.051484 logging_handler-1.0.4/src/logging_handler/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4549 2023-04-21 04:50:03.000000 logging_handler-1.0.4/src/logging_handler/__init__.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:51:33.051484 logging_handler-1.0.4/src/logging_handler.egg-info/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 04:51:33.000000 logging_handler-1.0.4/src/logging_handler.egg-info/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      236 2023-04-21 04:51:33.000000 logging_handler-1.0.4/src/logging_handler.egg-info/SOURCES.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-04-21 04:51:33.000000 logging_handler-1.0.4/src/logging_handler.egg-info/dependency_links.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       16 2023-04-21 04:51:33.000000 logging_handler-1.0.4/src/logging_handler.egg-info/top_level.txt
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:54:53.914944 logging_handler-1.0.5/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-01-27 21:59:39.000000 logging_handler-1.0.5/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 04:54:53.914944 logging_handler-1.0.5/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3278 2023-01-27 21:59:39.000000 logging_handler-1.0.5/README.md
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      804 2023-04-21 04:54:31.000000 logging_handler-1.0.5/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-04-21 04:54:53.914944 logging_handler-1.0.5/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:54:53.911611 logging_handler-1.0.5/src/
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:54:53.914944 logging_handler-1.0.5/src/logging_handler/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4548 2023-04-21 04:54:25.000000 logging_handler-1.0.5/src/logging_handler/__init__.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 04:54:53.914944 logging_handler-1.0.5/src/logging_handler.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 04:54:53.000000 logging_handler-1.0.5/src/logging_handler.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      236 2023-04-21 04:54:53.000000 logging_handler-1.0.5/src/logging_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-04-21 04:54:53.000000 logging_handler-1.0.5/src/logging_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       16 2023-04-21 04:54:53.000000 logging_handler-1.0.5/src/logging_handler.egg-info/top_level.txt
```

### Comparing `logging_handler-1.0.4/LICENSE` & `logging_handler-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_handler-1.0.4/PKG-INFO` & `logging_handler-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging_handler
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Library to quickly create logging handlers
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/python_logging_handler/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/logging_handler/issues
 Project-URL: Source Code, https://github.com/LearningToPi/logging_handler
 Keywords: logging,syslog
 Classifier: Topic :: System :: Logging
```

### Comparing `logging_handler-1.0.4/README.md` & `logging_handler-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `logging_handler-1.0.4/pyproject.toml` & `logging_handler-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "logging_handler"
-version = "1.0.4"
+version = "1.0.5"
 description = "Python Library to quickly create logging handlers"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["logging", "syslog"]
 readme = "README.md"
 requires-python =">=3.6"
 classifiers = [
     "Topic :: System :: Logging",
```

### Comparing `logging_handler-1.0.4/src/logging_handler/__init__.py` & `logging_handler-1.0.5/src/logging_handler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "ERROR": ERROR,
     "CRITICAL": CRITICAL
 }
 
 _supported_log_levels = [DEBUG, INFO, WARNING, ERROR, CRITICAL]
 
 
-def _create_logger(console_level=WARNING, log_file='', file_level=WARNING, name='', file_mode='a', console=True,
+def create_logger(console_level=WARNING, log_file='', file_level=WARNING, name='', file_mode='a', console=True,
                   syslog=False, syslog_script_name='', log_file_vars=[], log_file_retention_days=0, propagate=False):
     """ Creates a logger and returns the handle.
         Log file vars should be sent as a dict -> {"var": "{date}", "set": "%Y-%m-%d-%Y-%M"}
 
         Supported log file vars:
             {date} - will be replaced with the current date using the provided strftime format
```

### Comparing `logging_handler-1.0.4/src/logging_handler.egg-info/PKG-INFO` & `logging_handler-1.0.5/src/logging_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-handler
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Library to quickly create logging handlers
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/python_logging_handler/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/logging_handler/issues
 Project-URL: Source Code, https://github.com/LearningToPi/logging_handler
 Keywords: logging,syslog
 Classifier: Topic :: System :: Logging
```

