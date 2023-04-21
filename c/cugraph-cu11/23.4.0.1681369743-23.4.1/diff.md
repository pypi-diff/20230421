# Comparing `tmp/cugraph_cu11-23.4.0.1681369743.tar.gz` & `tmp/cugraph_cu11-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cugraph_cu11-23.4.0.1681369743.tar", last modified: Thu Apr 13 19:12:37 2023, max compression
+gzip compressed data, was "cugraph_cu11-23.4.1.tar", last modified: Fri Apr 21 21:02:22 2023, max compression
```

## Comparing `cugraph_cu11-23.4.0.1681369743.tar` & `cugraph_cu11-23.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:12:37.547224 cugraph_cu11-23.4.0.1681369743/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:25:31.000000 cugraph_cu11-23.4.0.1681369743/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1607 2023-04-13 19:12:37.547224 cugraph_cu11-23.4.0.1681369743/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:12:37.547224 cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1607 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:12:37.000000 cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:12:37.547224 cugraph_cu11-23.4.0.1681369743/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:25:31.000000 cugraph_cu11-23.4.0.1681369743/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 02:54:55.000000 cugraph_cu11-23.4.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 02:54:55.000000 cugraph_cu11-23.4.1/setup.py
```

### Comparing `cugraph_cu11-23.4.0.1681369743/LICENSE.md` & `cugraph_cu11-23.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cugraph_cu11-23.4.0.1681369743/PKG-INFO` & `cugraph_cu11-23.4.1/cugraph_cu11.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cugraph_cu11
-Version: 23.4.0.1681369743
+Name: cugraph-cu11
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cugraph_cu11-23.4.0.1681369743/cugraph_cu11.egg-info/PKG-INFO` & `cugraph_cu11-23.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cugraph-cu11
-Version: 23.4.0.1681369743
+Name: cugraph_cu11
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cugraph_cu11-23.4.0.1681369743/setup.py` & `cugraph_cu11-23.4.1/setup.py`

 * *Files identical despite different names*

