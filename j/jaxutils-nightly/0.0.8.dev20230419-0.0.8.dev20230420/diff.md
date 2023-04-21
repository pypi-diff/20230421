# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230419.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230419.tar", last modified: Wed Apr 19 00:06:27 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230420.tar", last modified: Thu Apr 20 00:06:33 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230419.tar` & `jaxutils-nightly-0.0.8.dev20230420.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-19 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-04-19 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-19 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-04-19 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-19 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-04-19 00:06:27.047801 jaxutils-nightly-0.0.8.dev20230419/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-04-19 00:06:21.000000 jaxutils-nightly-0.0.8.dev20230419/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-20 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-04-20 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-20 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-04-20 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-20 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-04-20 00:06:33.642346 jaxutils-nightly-0.0.8.dev20230420/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-04-20 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230420/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230419/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230419
+Version: 0.0.8.dev20230420
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230419/README.md` & `jaxutils-nightly-0.0.8.dev20230420/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230420/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230419
+Version: 0.0.8.dev20230420
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230419/setup.py` & `jaxutils-nightly-0.0.8.dev20230420/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230419/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230420/versioneer.py`

 * *Files identical despite different names*

