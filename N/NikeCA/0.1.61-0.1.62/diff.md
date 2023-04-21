# Comparing `tmp/NikeCA-0.1.61.tar.gz` & `tmp/NikeCA-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.61.tar", last modified: Wed Apr 19 04:47:22 2023, max compression
+gzip compressed data, was "NikeCA-0.1.62.tar", last modified: Fri Apr 21 00:06:17 2023, max compression
```

## Comparing `NikeCA-0.1.61.tar` & `NikeCA-0.1.62.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.296089 NikeCA-0.1.61/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.61/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-19 04:47:22.295635 NikeCA-0.1.61/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.61/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-19 04:47:22.296213 NikeCA-0.1.61/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-19 04:47:00.000000 NikeCA-0.1.61/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.290492 NikeCA-0.1.61/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.292812 NikeCA-0.1.61/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      444 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23489 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.366615 NikeCA-0.1.62/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.62/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:06:17.366120 NikeCA-0.1.62/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.62/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-21 00:06:17.366746 NikeCA-0.1.62/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2510 2023-04-21 00:05:59.000000 NikeCA-0.1.62/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.359492 NikeCA-0.1.62/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.360734 NikeCA-0.1.62/src/Dashboards/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.361604 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9028 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.362939 NikeCA-0.1.62/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/_ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       95 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/_Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3936 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-21 00:06:17.365500 NikeCA-0.1.62/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      722 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      368 2023-04-21 00:06:17.000000 NikeCA-0.1.62/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      342 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23530 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:29:19.000000 NikeCA-0.1.62/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-20 00:33:46.000000 NikeCA-0.1.62/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14114 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-20 23:15:49.000000 NikeCA-0.1.62/src/__init__.py
```

### Comparing `NikeCA-0.1.61/LICENSE` & `NikeCA-0.1.62/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/PKG-INFO` & `NikeCA-0.1.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.61
+Version: 0.1.62
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.61/README.md` & `NikeCA-0.1.62/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/setup.py` & `NikeCA-0.1.62/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.61',
+	version='0.1.62',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
-		"_Dashboards",
-		"_InclusionExclusion",
+		"Dashboards/_Dashboards",
+		"Dashboards/__init__",
+		"Dashboards/InclusionExclusion/_InclusionExclusion",
+		"Dashboards/InclusionExclusion/__init__",
+		"Dashboards/Telemetry/_ProductUsage",
+		"Dashboards/Telemetry/_Telemetry",
+		"Dashboards/Telemetry/__init__",
 		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
+		"Dashboards/*",
 		"NikeCA"
 	],
 	package_dir={'': 'src'},
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 3.11",
 		"License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
