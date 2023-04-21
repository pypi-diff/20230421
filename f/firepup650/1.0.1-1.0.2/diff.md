# Comparing `tmp/firepup650-1.0.1.tar.gz` & `tmp/firepup650-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepup650-1.0.1.tar", last modified: Thu Apr 20 13:49:39 2023, max compression
+gzip compressed data, was "firepup650-1.0.2.tar", last modified: Fri Apr 21 00:01:47 2023, max compression
```

## Comparing `firepup650-1.0.1.tar` & `firepup650-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-20 13:49:39.808548 firepup650-1.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1114 2023-04-20 13:49:39.808548 firepup650-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-04-20 13:48:55.000000 firepup650-1.0.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 firepup650-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-20 13:49:39.808548 firepup650-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-20 13:49:39.800547 firepup650-1.0.1/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-20 13:49:39.808548 firepup650-1.0.1/src/firepup650/
--rw-r--r--   0 runner    (1000) runner    (1000)     2776 2023-04-20 13:46:29.000000 firepup650-1.0.1/src/firepup650/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-20 13:49:39.808548 firepup650-1.0.1/src/firepup650.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1114 2023-04-20 13:49:39.000000 firepup650-1.0.1/src/firepup650.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-20 13:49:39.000000 firepup650-1.0.1/src/firepup650.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-20 13:49:39.000000 firepup650-1.0.1/src/firepup650.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-20 13:49:39.000000 firepup650-1.0.1/src/firepup650.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 00:01:47.432061 firepup650-1.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1176 2023-04-21 00:01:47.432061 firepup650-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      261 2023-04-21 00:00:22.000000 firepup650-1.0.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 firepup650-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-21 00:01:47.432061 firepup650-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 00:01:47.424061 firepup650-1.0.2/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 00:01:47.428061 firepup650-1.0.2/src/firepup650/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3340 2023-04-20 17:40:25.000000 firepup650-1.0.2/src/firepup650/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 00:01:47.432061 firepup650-1.0.2/src/firepup650.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1176 2023-04-21 00:01:46.000000 firepup650-1.0.2/src/firepup650.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-21 00:01:47.000000 firepup650-1.0.2/src/firepup650.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-21 00:01:46.000000 firepup650-1.0.2/src/firepup650.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-21 00:01:46.000000 firepup650-1.0.2/src/firepup650.egg-info/top_level.txt
```

### Comparing `firepup650-1.0.1/LICENSE` & `firepup650-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.1/PKG-INFO` & `firepup650-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.2:
+        Random shorthand (litterally)
         ###### v.1.0.1:
         Added animated typing function, sleep shorthand
         ###### v.1.0.0:
         Initial Release!
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `firepup650-1.0.1/setup.cfg` & `firepup650-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = firepup650
-version = 1.0.1
+version = 1.0.2
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = Package containing various shorthand things I use, and a few imports I almost always use
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/firepup650-PYPI
 project_urls =
```

### Comparing `firepup650-1.0.1/src/firepup650/__init__.py` & `firepup650-1.0.2/src/firepup650/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Firepup650's PYPI Package"""
 import os, sys, termios, tty, time
 import random as r
 import fkeycapture as fkey
+from collections import Sequence
 def clear() -> None:
   """# Function: clear
     Clears the screen
   # Inputs:
     None
 
   # Returns:
@@ -110,8 +111,29 @@
     seconds: float - How long to sleep for (in seconds), defaults to 0.5
   
   # Returns:
     None
   
   # Raises:
     None"""
-  time.sleep(seconds)
+  time.sleep(seconds)
+def rseed(seed: any = None, version: int = 2) -> None:
+  """# Function: rseed
+    reseed the random number generator
+  # Inputs:
+    seed: any - The seed, defaults to None
+    version: int - Version of the seed (1 or 2), defaults to 2
+  
+  # Returns:
+    None
+  
+  # Raises:
+    None"""
+  r.seed(seed, version)
+def robj(sequence: Sequence[object]) -> object:
+  """# Function: robj
+    Returns a random object from the provided sequence
+  # Input:
+    sequence: Sequence[object] - Any valid sequence
+  
+  # """
+  r.choice(sequence)
```

### Comparing `firepup650-1.0.1/src/firepup650.egg-info/PKG-INFO` & `firepup650-1.0.2/src/firepup650.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.2:
+        Random shorthand (litterally)
         ###### v.1.0.1:
         Added animated typing function, sleep shorthand
         ###### v.1.0.0:
         Initial Release!
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

