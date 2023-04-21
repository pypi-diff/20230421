# Comparing `tmp/cumulus_process-1.1.0.tar.gz` & `tmp/cumulus_process-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cumulus_process-1.1.0.tar", last modified: Fri Feb 10 16:46:50 2023, max compression
+gzip compressed data, was "dist/cumulus_process-1.2.0.tar", last modified: Fri Apr 21 15:10:34 2023, max compression
```

## Comparing `cumulus_process-1.1.0.tar` & `cumulus_process-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3337 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/handlers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2136 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/loggers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12371 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/process.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3500 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/cumulus_process/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      590 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/cumulus_process.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/example/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/example/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2862 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/example/main.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2441 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/test/test_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2873 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/test/test_example.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/test/test_loggers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4685 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/test/test_process.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3029 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/test/test_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1335 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2023-02-10 16:45:52.000000 cumulus_process-1.1.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-10 16:46:49.000000 cumulus_process-1.1.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1335 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/cumulus_process/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3337 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/handlers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2136 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/helpers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/loggers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12371 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/process.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3500 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/cumulus_process/version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/cumulus_process.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2023-04-21 15:10:34.000000 cumulus_process-1.2.0/cumulus_process.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2023-04-21 15:10:34.000000 cumulus_process-1.2.0/cumulus_process.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-21 15:10:34.000000 cumulus_process-1.2.0/cumulus_process.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-04-21 15:10:34.000000 cumulus_process-1.2.0/cumulus_process.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-04-21 15:10:34.000000 cumulus_process-1.2.0/cumulus_process.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/example/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/example/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2862 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/example/main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-21 15:10:34.289893 cumulus_process-1.2.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2441 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/test/test_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2873 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/test/test_example.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/test/test_loggers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4685 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/test/test_process.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3029 2023-04-21 15:09:38.000000 cumulus_process-1.2.0/test/test_s3.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cumulus_process-1.1.0/cumulus_process/cli.py` & `cumulus_process-1.2.0/cumulus_process/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process/handlers.py` & `cumulus_process-1.2.0/cumulus_process/handlers.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process/helpers.py` & `cumulus_process-1.2.0/cumulus_process/helpers.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process/loggers.py` & `cumulus_process-1.2.0/cumulus_process/loggers.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process/process.py` & `cumulus_process-1.2.0/cumulus_process/process.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process/s3.py` & `cumulus_process-1.2.0/cumulus_process/s3.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/cumulus_process.egg-info/PKG-INFO` & `cumulus_process-1.2.0/cumulus_process.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: cumulus-process
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for creating Cumulus Process tasks in Python
 Home-page: https://github.com/nasa-cumulus/cumulus-process-py
 Author: Matthew Hanson (matthewhanson), Alireza J (scisco)
+Author-email: UNKNOWN
 License: Apache 2.0
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cumulus_process-1.1.0/cumulus_process.egg-info/SOURCES.txt` & `cumulus_process-1.2.0/cumulus_process.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 cumulus_process/__init__.py
 cumulus_process/cli.py
 cumulus_process/handlers.py
```

### Comparing `cumulus_process-1.1.0/example/main.py` & `cumulus_process-1.2.0/example/main.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/test/test_cli.py` & `cumulus_process-1.2.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/test/test_example.py` & `cumulus_process-1.2.0/test/test_example.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/test/test_loggers.py` & `cumulus_process-1.2.0/test/test_loggers.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/test/test_process.py` & `cumulus_process-1.2.0/test/test_process.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/test/test_s3.py` & `cumulus_process-1.2.0/test/test_s3.py`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/README.md` & `cumulus_process-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_process-1.1.0/setup.py` & `cumulus_process-1.2.0/setup.py`

 * *Files identical despite different names*

