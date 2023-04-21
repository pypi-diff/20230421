# Comparing `tmp/raster-tools-0.1.4.tar.gz` & `tmp/raster-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-tools-0.1.4.tar", last modified: Tue Apr 18 22:06:30 2023, max compression
+gzip compressed data, was "raster-tools-0.1.5.tar", last modified: Fri Apr 21 21:04:19 2023, max compression
```

## Comparing `raster-tools-0.1.4.tar` & `raster-tools-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.4/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.4/MANIFEST.in
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-18 22:06:30.142218 raster-tools-0.1.4/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.4/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.4/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.138218 raster-tools-0.1.4/raster_tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.4/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.4/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-18 22:06:23.000000 raster-tools-0.1.4/raster_tools/_version.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/batch.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.4/raster_tools/clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.4/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.4/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.138218 raster-tools-0.1.4/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.4/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.4/raster_tools/distance/_heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/distance/cost_distance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.4/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.4/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.4/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    35261 2023-04-11 22:00:22.000000 raster-tools-0.1.4/raster_tools/general.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.4/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.4/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    46873 2023-04-11 21:59:29.000000 raster-tools-0.1.4/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.4/raster_tools/stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.4/raster_tools/surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-04-18 19:26:49.000000 raster-tools-0.1.4/raster_tools/utils.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    30306 2023-04-18 19:37:34.000000 raster-tools-0.1.4/raster_tools/vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.4/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/raster_tools.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/requirements/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.4/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-18 22:06:30.142218 raster-tools-0.1.4/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.4/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.4/tests/test_clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.4/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.4/tests/test_distance__heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.4/tests/test_distance_proximity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.4/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    22392 2023-02-01 19:59:47.000000 raster-tools-0.1.4/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.4/tests/test_line_stats.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    56488 2023-04-18 19:37:34.000000 raster-tools-0.1.4/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.4/tests/test_stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.4/tests/test_surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.4/tests/test_vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.4/tests/test_zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.5/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.5/MANIFEST.in
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-21 21:04:19.825049 raster-tools-0.1.5/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.5/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.5/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/raster_tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.5/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.5/raster_tools/_compat.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-21 21:02:29.000000 raster-tools-0.1.5/raster_tools/_version.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.5/raster_tools/batch.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.5/raster_tools/clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.5/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.5/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.5/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.5/raster_tools/distance/_heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.5/raster_tools/distance/cost_distance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.5/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.5/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.5/raster_tools/focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35264 2023-04-21 20:58:12.000000 raster-tools-0.1.5/raster_tools/general.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.5/raster_tools/io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.5/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.5/raster_tools/masking.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    47679 2023-04-21 21:02:59.000000 raster-tools-0.1.5/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.5/raster_tools/stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.5/raster_tools/surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-04-18 19:26:49.000000 raster-tools-0.1.5/raster_tools/utils.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    30306 2023-04-21 21:02:59.000000 raster-tools-0.1.5/raster_tools/vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.5/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/raster_tools.egg-info/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-21 21:04:19.000000 raster-tools-0.1.5/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-21 21:04:19.000000 raster-tools-0.1.5/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-21 21:04:19.000000 raster-tools-0.1.5/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-21 21:04:19.000000 raster-tools-0.1.5/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-21 21:04:19.000000 raster-tools-0.1.5/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/requirements/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.5/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-21 21:04:19.825049 raster-tools-0.1.5/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.5/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-21 21:04:19.825049 raster-tools-0.1.5/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.5/tests/test_clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.5/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.5/tests/test_distance__heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.5/tests/test_distance_proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.5/tests/test_focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    24340 2023-04-21 20:48:50.000000 raster-tools-0.1.5/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.5/tests/test_line_stats.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    56488 2023-04-21 21:02:59.000000 raster-tools-0.1.5/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.5/tests/test_stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.5/tests/test_surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.5/tests/test_vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.5/tests/test_zonal.py
```

### Comparing `raster-tools-0.1.4/LICENSE` & `raster-tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/PKG-INFO` & `raster-tools-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.4/README.md` & `raster-tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/__init__.py` & `raster-tools-0.1.5/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/batch.py` & `raster-tools-0.1.5/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/clipping.py` & `raster-tools-0.1.5/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/creation.py` & `raster-tools-0.1.5/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/dask_utils.py` & `raster-tools-0.1.5/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/distance/_heap.py` & `raster-tools-0.1.5/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/distance/cost_distance.py` & `raster-tools-0.1.5/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/distance/proximity.py` & `raster-tools-0.1.5/raster_tools/distance/proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/dtypes.py` & `raster-tools-0.1.5/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/focal.py` & `raster-tools-0.1.5/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/general.py` & `raster-tools-0.1.5/raster_tools/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -972,15 +972,15 @@
     out = np.empty_like(x)
     nb, ny, nx = x.shape
     for b in range(nb):
         for i in range(ny):
             for j in range(nx):
                 if mask[b, i, j]:
                     out[b, i, j] = null
