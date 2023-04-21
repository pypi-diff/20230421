# Comparing `tmp/commutation-0.0.2.tar.gz` & `tmp/commutation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutation-0.0.2.tar", last modified: Fri Apr 21 19:40:22 2023, max compression
+gzip compressed data, was "commutation-0.0.3.tar", last modified: Fri Apr 21 19:56:00 2023, max compression
```

## Comparing `commutation-0.0.2.tar` & `commutation-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:40:22.258373 commutation-0.0.2/
--rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.0.2/LICENSE
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 19:40:22.258236 commutation-0.0.2/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.0.2/README.md
--rw-r--r--   0 alaricsanders   (501) staff       (20)      624 2023-04-21 19:40:02.000000 commutation-0.0.2/pyproject.toml
--rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 19:40:22.258412 commutation-0.0.2/setup.cfg
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:40:22.256242 commutation-0.0.2/src/
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:40:22.257575 commutation-0.0.2/src/commutation.egg-info/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 19:40:22.000000 commutation-0.0.2/src/commutation.egg-info/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)      271 2023-04-21 19:40:22.000000 commutation-0.0.2/src/commutation.egg-info/SOURCES.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 19:40:22.000000 commutation-0.0.2/src/commutation.egg-info/dependency_links.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)       24 2023-04-21 19:40:22.000000 commutation-0.0.2/src/commutation.egg-info/top_level.txt
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:40:22.257775 commutation-0.0.2/src/commutation_Spuriosity1/
--rw-r--r--   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:20:41.000000 commutation-0.0.2/src/commutation_Spuriosity1/__init__.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)    27553 2023-04-21 19:16:47.000000 commutation-0.0.2/src/commutation_Spuriosity1/commutation.py
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:56:00.891597 commutation-0.0.3/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.0.3/LICENSE
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 19:56:00.891483 commutation-0.0.3/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.0.3/README.md
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      624 2023-04-21 19:55:50.000000 commutation-0.0.3/pyproject.toml
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 19:56:00.891633 commutation-0.0.3/setup.cfg
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:56:00.890116 commutation-0.0.3/src/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       64 2023-04-21 19:54:11.000000 commutation-0.0.3/src/__init__.py
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:56:00.890853 commutation-0.0.3/src/commutation.egg-info/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 19:56:00.000000 commutation-0.0.3/src/commutation.egg-info/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      287 2023-04-21 19:56:00.000000 commutation-0.0.3/src/commutation.egg-info/SOURCES.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 19:56:00.000000 commutation-0.0.3/src/commutation.egg-info/dependency_links.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       33 2023-04-21 19:56:00.000000 commutation-0.0.3/src/commutation.egg-info/top_level.txt
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:56:00.891061 commutation-0.0.3/src/commutation_Spuriosity1/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:20:41.000000 commutation-0.0.3/src/commutation_Spuriosity1/__init__.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    27553 2023-04-21 19:16:47.000000 commutation-0.0.3/src/commutation_Spuriosity1/commutation.py
```

### Comparing `commutation-0.0.2/LICENSE` & `commutation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commutation-0.0.2/PKG-INFO` & `commutation-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `commutation-0.0.2/README.md` & `commutation-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `commutation-0.0.2/pyproject.toml` & `commutation-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commutation"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alaric Sanders", email="als217@cam.ac.uk" },
 ]
 description = "A library for doing noncommutative operator algebra"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commutation-0.0.2/src/commutation.egg-info/PKG-INFO` & `commutation-0.0.3/src/commutation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `commutation-0.0.2/src/commutation_Spuriosity1/commutation.py` & `commutation-0.0.3/src/commutation_Spuriosity1/commutation.py`

 * *Files identical despite different names*

