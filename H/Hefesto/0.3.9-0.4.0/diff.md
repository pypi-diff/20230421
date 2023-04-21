# Comparing `tmp/Hefesto-0.3.9.tar.gz` & `tmp/Hefesto-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.3.9.tar", last modified: Wed Apr 19 08:27:39 2023, max compression
+gzip compressed data, was "Hefesto-0.4.0.tar", last modified: Fri Apr 21 09:51:58 2023, max compression
```

## Comparing `Hefesto-0.3.9.tar` & `Hefesto-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.3.9/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12019 2023-04-19 08:22:40.000000 Hefesto-0.3.9/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8595 2023-04-19 07:55:36.000000 Hefesto-0.3.9/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.3.9/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-19 08:27:39.389428 Hefesto-0.3.9/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.3.9/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.3.9/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-04-19 08:27:39.389428 Hefesto-0.3.9/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-04-19 08:27:35.000000 Hefesto-0.3.9/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.0/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11950 2023-04-21 09:50:03.000000 Hefesto-0.4.0/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8594 2023-04-21 09:41:24.000000 Hefesto-0.4.0/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.0/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-21 09:51:58.443345 Hefesto-0.4.0/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.0/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.0/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-04-21 09:51:58.443345 Hefesto-0.4.0/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-04-21 09:51:44.000000 Hefesto-0.4.0/setup.py
```

### Comparing `Hefesto-0.3.9/Hefesto/main.py` & `Hefesto-0.4.0/Hefesto/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from perseo.main import milisec
-# from template import Template
-from Hefesto.template import Template
+from template import Template
+# from Hefesto.template import Template
 import sys
 import yaml
 import math
 import requests
 
 class Hefesto():
 
@@ -162,30 +162,26 @@
         for index, row in resulting_df.iterrows():
             for k,v in datatype_relationship.items():
                 
 
                 # value ---> value_DATATYPE:
                 if row["value_datatype"] == k:
                     resulting_df.at[index, v] = resulting_df["value"][index]
-
-                # # valueIRI ---> process_type for Disability
-                # if row["model"] == "Disability" and row["valueIRI"] != None:
-                #     resulting_df.at[index, "process_type"] = resulting_df["valueIRI"][index]
-                #     resulting_df["valueIRI"][index] = None
+                    resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
                 # enddate correction:
                 if row["startdate"] != None and row["enddate"] == None:
                     resulting_df["enddate"][index] = resulting_df["startdate"][index]
+                    resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
 
         # clean blanks
         for row_final in resulting_df.iterrows():
-            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None:
+            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
                 resulting_df = resulting_df.drop(row_final[0])
-                
         del resulting_df["value"]
 
 
         # # valueIRI ---> valueAttributeIRI:
         # del resulting_df["valueAttributeIRI"]
         # resulting_df.rename(columns={'valueIRI':'valueAttributeIRI'}, inplace=True)
```

### Comparing `Hefesto-0.3.9/Hefesto/template.py` & `Hefesto-0.4.0/Hefesto/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,12 +276,12 @@
       agent_type = "http://purl.obolibrary.org/obo/NCIT_C177929",
       value_datatype= "xsd:float",
       startdate= None ,
       enddate = None ,
       comments = None ,
       pid = None ,
       context_id = None 
-    ),
+    )
 
 
   )
```

### Comparing `Hefesto-0.3.9/README.md` & `Hefesto-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.3.9/setup.py` & `Hefesto-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.3.9",
+    version="0.4.0",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

