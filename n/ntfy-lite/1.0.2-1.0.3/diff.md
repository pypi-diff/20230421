# Comparing `tmp/ntfy_lite-1.0.2.tar.gz` & `tmp/ntfy_lite-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntfy_lite-1.0.2.tar", max compression
+gzip compressed data, was "ntfy_lite-1.0.3.tar", max compression
```

## Comparing `ntfy_lite-1.0.2.tar` & `ntfy_lite-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1552 2023-04-12 13:02:43.946112 ntfy_lite-1.0.2/LICENSE
--rw-r--r--   0        0        0     1359 2023-04-19 09:16:58.591608 ntfy_lite-1.0.2/README.md
--rw-r--r--   0        0        0      275 2023-04-18 11:39:06.880631 ntfy_lite-1.0.2/ntfy_lite/__init__.py
--rw-r--r--   0        0        0     3051 2023-04-18 11:26:45.513790 ntfy_lite-1.0.2/ntfy_lite/actions.py
--rw-r--r--   0        0        0      703 2023-04-13 11:01:57.455399 ntfy_lite-1.0.2/ntfy_lite/defaults.py
--rw-r--r--   0        0        0     3845 2023-04-18 11:26:24.677934 ntfy_lite-1.0.2/ntfy_lite/demo_logging.py
--rw-r--r--   0        0        0     2189 2023-04-18 11:26:24.657934 ntfy_lite-1.0.2/ntfy_lite/demo_push.py
--rw-r--r--   0        0        0      407 2023-04-12 13:02:43.946112 ntfy_lite-1.0.2/ntfy_lite/error.py
--rw-r--r--   0        0        0     5311 2023-04-18 11:27:00.921683 ntfy_lite-1.0.2/ntfy_lite/handler.py
--rw-r--r--   0        0        0     6692 2023-04-18 11:26:24.689934 ntfy_lite-1.0.2/ntfy_lite/ntfy.py
--rw-r--r--   0        0        0     1185 2023-04-18 11:26:24.657934 ntfy_lite-1.0.2/ntfy_lite/ntfy2logging.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:43.946112 ntfy_lite-1.0.2/ntfy_lite/py.typed
--rw-r--r--   0        0        0      565 2023-04-13 11:50:46.209632 ntfy_lite-1.0.2/ntfy_lite/utils.py
--rw-r--r--   0        0        0       76 2023-04-18 11:39:34.340439 ntfy_lite-1.0.2/ntfy_lite/version.py
--rw-r--r--   0        0        0      945 2023-04-19 09:02:42.873474 ntfy_lite-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 ntfy_lite-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1552 2023-04-12 13:02:43.946112 ntfy_lite-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1359 2023-04-19 09:16:58.591608 ntfy_lite-1.0.3/README.md
+-rw-r--r--   0        0        0      275 2023-04-18 11:39:06.880631 ntfy_lite-1.0.3/ntfy_lite/__init__.py
+-rw-r--r--   0        0        0     3051 2023-04-18 11:26:45.513790 ntfy_lite-1.0.3/ntfy_lite/actions.py
+-rw-r--r--   0        0        0      703 2023-04-13 11:01:57.455399 ntfy_lite-1.0.3/ntfy_lite/defaults.py
+-rw-r--r--   0        0        0     3845 2023-04-18 11:26:24.677934 ntfy_lite-1.0.3/ntfy_lite/demo_logging.py
+-rw-r--r--   0        0        0     2189 2023-04-18 11:26:24.657934 ntfy_lite-1.0.3/ntfy_lite/demo_push.py
+-rw-r--r--   0        0        0      407 2023-04-12 13:02:43.946112 ntfy_lite-1.0.3/ntfy_lite/error.py
+-rw-r--r--   0        0        0     5311 2023-04-18 11:27:00.921683 ntfy_lite-1.0.3/ntfy_lite/handler.py
+-rw-r--r--   0        0        0     6694 2023-04-19 12:36:08.121485 ntfy_lite-1.0.3/ntfy_lite/ntfy.py
+-rw-r--r--   0        0        0     1185 2023-04-18 11:26:24.657934 ntfy_lite-1.0.3/ntfy_lite/ntfy2logging.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:43.946112 ntfy_lite-1.0.3/ntfy_lite/py.typed
+-rw-r--r--   0        0        0      565 2023-04-13 11:50:46.209632 ntfy_lite-1.0.3/ntfy_lite/utils.py
+-rw-r--r--   0        0        0       76 2023-04-18 11:39:34.340439 ntfy_lite-1.0.3/ntfy_lite/version.py
+-rw-r--r--   0        0        0      963 2023-04-21 09:35:11.499558 ntfy_lite-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ntfy_lite-1.0.3/PKG-INFO
```

### Comparing `ntfy_lite-1.0.2/LICENSE` & `ntfy_lite-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/README.md` & `ntfy_lite-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/actions.py` & `ntfy_lite-1.0.3/ntfy_lite/actions.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/defaults.py` & `ntfy_lite-1.0.3/ntfy_lite/defaults.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/demo_logging.py` & `ntfy_lite-1.0.3/ntfy_lite/demo_logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/demo_push.py` & `ntfy_lite-1.0.3/ntfy_lite/demo_push.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/handler.py` & `ntfy_lite-1.0.3/ntfy_lite/handler.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/ntfy.py` & `ntfy_lite-1.0.3/ntfy_lite/ntfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """
     An optional value of DryRun may be passed as an argument to the [ntfy_lite.ntfy.push][] function.
 
     - If 'off' is passed (default), then the [ntfy_lite.ntfy.push][] function will publish to ntfy.
 
     - If 'on' is passed, then the [ntfy_lite.ntfy.push][] function will *not* publish to ntfy.
 
-    - If 'error' is passed, then the [ntfy_lite.ntfy.push][] function will raise an [ntfy_lite.error.NtfyError].
+    - If 'error' is passed, then the [ntfy_lite.ntfy.push][] function will raise an [ntfy_lite.error.NtfyError][].
 
     This is meant for testing.
     """
 
     on = auto()
     off = auto()
     error = auto()