-                    break
+                    continue
                 v = x[b, i, j]
                 reclass = v in mapping
                 if reclass:
                     out[b, i, j] = mapping[v]
                 elif unmapped_to_null:
                     out[b, i, j] = null
                 else:
```

### Comparing `raster-tools-0.1.4/raster_tools/io.py` & `raster-tools-0.1.5/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/line_stats.py` & `raster-tools-0.1.5/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/masking.py` & `raster-tools-0.1.5/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/raster.py` & `raster-tools-0.1.5/raster_tools/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import dask.array as da
 import dask.dataframe as dd
 import geopandas as gpd
 import numpy as np
 import xarray as xr
 from affine import Affine
 from numba import jit
-from shapely.geometry import Point
+from shapely.geometry import Point, box
 
 from raster_tools.dask_utils import dask_nanmax, dask_nanmin
 from raster_tools.dtypes import (
     DTYPE_INPUT_TO_DTYPE,
     is_bool,
     is_float,
     is_int,
@@ -1369,14 +1369,39 @@
             )
             ds = make_raster_ds(xdata_quad, xmask_quad)
             if self.crs is not None:
                 ds = ds.rio.write_crs(self.crs)
             results.append(Raster(ds, _fast_path=True))
         return RasterQuadrantsResult(*results)
 
+    def chunk_geometries(self):
+        _, ychunks, xchunks = self.data.chunks
+        i = 0
+        j = 0
+        chunk_boxes = []
+        rows = []
+        cols = []
+        for row, yc in enumerate(ychunks):
+            for col, xc in enumerate(xchunks):
+                y = self.y[i : i + yc]
+                x = self.x[j : j + xc]
+                j += xc
+                bounds = xr.DataArray(
+                    da.empty((yc, xc)), dims=("y", "x"), coords=(y, x)
+                ).rio.bounds()
+                chunk_boxes.append(box(*bounds))
+                rows.append(row)
+                cols.append(col)
+            i += yc
+            j = 0
+        return gpd.GeoDataFrame(
+            {"chunk_row": rows, "chunk_col": cols, "geometry": chunk_boxes},
+            crs=self.crs,
+        )
+
 
 _offset_name_to_rc_offset = {
     "center": (0.5, 0.5),
     "ul": (0, 0),
     "ur": (0, 1),
     "ll": (1, 0),
     "lr": (1, 1),
```

### Comparing `raster-tools-0.1.4/raster_tools/stat_common.py` & `raster-tools-0.1.5/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/surface.py` & `raster-tools-0.1.5/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/utils.py` & `raster-tools-0.1.5/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/vector.py` & `raster-tools-0.1.5/raster_tools/vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools/zonal.py` & `raster-tools-0.1.5/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/raster_tools.egg-info/PKG-INFO` & `raster-tools-0.1.5/raster_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.4/raster_tools.egg-info/SOURCES.txt` & `raster-tools-0.1.5/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/setup.py` & `raster-tools-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_clipping.py` & `raster-tools-0.1.5/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_distance.py` & `raster-tools-0.1.5/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_distance__heap.py` & `raster-tools-0.1.5/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_distance_proximity.py` & `raster-tools-0.1.5/tests/test_distance_proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_focal.py` & `raster-tools-0.1.5/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_general.py` & `raster-tools-0.1.5/tests/test_general.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     nan_unique_count_jit,
     nanargmax_jit,
     nanargmin_jit,
     nanasm_jit,
     nanentropy_jit,
     nanmode_jit,
 )
