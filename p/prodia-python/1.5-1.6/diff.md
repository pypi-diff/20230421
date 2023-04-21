# Comparing `tmp/prodia-python-1.5.tar.gz` & `tmp/prodia-python-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodia-python-1.5.tar", last modified: Fri Apr 21 19:09:56 2023, max compression
+gzip compressed data, was "prodia-python-1.6.tar", last modified: Fri Apr 21 19:13:22 2023, max compression
```

## Comparing `prodia-python-1.5.tar` & `prodia-python-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:09:56.930176 prodia-python-1.5/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-1.5/LICENSE
--rw-rw-rw-   0        0        0     1695 2023-04-21 19:09:56.930176 prodia-python-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1469 2023-04-21 18:41:23.000000 prodia-python-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 19:09:56.917975 prodia-python-1.5/prodia/
--rw-rw-rw-   0        0        0       35 2023-04-21 18:53:57.000000 prodia-python-1.5/prodia/__init__.py
--rw-rw-rw-   0        0        0     1873 2023-04-21 18:54:11.000000 prodia-python-1.5/prodia/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:09:56.928108 prodia-python-1.5/prodia_python.egg-info/
--rw-rw-rw-   0        0        0     1695 2023-04-21 19:09:56.000000 prodia-python-1.5/prodia_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-21 19:09:56.000000 prodia-python-1.5/prodia_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:09:56.000000 prodia-python-1.5/prodia_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 19:09:56.000000 prodia-python-1.5/prodia_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 19:09:56.000000 prodia-python-1.5/prodia_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 19:09:56.930923 prodia-python-1.5/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-04-21 19:09:25.000000 prodia-python-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.367084 prodia-python-1.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-1.6/LICENSE
+-rw-rw-rw-   0        0        0     1741 2023-04-21 19:13:22.366566 prodia-python-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1515 2023-04-21 19:12:58.000000 prodia-python-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.358615 prodia-python-1.6/prodia/
+-rw-rw-rw-   0        0        0       35 2023-04-21 18:53:57.000000 prodia-python-1.6/prodia/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-04-21 19:12:05.000000 prodia-python-1.6/prodia/run.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.365075 prodia-python-1.6/prodia_python.egg-info/
+-rw-rw-rw-   0        0        0     1741 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:13:22.367084 prodia-python-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-04-21 19:12:54.000000 prodia-python-1.6/setup.py
```

### Comparing `prodia-python-1.5/LICENSE` & `prodia-python-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prodia-python-1.5/PKG-INFO` & `prodia-python-1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 1.5
+Version: 1.6
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
 pip install git+https://github.com/yoou3-cyber/prodia-python
 ```
+or
+```
+pip install prodia-python==1.6
+```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of usage
 ```python
 import prodia
```

### Comparing `prodia-python-1.5/README.md` & `prodia-python-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
 pip install git+https://github.com/yoou3-cyber/prodia-python
 ```
+or
+```
+pip install prodia-python==1.6
+```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of usage
 ```python
 import prodia
```

### Comparing `prodia-python-1.5/prodia/run.py` & `prodia-python-1.6/prodia/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 def run(key=None, prompt="kittens on cloud", negative_prompt="", model="v1-5-pruned-emaonly.ckpt [81761151]", sampler="Euler", aspect_ratio="square", steps=25, cfg_scale=7, seed=-1, upscale=False):
     if key is None:
         print("API key cant be None, get your API kay at https://app.prodia.com/api")
     else:
         if prompt=="kittens on cloud":
-            print("Prompt not defined, used default (kittens on cloud))
+            print("Prompt not defined, used default (kittens on cloud)")
         url = "https://api.prodia.com/v1/job"
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
```

### Comparing `prodia-python-1.5/prodia_python.egg-info/PKG-INFO` & `prodia-python-1.6/prodia_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 1.5
+Version: 1.6
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
 pip install git+https://github.com/yoou3-cyber/prodia-python
 ```
+or
+```
+pip install prodia-python==1.6
+```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of usage
 ```python
 import prodia
```

