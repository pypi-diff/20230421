# Comparing `tmp/alacorder-79.5.6.tar.gz` & `tmp/alacorder-79.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.5.6.tar", max compression
+gzip compressed data, was "alacorder-79.5.7.tar", max compression
```

## Comparing `alacorder-79.5.6.tar` & `alacorder-79.5.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.5.6/LICENSE
--rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.5.6/README.md
--rw-r--r--   0        0        0      682 2023-04-20 13:54:01.080981 alacorder-79.5.6/pyproject.toml
--rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.5.6/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.5.6/src/alacorder/.python-version
--rw-r--r--   0        0        0     2157 2023-04-19 22:05:38.789380 alacorder-79.5.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   136382 2023-04-20 13:53:28.692686 alacorder-79.5.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   136382 2023-04-20 13:53:33.358090 alacorder-79.5.6/src/alacorder/alac.py
--rw-r--r--   0        0        0   136381 2023-04-20 13:53:39.633924 alacorder-79.5.6/src/alacorder/gui.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.5.6/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 alacorder-79.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.5.7/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.5.7/README.md
+-rw-r--r--   0        0        0      682 2023-04-20 15:02:34.700929 alacorder-79.5.7/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.5.7/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.5.7/src/alacorder/.python-version
+-rw-r--r--   0        0        0     2157 2023-04-19 22:05:38.789380 alacorder-79.5.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   136382 2023-04-20 15:01:27.553911 alacorder-79.5.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   136382 2023-04-20 15:00:34.925298 alacorder-79.5.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.5.7/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 alacorder-79.5.7/PKG-INFO
```

### Comparing `alacorder-79.5.6/LICENSE` & `alacorder-79.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.6/README.md` & `alacorder-79.5.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.6/pyproject.toml` & `alacorder-79.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.5.6"
+version = "79.5.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.5.6/src/alacorder/__init__.py` & `alacorder-79.5.7/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.6/src/alacorder/__main__.py` & `alacorder-79.5.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.5.6"
+version = "79.5.7"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
@@ -2813,15 +2813,15 @@
 
     # add other temp columns as empty
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
     if goodquery:
-        print(f"{query.shape[1]} queries found in input query file.")
+        print(f"{query.shape[0]} queries found in input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
```

### Comparing `alacorder-79.5.6/src/alacorder/alac.py` & `alacorder-79.5.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.5.6"
+version = "79.5.7"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
@@ -2813,15 +2813,15 @@
 
     # add other temp columns as empty
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
     if goodquery:
-        print(f"{query.shape[1]} queries found in input query file.")
+        print(f"{query.shape[0]} queries found in input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
```

### Comparing `alacorder-79.5.6/PKG-INFO` & `alacorder-79.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.5.6
+Version: 79.5.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

