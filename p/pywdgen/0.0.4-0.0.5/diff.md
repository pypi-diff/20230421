# Comparing `tmp/pywdgen-0.0.4.tar.gz` & `tmp/pywdgen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywdgen-0.0.4.tar", last modified: Thu Apr 20 17:42:44 2023, max compression
+gzip compressed data, was "pywdgen-0.0.5.tar", last modified: Fri Apr 21 11:40:13 2023, max compression
```

## Comparing `pywdgen-0.0.4.tar` & `pywdgen-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-20 17:42:44.688459 pywdgen-0.0.4/
--rw-r--r--   0 hugo       (501) staff       (20)     1070 2023-04-20 15:36:57.000000 pywdgen-0.0.4/LICENSE
--rw-r--r--   0 hugo       (501) staff       (20)      567 2023-04-20 17:42:44.688259 pywdgen-0.0.4/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)       22 2023-04-06 21:26:13.000000 pywdgen-0.0.4/README.md
--rw-r--r--   0 hugo       (501) staff       (20)      684 2023-04-20 17:42:38.000000 pywdgen-0.0.4/pyproject.toml
--rw-r--r--   0 hugo       (501) staff       (20)       38 2023-04-20 17:42:44.688496 pywdgen-0.0.4/setup.cfg
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-20 17:42:44.681805 pywdgen-0.0.4/src/
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-20 17:42:44.685807 pywdgen-0.0.4/src/pywdgen/
--rw-r--r--   0 hugo       (501) staff       (20)        0 2023-04-20 17:41:07.000000 pywdgen-0.0.4/src/pywdgen/__init__.py
--rw-r--r--   0 hugo       (501) staff       (20)      421 2023-04-20 15:44:29.000000 pywdgen-0.0.4/src/pywdgen/checker.py
--rw-r--r--   0 hugo       (501) staff       (20)        0 2023-04-20 15:28:21.000000 pywdgen-0.0.4/src/pywdgen/config.py
--rw-r--r--   0 hugo       (501) staff       (20)      714 2023-04-20 15:44:29.000000 pywdgen-0.0.4/src/pywdgen/eval.py
--rwxr-xr-x   0 hugo       (501) staff       (20)     2117 2023-04-20 15:51:45.000000 pywdgen-0.0.4/src/pywdgen/generator.py
--rw-r--r--   0 hugo       (501) staff       (20)      185 2023-04-20 15:44:29.000000 pywdgen-0.0.4/src/pywdgen/hasher.py
--rw-r--r--   0 hugo       (501) staff       (20)     1693 2023-04-20 17:14:34.000000 pywdgen-0.0.4/src/pywdgen/main.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-20 17:42:44.687894 pywdgen-0.0.4/src/pywdgen.egg-info/
--rw-r--r--   0 hugo       (501) staff       (20)      567 2023-04-20 17:42:44.000000 pywdgen-0.0.4/src/pywdgen.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)      366 2023-04-20 17:42:44.000000 pywdgen-0.0.4/src/pywdgen.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (501) staff       (20)        1 2023-04-20 17:42:44.000000 pywdgen-0.0.4/src/pywdgen.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (501) staff       (20)       41 2023-04-20 17:42:44.000000 pywdgen-0.0.4/src/pywdgen.egg-info/entry_points.txt
--rw-r--r--   0 hugo       (501) staff       (20)        8 2023-04-20 17:42:44.000000 pywdgen-0.0.4/src/pywdgen.egg-info/top_level.txt
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-21 11:40:13.424240 pywdgen-0.0.5/
+-rw-r--r--   0 hugo       (501) staff       (20)     1070 2023-04-20 15:36:57.000000 pywdgen-0.0.5/LICENSE
+-rw-r--r--   0 hugo       (501) staff       (20)      567 2023-04-21 11:40:13.423973 pywdgen-0.0.5/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)       22 2023-04-06 21:26:13.000000 pywdgen-0.0.5/README.md
+-rw-r--r--   0 hugo       (501) staff       (20)      684 2023-04-21 11:39:59.000000 pywdgen-0.0.5/pyproject.toml
+-rw-r--r--   0 hugo       (501) staff       (20)       38 2023-04-21 11:40:13.424287 pywdgen-0.0.5/setup.cfg
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-21 11:40:13.417388 pywdgen-0.0.5/src/
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-21 11:40:13.421672 pywdgen-0.0.5/src/pywdgen/
+-rw-r--r--   0 hugo       (501) staff       (20)        0 2023-04-20 17:49:14.000000 pywdgen-0.0.5/src/pywdgen/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)      421 2023-04-20 15:44:29.000000 pywdgen-0.0.5/src/pywdgen/checker.py
+-rw-r--r--   0 hugo       (501) staff       (20)      714 2023-04-20 15:44:29.000000 pywdgen-0.0.5/src/pywdgen/eval.py
+-rwxr-xr-x   0 hugo       (501) staff       (20)     2117 2023-04-20 15:51:45.000000 pywdgen-0.0.5/src/pywdgen/generator.py
+-rw-r--r--   0 hugo       (501) staff       (20)      185 2023-04-20 15:44:29.000000 pywdgen-0.0.5/src/pywdgen/hasher.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1693 2023-04-20 17:49:52.000000 pywdgen-0.0.5/src/pywdgen/main.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-04-21 11:40:13.423591 pywdgen-0.0.5/src/pywdgen.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)      567 2023-04-21 11:40:13.000000 pywdgen-0.0.5/src/pywdgen.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      344 2023-04-21 11:40:13.000000 pywdgen-0.0.5/src/pywdgen.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2023-04-21 11:40:13.000000 pywdgen-0.0.5/src/pywdgen.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       41 2023-04-21 11:40:13.000000 pywdgen-0.0.5/src/pywdgen.egg-info/entry_points.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        8 2023-04-21 11:40:13.000000 pywdgen-0.0.5/src/pywdgen.egg-info/top_level.txt
```

### Comparing `pywdgen-0.0.4/LICENSE` & `pywdgen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pywdgen-0.0.4/PKG-INFO` & `pywdgen-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywdgen
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that allows you to generate passwords and check their security
 Author-email: Hugo Camerola <hugo.camerola@example.com>
 Project-URL: Homepage, https://github.com/Zey120/pywdgen
 Project-URL: Bug Tracker, https://github.com/Zey120/pywdgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywdgen-0.0.4/pyproject.toml` & `pywdgen-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pycryptodome>=3.17"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pywdgen"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Hugo Camerola", email="hugo.camerola@example.com" },
 ]
 description = "A package that allows you to generate passwords and check their security"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywdgen-0.0.4/src/pywdgen/eval.py` & `pywdgen-0.0.5/src/pywdgen/eval.py`

 * *Files identical despite different names*

### Comparing `pywdgen-0.0.4/src/pywdgen/generator.py` & `pywdgen-0.0.5/src/pywdgen/generator.py`

 * *Files identical despite different names*

### Comparing `pywdgen-0.0.4/src/pywdgen/main.py` & `pywdgen-0.0.5/src/pywdgen/main.py`

 * *Files identical despite different names*

### Comparing `pywdgen-0.0.4/src/pywdgen.egg-info/PKG-INFO` & `pywdgen-0.0.5/src/pywdgen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywdgen
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that allows you to generate passwords and check their security
 Author-email: Hugo Camerola <hugo.camerola@example.com>
 Project-URL: Homepage, https://github.com/Zey120/pywdgen
 Project-URL: Bug Tracker, https://github.com/Zey120/pywdgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

