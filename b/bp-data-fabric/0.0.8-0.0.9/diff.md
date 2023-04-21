# Comparing `tmp/bp_data_fabric-0.0.8.tar.gz` & `tmp/bp_data_fabric-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.8.tar", last modified: Fri Apr 21 06:21:07 2023, max compression
+gzip compressed data, was "bp_data_fabric-0.0.9.tar", last modified: Fri Apr 21 06:23:51 2023, max compression
```

## Comparing `bp_data_fabric-0.0.8.tar` & `bp_data_fabric-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.798644 bp_data_fabric-0.0.8/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.8/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:21:07.798195 bp_data_fabric-0.0.8/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.8/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.796044 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.797237 bp_data_fabric-0.0.8/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.8/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.8/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 06:21:07.798844 bp_data_fabric-0.0.8/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      603 2023-04-21 06:14:22.000000 bp_data_fabric-0.0.8/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.243447 bp_data_fabric-0.0.9/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.9/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:23:51.243108 bp_data_fabric-0.0.9/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.9/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.241689 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.242529 bp_data_fabric-0.0.9/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.9/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.9/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 06:23:51.243652 bp_data_fabric-0.0.9/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      712 2023-04-21 06:23:36.000000 bp_data_fabric-0.0.9/setup.py
```

### Comparing `bp_data_fabric-0.0.8/LICENSE` & `bp_data_fabric-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.8/data_fabric/__init__.py` & `bp_data_fabric-0.0.9/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.8/data_fabric/components.py` & `bp_data_fabric-0.0.9/data_fabric/components.py`

 * *Files identical despite different names*

