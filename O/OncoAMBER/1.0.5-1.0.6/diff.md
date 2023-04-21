# Comparing `tmp/OncoAMBER-1.0.5.tar.gz` & `tmp/OncoAMBER-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.0.5.tar", last modified: Fri Apr 21 14:03:36 2023, max compression
+gzip compressed data, was "OncoAMBER-1.0.6.tar", last modified: Fri Apr 21 14:04:48 2023, max compression
```

## Comparing `OncoAMBER-1.0.5.tar` & `OncoAMBER-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:03:36.493335 OncoAMBER-1.0.5/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:03:36.492598 OncoAMBER-1.0.5/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:03:36.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      214 2023-04-21 14:03:36.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:03:36.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 13:12:43.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       39 2023-04-21 14:03:36.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:03:36.000000 OncoAMBER-1.0.5/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:03:36.493017 OncoAMBER-1.0.5/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2876 2023-04-20 19:28:15.000000 OncoAMBER-1.0.5/README.md
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 14:03:36.493437 OncoAMBER-1.0.5/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     2956 2023-04-21 14:03:32.000000 OncoAMBER-1.0.5/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:04:48.239132 OncoAMBER-1.0.6/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 14:04:48.238363 OncoAMBER-1.0.6/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      214 2023-04-21 14:04:48.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 13:12:43.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       39 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 14:04:47.000000 OncoAMBER-1.0.6/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3631 2023-04-21 14:04:48.238826 OncoAMBER-1.0.6/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2876 2023-04-20 19:28:15.000000 OncoAMBER-1.0.6/README.md
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 14:04:48.239258 OncoAMBER-1.0.6/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2956 2023-04-21 14:04:44.000000 OncoAMBER-1.0.6/setup.py
```

### Comparing `OncoAMBER-1.0.5/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.0.6/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.5
+Version: 1.0.6
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.5/PKG-INFO` & `OncoAMBER-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.5
+Version: 1.0.6
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.5/README.md` & `OncoAMBER-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.5/setup.py` & `OncoAMBER-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib'] }
```

