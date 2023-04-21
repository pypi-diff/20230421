# Comparing `tmp/commutation-0.0.6.tar.gz` & `tmp/commutation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutation-0.0.6.tar", last modified: Fri Apr 21 20:46:29 2023, max compression
+gzip compressed data, was "commutation-0.0.7.tar", last modified: Fri Apr 21 21:07:11 2023, max compression
```

## Comparing `commutation-0.0.6.tar` & `commutation-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 20:46:29.477088 commutation-0.0.6/
--rw-r--r--   0 alaricsanders   (501) staff       (20)       43 2023-04-21 19:55:14.000000 commutation-0.0.6/.gitignore
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 20:46:29.475676 commutation-0.0.6/Examples/
--rw-r--r--   0 alaricsanders   (501) staff       (20)    22896 2023-04-21 19:59:01.000000 commutation-0.0.6/Examples/Demonstrations.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/KKJ.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/Ringflip.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1937 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/Spin Algebra.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/Triangles.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/hexamer.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     8225 2023-04-21 19:16:47.000000 commutation-0.0.6/Examples/test.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.0.6/LICENSE
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 20:46:29.476919 commutation-0.0.6/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.0.6/README.md
--rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 20:46:11.000000 commutation-0.0.6/pyproject.toml
--rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 20:46:29.477127 commutation-0.0.6/setup.cfg
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 20:46:29.475827 commutation-0.0.6/src/
--rw-r--r--   0 alaricsanders   (501) staff       (20)       64 2023-04-21 19:54:11.000000 commutation-0.0.6/src/__init__.py
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 20:46:29.476217 commutation-0.0.6/src/commutation/
--rw-r--r--   0 alaricsanders   (501) staff       (20)        0 2023-04-21 19:20:41.000000 commutation-0.0.6/src/commutation/__init__.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)    27553 2023-04-21 19:16:47.000000 commutation-0.0.6/src/commutation/commutation.py
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 20:46:29.476740 commutation-0.0.6/src/commutation.egg-info/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 20:46:29.000000 commutation-0.0.6/src/commutation.egg-info/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)      443 2023-04-21 20:46:29.000000 commutation-0.0.6/src/commutation.egg-info/SOURCES.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 20:46:29.000000 commutation-0.0.6/src/commutation.egg-info/dependency_links.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)       21 2023-04-21 20:46:29.000000 commutation-0.0.6/src/commutation.egg-info/top_level.txt
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.569575 commutation-0.0.7/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       43 2023-04-21 19:55:14.000000 commutation-0.0.7/.gitignore
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.568145 commutation-0.0.7/Examples/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    22896 2023-04-21 19:59:01.000000 commutation-0.0.7/Examples/Demonstrations.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/KKJ.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Ringflip.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1937 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Spin Algebra.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Triangles.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/hexamer.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     8225 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/test.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.0.7/LICENSE
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:07:11.569339 commutation-0.0.7/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.0.7/README.md
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 21:07:01.000000 commutation-0.0.7/pyproject.toml
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 21:07:11.569619 commutation-0.0.7/setup.cfg
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.564825 commutation-0.0.7/src/
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.568541 commutation-0.0.7/src/commutation/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       63 2023-04-21 21:06:36.000000 commutation-0.0.7/src/commutation/__init__.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    27553 2023-04-21 19:16:47.000000 commutation-0.0.7/src/commutation/main.py
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.569117 commutation-0.0.7/src/commutation.egg-info/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      420 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/SOURCES.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/dependency_links.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       12 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/top_level.txt
```

### Comparing `commutation-0.0.6/Examples/Demonstrations.ipynb` & `commutation-0.0.7/Examples/Demonstrations.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/KKJ.ipynb` & `commutation-0.0.7/Examples/KKJ.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/Ringflip.ipynb` & `commutation-0.0.7/Examples/Ringflip.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/Spin Algebra.ipynb` & `commutation-0.0.7/Examples/Spin Algebra.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/Triangles.ipynb` & `commutation-0.0.7/Examples/Triangles.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/hexamer.ipynb` & `commutation-0.0.7/Examples/hexamer.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/Examples/test.ipynb` & `commutation-0.0.7/Examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/LICENSE` & `commutation-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/PKG-INFO` & `commutation-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `commutation-0.0.6/README.md` & `commutation-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/pyproject.toml` & `commutation-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "commutation"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Alaric Sanders", email="als217@cam.ac.uk" },
 ]
 description = "A library for doing noncommutative operator algebra"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commutation-0.0.6/src/commutation/commutation.py` & `commutation-0.0.7/src/commutation/main.py`

 * *Files identical despite different names*

### Comparing `commutation-0.0.6/src/commutation.egg-info/PKG-INFO` & `commutation-0.0.7/src/commutation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