```

### Comparing `ntfy_lite-1.0.2/ntfy_lite/ntfy2logging.py` & `ntfy_lite-1.0.3/ntfy_lite/ntfy2logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/ntfy_lite/utils.py` & `ntfy_lite-1.0.3/ntfy_lite/utils.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.2/pyproject.toml` & `ntfy_lite-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntfy-lite"
-version = "1.0.2"
+version = "1.0.3"
 description = "minimalistic python API for sending ntfy notifications"
 authors = ["Vincent Berenz <vberenz@tuebingen.mpg.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "ntfy_lite"}]
 
 [[tool.poetry.source]]
@@ -17,14 +17,15 @@
 ntfy_lite_push_demo = 'ntfy_lite.demo_push:run'
 ntfy_lite_logging_demo = 'ntfy_lite.demo_logging:run'
 
 [tool.poetry.dependencies]
 python = ">3.8.1,<4"
 requests = "^2.28.2"
 validators = "^0.20.0"
+pandas = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 flake8 = "^6.0.0"
 pytest = "^7.3.0"
 types-requests = "^2.28.11.17"
 ipython = "^8.12.0"
```

### Comparing `ntfy_lite-1.0.2/PKG-INFO` & `ntfy_lite-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ntfy-lite
-Version: 1.0.2
+Version: 1.0.3
 Summary: minimalistic python API for sending ntfy notifications
 License: BSD-3-Clause
 Author: Vincent Berenz
 Author-email: vberenz@tuebingen.mpg.de
 Requires-Python: >3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 ![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)
 [![documentation](https://github.com/MPI-IS/ntfy_lite/actions/workflows/mkdocs.yaml/badge.svg)](https://mpi-is.github.io/ntfy_lite/)
```

