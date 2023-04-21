# Comparing `tmp/failures-0.1.0b0.tar.gz` & `tmp/failures-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failures-0.1.0b0.tar", last modified: Sun Apr  2 12:14:50 2023, max compression
+gzip compressed data, was "failures-0.2.0.tar", last modified: Fri Apr 21 08:50:09 2023, max compression
```

## Comparing `failures-0.1.0b0.tar` & `failures-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:14:50.116320 failures-0.1.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-02 12:14:30.000000 failures-0.1.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-02 12:14:50.116320 failures-0.1.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-02 12:14:30.000000 failures-0.1.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:14:50.116320 failures-0.1.0b0/failures/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-02 12:14:30.000000 failures-0.1.0b0/failures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-02 12:14:30.000000 failures-0.1.0b0/failures/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-02 12:14:30.000000 failures-0.1.0b0/failures/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 12:14:30.000000 failures-0.1.0b0/failures/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:14:50.116320 failures-0.1.0b0/failures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-02 12:14:50.000000 failures-0.1.0b0/failures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-02 12:14:50.000000 failures-0.1.0b0/failures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 12:14:50.000000 failures-0.1.0b0/failures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-02 12:14:50.000000 failures-0.1.0b0/failures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-02 12:14:50.000000 failures-0.1.0b0/failures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-02 12:14:30.000000 failures-0.1.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 12:14:50.116320 failures-0.1.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:14:50.116320 failures-0.1.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-02 12:14:30.000000 failures-0.1.0b0/tests/test_failure_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-02 12:14:30.000000 failures-0.1.0b0/tests/test_failure_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 08:49:49.000000 failures-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-21 08:50:09.235409 failures-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-21 08:49:49.000000 failures-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-21 08:49:49.000000 failures-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 08:49:49.000000 failures-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:50:09.235409 failures-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.231409 failures-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/src/failures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/src/failures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_handler_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_print_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_scope_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_scoped_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_version_compatibility.py
```

### Comparing `failures-0.1.0b0/LICENSE` & `failures-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `failures-0.1.0b0/pyproject.toml` & `failures-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "failures"
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 description = "Labeling failures for humans"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">=3.8"
-authors = [
-    {name = "MARSO Adnan", email = "mediadnan@gmail.com"},
-]
-maintainers = [
-    {name = "MARSO Adnan", email = "mediadnan@gmail.com"},
-]
-keywords = [
-    "label",
-    "failures",
-    "handle",
-    "handling",
-    "report",
-    "track",
-]
+authors = [ {name = "MARSO Adnan", email = "mediadnan@gmail.com"} ]
+maintainers = [ {name = "MARSO Adnan", email = "mediadnan@gmail.com"} ]
+keywords = [ "label", "failures", "handle", "handling", "report", "track" ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Development Status :: 4 - Beta",
-#    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -38,25 +26,24 @@
     "Typing :: Typed"
 ]
 
 [project.urls]
 documentation = "https://failures.readthedocs.org"
 repository = "https://github.com/mediadnan/failures"
 
+[tool.setuptools]
+package-dir = {"" = "src"}
+packages = ["failures"]
+
 [tool.setuptools.dynamic]
 version = {attr = "failures.__version__"}
+dependencies = {file = "requirements.txt"}
 
 [project.optional-dependencies]
-colors = ["colorama==0.4.*"]
+colors = ["colorama>=0.4,<1.0"]
 
-[tool.setuptools]
-packages = ["failures"]
-package-data = { failures = ["py.typed"] }
+[tool.pytest.ini_options]
+pythonpath = ["src"]
+filterwarnings = ['ignore:.*will be removed in failures \d.0.*:DeprecationWarning',]
 
-[tool.black]
-line-length = 120
-target-version = [
-    'py38',
-    'py39',
-    'py310',
-    'py311'
-]
+[tool.mypy]
+implicit_optional = true
```

