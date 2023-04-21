# Comparing `tmp/NikeCA-0.1.65.tar.gz` & `tmp/NikeCA-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.65.tar", last modified: Fri Apr 21 01:36:47 2023, max compression
+gzip compressed data, was "NikeCA-0.1.66.tar", last modified: Fri Apr 21 02:48:48 2023, max compression
```

## Comparing `NikeCA-0.1.65.tar` & `NikeCA-0.1.66.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.319908 NikeCA-0.1.65/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.65/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 01:36:47.319440 NikeCA-0.1.65/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.65/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 01:36:47.320046 NikeCA-0.1.65/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2461 2023-04-21 01:36:21.000000 NikeCA-0.1.65/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.312685 NikeCA-0.1.65/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.313172 NikeCA-0.1.65/src/Dashboards/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.314629 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.316195 NikeCA-0.1.65/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 01:36:47.318720 NikeCA-0.1.65/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      643 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      329 2023-04-21 01:36:47.000000 NikeCA-0.1.65/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 01:13:19.000000 NikeCA-0.1.65/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23497 2023-04-21 01:29:28.000000 NikeCA-0.1.65/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 00:38:26.000000 NikeCA-0.1.65/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      180 2023-04-21 01:34:15.000000 NikeCA-0.1.65/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.113999 NikeCA-0.1.66/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.66/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 02:48:48.113353 NikeCA-0.1.66/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.66/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 02:48:48.114214 NikeCA-0.1.66/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2461 2023-04-21 02:48:43.000000 NikeCA-0.1.66/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.106108 NikeCA-0.1.66/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.106727 NikeCA-0.1.66/src/Dashboards/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.107711 NikeCA-0.1.66/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9022 2023-04-21 02:46:42.000000 NikeCA-0.1.66/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.109822 NikeCA-0.1.66/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      115 2023-04-21 02:06:07.000000 NikeCA-0.1.66/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 02:48:48.112638 NikeCA-0.1.66/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 02:48:47.000000 NikeCA-0.1.66/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      643 2023-04-21 02:48:47.000000 NikeCA-0.1.66/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 02:48:47.000000 NikeCA-0.1.66/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 02:48:47.000000 NikeCA-0.1.66/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      329 2023-04-21 02:48:47.000000 NikeCA-0.1.66/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 01:13:19.000000 NikeCA-0.1.66/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23497 2023-04-21 01:29:28.000000 NikeCA-0.1.66/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 00:38:26.000000 NikeCA-0.1.66/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      194 2023-04-21 02:02:24.000000 NikeCA-0.1.66/src/__init__.py
```

### Comparing `NikeCA-0.1.65/LICENSE` & `NikeCA-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/PKG-INFO` & `NikeCA-0.1.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.65
+Version: 0.1.66
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.65/README.md` & `NikeCA-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/setup.py` & `NikeCA-0.1.66/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.65',
+	version='0.1.66',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.65/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.66/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 ):
 
         import polars as pl
         import pandas as pd
         import configparser
 
         config = configparser.ConfigParser()
-        config.read('../../pip.ini')
+        config.read('pip.ini')
 
         a = config['inclusion_exclusion_summary_and_home'].get('col_a')
         b = config['inclusion_exclusion_summary_and_home'].get('col_b')
         c = config['inclusion_exclusion_summary_and_home'].get('col_c')
 
         df = InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
                                                         database=database, role=role, columns=columns, filters=filters,
```

### Comparing `NikeCA-0.1.65/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.66/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.65
+Version: 0.1.66
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.65/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.66/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.66/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/NikeQA.py` & `NikeCA-0.1.66/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/NikeSF.py` & `NikeCA-0.1.66/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_BuildSearchQuery.py` & `NikeCA-0.1.66/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_GitHub.py` & `NikeCA-0.1.66/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_QA.py` & `NikeCA-0.1.66/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_SearchFiles.py` & `NikeCA-0.1.66/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_SnowflakeData.py` & `NikeCA-0.1.66/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_SnowflakeDependencies.py` & `NikeCA-0.1.66/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.65/src/_SnowflakePull.py` & `NikeCA-0.1.66/src/_SnowflakePull.py`

 * *Files identical despite different names*

