# Comparing `tmp/kalm-0.1.4.tar.gz` & `tmp/kalm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.1.4.tar", last modified: Fri Apr 21 10:38:42 2023, max compression
+gzip compressed data, was "kalm-0.1.5.tar", last modified: Fri Apr 21 10:42:25 2023, max compression
```

## Comparing `kalm-0.1.4.tar` & `kalm-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/
--rw-rw-r--   0 jho       (1000) jho       (1000)     1081 2023-04-21 06:37:05.000000 kalm-0.1.4/LICENSE.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:38:42.318096 kalm-0.1.4/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      705 2023-04-21 06:37:05.000000 kalm-0.1.4/README.md
--rw-rw-r--   0 jho       (1000) jho       (1000)     1282 2023-04-21 10:38:35.000000 kalm-0.1.4/pyproject.toml
--rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:38:42.318096 kalm-0.1.4/setup.cfg
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.316096 kalm-0.1.4/src/
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.317096 kalm-0.1.4/src/kalm/
--rw-rw-r--   0 jho       (1000) jho       (1000)    10449 2023-04-21 06:51:36.000000 kalm-0.1.4/src/kalm/__init__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)    31998 2023-04-21 06:53:06.000000 kalm-0.1.4/src/kalm/kalm.py
--rw-rw-r--   0 jho       (1000) jho       (1000)     1296 2023-04-21 06:37:05.000000 kalm-0.1.4/src/kalm/netbox.py
--rw-rw-r--   0 jho       (1000) jho       (1000)        9 2023-04-21 06:37:05.000000 kalm-0.1.4/src/kalm/package_data.dat
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:41:48.000000 kalm-0.1.4/src/kalm/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/src/kalm.egg-info/
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      377 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/SOURCES.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/dependency_links.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       35 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/entry_points.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/requires.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       13 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/top_level.txt
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/src/toolbox/
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:46:41.000000 kalm-0.1.4/src/toolbox/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/tests/
--rw-rw-r--   0 jho       (1000) jho       (1000)      417 2023-04-21 06:37:05.000000 kalm-0.1.4/tests/test_simple.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1081 2023-04-21 06:37:05.000000 kalm-0.1.5/LICENSE.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:42:25.813122 kalm-0.1.5/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)      705 2023-04-21 06:37:05.000000 kalm-0.1.5/README.md
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1282 2023-04-21 10:41:59.000000 kalm-0.1.5/pyproject.toml
+-rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:42:25.813122 kalm-0.1.5/setup.cfg
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.811123 kalm-0.1.5/src/
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.812122 kalm-0.1.5/src/kalm/
+-rw-rw-r--   0 jho       (1000) jho       (1000)    10421 2023-04-21 10:40:56.000000 kalm-0.1.5/src/kalm/__init__.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)    32279 2023-04-21 10:40:49.000000 kalm-0.1.5/src/kalm/kalm.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1296 2023-04-21 06:37:05.000000 kalm-0.1.5/src/kalm/netbox.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)        9 2023-04-21 06:37:05.000000 kalm-0.1.5/src/kalm/package_data.dat
+-rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:41:48.000000 kalm-0.1.5/src/kalm/toolbox.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/src/kalm.egg-info/
+-rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)      377 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       35 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/entry_points.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/requires.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       13 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/top_level.txt
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/src/toolbox/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:46:41.000000 kalm-0.1.5/src/toolbox/toolbox.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/tests/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      417 2023-04-21 06:37:05.000000 kalm-0.1.5/tests/test_simple.py
```

### Comparing `kalm-0.1.4/LICENSE.txt` & `kalm-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.1.4/PKG-INFO` & `kalm-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Jakob Holst <jho@miracle.dk>
 Maintainer-email: Jakob Holst <jho@miracle.dk>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `kalm-0.1.4/README.md` & `kalm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kalm-0.1.4/pyproject.toml` & `kalm-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kalm"  
-version = "0.1.4" 
+version = "0.1.5" 
 description = "" 
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.1.4/src/kalm/__init__.py` & `kalm-0.1.5/src/kalm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from kalm import kalm
-from kalm import prettyllog
 import os
 import sys
 import redis
 import time
 import subprocess
 import json
 import argparse
```

### Comparing `kalm-0.1.4/src/kalm/kalm.py` & `kalm-0.1.5/src/kalm/kalm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 import json
 import requests
 import hvac
 import os
 import sys
 import datetime
 import pynetbox
-from toolbox import prettyllog
+import datetime
+
+def prettyllog(function, action, item, organization, statuscode, text):
+  d_date = datetime.datetime.now()
+  reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
+  print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
+  
 
 
 #def prettyllog(function, action, item, organization, statuscode, text):
  # d_date = datetime.datetime.now()
  # reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
  # print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
```

### Comparing `kalm-0.1.4/src/kalm/netbox.py` & `kalm-0.1.5/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.1.4/src/kalm.egg-info/PKG-INFO` & `kalm-0.1.5/src/kalm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Jakob Holst <jho@miracle.dk>
 Maintainer-email: Jakob Holst <jho@miracle.dk>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

