# Comparing `tmp/gspWeb-0.0.7.tar.gz` & `tmp/gspWeb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspWeb-0.0.7.tar", last modified: Fri Apr 21 08:14:36 2023, max compression
+gzip compressed data, was "gspWeb-0.0.8.tar", last modified: Fri Apr 21 08:24:11 2023, max compression
```

## Comparing `gspWeb-0.0.7.tar` & `gspWeb-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:14:36.424033 gspWeb-0.0.7/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1075 2023-04-02 14:08:08.000000 gspWeb-0.0.7/LICENSE.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      642 2023-04-21 08:14:36.423854 gspWeb-0.0.7/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      420 2023-04-02 14:26:03.000000 gspWeb-0.0.7/README.rst
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 08:14:36.424319 gspWeb-0.0.7/setup.cfg
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1085 2023-04-21 08:12:18.000000 gspWeb-0.0.7/setup.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:14:36.420767 gspWeb-0.0.7/src/
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:14:36.421835 gspWeb-0.0.7/src/gspWeb/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 gspWeb-0.0.7/src/gspWeb/__init__.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:14:36.423584 gspWeb-0.0.7/src/gspWeb/econometrics/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 gspWeb-0.0.7/src/gspWeb/econometrics/__init__.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16158 2023-04-21 08:12:01.000000 gspWeb-0.0.7/src/gspWeb/econometrics/olsModel.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:14:36.423168 gspWeb-0.0.7/src/gspWeb.egg-info/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      642 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      328 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/SOURCES.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/dependency_links.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/not-zip-safe
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       73 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/requires.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        7 2023-04-21 08:14:36.000000 gspWeb-0.0.7/src/gspWeb.egg-info/top_level.txt
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:24:11.594163 gspWeb-0.0.8/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1075 2023-04-02 14:08:08.000000 gspWeb-0.0.8/LICENSE.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      642 2023-04-21 08:24:11.593960 gspWeb-0.0.8/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      420 2023-04-02 14:26:03.000000 gspWeb-0.0.8/README.rst
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 08:24:11.594241 gspWeb-0.0.8/setup.cfg
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1085 2023-04-21 08:23:37.000000 gspWeb-0.0.8/setup.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:24:11.590892 gspWeb-0.0.8/src/
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:24:11.591827 gspWeb-0.0.8/src/gspWeb/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 gspWeb-0.0.8/src/gspWeb/__init__.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:24:11.593643 gspWeb-0.0.8/src/gspWeb/econometrics/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 gspWeb-0.0.8/src/gspWeb/econometrics/__init__.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16158 2023-04-21 08:18:22.000000 gspWeb-0.0.8/src/gspWeb/econometrics/olsModel.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:24:11.593180 gspWeb-0.0.8/src/gspWeb.egg-info/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      642 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      328 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/not-zip-safe
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       73 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/requires.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        7 2023-04-21 08:24:11.000000 gspWeb-0.0.8/src/gspWeb.egg-info/top_level.txt
```

### Comparing `gspWeb-0.0.7/LICENSE.txt` & `gspWeb-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gspWeb-0.0.7/PKG-INFO` & `gspWeb-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspWeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fitting ols model in python
 Home-page: 
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `gspWeb-0.0.7/setup.py` & `gspWeb-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path, "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gspWeb',
 
-    version='0.0.7',
+    version='0.0.8',
 
     description='Fitting ols model in python',
 
     packages=['gspWeb', 'gspWeb.econometrics'],
 
     # directory in which code file is stored
     package_dir={'':'src'},
```

### Comparing `gspWeb-0.0.7/src/gspWeb/econometrics/olsModel.py` & `gspWeb-0.0.8/src/gspWeb/econometrics/olsModel.py`

 * *Files identical despite different names*

### Comparing `gspWeb-0.0.7/src/gspWeb.egg-info/PKG-INFO` & `gspWeb-0.0.8/src/gspWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspWeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fitting ols model in python
 Home-page: 
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

