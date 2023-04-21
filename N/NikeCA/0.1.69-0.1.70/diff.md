# Comparing `tmp/NikeCA-0.1.69.tar.gz` & `tmp/NikeCA-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.69.tar", last modified: Fri Apr 21 03:27:54 2023, max compression
+gzip compressed data, was "NikeCA-0.1.70.tar", last modified: Fri Apr 21 03:29:52 2023, max compression
```

## Comparing `NikeCA-0.1.69.tar` & `NikeCA-0.1.70.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.419041 NikeCA-0.1.69/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.69/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 03:27:54.418508 NikeCA-0.1.69/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.69/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 03:27:54.419187 NikeCA-0.1.69/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2461 2023-04-21 03:27:46.000000 NikeCA-0.1.69/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.410812 NikeCA-0.1.69/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.411746 NikeCA-0.1.69/src/Dashboards/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.413088 NikeCA-0.1.69/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.415342 NikeCA-0.1.69/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.69/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:27:54.417787 NikeCA-0.1.69/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 03:27:54.000000 NikeCA-0.1.69/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      643 2023-04-21 03:27:54.000000 NikeCA-0.1.69/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 03:27:54.000000 NikeCA-0.1.69/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 03:27:54.000000 NikeCA-0.1.69/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      329 2023-04-21 03:27:54.000000 NikeCA-0.1.69/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14079 2023-04-21 03:27:36.000000 NikeCA-0.1.69/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.69/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.189932 NikeCA-0.1.70/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.70/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 03:29:52.189642 NikeCA-0.1.70/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.70/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 03:29:52.190064 NikeCA-0.1.70/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2461 2023-04-21 03:29:44.000000 NikeCA-0.1.70/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.182773 NikeCA-0.1.70/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.183498 NikeCA-0.1.70/src/Dashboards/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.184621 NikeCA-0.1.70/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.186962 NikeCA-0.1.70/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.70/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:29:52.188970 NikeCA-0.1.70/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 03:29:52.000000 NikeCA-0.1.70/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      643 2023-04-21 03:29:52.000000 NikeCA-0.1.70/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 03:29:52.000000 NikeCA-0.1.70/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 03:29:52.000000 NikeCA-0.1.70/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      329 2023-04-21 03:29:52.000000 NikeCA-0.1.70/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14034 2023-04-21 03:29:33.000000 NikeCA-0.1.70/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.70/src/__init__.py
```

### Comparing `NikeCA-0.1.69/LICENSE` & `NikeCA-0.1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/PKG-INFO` & `NikeCA-0.1.70/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.69
+Version: 0.1.70
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.69/README.md` & `NikeCA-0.1.70/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/setup.py` & `NikeCA-0.1.70/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.69',
+	version='0.1.70',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.69/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.70/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.70/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.69
+Version: 0.1.70
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.69/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.70/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.70/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/NikeQA.py` & `NikeCA-0.1.70/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/NikeSF.py` & `NikeCA-0.1.70/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_BuildSearchQuery.py` & `NikeCA-0.1.70/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_GitHub.py` & `NikeCA-0.1.70/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_QA.py` & `NikeCA-0.1.70/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_SearchFiles.py` & `NikeCA-0.1.70/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_SnowflakeData.py` & `NikeCA-0.1.70/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import _BuildSearchQuery
 import _SnowflakePull
 import _SnowflakeDependencies
-from Dashboards.Dashboards import Dashboards
 
 
 class SnowflakeData(_SnowflakePull.SnowflakePull
                     , _SnowflakeDependencies.SnowflakeDependencies
                     , _BuildSearchQuery.BuildSearchQuery):
 
     def snowflake_pull(self, query: str | dict | None, un, wh, db, role, schema=None, table=None,
```

### Comparing `NikeCA-0.1.69/src/_SnowflakeDependencies.py` & `NikeCA-0.1.70/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.69/src/_SnowflakePull.py` & `NikeCA-0.1.70/src/_SnowflakePull.py`

 * *Files identical despite different names*