```

### Comparing `NikeCA-0.1.61/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.62/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.61
+Version: 0.1.62
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.61/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.62/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/NikeQA.py` & `NikeCA-0.1.62/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/NikeSF.py` & `NikeCA-0.1.62/src/NikeSF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
-from _Dashboards import Dashboards
-from _InclusionExclusion import InclusionExclusion
+from Dashboards._Dashboards import Dashboards
+from Dashboards.InclusionExclusion._InclusionExclusion import InclusionExclusion
 
 
 class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery, InclusionExclusion):
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
```

### Comparing `NikeCA-0.1.61/src/_BuildSearchQuery.py` & `NikeCA-0.1.62/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_Dashboards.py` & `NikeCA-0.1.62/src/_Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_GitHub.py` & `NikeCA-0.1.62/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_InclusionExclusion.py` & `NikeCA-0.1.62/src/Dashboards/InclusionExclusion/_InclusionExclusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+
 class InclusionExclusion:
 
     def pos_data_quality_review(self
                                 , username: str
                                 , warehouse: str
                                 , database: str
                                 , role: str
@@ -65,16 +66,14 @@
                 
             ORDER BY
                 {order_by}
                 
             ;
         """
 
-        print(query)
-
         df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
                                     role=role).snowflake_pull(query=query, polars=polars))
 
         if start_date is None and end_date is None:
             return df.filter(pl.col(a) == pl.col(a).max())
         elif end_date is None:
             return df.filter((pl.col(a) >= datetime.datetime.strptime(start_date, '%Y-%m-%d')))
@@ -98,15 +97,15 @@
                 ):
 
         import polars as pl
         import pandas as pd
         import configparser
 
         config = configparser.ConfigParser()
-        config.read('pip.ini')
+        config.read('../../pip.ini')
 
         a = config['inclusion_exclusion_summary_and_home'].get('col_a')
         b = config['inclusion_exclusion_summary_and_home'].get('col_b')
         c = config['inclusion_exclusion_summary_and_home'].get('col_c')
 
         df = InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
                                                         database=database, role=role, columns=columns, filters=filters,
@@ -141,15 +140,15 @@
 
         import datetime
 
         import polars as pl
         import configparser
 
         config = configparser.ConfigParser()
-        config.read('pip.ini')
+        config.read('../../pip.ini')
 
         a = config['inclusion_exclusion_summary_and_home'].get('col_a')
         b = config['inclusion_exclusion_summary_and_home'].get('col_b')
         c = config['inclusion_exclusion_summary_and_home'].get('col_c')
         d = config['inclusion_exclusion_summary_and_home'].get('col_d')
         e = config['inclusion_exclusion_summary_and_home'].get('col_e')
         f = config['inclusion_exclusion_summary_and_home'].get('col_f')
@@ -172,27 +171,27 @@
                     pl.col(c) == 'N'
                     ).count().over(d).alias('EXCLUDED')
                 , pl.col(e).filter(
                     pl.col(e) == 'Y'
                     ).count().over(d).alias('SALE AVLB')
                 , pl.col(e).filter(
                     pl.col(e) == 'N'
-                    ).count().over('RETAILER_GEO_ID').alias('SALE UNAVLB')
+                    ).count().over(d).alias('SALE UNAVLB')
                 , pl.col(f).filter(
                     pl.col(f) == 'Y'
-                ).count().over(d).alias('SALE IN TREND')
+                    ).count().over(d).alias('SALE IN TREND')
                 , pl.col(f).filter(
                     pl.col(f) == 'N'
-                ).count().over(d).alias('SALE NOT IN TREND')
+                    ).count().over(d).alias('SALE NOT IN TREND')
                 , pl.col(g).filter(
                     pl.col(g) == 'Y'
-                ).count().over(d).alias('INV IN TREND')
+                    ).count().over(d).alias('INV IN TREND')
                 , pl.col(g).filter(
                     pl.col(g) == 'N'
-                ).count().over(d).alias('INV NOT IN TREND')
+                    ).count().over(d).alias('INV NOT IN TREND')
 
 
             ])
         ).select([h, 'Total Retailers', 'INCLUDED', 'EXCLUDED', 'SALE AVLB', 'SALE UNAVLB',
                   'SALE IN TREND', 'SALE NOT IN TREND', 'INV IN TREND', 'INV NOT IN TREND']).unique()
 
         df_count = (df_count
```

### Comparing `NikeCA-0.1.61/src/_QA.py` & `NikeCA-0.1.62/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_SearchFiles.py` & `NikeCA-0.1.62/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_SnowflakeData.py` & `NikeCA-0.1.62/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import _BuildSearchQuery
 import _SnowflakePull
 import _SnowflakeDependencies
-import _Dashboards
+from Dashboards import _Dashboards
 
 
 class SnowflakeData(_Dashboards.Dashboards
                     , _SnowflakePull.SnowflakePull
                     , _SnowflakeDependencies.SnowflakeDependencies
                     , _BuildSearchQuery.BuildSearchQuery):
```

### Comparing `NikeCA-0.1.61/src/_SnowflakeDependencies.py` & `NikeCA-0.1.62/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.61/src/_SnowflakePull.py` & `NikeCA-0.1.62/src/_SnowflakePull.py`

 * *Files identical despite different names*

