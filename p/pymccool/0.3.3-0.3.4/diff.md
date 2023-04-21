# Comparing `tmp/pymccool-0.3.3.tar.gz` & `tmp/pymccool-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymccool-0.3.3.tar", last modified: Fri Apr 21 10:58:08 2023, max compression
+gzip compressed data, was "pymccool-0.3.4.tar", last modified: Fri Apr 21 11:05:29 2023, max compression
```

## Comparing `pymccool-0.3.3.tar` & `pymccool-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 10:58:00.000000 pymccool-0.3.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 10:58:00.000000 pymccool-0.3.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 10:58:00.000000 pymccool-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 10:58:00.000000 pymccool-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-21 10:58:08.275955 pymccool-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 10:58:00.000000 pymccool-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 10:58:00.000000 pymccool-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 10:58:00.000000 pymccool-0.3.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 10:58:08.275955 pymccool-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 10:58:00.000000 pymccool-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/pymccool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-21 10:58:00.000000 pymccool-0.3.3/src/pymccool/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/src/pymccool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 10:58:08.000000 pymccool-0.3.3/src/pymccool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:08.275955 pymccool-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/e2e_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_full_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-21 10:58:00.000000 pymccool-0.3.3/test/test_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.975390 pymccool-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.971389 pymccool-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.971389 pymccool-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 11:05:19.000000 pymccool-0.3.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-21 11:05:19.000000 pymccool-0.3.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 11:05:19.000000 pymccool-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 11:05:19.000000 pymccool-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-21 11:05:29.975390 pymccool-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-21 11:05:19.000000 pymccool-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 11:05:19.000000 pymccool-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 11:05:19.000000 pymccool-0.3.4/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 11:05:29.975390 pymccool-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 11:05:19.000000 pymccool-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.971389 pymccool-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.975390 pymccool-0.3.4/src/pymccool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:19.000000 pymccool-0.3.4/src/pymccool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-21 11:05:19.000000 pymccool-0.3.4/src/pymccool/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-21 11:05:19.000000 pymccool-0.3.4/src/pymccool/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.975390 pymccool-0.3.4/src/pymccool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-21 11:05:29.000000 pymccool-0.3.4/src/pymccool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 11:05:29.000000 pymccool-0.3.4/src/pymccool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:05:29.000000 pymccool-0.3.4/src/pymccool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 11:05:29.000000 pymccool-0.3.4/src/pymccool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 11:05:29.000000 pymccool-0.3.4/src/pymccool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:05:29.975390 pymccool-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-21 11:05:19.000000 pymccool-0.3.4/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 11:05:19.000000 pymccool-0.3.4/test/e2e_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-21 11:05:19.000000 pymccool-0.3.4/test/test_full_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-21 11:05:19.000000 pymccool-0.3.4/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-21 11:05:19.000000 pymccool-0.3.4/test/test_tracer.py
```

### Comparing `pymccool-0.3.3/.github/workflows/tests.yaml` & `pymccool-0.3.4/.github/workflows/tests.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         # Run in all these versions of Python
-        python-version: ["3.10", "3.9", "3.8"]
+        python-version: ["3.11", "3.10", "3.9", "3.8"]
 
     steps:
       # Checkout the latest code from the repo
       - name: Checkout Repo
         uses: actions/checkout@v3
       # Setup which version of Python to use
       - name: Set Up Python ${{ matrix.python-version }}
```

### Comparing `pymccool-0.3.3/LICENSE` & `pymccool-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/PKG-INFO` & `pymccool-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pymccool
-Version: 0.3.3
+Version: 0.3.4
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
-- To install from commandline:
-    `pip install git+https://github.com/bmccool/pymccool`
-- To install via requirements.txt with e.g. specific tag v0.2.0
-  `git+https://github.com/bmccool/pymccool@v0.2.0#egg=pymccool`
+  - `pip install pymccool`
 
 # Usage
 - For basic, no-nonsense console and file logging:
   ```python
   from pymccool.logging import Logger
   logger = Logger(app_name="<your app name>")
   ```
```

### Comparing `pymccool-0.3.3/README.md` & `pymccool-0.3.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # Installation
-- To install from commandline:
-    `pip install git+https://github.com/bmccool/pymccool`
-- To install via requirements.txt with e.g. specific tag v0.2.0
-  `git+https://github.com/bmccool/pymccool@v0.2.0#egg=pymccool`
+  - `pip install pymccool`
 
 # Usage
 - For basic, no-nonsense console and file logging:
   ```python
   from pymccool.logging import Logger
   logger = Logger(app_name="<your app name>")
   ```
```

### Comparing `pymccool-0.3.3/pyproject.toml` & `pymccool-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/src/pymccool/logging.py` & `pymccool-0.3.4/src/pymccool/logging.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/src/pymccool/tracing.py` & `pymccool-0.3.4/src/pymccool/tracing.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/src/pymccool.egg-info/PKG-INFO` & `pymccool-0.3.4/src/pymccool.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pymccool
-Version: 0.3.3
+Version: 0.3.4
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
-- To install from commandline:
-    `pip install git+https://github.com/bmccool/pymccool`
-- To install via requirements.txt with e.g. specific tag v0.2.0
-  `git+https://github.com/bmccool/pymccool@v0.2.0#egg=pymccool`
+  - `pip install pymccool`
 
 # Usage
 - For basic, no-nonsense console and file logging:
   ```python
   from pymccool.logging import Logger
   logger = Logger(app_name="<your app name>")
   ```
```

### Comparing `pymccool-0.3.3/test/conftest.py` & `pymccool-0.3.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/test/test_full_stack.py` & `pymccool-0.3.4/test/test_full_stack.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/test/test_logger.py` & `pymccool-0.3.4/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `pymccool-0.3.3/test/test_tracer.py` & `pymccool-0.3.4/test/test_tracer.py`

 * *Files identical despite different names*

