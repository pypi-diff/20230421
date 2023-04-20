# Comparing `tmp/nheri_simcenter-0.9.7.tar.gz` & `tmp/nheri_simcenter-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nheri_simcenter-0.9.7.tar", last modified: Wed Apr 12 17:34:22 2023, max compression
+gzip compressed data, was "nheri_simcenter-0.9.8.tar", last modified: Thu Apr 20 23:41:54 2023, max compression
```

## Comparing `nheri_simcenter-0.9.7.tar` & `nheri_simcenter-0.9.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.043329 nheri_simcenter-0.9.7/
--rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.7/LICENSE
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-12 17:34:22.043160 nheri_simcenter-0.9.7/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.7/README.md
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.041941 nheri_simcenter-0.9.7/nheri_simcenter/
--rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-04-12 17:32:46.000000 nheri_simcenter-0.9.7/nheri_simcenter/__init__.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.042891 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/SOURCES.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/dependency_links.txt
--rw-r--r--   0 adamzs     (504) staff       (20)      145 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/requires.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/top_level.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-04-12 17:34:22.043374 nheri_simcenter-0.9.7/setup.cfg
--rw-r--r--   0 adamzs     (504) staff       (20)     2028 2023-04-12 17:32:32.000000 nheri_simcenter-0.9.7/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.613474 nheri_simcenter-0.9.8/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.8/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-20 23:41:54.613307 nheri_simcenter-0.9.8/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.8/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.612333 nheri_simcenter-0.9.8/nheri_simcenter/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-04-20 23:39:12.000000 nheri_simcenter-0.9.8/nheri_simcenter/__init__.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.612979 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)      155 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-04-20 23:41:54.613522 nheri_simcenter-0.9.8/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2050 2023-04-20 23:38:54.000000 nheri_simcenter-0.9.8/setup.py
```

### Comparing `nheri_simcenter-0.9.7/LICENSE` & `nheri_simcenter-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.7/PKG-INFO` & `nheri_simcenter-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri_simcenter
-Version: 0.9.7
+Version: 0.9.8
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.7/README.md` & `nheri_simcenter-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.7/nheri_simcenter/__init__.py` & `nheri_simcenter-0.9.8/nheri_simcenter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # nheri_simcenter. If not, see <http://www.opensource.org/licenses/>.
 #
 # Contributors:
 # Adam Zsarnóczay
 
 name = "nheri_simcenter"
 
-__version__ = '0.9.7'
+__version__ = '0.9.8'
 
 __copyright__ = """Copyright (c) 2018 Leland Stanford Junior University and
 The Regents of the University of California"""
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `nheri_simcenter-0.9.7/nheri_simcenter.egg-info/PKG-INFO` & `nheri_simcenter-0.9.8/nheri_simcenter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri-simcenter
-Version: 0.9.7
+Version: 0.9.8
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.7/setup.py` & `nheri_simcenter-0.9.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,17 @@
     install_requires=[
         'numpy>=1.23.5, <2.0',
         'scipy>=1.9.3, <2.0',
         'pandas>=1.5.2, <2.0',
         'openpyxl',
         'tables',
         'openseespy',
-        'sklearn',
         'scikit-learn',
+        'plotly',
+        'colorlover',
         'jpype1',
         'tqdm',
         'gpy',
         'emukit'
     ],
     classifiers = [
         'Programming Language :: Python',
```

