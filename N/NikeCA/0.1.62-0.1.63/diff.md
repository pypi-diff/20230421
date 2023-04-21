# Comparing `tmp/NikeCA-0.1.62.tar.gz` & `tmp/NikeCA-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.62.tar", last modified: Fri Apr 21 00:06:17 2023, max compression
+gzip compressed data, was "NikeCA-0.1.63.tar", last modified: Fri Apr 21 00:39:37 2023, max compression
```

## Comparing `NikeCA-0.1.62.tar` & `NikeCA-0.1.63.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.366615 NikeCA-0.1.62/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.62/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:06:17.366120 NikeCA-0.1.62/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.62/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 00:06:17.366746 NikeCA-0.1.62/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2510 2023-04-21 00:05:59.000000 NikeCA-0.1.62/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.359492 NikeCA-0.1.62/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.360734 NikeCA-0.1.62/src/Dashboards/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.361604 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.362939 NikeCA-0.1.62/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/_ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       95 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/_Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3936 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.365500 NikeCA-0.1.62/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      722 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      368 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      342 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23530 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:29:19.000000 NikeCA-0.1.62/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-20 00:33:46.000000 NikeCA-0.1.62/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14114 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.830440 NikeCA-0.1.63/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.63/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:39:37.830041 NikeCA-0.1.63/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.63/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 00:39:37.830597 NikeCA-0.1.63/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2507 2023-04-21 00:39:17.000000 NikeCA-0.1.63/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.822843 NikeCA-0.1.63/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.824169 NikeCA-0.1.63/src/Dashboards/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.825189 NikeCA-0.1.63/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.827013 NikeCA-0.1.63/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3936 2023-04-20 23:15:49.000000 NikeCA-0.1.63/src/Dashboards/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:39:37.829356 NikeCA-0.1.63/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:39:37.000000 NikeCA-0.1.63/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      719 2023-04-21 00:39:37.000000 NikeCA-0.1.63/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 00:39:37.000000 NikeCA-0.1.63/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 00:39:37.000000 NikeCA-0.1.63/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      365 2023-04-21 00:39:37.000000 NikeCA-0.1.63/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23558 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:29:19.000000 NikeCA-0.1.63/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-20 00:33:46.000000 NikeCA-0.1.63/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      227 2023-04-21 00:38:26.000000 NikeCA-0.1.63/src/__init__.py
```

### Comparing `NikeCA-0.1.62/LICENSE` & `NikeCA-0.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/PKG-INFO` & `NikeCA-0.1.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.62
+Version: 0.1.63
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.62/README.md` & `NikeCA-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/setup.py` & `NikeCA-0.1.63/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.62',
+	version='0.1.63',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/_Dashboards",
 		"Dashboards/__init__",
-		"Dashboards/InclusionExclusion/_InclusionExclusion",
+		"Dashboards/InclusionExclusion/InclusionExclusion",
 		"Dashboards/InclusionExclusion/__init__",
-		"Dashboards/Telemetry/_ProductUsage",
-		"Dashboards/Telemetry/_Telemetry",
+		"Dashboards/Telemetry/ProductUsage",
+		"Dashboards/Telemetry/Telemetry",
 		"Dashboards/Telemetry/__init__",
 		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
```

### Comparing `NikeCA-0.1.62/src/Dashboards/InclusionExclusion/_InclusionExclusion.py` & `NikeCA-0.1.63/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/Dashboards/_Dashboards.py` & `NikeCA-0.1.63/src/Dashboards/_Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.63/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.62
+Version: 0.1.63
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.62/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.63/src/NikeCA.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 src/_SearchFiles.py
 src/_SnowflakeData.py
 src/_SnowflakeDependencies.py
 src/_SnowflakePull.py
 src/__init__.py
 src/Dashboards/_Dashboards.py
 src/Dashboards/__init__.py
-src/Dashboards/InclusionExclusion/_InclusionExclusion.py
+src/Dashboards/InclusionExclusion/InclusionExclusion.py
 src/Dashboards/InclusionExclusion/__init__.py
-src/Dashboards/Telemetry/_ProductUsage.py
-src/Dashboards/Telemetry/_Telemetry.py
+src/Dashboards/Telemetry/ProductUsage.py
+src/Dashboards/Telemetry/Telemetry.py
 src/Dashboards/Telemetry/__init__.py
 src/NikeCA.egg-info/PKG-INFO
 src/NikeCA.egg-info/SOURCES.txt
 src/NikeCA.egg-info/dependency_links.txt
 src/NikeCA.egg-info/requires.txt
 src/NikeCA.egg-info/top_level.txt
```

### Comparing `NikeCA-0.1.62/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.63/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/NikeQA.py` & `NikeCA-0.1.63/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/NikeSF.py` & `NikeCA-0.1.63/src/NikeSF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
-from Dashboards._Dashboards import Dashboards
-from Dashboards.InclusionExclusion._InclusionExclusion import InclusionExclusion
+from Dashboards.Dashboards import Dashboards
+from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
 
 
 class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery, InclusionExclusion):
+
+    Dashboards = Dashboards
+
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
```

### Comparing `NikeCA-0.1.62/src/_BuildSearchQuery.py` & `NikeCA-0.1.63/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_Dashboards.py` & `NikeCA-0.1.63/src/_Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_GitHub.py` & `NikeCA-0.1.63/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_InclusionExclusion.py` & `NikeCA-0.1.63/src/_InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_QA.py` & `NikeCA-0.1.63/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_SearchFiles.py` & `NikeCA-0.1.63/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_SnowflakeData.py` & `NikeCA-0.1.63/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import _BuildSearchQuery
 import _SnowflakePull
 import _SnowflakeDependencies
-from Dashboards import _Dashboards
+from Dashboards import Dashboards
 
 
-class SnowflakeData(_Dashboards.Dashboards
+class SnowflakeData(Dashboards.Dashboards
                     , _SnowflakePull.SnowflakePull
                     , _SnowflakeDependencies.SnowflakeDependencies
                     , _BuildSearchQuery.BuildSearchQuery):
 
     def snowflake_pull(self, query: str | dict | None, un, wh, db, role, schema=None, table=None,
                        sample_table: bool = False, sample_val: bool = False, table_sample: dict = None,
                        dtypes_conv=None, separate_dataframes: bool = True, polars: bool = True): # -> pandas.DataFrame:
```

### Comparing `NikeCA-0.1.62/src/_SnowflakeDependencies.py` & `NikeCA-0.1.63/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.62/src/_SnowflakePull.py` & `NikeCA-0.1.63/src/_SnowflakePull.py`

 * *Files identical despite different names*

