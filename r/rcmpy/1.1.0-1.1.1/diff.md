# Comparing `tmp/rcmpy-1.1.0.tar.gz` & `tmp/rcmpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.1.0.tar", last modified: Thu Apr 20 07:35:17 2023, max compression
+gzip compressed data, was "rcmpy-1.1.1.tar", last modified: Fri Apr 21 01:18:13 2023, max compression
```

## Comparing `rcmpy-1.1.0.tar` & `rcmpy-1.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.429541 rcmpy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 07:34:06.000000 rcmpy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-20 07:35:17.425541 rcmpy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-20 07:34:06.000000 rcmpy-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 07:34:06.000000 rcmpy-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.421541 rcmpy-1.1.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:35:17.429541 rcmpy-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 07:34:06.000000 rcmpy-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 01:17:09.000000 rcmpy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-21 01:18:13.222054 rcmpy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-21 01:17:09.000000 rcmpy-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 01:17:09.000000 rcmpy-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 01:18:13.222054 rcmpy-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 01:17:09.000000 rcmpy-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_xdg.py
```

### Comparing `rcmpy-1.1.0/LICENSE` & `rcmpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/PKG-INFO` & `rcmpy-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d6cd0e307dd25044b7eb3a7adaf13b33
+    hash=e17a2a1feecf3316dd227e4ef69c4351
     =====================================
 -->
 
-# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.0/README.md` & `rcmpy-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d6cd0e307dd25044b7eb3a7adaf13b33
+    hash=e17a2a1feecf3316dd227e4ef69c4351
     =====================================
 -->
 
-# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.0/pyproject.toml` & `rcmpy-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.1.0"
+version = "1.1.1"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.1.0/rcmpy/app.py` & `rcmpy-1.1.1/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/commands/all.py` & `rcmpy-1.1.1/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/commands/apply.py` & `rcmpy-1.1.1/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/commands/use.py` & `rcmpy-1.1.1/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/commands/variant.py` & `rcmpy-1.1.1/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/commands/watch.py` & `rcmpy-1.1.1/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/config/__init__.py` & `rcmpy-1.1.1/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/config/file.py` & `rcmpy-1.1.1/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/entry.py` & `rcmpy-1.1.1/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/environment/__init__.py` & `rcmpy-1.1.1/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/environment/base.py` & `rcmpy-1.1.1/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/environment/template.py` & `rcmpy-1.1.1/rcmpy/environment/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,18 @@
 
     def _init_templates(self, template_names: Set[str]) -> bool:
         """
         Initialize the template environment based on a set of template names
         that may be relevant to some task.
         """
 
-        candidates = self.state.root_directories("templates")
+        # The variant's template directory takes precedence.
+        candidates = self.state.root_directories(
+            "templates", common_first=False
+        )
 
         # Prefer variant templates, if the variant template-directory
         # exists.
         self.jinja = environment(
             loader=FileSystemLoader(candidates, followlinks=True)
         )
```

### Comparing `rcmpy-1.1.0/rcmpy/paths/__init__.py` & `rcmpy-1.1.1/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/schemas.py` & `rcmpy-1.1.1/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy/state/__init__.py` & `rcmpy-1.1.1/rcmpy/state/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,25 +82,30 @@
         )
 
     def update_manifest(self, data: Dict[str, Any]) -> None:
         """Set new manifest data."""
         self.manifest_new = self.manifest != data
         self.manifest = data
 
-    def root_directories(self, subdir: str) -> List[Path]:
+    def root_directories(
+        self, subdir: str, common_first: bool = True
+    ) -> List[Path]:
         """
         Get up to a pair of directories from some sub-directory of the current
         root.
         """
 
         root = self.directory.joinpath(subdir)
 
         candidates = [root.joinpath("common")]
         if self.variant:
-            candidates.insert(0, root.joinpath(self.variant))
+            if common_first:
+                candidates.append(root.joinpath(self.variant))
+            else:
+                candidates.insert(0, root.joinpath(self.variant))
 
         return [x for x in candidates if x.is_dir()]
 
     def _load_configs(self) -> None:
         """Load data for configs."""
 
         with ExitStack() as stack:
@@ -120,14 +125,15 @@
                         logger=self.logger,
                         require_success=True,
                         recurse=True,
                         includes_key="includes",
                         expect_overwrite=True,
                         preprocessor=preprocessor,
                     ).data,
+                    expect_overwrite=True,
                     logger=self.logger,
                 )
 
         self.configs_new = self.configs != self.previous["configs"]
         self.previous["configs"] = self.configs
 
         if self.configs_new:
@@ -143,14 +149,15 @@
                     path,
                     logger=self.logger,
                     require_success=True,
                     recurse=True,
                     includes_key="includes",
                     expect_overwrite=True,
                 ).data,
+                expect_overwrite=True,
                 logger=self.logger,
             )
 
         self.variables_new = self.variables != self.previous["variables"]
         self.previous["variables"] = self.variables
 
         if self.variables_new:
```

### Comparing `rcmpy-1.1.0/rcmpy/xdg/__init__.py` & `rcmpy-1.1.1/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.1.1/rcmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d6cd0e307dd25044b7eb3a7adaf13b33
+    hash=e17a2a1feecf3316dd227e4ef69c4351
     =====================================
 -->
 
-# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.1.1/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/setup.py` & `rcmpy-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.0/tests/test_entry.py` & `rcmpy-1.1.1/tests/test_entry.py`

 * *Files identical despite different names*

