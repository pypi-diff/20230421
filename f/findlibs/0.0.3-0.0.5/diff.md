# Comparing `tmp/findlibs-0.0.3.tar.gz` & `tmp/findlibs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlibs-0.0.3.tar", last modified: Fri Apr 21 08:32:11 2023, max compression
+gzip compressed data, was "findlibs-0.0.5.tar", last modified: Fri Apr 21 10:05:11 2023, max compression
```

## Comparing `findlibs-0.0.3.tar` & `findlibs-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 08:31:58.000000 findlibs-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 08:32:11.515379 findlibs-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-21 08:31:58.000000 findlibs-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/findlibs/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 08:31:58.000000 findlibs-0.0.3/findlibs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/findlibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:32:11.515379 findlibs-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-21 08:31:58.000000 findlibs-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:05:11.435361 findlibs-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 10:04:57.000000 findlibs-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 10:05:11.435361 findlibs-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-21 10:04:57.000000 findlibs-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:05:11.431362 findlibs-0.0.5/findlibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 10:04:57.000000 findlibs-0.0.5/findlibs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:05:11.431362 findlibs-0.0.5/findlibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 10:05:11.000000 findlibs-0.0.5/findlibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 10:05:11.000000 findlibs-0.0.5/findlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:05:11.000000 findlibs-0.0.5/findlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 10:05:11.000000 findlibs-0.0.5/findlibs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:05:11.000000 findlibs-0.0.5/findlibs.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:05:11.435361 findlibs-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-21 10:04:57.000000 findlibs-0.0.5/setup.py
```

### Comparing `findlibs-0.0.3/LICENSE` & `findlibs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findlibs-0.0.3/PKG-INFO` & `findlibs-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlibs
-Version: 0.0.3
+Version: 0.0.5
 Summary: A packages to search for shared libraries on various platforms
 Home-page: https://github.com/ecmwf/findlibs
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `findlibs-0.0.3/findlibs/__init__.py` & `findlibs-0.0.5/findlibs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # nor does it submit to any jurisdiction.
 #
 
 import ctypes.util
 import os
 import sys
 
-__version__ = "0.0.3"
+__version__ = "0.0.5"
 
 EXTENSIONS = {
     "darwin": ".dylib",
     "win32": ".dll",
 }
```

### Comparing `findlibs-0.0.3/findlibs.egg-info/PKG-INFO` & `findlibs-0.0.5/findlibs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlibs
-Version: 0.0.3
+Version: 0.0.5
 Summary: A packages to search for shared libraries on various platforms
 Home-page: https://github.com/ecmwf/findlibs
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `findlibs-0.0.3/setup.py` & `findlibs-0.0.5/setup.py`

 * *Files identical despite different names*

