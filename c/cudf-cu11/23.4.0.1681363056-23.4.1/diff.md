# Comparing `tmp/cudf_cu11-23.4.0.1681363056.tar.gz` & `tmp/cudf_cu11-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudf_cu11-23.4.0.1681363056.tar", last modified: Thu Apr 13 19:10:44 2023, max compression
+gzip compressed data, was "cudf_cu11-23.4.1.tar", last modified: Fri Apr 21 21:03:00 2023, max compression
```

## Comparing `cudf_cu11-23.4.0.1681363056.tar` & `cudf_cu11-23.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 14:11:27.000000 cudf_cu11-23.4.0.1681363056/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 14:11:27.000000 cudf_cu11-23.4.0.1681363056/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:03:00.900260 cudf_cu11-23.4.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 02:54:55.000000 cudf_cu11-23.4.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-04-21 21:03:00.896260 cudf_cu11-23.4.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:03:00.896260 cudf_cu11-23.4.1/cudf_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/cudf_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/cudf_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/cudf_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:03:00.000000 cudf_cu11-23.4.1/cudf_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:03:00.900260 cudf_cu11-23.4.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 02:54:55.000000 cudf_cu11-23.4.1/setup.py
```

### Comparing `cudf_cu11-23.4.0.1681363056/LICENSE.md` & `cudf_cu11-23.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cudf_cu11-23.4.0.1681363056/PKG-INFO` & `cudf_cu11-23.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf_cu11
-Version: 23.4.0.1681363056
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/PKG-INFO` & `cudf_cu11-23.4.1/cudf_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf-cu11
-Version: 23.4.0.1681363056
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf_cu11-23.4.0.1681363056/setup.py` & `cudf_cu11-23.4.1/setup.py`

 * *Files identical despite different names*

