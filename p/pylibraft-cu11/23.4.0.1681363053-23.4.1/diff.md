# Comparing `tmp/pylibraft_cu11-23.4.0.1681363053.tar.gz` & `tmp/pylibraft_cu11-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibraft_cu11-23.4.0.1681363053.tar", last modified: Thu Apr 13 18:23:03 2023, max compression
+gzip compressed data, was "pylibraft_cu11-23.4.1.tar", last modified: Fri Apr 21 19:02:13 2023, max compression
```

## Comparing `pylibraft_cu11-23.4.0.1681363053.tar` & `pylibraft_cu11-23.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:23:03.951620 pylibraft_cu11-23.4.0.1681363053/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:16:23.000000 pylibraft_cu11-23.4.0.1681363053/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 18:23:03.951620 pylibraft_cu11-23.4.0.1681363053/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:23:03.950620 pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:23:03.000000 pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 18:23:03.951620 pylibraft_cu11-23.4.0.1681363053/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:16:23.000000 pylibraft_cu11-23.4.0.1681363053/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:02:13.535813 pylibraft_cu11-23.4.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:16:23.000000 pylibraft_cu11-23.4.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-21 19:02:13.535813 pylibraft_cu11-23.4.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:02:13.534813 pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:02:13.000000 pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 19:02:13.535813 pylibraft_cu11-23.4.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:16:23.000000 pylibraft_cu11-23.4.1/setup.py
```

### Comparing `pylibraft_cu11-23.4.0.1681363053/LICENSE.md` & `pylibraft_cu11-23.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylibraft_cu11-23.4.0.1681363053/PKG-INFO` & `pylibraft_cu11-23.4.1/pylibraft_cu11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pylibraft_cu11
-Version: 23.4.0.1681363053
+Name: pylibraft-cu11
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibraft_cu11-23.4.0.1681363053/pylibraft_cu11.egg-info/PKG-INFO` & `pylibraft_cu11-23.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pylibraft-cu11
-Version: 23.4.0.1681363053
+Name: pylibraft_cu11
+Version: 23.4.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibraft_cu11-23.4.0.1681363053/setup.py` & `pylibraft_cu11-23.4.1/setup.py`

 * *Files identical despite different names*

