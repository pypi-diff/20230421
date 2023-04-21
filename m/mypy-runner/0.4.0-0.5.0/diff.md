# Comparing `tmp/mypy-runner-0.4.0.tar.gz` & `tmp/mypy_runner-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-runner-0.4.0.tar", last modified: Sat Jan  7 01:32:44 2023, max compression
+gzip compressed data, was "mypy_runner-0.5.0.tar", max compression
```

## Comparing `mypy-runner-0.4.0.tar` & `mypy_runner-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     4122 2023-01-07 01:26:57.013408 mypy-runner-0.4.0/README.rst
--rw-r--r--   0        0        0    27383 2023-01-07 01:26:57.013363 mypy-runner-0.4.0/mypyrun.py
--rw-r--r--   0        0        0     1581 2023-01-07 01:26:57.088801 mypy-runner-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4999 2023-01-07 01:32:44.872314 mypy-runner-0.4.0/setup.py
--rw-r--r--   0        0        0     5305 2023-01-07 01:32:44.873108 mypy-runner-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4122 2023-01-07 01:26:57.013408 mypy_runner-0.5.0/README.rst
+-rw-r--r--   0        0        0    27381 2023-04-20 00:24:52.517780 mypy_runner-0.5.0/mypyrun.py
+-rw-r--r--   0        0        0     1581 2023-04-21 21:35:29.733481 mypy_runner-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5655 1970-01-01 00:00:00.000000 mypy_runner-0.5.0/PKG-INFO
```

### Comparing `mypy-runner-0.4.0/README.rst` & `mypy_runner-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mypy-runner-0.4.0/mypyrun.py` & `mypy_runner-0.5.0/mypyrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     warning_filters = None  # type: List[Pattern]
 
     # global-only options:
     args = None  # type: List[str]
     color = True
     show_ignored = False
     daemon = False
-    mypy_executable = None  # type: Optional[str]
+    mypy_executable = ''  # type: Optional[str]
     add_missing_imports = False
 
     def __init__(self):
         self.select = ALL
         self.ignore = set()
         self.warn = set()
         self.include = []
```

### Comparing `mypy-runner-0.4.0/pyproject.toml` & `mypy_runner-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mypy-runner"
-version = "0.4.0"
+version = "0.5.0"
 description = "Run mypy with options to filter errors and colorize output"
 authors = ["Chad Dombrova <chadrik@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/chadrik/mypy-runner"
 packages = [
     { include = "mypyrun.py" },
```

### Comparing `mypy-runner-0.4.0/PKG-INFO` & `mypy_runner-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-runner
-Version: 0.4.0
+Version: 0.5.0
 Summary: Run mypy with options to filter errors and colorize output
 Home-page: https://github.com/chadrik/mypy-runner
 License: MIT
 Keywords: pep484,typing,annotations,mypy
 Author: Chad Dombrova
 Author-email: chadrik@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: tests
 Requires-Dist: configparser
-Requires-Dist: coverage; extra == "tests"
-Requires-Dist: pytest (>=6.1,<7.0); extra == "tests"
+Requires-Dist: coverage ; extra == "tests"
+Requires-Dist: pytest (>=6.1,<7.0) ; extra == "tests"
 Project-URL: Repository, https://github.com/chadrik/mypy-runner
 Description-Content-Type: text/x-rst
 
 mypy-runner
 ===========
 
 Ease your way into static type checking by focusing on a small set of problems at a time.
```

