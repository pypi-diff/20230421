# Comparing `tmp/pymccool-0.2.3.tar.gz` & `tmp/pymccool-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymccool-0.2.3.tar", last modified: Fri Apr 21 00:33:40 2023, max compression
+gzip compressed data, was "pymccool-0.3.3.tar", last modified: Fri Apr 21 10:58:08 2023, max compression
```

## Comparing `pymccool-0.2.3.tar` & `pymccool-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.330292 pymccool-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.326292 pymccool-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.326292 pymccool-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 00:33:29.000000 pymccool-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 00:33:29.000000 pymccool-0.2.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 00:33:29.000000 pymccool-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 00:33:29.000000 pymccool-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-21 00:33:40.330292 pymccool-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 00:33:29.000000 pymccool-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 00:33:29.000000 pymccool-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 00:33:40.330292 pymccool-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 00:33:29.000000 pymccool-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.326292 pymccool-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.326292 pymccool-0.2.3/src/pymccool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:29.000000 pymccool-0.2.3/src/pymccool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-21 00:33:29.000000 pymccool-0.2.3/src/pymccool/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-21 00:33:29.000000 pymccool-0.2.3/src/pymccool/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.330292 pymccool-0.2.3/src/pymccool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-21 00:33:40.000000 pymccool-0.2.3/src/pymccool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-21 00:33:40.000000 pymccool-0.2.3/src/pymccool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:33:40.000000 pymccool-0.2.3/src/pymccool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 00:33:40.000000 pymccool-0.2.3/src/pymccool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 00:33:40.000000 pymccool-0.2.3/src/pymccool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:33:40.330292 pymccool-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-21 00:33:29.000000 pymccool-0.2.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 00:33:29.000000 pymccool-0.2.3/test/e2e_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-21 00:33:29.000000 pymccool-0.2.3/test/test_full_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-21 00:33:29.000000 pymccool-0.2.3/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-21 00:33:29.000000 pymccool-0.2.3/test/test_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 10:58:00.000000 pymccool-0.3.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 10:58:00.000000 pymccool-0.3.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 10:58:00.000000 pymccool-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 10:58:00.000000 pymccool-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-21 10:58:08.275955 pymccool-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 10:58:00.000000 pymccool-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 10:58:00.000000 pymccool-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 10:58:00.000000 pymccool-0.3.3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 10:58:08.275955 pymccool-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 10:58:00.000000 pymccool-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/pymccool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/pymccool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/e2e_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_full_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_tracer.py
```

### Comparing `pymccool-0.2.3/.github/workflows/tests.yaml` & `pymccool-0.3.3/.github/workflows/tests.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
       matrix:
         # Run in all these versions of Python
         python-version: ["3.10", "3.9", "3.8"]
 
     steps:
       # Checkout the latest code from the repo
       - name: Checkout Repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       # Setup which version of Python to use
       - name: Set Up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       # Display the Python version being used
       - name: Display Python Version
         run: python -c "import sys; print(sys.version)"
       # Install the package
       - name: Install Package
```

### Comparing `pymccool-0.2.3/LICENSE` & `pymccool-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/PKG-INFO` & `pymccool-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: pymccool
-Version: 0.2.3
+Version: 0.3.3
 Summary: Reusable Python Utilities by McCool
 Author-email: Brendon McCool <brendonmccool@gmail.com>
 Project-URL: Homepage, https://github.com/bmccool/pyMcCool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Installation
 - To install from commandline:
     `pip install git+https://github.com/bmccool/pymccool`
-- To isntall via requirements.txt with e.g. specific tag v0.2.0
+- To install via requirements.txt with e.g. specific tag v0.2.0
   `git+https://github.com/bmccool/pymccool@v0.2.0#egg=pymccool`
 
 # Usage
 - For basic, no-nonsense console and file logging:
-  ```
+  ```python
   from pymccool.logging import Logger
   logger = Logger(app_name="<your app name>")
   ```
 
 - For more options, use LoggerKwargs
-    ```
+    ```python
     from pymccool.logging import Logger, LoggerKwargs
     logger = Logger(
             LoggerKwargs(
                 app_name="test_logger_loki",
                 default_level=Logger.VERBOSE,
                 stream_level=Logger.VERBOSE,
                 grafana_loki_endpoint="https://loki.end.point.com/loki/api/v1/push")
     )
     ```
 
 - To use the Tracer:
-  ```
+  ```python
   from uuid import uuid1
   from pymccool.tracing import get_tracer, get_decorator
   from pymccool.logging import Logger, LoggerKwargs
   logger = Logger(
           LoggerKwargs(
               app_name="test_logger_loki",
               default_level=Logger.VERBOSE,
```

### Comparing `pymccool-0.2.3/README.md` & `pymccool-0.3.3/src/pymccool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,47 @@
+Metadata-Version: 2.1
+Name: pymccool
+Version: 0.3.3
+Summary: Reusable Python Utilities by McCool
+Author-email: Brendon McCool <brendonmccool@gmail.com>
+Project-URL: Homepage, https://github.com/bmccool/pyMcCool
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Installation
 - To install from commandline:
     `pip install git+https://github.com/bmccool/pymccool`
-- To isntall via requirements.txt with e.g. specific tag v0.2.0
+- To install via requirements.txt with e.g. specific tag v0.2.0
   `git+https://github.com/bmccool/pymccool@v0.2.0#egg=pymccool`
 
 # Usage
 - For basic, no-nonsense console and file logging:
-  ```
+  ```python
   from pymccool.logging import Logger
   logger = Logger(app_name="<your app name>")
   ```
 
 - For more options, use LoggerKwargs
-    ```
+    ```python
     from pymccool.logging import Logger, LoggerKwargs
     logger = Logger(
             LoggerKwargs(
                 app_name="test_logger_loki",
                 default_level=Logger.VERBOSE,
                 stream_level=Logger.VERBOSE,
                 grafana_loki_endpoint="https://loki.end.point.com/loki/api/v1/push")
     )
     ```
 
 - To use the Tracer:
-  ```
+  ```python
   from uuid import uuid1
   from pymccool.tracing import get_tracer, get_decorator
   from pymccool.logging import Logger, LoggerKwargs
   logger = Logger(
           LoggerKwargs(
               app_name="test_logger_loki",
               default_level=Logger.VERBOSE,
```

### Comparing `pymccool-0.2.3/pyproject.toml` & `pymccool-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymccool"
-version = "0.2.3"
+dynamic = ["version"]
 authors = [
   { name="Brendon McCool", email="brendonmccool@gmail.com" },
 ]
 description = "Reusable Python Utilities by McCool"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pymccool-0.2.3/src/pymccool/logging.py` & `pymccool-0.3.3/src/pymccool/logging.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/src/pymccool/tracing.py` & `pymccool-0.3.3/src/pymccool/tracing.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/test/conftest.py` & `pymccool-0.3.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/test/test_full_stack.py` & `pymccool-0.3.3/test/test_full_stack.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/test/test_logger.py` & `pymccool-0.3.3/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.2.3/test/test_tracer.py` & `pymccool-0.3.3/test/test_tracer.py`

 * *Files identical despite different names*

