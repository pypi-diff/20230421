# Comparing `tmp/maxilearn-0.0.6.tar.gz` & `tmp/maxilearn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "maxilearn-0.0.7.tar", last modified: Fri Apr 21 15:47:25 2023, max compression
```

## Comparing `maxilearn-0.0.6.tar` & `maxilearn-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 maxilearn-0.0.6/.DS_Store
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 maxilearn-0.0.6/setup.cfg
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 maxilearn-0.0.6/update.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/__init__.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/classificators.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/data_processing.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/linear_algebra.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/metrics.py
--rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 maxilearn-0.0.6/src/maxilearn/regressors.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 maxilearn-0.0.6/LICENSE
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 maxilearn-0.0.6/README.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 maxilearn-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 maxilearn-0.0.6/PKG-INFO
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:47:25.747207 maxilearn-0.0.7/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.0.7/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      641 2023-04-21 15:47:25.746447 maxilearn-0.0.7/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.0.7/README.md
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      586 2023-04-21 15:47:07.000000 maxilearn-0.0.7/pyproject.toml
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 15:47:25.747281 maxilearn-0.0.7/setup.cfg
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:47:25.740450 maxilearn-0.0.7/src/
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:47:25.743318 maxilearn-0.0.7/src/maxilearn/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 12:46:18.000000 maxilearn-0.0.7/src/maxilearn/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    14060 2023-04-21 15:11:54.000000 maxilearn-0.0.7/src/maxilearn/classificators.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-0.0.7/src/maxilearn/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-0.0.7/src/maxilearn/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-0.0.7/src/maxilearn/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-0.0.7/src/maxilearn/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:47:25.745780 maxilearn-0.0.7/src/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      641 2023-04-21 15:47:25.000000 maxilearn-0.0.7/src/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      392 2023-04-21 15:47:25.000000 maxilearn-0.0.7/src/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 15:47:25.000000 maxilearn-0.0.7/src/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       71 2023-04-21 15:47:25.000000 maxilearn-0.0.7/src/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-21 15:47:25.000000 maxilearn-0.0.7/src/maxilearn.egg-info/top_level.txt
```

### Comparing `maxilearn-0.0.6/src/maxilearn/classificators.py` & `maxilearn-0.0.7/src/maxilearn/classificators.py`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/src/maxilearn/data_processing.py` & `maxilearn-0.0.7/src/maxilearn/data_processing.py`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/src/maxilearn/linear_algebra.py` & `maxilearn-0.0.7/src/maxilearn/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/src/maxilearn/metrics.py` & `maxilearn-0.0.7/src/maxilearn/metrics.py`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/src/maxilearn/regressors.py` & `maxilearn-0.0.7/src/maxilearn/regressors.py`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/LICENSE` & `maxilearn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `maxilearn-0.0.6/PKG-INFO` & `maxilearn-0.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 0.0.6
+Version: 0.0.7
 Summary: Machine Learning Package
 Author-email: Gleb Maksimov <glebmaksimov@gmail.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Machine Learning Package maxilearn
 
 ## About
 Cancel changes
 In this GitHub Repository, I have made many Machine learning Algorithms from scratch.
 
 You can learn what is happening Under The Hood of all these Algorithms.
 
 ## Installation
 
 ```
 pip install maxilearn
-```
+```
```

