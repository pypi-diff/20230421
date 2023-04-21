# Comparing `tmp/nudeny-0.0.5.tar.gz` & `tmp/nudeny-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudeny-0.0.5.tar", max compression
+gzip compressed data, was "nudeny-0.0.6.tar", max compression
```

## Comparing `nudeny-0.0.5.tar` & `nudeny-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1091 2023-03-15 12:14:48.958841 nudeny-0.0.5/LICENSE
--rw-r--r--   0        0        0      527 2023-03-15 16:07:14.205875 nudeny-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-15 16:07:07.562311 nudeny-0.0.5/src/nudeny/__init__.py
--rw-r--r--   0        0        0     5185 2023-03-07 13:37:17.790160 nudeny-0.0.5/src/nudeny/nudeny.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-25 16:00:24.478955 nudeny-0.0.6/LICENSE
+-rw-r--r--   0        0        0      527 2023-04-21 16:36:09.058748 nudeny-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-03-25 16:00:24.478955 nudeny-0.0.6/src/nudeny/__init__.py
+-rw-r--r--   0        0        0     5281 2023-04-21 16:35:44.022507 nudeny-0.0.6/src/nudeny/nudeny.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.6/PKG-INFO
```

### Comparing `nudeny-0.0.5/LICENSE` & `nudeny-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nudeny-0.0.5/pyproject.toml` & `nudeny-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Nudeny"
-version = "0.0.5"
+version = "0.0.6"
 description = "Image nudity classification and detection package."
 authors = ["Nudeny <thesis.nudeny69@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Nudeny/Nudeny-python-module"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `nudeny-0.0.5/src/nudeny/nudeny.py` & `nudeny-0.0.6/src/nudeny/nudeny.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import requests
 from urllib.parse import urlparse
 from PIL import Image
 
 class Classify:
     def __init__(self):
-        self.URL = "http://127.0.0.1:8000/"
+        self.LOCALHOST_URL = "http://127.0.0.1:8000/"
+        self.URL = "http://ec2-18-142-227-173.ap-southeast-1.compute.amazonaws.com/"
     
     def imageClassify(self, paths=[]):
         """
         Classify an image, from path provided, if it contains nudity, or if it is sexy or safe.
 
         Args:
             paths (list): List of Image path
```

### Comparing `nudeny-0.0.5/PKG-INFO` & `nudeny-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudeny
-Version: 0.0.5
+Version: 0.0.6
 Summary: Image nudity classification and detection package.
 Home-page: https://github.com/Nudeny/Nudeny-python-module
 License: MIT
 Author: Nudeny
 Author-email: thesis.nudeny69@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

