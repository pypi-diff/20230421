# Comparing `tmp/NikeCA-0.1.64.tar.gz` & `tmp/NikeCA-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.64.tar", last modified: Fri Apr 21 00:59:09 2023, max compression
+gzip compressed data, was "NikeCA-0.1.65.tar", last modified: Fri Apr 21 01:36:47 2023, max compression
```

## Comparing `NikeCA-0.1.64.tar` & `NikeCA-0.1.65.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.154630 NikeCA-0.1.64/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.64/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:59:09.154215 NikeCA-0.1.64/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.64/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 00:59:09.154830 NikeCA-0.1.64/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2507 2023-04-21 00:58:25.000000 NikeCA-0.1.64/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.141853 NikeCA-0.1.64/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.143508 NikeCA-0.1.64/src/Dashboards/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.145276 NikeCA-0.1.64/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.148103 NikeCA-0.1.64/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3936 2023-04-20 23:15:49.000000 NikeCA-0.1.64/src/Dashboards/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:59:09.153319 NikeCA-0.1.64/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:59:08.000000 NikeCA-0.1.64/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      719 2023-04-21 00:59:08.000000 NikeCA-0.1.64/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 00:59:08.000000 NikeCA-0.1.64/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 00:59:08.000000 NikeCA-0.1.64/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      365 2023-04-21 00:59:08.000000 NikeCA-0.1.64/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 00:58:07.000000 NikeCA-0.1.64/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23558 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:29:19.000000 NikeCA-0.1.64/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-20 00:33:46.000000 NikeCA-0.1.64/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 00:38:26.000000 NikeCA-0.1.64/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      223 2023-04-21 00:57:46.000000 NikeCA-0.1.64/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.319908 NikeCA-0.1.65/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.65/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 01:36:47.319440 NikeCA-0.1.65/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.65/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 01:36:47.320046 NikeCA-0.1.65/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2461 2023-04-21 01:36:21.000000 NikeCA-0.1.65/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.312685 NikeCA-0.1.65/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.313172 NikeCA-0.1.65/src/Dashboards/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.314629 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.316195 NikeCA-0.1.65/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.318720 NikeCA-0.1.65/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      643 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      329 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 01:13:19.000000 NikeCA-0.1.65/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23497 2023-04-21 01:29:28.000000 NikeCA-0.1.65/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      180 2023-04-21 01:34:15.000000 NikeCA-0.1.65/src/__init__.py
```

### Comparing `NikeCA-0.1.64/LICENSE` & `NikeCA-0.1.65/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/PKG-INFO` & `NikeCA-0.1.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.64
+Version: 0.1.65
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.64/README.md` & `NikeCA-0.1.65/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/setup.py` & `NikeCA-0.1.65/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.64',
+	version='0.1.65',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
-		"Dashboards/_Dashboards",
 		"Dashboards/__init__",
 		"Dashboards/InclusionExclusion/InclusionExclusion",
 		"Dashboards/InclusionExclusion/__init__",
 		"Dashboards/Telemetry/ProductUsage",
 		"Dashboards/Telemetry/Telemetry",
 		"Dashboards/Telemetry/__init__",
 		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
-		"Dashboards/*",
 		"NikeCA"
 	],
 	package_dir={'': 'src'},
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 3.11",
 		"License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
```

### Comparing `NikeCA-0.1.64/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.65/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.65/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.64
+Version: 0.1.65
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.64/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.65/src/NikeCA.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 LICENSE
 README.md
 setup.py
 src/NikeCA.py
 src/NikeQA.py
 src/NikeSF.py
 src/_BuildSearchQuery.py
-src/_Dashboards.py
 src/_GitHub.py
-src/_InclusionExclusion.py
 src/_QA.py
 src/_SearchFiles.py
 src/_SnowflakeData.py
 src/_SnowflakeDependencies.py
 src/_SnowflakePull.py
 src/__init__.py
-src/Dashboards/_Dashboards.py
 src/Dashboards/__init__.py
 src/Dashboards/InclusionExclusion/InclusionExclusion.py
 src/Dashboards/InclusionExclusion/__init__.py
 src/Dashboards/Telemetry/ProductUsage.py
 src/Dashboards/Telemetry/Telemetry.py
 src/Dashboards/Telemetry/__init__.py
 src/NikeCA.egg-info/PKG-INFO
```

### Comparing `NikeCA-0.1.64/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.65/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/NikeQA.py` & `NikeCA-0.1.65/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/NikeSF.py` & `NikeCA-0.1.65/src/NikeSF.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
 from Dashboards.Dashboards import Dashboards
 from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
 
 
-class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery, InclusionExclusion):
-
-    Dashboards = Dashboards
+class Snowflake(SnowflakeData, SnowflakeDependencies, BuildSearchQuery):
 
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
```

### Comparing `NikeCA-0.1.64/src/_BuildSearchQuery.py` & `NikeCA-0.1.65/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_GitHub.py` & `NikeCA-0.1.65/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_QA.py` & `NikeCA-0.1.65/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_SearchFiles.py` & `NikeCA-0.1.65/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_SnowflakeData.py` & `NikeCA-0.1.65/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_SnowflakeDependencies.py` & `NikeCA-0.1.65/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.64/src/_SnowflakePull.py` & `NikeCA-0.1.65/src/_SnowflakePull.py`

 * *Files identical despite different names*

