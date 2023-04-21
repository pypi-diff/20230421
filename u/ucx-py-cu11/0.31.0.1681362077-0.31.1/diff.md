# Comparing `tmp/ucx_py_cu11-0.31.0.1681362077.tar.gz` & `tmp/ucx_py_cu11-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucx_py_cu11-0.31.0.1681362077.tar", last modified: Thu Apr 13 19:15:14 2023, max compression
+gzip compressed data, was "ucx_py_cu11-0.31.1.tar", last modified: Fri Apr 21 21:01:43 2023, max compression
```

## Comparing `ucx_py_cu11-0.31.0.1681362077.tar` & `ucx_py_cu11-0.31.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:15:14.004041 ucx_py_cu11-0.31.0.1681362077/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      443 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:15:03.000000 ucx_py_cu11-0.31.0.1681362077/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1603 2023-04-13 19:15:14.002041 ucx_py_cu11-0.31.0.1681362077/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:15:14.004041 ucx_py_cu11-0.31.0.1681362077/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:15:03.000000 ucx_py_cu11-0.31.0.1681362077/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:15:14.002041 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1603 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      443 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 03:15:24.000000 ucx_py_cu11-0.31.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 03:15:24.000000 ucx_py_cu11-0.31.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/top_level.txt
```

### Comparing `ucx_py_cu11-0.31.0.1681362077/LICENSE.md` & `ucx_py_cu11-0.31.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.31.0.1681362077/PKG-INFO` & `ucx_py_cu11-0.31.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucx_py_cu11
-Version: 0.31.0.1681362077
+Version: 0.31.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `ucx_py_cu11-0.31.0.1681362077/setup.py` & `ucx_py_cu11-0.31.1/setup.py`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/PKG-INFO` & `ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucx-py-cu11
-Version: 0.31.0.1681362077
+Version: 0.31.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