-from tests.utils import assert_valid_raster
+from tests.utils import arange_nd, assert_valid_raster
 
 stat_funcs = {
     "max": partial(np.nanmax, axis=0),
     "mean": partial(np.nanmean, axis=0),
     "median": partial(np.nanmedian, axis=0),
     "min": partial(np.nanmin, axis=0),
     "prod": partial(np.nanprod, axis=0),
@@ -641,14 +641,89 @@
     assert result.null_value == truth.null_value
     assert np.allclose(result.xmask, truth.xmask)
     assert result.data.chunks == truth.data.chunks
     assert result.crs is not None
     assert result.crs == "EPSG:3857"
 
 
+@pytest.mark.parametrize("unmapped_to_null", [False, True])
+@pytest.mark.parametrize(
+    "mapping",
+    [{0: -1, 1: -2, 2: -3, 5: 1, 10: 20, 14: 2}, {k: 20 for k in range(10)}],
+)
+@pytest.mark.parametrize(
+    "mask",
+    [
+        np.array(
+            [
+                [
+                    [1, 1, 1, 1],
+                    [1, 1, 1, 0],
+                    [1, 1, 0, 0],
+                    [1, 0, 0, 0],
+                ]
+            ]
+        ).astype(bool),
+        np.array(
+            [
+                [
+                    [1, 1, 0, 0],
+                    [1, 1, 0, 0],
+                    [1, 1, 0, 0],
+                    [1, 1, 0, 0],
+                ]
+            ]
+        ).astype(bool),
+        np.array(
+            [
+                [
+                    [1, 0, 0, 0],
+                    [0, 1, 0, 0],
+                    [0, 0, 1, 0],
+                    [0, 0, 0, 1],
+                ]
+            ]
+        ).astype(bool),
+    ],
+)
+@pytest.mark.parametrize(
+    "data",
+    [
+        arange_nd((1, 4, 4)),
+        arange_nd((1, 4, 4)).astype(float),
+        arange_nd((1, 4, 4)).astype("int16"),
+        arange_nd((1, 4, 4))[..., ::-1, ::-1],
+    ],
+)
+def test__reclassify_chunk(data, mask, mapping, unmapped_to_null):
+    nv = -99
+    map_array = np.array([(k, v) for k, v in mapping.items()]).astype(
+        data.dtype
+    )
+    all_values = set(np.unique(data))
+    mapped = set(mapping)
+    unmapped = set(all_values) - mapped
+    truth = data.copy()
+    tmask = mask.copy()
+    if unmapped_to_null:
+        for v in unmapped:
+            tmask |= data == v
+    for k, v in map_array[::-1]:
+        truth[data == k] = v
+    truth = np.where(tmask, nv, truth)
+
+    result = general._reclassify_chunk(
+        data, mask, map_array, unmapped_to_null, nv
+    )
+    assert result.ndim == 3
+    assert result.shape == truth.shape
+    assert result.dtype == truth.dtype
+    assert np.allclose(truth, result)
+
+
 @pytest.mark.parametrize("method", [False, True])
 def test_reclassify(method):
     data = np.arange(100).reshape((10, 10))
     rast = Raster(Raster(data)._ds.rio.write_crs("EPSG:3857"))
     mapping = {k: v for k, v in zip(np.arange(40), np.arange(20, 60))}
     included_mask = np.array([v in mapping for v in data.ravel()]).reshape(
         (10, 10)
```

### Comparing `raster-tools-0.1.4/tests/test_line_stats.py` & `raster-tools-0.1.5/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_raster.py` & `raster-tools-0.1.5/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_stat_common.py` & `raster-tools-0.1.5/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_surface.py` & `raster-tools-0.1.5/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_vector.py` & `raster-tools-0.1.5/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.4/tests/test_zonal.py` & `raster-tools-0.1.5/tests/test_zonal.py`

 * *Files identical despite different names*

