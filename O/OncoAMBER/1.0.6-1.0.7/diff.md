# Comparing `tmp/OncoAMBER-1.0.6.tar.gz` & `tmp/OncoAMBER-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.0.6.tar", last modified: Fri Apr 21 14:04:48 2023, max compression
+gzip compressed data, was "OncoAMBER-1.0.7.tar", last modified: Fri Apr 21 14:52:14 2023, max compression
```

## Comparing `OncoAMBER-1.0.6.tar` & `OncoAMBER-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,29 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:04:48.239132 OncoAMBER-1.0.6/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:04:48.238363 OncoAMBER-1.0.6/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      214 2023-04-21 14:04:48.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 13:12:43.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       39 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:04:48.238826 OncoAMBER-1.0.6/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2876 2023-04-20 19:28:15.000000 OncoAMBER-1.0.6/README.md
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 14:04:48.239258 OncoAMBER-1.0.6/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     2956 2023-04-21 14:04:44.000000 OncoAMBER-1.0.6/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:52:14.887452 OncoAMBER-1.0.7/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:52:14.850623 OncoAMBER-1.0.7/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:52:14.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      515 2023-04-21 14:52:14.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:52:14.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 13:12:43.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 14:52:14.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        4 2023-04-21 14:52:14.000000 OncoAMBER-1.0.7/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:52:14.887196 OncoAMBER-1.0.7/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2876 2023-04-20 19:28:15.000000 OncoAMBER-1.0.7/README.md
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 14:52:14.887545 OncoAMBER-1.0.7/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2967 2023-04-21 14:52:08.000000 OncoAMBER-1.0.7/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:52:14.885734 OncoAMBER-1.0.7/src/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-20 19:02:38.000000 OncoAMBER-1.0.7/src/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1782 2023-04-20 19:20:16.000000 OncoAMBER-1.0.7/src/Cell.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:52:14.886801 OncoAMBER-1.0.7/src/Micro-Oxygenation/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 14:49:09.000000 OncoAMBER-1.0.7/src/Micro-Oxygenation/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:16:18.000000 OncoAMBER-1.0.7/src/Micro-Oxygenation/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    20610 2023-04-20 23:09:01.000000 OncoAMBER-1.0.7/src/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1607 2023-04-20 19:11:28.000000 OncoAMBER-1.0.7/src/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      752 2023-04-21 14:51:16.000000 OncoAMBER-1.0.7/src/RunTopas.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-20 23:09:01.000000 OncoAMBER-1.0.7/src/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-11 13:27:24.000000 OncoAMBER-1.0.7/src/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14138 2023-04-20 20:26:57.000000 OncoAMBER-1.0.7/src/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6179 2023-04-20 19:22:34.000000 OncoAMBER-1.0.7/src/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    20862 2023-04-20 23:09:01.000000 OncoAMBER-1.0.7/src/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-20 18:58:39.000000 OncoAMBER-1.0.7/src/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-20 17:57:39.000000 OncoAMBER-1.0.7/src/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      172 2023-04-21 14:35:05.000000 OncoAMBER-1.0.7/src/config_instance.py
```

### Comparing `OncoAMBER-1.0.6/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.0.7/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.6
+Version: 1.0.7
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.6/PKG-INFO` & `OncoAMBER-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.6
+Version: 1.0.7
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.6/README.md` & `OncoAMBER-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.6/setup.py` & `OncoAMBER-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
-EXTRAS = { 'plots' :['matplotlib'] }
+EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
```

