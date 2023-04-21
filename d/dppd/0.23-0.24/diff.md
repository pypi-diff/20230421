# Comparing `tmp/dppd-0.23.tar.gz` & `tmp/dppd-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dppd-0.23.tar", last modified: Wed Jan 11 13:03:08 2023, max compression
+gzip compressed data, was "dppd-0.24.tar", last modified: Fri Apr 21 14:17:12 2023, max compression
```

## Comparing `dppd-0.23.tar` & `dppd-0.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:03:08.727392 dppd-0.23/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-11 13:03:07.000000 dppd-0.23/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-11 13:03:07.000000 dppd-0.23/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-11 13:03:08.727392 dppd-0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-01-11 13:03:07.000000 dppd-0.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-11 13:03:08.731392 dppd-0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-01-11 13:03:07.000000 dppd-0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:03:08.727392 dppd-0.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:03:08.727392 dppd-0.23/src/dppd/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-11 13:03:07.000000 dppd-0.23/src/dppd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-01-11 13:03:07.000000 dppd-0.23/src/dppd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-01-11 13:03:07.000000 dppd-0.23/src/dppd/column_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-11 13:03:07.000000 dppd-0.23/src/dppd/non_df_verbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-01-11 13:03:07.000000 dppd-0.23/src/dppd/single_verbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:03:08.727392 dppd-0.23/src/dppd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-11 13:03:08.000000 dppd-0.23/src/dppd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:17:12.968408 dppd-0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-21 14:17:11.000000 dppd-0.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-21 14:17:11.000000 dppd-0.24/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-21 14:17:12.968408 dppd-0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-21 14:17:11.000000 dppd-0.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 14:17:12.968408 dppd-0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 14:17:11.000000 dppd-0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:17:12.960408 dppd-0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:17:12.964408 dppd-0.24/src/dppd/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 14:17:11.000000 dppd-0.24/src/dppd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-21 14:17:11.000000 dppd-0.24/src/dppd/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-04-21 14:17:11.000000 dppd-0.24/src/dppd/column_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 14:17:11.000000 dppd-0.24/src/dppd/non_df_verbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-04-21 14:17:11.000000 dppd-0.24/src/dppd/single_verbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:17:12.968408 dppd-0.24/src/dppd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 14:17:12.000000 dppd-0.24/src/dppd.egg-info/top_level.txt
```

### Comparing `dppd-0.23/LICENSE.txt` & `dppd-0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dppd-0.23/PKG-INFO` & `dppd-0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dppd
-Version: 0.23
+Version: 0.24
 Summary: A pythonic dplyr clone
 Home-page: https://github.com/TyberiusPrime/dppd
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dppd-0.23/README.md` & `dppd-0.24/README.md`

 * *Files identical despite different names*

### Comparing `dppd-0.23/setup.cfg` & `dppd-0.24/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = dppd
 description = A pythonic dplyr clone
-version = 0.23
+version = 0.24
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
 license = mit
 url = https://github.com/TyberiusPrime/dppd
 long-description = file: README.md
 long_description_content_type = text/markdown
 platforms = any
@@ -32,15 +32,15 @@
 	tests
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	plotnine
-	pandas
+	pandas<2.0
 	flake8
 doc = 
 	sphinx
 	sphinx-bootstrap-theme
 	numpydoc
 	pandas
 
@@ -84,15 +84,11 @@
 	build
 	dist
 	.eggs
 	docs/conf.py
 max-line-length = 88
 ignore = E501, E713
 
-[pyscaffold]
-version = 3.1
-package = dppd
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dppd-0.23/src/dppd/base.py` & `dppd-0.24/src/dppd/base.py`

 * *Files identical despite different names*

### Comparing `dppd-0.23/src/dppd/column_spec.py` & `dppd-0.24/src/dppd/column_spec.py`

 * *Files identical despite different names*

### Comparing `dppd-0.23/src/dppd/single_verbs.py` & `dppd-0.24/src/dppd/single_verbs.py`

 * *Files identical despite different names*

### Comparing `dppd-0.23/src/dppd.egg-info/PKG-INFO` & `dppd-0.24/src/dppd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dppd
-Version: 0.23
+Version: 0.24
 Summary: A pythonic dplyr clone
 Home-page: https://github.com/TyberiusPrime/dppd
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

