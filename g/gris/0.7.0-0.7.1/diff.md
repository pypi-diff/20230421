# Comparing `tmp/gris-0.7.0.tar.gz` & `tmp/gris-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gris-0.7.0.tar", last modified: Fri Apr 21 01:13:54 2023, max compression
+gzip compressed data, was "gris-0.7.1.tar", last modified: Fri Apr 21 05:03:25 2023, max compression
```

## Comparing `gris-0.7.0.tar` & `gris-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 01:13:54.528541 gris-0.7.0/
--rw-r--r--   0 anglyan    (502) staff       (20)    18092 2023-04-21 00:57:42.000000 gris-0.7.0/LICENSE.txt
--rw-r--r--   0 anglyan    (502) staff       (20)       27 2023-04-21 00:57:42.000000 gris-0.7.0/MANIFEST.in
--rw-r--r--   0 anglyan    (502) staff       (20)     1382 2023-04-21 01:13:54.528408 gris-0.7.0/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)      648 2023-04-21 01:09:14.000000 gris-0.7.0/README.md
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 01:13:54.528251 gris-0.7.0/gris.egg-info/
--rw-r--r--   0 anglyan    (502) staff       (20)     1382 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)      169 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/SOURCES.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/dependency_links.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/top_level.txt
--rw-r--r--   0 anglyan    (502) staff       (20)      689 2023-04-21 01:06:52.000000 gris-0.7.0/pyproject.toml
--rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-21 01:13:54.528576 gris-0.7.0/setup.cfg
--rw-r--r--   0 anglyan    (502) staff       (20)     1075 2023-04-21 01:07:39.000000 gris-0.7.0/setup.py
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.976763 gris-0.7.1/
+-rw-r--r--   0 anglyan    (502) staff       (20)    18092 2023-04-21 00:57:42.000000 gris-0.7.1/LICENSE.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)       27 2023-04-21 00:57:42.000000 gris-0.7.1/MANIFEST.in
+-rw-r--r--   0 anglyan    (502) staff       (20)     1276 2023-04-21 05:03:25.976544 gris-0.7.1/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      648 2023-04-21 01:09:14.000000 gris-0.7.1/README.md
+-rw-r--r--   0 anglyan    (502) staff       (20)      689 2023-04-21 05:02:50.000000 gris-0.7.1/pyproject.toml
+-rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-21 05:03:25.976810 gris-0.7.1/setup.cfg
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.972893 gris-0.7.1/src/
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.974290 gris-0.7.1/src/gris/
+-rw-r--r--   0 anglyan    (502) staff       (20)       20 2023-04-21 01:09:48.000000 gris-0.7.1/src/gris/__init__.py
+-rw-r--r--   0 anglyan    (502) staff       (20)    10150 2023-04-21 01:09:48.000000 gris-0.7.1/src/gris/gris.py
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.975749 gris-0.7.1/src/gris.egg-info/
+-rw-r--r--   0 anglyan    (502) staff       (20)     1276 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      214 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/SOURCES.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/dependency_links.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        5 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/top_level.txt
```

### Comparing `gris-0.7.0/LICENSE.txt` & `gris-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gris-0.7.0/PKG-INFO` & `gris-0.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: gris
-Version: 0.7.0
+Version: 0.7.1
 Summary: Parser of RIS file format
-Home-page: https://github.com/anglyan/gris.git
 Author: Angel Yanguas-Gil
-Author-email: angel.yanguas@gmail.com
 Project-URL: Homepage, https://github.com/anglyan/gris.git
 Keywords: RIS file format,RefMan RIS,bibliography,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 README
 ======
 
 About gris
```

### Comparing `gris-0.7.0/README.md` & `gris-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gris-0.7.0/gris.egg-info/PKG-INFO` & `gris-0.7.1/src/gris.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: gris
-Version: 0.7.0
+Version: 0.7.1
 Summary: Parser of RIS file format
-Home-page: https://github.com/anglyan/gris.git
 Author: Angel Yanguas-Gil
-Author-email: angel.yanguas@gmail.com
 Project-URL: Homepage, https://github.com/anglyan/gris.git
 Keywords: RIS file format,RefMan RIS,bibliography,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 README
 ======
 
 About gris
```

