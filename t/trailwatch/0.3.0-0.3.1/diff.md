# Comparing `tmp/trailwatch-0.3.0.tar.gz` & `tmp/trailwatch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailwatch-0.3.0.tar", max compression
+gzip compressed data, was "trailwatch-0.3.1.tar", max compression
```

## Comparing `trailwatch-0.3.0.tar` & `trailwatch-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-04-20 01:52:59.126414 trailwatch-0.3.0/LICENSE
--rw-r--r--   0        0        0     7527 2023-04-20 01:52:59.130415 trailwatch-0.3.0/README.md
--rw-r--r--   0        0        0     2026 2023-04-20 01:52:59.130415 trailwatch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3195 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/__init__.py
--rw-r--r--   0        0        0     6071 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/config.py
--rw-r--r--   0        0        0        0 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/__init__.py
--rw-r--r--   0        0        0       85 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/__init__.py
--rw-r--r--   0        0        0     8308 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/api.py
--rw-r--r--   0        0        0     3898 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/connector.py
--rw-r--r--   0        0        0      809 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/handler.py
--rw-r--r--   0        0        0     1081 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/base.py
--rw-r--r--   0        0        0      306 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/salesforce/__init__.py
--rw-r--r--   0        0        0     6116 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/salesforce/connector.py
--rw-r--r--   0        0        0     7103 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/context.py
--rw-r--r--   0        0        0      414 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/exceptions.py
--rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 15:40:39.231816 trailwatch-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7527 2023-04-20 15:40:39.231816 trailwatch-0.3.1/README.md
+-rw-r--r--   0        0        0     2026 2023-04-20 15:40:39.235816 trailwatch-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3634 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/__init__.py
+-rw-r--r--   0        0        0     6071 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/config.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/__init__.py
+-rw-r--r--   0        0        0     8308 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/api.py
+-rw-r--r--   0        0        0     3912 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/connector.py
+-rw-r--r--   0        0        0      809 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/handler.py
+-rw-r--r--   0        0        0     1081 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/base.py
+-rw-r--r--   0        0        0      306 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/salesforce/__init__.py
+-rw-r--r--   0        0        0     6116 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/salesforce/connector.py
+-rw-r--r--   0        0        0     7103 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/context.py
+-rw-r--r--   0        0        0      414 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/exceptions.py
+-rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.1/PKG-INFO
```

### Comparing `trailwatch-0.3.0/LICENSE` & `trailwatch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/README.md` & `trailwatch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/pyproject.toml` & `trailwatch-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trailwatch"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python SDK for TrailWatch by Kicksaw"
 license = "Apache-2.0"
 authors = ["George Bocharov <george@kicksaw.com>"]
 readme = "README.md"
 homepage = "https://www.kicksaw.com/"
 repository = "https://github.com/Kicksaw-Consulting/trailwatch-python-sdk"
 packages = [
```

### Comparing `trailwatch-0.3.0/src/trailwatch/__init__.py` & `trailwatch-0.3.1/src/trailwatch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,27 @@
     "configure",
     "TrailwatchContext",
     "watch",
 ]
 
 import functools
 import inspect
+import re
 
 from typing import Callable, TypeVar
 
 from typing_extensions import Concatenate, ParamSpec
 
 from .config import DEFAULT, Default, configure
 from .context import TrailwatchContext
 
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
 
 
-# TODO - add support for uploading files (inspect for argument)
 def watch(
     job: str | None = None,
     job_description: str | None = None,
     loggers: list[str] | Default | None = DEFAULT,
     execution_ttl: int | Default | None = DEFAULT,
     log_ttl: int | Default | None = DEFAULT,
     error_ttl: int | Default | None = DEFAULT,
@@ -62,17 +62,27 @@
 
     def wrapper(
         func: Callable[Concatenate[TrailwatchContext, _P], _T]
     ) -> Callable[_P, _T]:
         if inspect.iscoroutinefunction(func):
             raise NotImplementedError("Coroutine functions are not supported")
 
+        # Generate job description from docstring if not provided explicitly
+        _job_description = job_description or func.__doc__
+        if _job_description is not None:
+            # Remove indentation from docstring
+            _job_description = re.sub(r"\n\s+", " ", _job_description)
+            # Remove multiple spaces
+            _job_description = re.sub(r"\s+", " ", _job_description)
+            # Remove leading and trailing spaces
+            _job_description = _job_description.strip()
+
         decorator_kwargs = {
             "job": job or func.__name__,
-            "job_description": job_description or func.__doc__,
+            "job_description": _job_description,
             "loggers": loggers,
             "execution_ttl": execution_ttl,
             "log_ttl": log_ttl,
             "error_ttl": error_ttl,
             "timeout": timeout,
         }
         if decorator_kwargs["job_description"] is None:
```

### Comparing `trailwatch-0.3.0/src/trailwatch/config.py` & `trailwatch-0.3.1/src/trailwatch/config.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/src/trailwatch/connectors/aws/api.py` & `trailwatch-0.3.1/src/trailwatch/connectors/aws/api.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/src/trailwatch/connectors/aws/connector.py` & `trailwatch-0.3.1/src/trailwatch/connectors/aws/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.execution_id: str | None = None
         self.handler: AwsHandler | None = None
 
     @property
     def execution_url(self) -> str | None:
         if self.execution_id is None:
             return None
-        return "/".join([self.api.url, self.execution_id])
+        return "/".join([self.api.url, "executions", self.execution_id])
 
     def start_execution(self) -> None:
         # Create entries in TrailWatch database
         self.api.upsert_project(
             self.config.project,
             self.config.project_description,
         )
```

### Comparing `trailwatch-0.3.0/src/trailwatch/connectors/aws/handler.py` & `trailwatch-0.3.1/src/trailwatch/connectors/aws/handler.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/src/trailwatch/connectors/base.py` & `trailwatch-0.3.1/src/trailwatch/connectors/base.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/src/trailwatch/connectors/salesforce/connector.py` & `trailwatch-0.3.1/src/trailwatch/connectors/salesforce/connector.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/src/trailwatch/context.py` & `trailwatch-0.3.1/src/trailwatch/context.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.0/PKG-INFO` & `trailwatch-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailwatch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for TrailWatch by Kicksaw
 Home-page: https://www.kicksaw.com/
 License: Apache-2.0
 Author: George Bocharov
 Author-email: george@kicksaw.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

