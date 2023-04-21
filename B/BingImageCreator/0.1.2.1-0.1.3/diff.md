# Comparing `tmp/BingImageCreator-0.1.2.1.tar.gz` & `tmp/BingImageCreator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.1.2.1.tar", last modified: Fri Apr  7 02:57:24 2023, max compression
+gzip compressed data, was "BingImageCreator-0.1.3.tar", last modified: Fri Apr 21 10:17:24 2023, max compression
```

## Comparing `BingImageCreator-0.1.2.1.tar` & `BingImageCreator-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:57:24.208852 BingImageCreator-0.1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 02:57:03.000000 BingImageCreator-0.1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-07 02:57:24.208852 BingImageCreator-0.1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-07 02:57:03.000000 BingImageCreator-0.1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 02:57:24.208852 BingImageCreator-0.1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-07 02:57:03.000000 BingImageCreator-0.1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:57:24.208852 BingImageCreator-0.1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:57:24.208852 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-07 02:57:24.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-07 02:57:24.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 02:57:24.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-07 02:57:24.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-07 02:57:24.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-07 02:57:03.000000 BingImageCreator-0.1.2.1/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.153638 BingImageCreator-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/src/BingImageCreator.py
```

### Comparing `BingImageCreator-0.1.2.1/LICENSE` & `BingImageCreator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.2.1/PKG-INFO` & `BingImageCreator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.2.1
+Version: 0.1.3
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.2.1/README.md` & `BingImageCreator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.2.1/setup.py` & `BingImageCreator-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.1.2.1",
+    version="0.1.3",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
     project_urls={
         "Bug Report": "https://github.com/acheong08/BingImageCreator/issues/new",
     },
     install_requires=[
+        "aiohttp",
         "regex",
         "requests",
     ],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["BingImageCreator"],
     classifiers=[
```

### Comparing `BingImageCreator-0.1.2.1/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.1.3/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.2.1
+Version: 0.1.3
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.2.1/src/BingImageCreator.py` & `BingImageCreator-0.1.3/src/BingImageCreator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import sys
 import time
 import aiohttp
 import pkg_resources
 import regex
 import requests
 from typing import Union
-
-BING_URL = "https://www.bing.com"
+if(os.environ.get('BING_URL') == None):
+    BING_URL = "https://www.bing.com"
+else:
+    BING_URL = os.environ.get('BING_URL')
 # Generate random IP between range 13.104.0.0/14
 FORWARDED_IP = (
     f"13.{random.randint(104, 107)}.{random.randint(0, 255)}.{random.randint(0, 255)}"
 )
 HEADERS = {
     "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "accept-language": "en-US,en;q=0.9",
```

