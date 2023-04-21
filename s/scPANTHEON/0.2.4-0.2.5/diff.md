# Comparing `tmp/scPANTHEON-0.2.4.tar.gz` & `tmp/scPANTHEON-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.2.4.tar", last modified: Thu Apr 13 11:05:40 2023, max compression
+gzip compressed data, was "scPANTHEON-0.2.5.tar", last modified: Fri Apr 21 02:49:38 2023, max compression
```

## Comparing `scPANTHEON-0.2.4.tar` & `scPANTHEON-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.950222 scPANTHEON-0.2.4/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-04-13 11:05:40.949218 scPANTHEON-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.904047 scPANTHEON-0.2.4/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.913632 scPANTHEON-0.2.4/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.889197 scPANTHEON-0.2.4/scpantheon/extension/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.915264 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.919311 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.920314 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.922527 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/
--rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.924042 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.927599 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.929695 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.932834 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.934353 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.937463 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.939476 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.943067 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.944592 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.948213 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/module.py
--rw-rw-rw-   0        0        0     1026 2023-04-05 05:30:01.000000 scPANTHEON-0.2.4/scpantheon/main.py
--rw-rw-rw-   0        0        0     5551 2023-04-05 05:25:57.000000 scPANTHEON-0.2.4/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/run.py
--rw-rw-rw-   0        0        0    59203 2023-04-05 05:26:39.000000 scPANTHEON-0.2.4/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-04-13 11:05:40.950222 scPANTHEON-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-04-13 11:05:25.000000 scPANTHEON-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.856409 scPANTHEON-0.2.5/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-04-21 02:49:38.855409 scPANTHEON-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.814609 scPANTHEON-0.2.5/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1676 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 02:49:38.000000 scPANTHEON-0.2.5/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.823885 scPANTHEON-0.2.5/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.799620 scPANTHEON-0.2.5/scpantheon/extension/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.824889 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.827899 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/
+-rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.5/scpantheon/extension/Change_Color/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.829901 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.832005 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/
+-rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.833007 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.837027 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.838033 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.841060 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
+-rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.842063 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.845311 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/
+-rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.846392 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.849403 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.851408 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/
+drwxrwxrwx   0        0        0        0 2023-04-21 02:49:38.854409 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/
+-rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.5/scpantheon/extension/TOMAS/module.py
+-rw-rw-rw-   0        0        0     1040 2023-04-20 09:00:00.000000 scPANTHEON-0.2.5/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-04-21 02:43:50.000000 scPANTHEON-0.2.5/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/run.py
+-rw-rw-rw-   0        0        0    59203 2023-04-20 04:56:28.000000 scPANTHEON-0.2.5/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.5/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 02:49:38.856409 scPANTHEON-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-04-21 02:49:34.000000 scPANTHEON-0.2.5/setup.py
```

### Comparing `scPANTHEON-0.2.4/scPANTHEON.egg-info/SOURCES.txt` & `scPANTHEON-0.2.5/scPANTHEON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Change_Color/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Check_Histogram/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Clustering_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Differential_Expression_Analysis/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Find_Marker_Gene/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/Preprocessing_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/module.py` & `scPANTHEON-0.2.5/scpantheon/extension/TOMAS/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/main.py` & `scPANTHEON-0.2.5/scpantheon/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from multiprocessing import freeze_support
-freeze_support()
+'''from multiprocessing import freeze_support
+freeze_support()'''
 
 import warnings
 
 from bokeh.server.server import Server
 import multiprocessing
 import warnings
 
 class InstallWarning(Warning):
     def __init__(self, message):
         self.message = message
     def __str__(self):
         return repr(self.message)
-
+        
 try: 
     from scpantheon import qt, source # import from online
 except:
     warnings.warn('YOU HAVE TO INSTALL PyQt5',InstallWarning)
 
 def run():
     global server
```

### Comparing `scPANTHEON-0.2.4/scpantheon/qt.py` & `scPANTHEON-0.2.5/scpantheon/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from PyQt5 import QtCore, QtGui
 # import mysql.connector
 from pathlib import Path
 from appdirs import AppDirs
 
 sys.path.append(str(Path(__file__).resolve().parents[1]))
 try:
-    from source import connection
-except:
     from scpantheon.source import connection
+except:
+    from source import connection
 '''
 def myconnect():
     global mydb,mycursor
     mydb = mysql.connector.connect(
         host="localhost",
         #  port=3360,
         user="root",
@@ -129,23 +129,26 @@
         Dialog.setWindowTitle(_translate("ScPantheon", "ScPantheon"))
 
 
 def mkdir(path):
     isExists = os.path.exists(path)
     if not isExists:
         os.makedirs(path)
-        print(path + 'successful creat')
+        print(path + ' successful creat')
         return True
     else:
-        print(path + 'already exist')
+        print(path + ' already exist')
 
 
 def text_create(name, msg):
     path = dir + "\\" + name + '.txt'
     print("-========- path:", path)
+    with open(path, "w") as f:
+        f.truncate(0)
+        f.close()
     file = open(path, 'w')
     file.write(msg)
     file.close()
 
 
 def main():
     global dir
```

### Comparing `scPANTHEON-0.2.4/scpantheon/source.py` & `scPANTHEON-0.2.5/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/scpantheon/transform.py` & `scPANTHEON-0.2.5/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.4/setup.py` & `scPANTHEON-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.2.4',#版本
+    version='0.2.5',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
-    install_requires=['bokeh==2.4.3','pandas','anndata==0.8.0','colorcet','scanpy','numpy','PyQt5==5.15.9','PyQtWebEngine==5.15.6','appdirs==1.4.4'], # 依赖包,如果没有,可以不要
+    install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
+                        'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'],
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

