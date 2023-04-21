# Comparing `tmp/prodia-python-1.1.tar.gz` & `tmp/prodia-python-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodia-python-1.1.tar", last modified: Fri Apr 21 18:51:28 2023, max compression
+gzip compressed data, was "prodia-python-1.2.tar", last modified: Fri Apr 21 18:56:42 2023, max compression
```

## Comparing `prodia-python-1.1.tar` & `prodia-python-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:51:28.648040 prodia-python-1.1/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-1.1/LICENSE
--rw-rw-rw-   0        0        0      196 2023-04-21 18:51:28.647042 prodia-python-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1469 2023-04-21 18:41:23.000000 prodia-python-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 18:51:28.640207 prodia-python-1.1/prodia/
--rw-rw-rw-   0        0        0       54 2023-04-21 18:41:23.000000 prodia-python-1.1/prodia/__init__.py
--rw-rw-rw-   0        0        0     1873 2023-04-21 18:49:45.000000 prodia-python-1.1/prodia/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:51:28.646039 prodia-python-1.1/prodia_python.egg-info/
--rw-rw-rw-   0        0        0      196 2023-04-21 18:51:28.000000 prodia-python-1.1/prodia_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-21 18:51:28.000000 prodia-python-1.1/prodia_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:51:28.000000 prodia-python-1.1/prodia_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:51:28.000000 prodia-python-1.1/prodia_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 18:51:28.000000 prodia-python-1.1/prodia_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:51:28.648040 prodia-python-1.1/setup.cfg
--rw-rw-rw-   0        0        0      276 2023-04-21 18:51:02.000000 prodia-python-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:56:42.294522 prodia-python-1.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-1.2/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-04-21 18:56:42.294522 prodia-python-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1469 2023-04-21 18:41:23.000000 prodia-python-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 18:56:42.286523 prodia-python-1.2/prodia/
+-rw-rw-rw-   0        0        0       35 2023-04-21 18:53:57.000000 prodia-python-1.2/prodia/__init__.py
+-rw-rw-rw-   0        0        0     1873 2023-04-21 18:54:11.000000 prodia-python-1.2/prodia/run.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:56:42.293525 prodia-python-1.2/prodia_python.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-04-21 18:56:42.000000 prodia-python-1.2/prodia_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-21 18:56:42.000000 prodia-python-1.2/prodia_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:56:42.000000 prodia-python-1.2/prodia_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:56:42.000000 prodia-python-1.2/prodia_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 18:56:42.000000 prodia-python-1.2/prodia_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:56:42.294522 prodia-python-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      276 2023-04-21 18:56:19.000000 prodia-python-1.2/setup.py
```

### Comparing `prodia-python-1.1/LICENSE` & `prodia-python-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prodia-python-1.1/README.md` & `prodia-python-1.2/README.md`

 * *Files identical despite different names*

### Comparing `prodia-python-1.1/prodia/run.py` & `prodia-python-1.2/prodia/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 def run(key=None, prompt="kittens on cloud", negative_prompt="", model="v1-5-pruned-emaonly.ckpt [81761151]", sampler="Euler", aspect_ratio="square", steps=25, cfg_scale=7, seed=-1, upscale=False):
     if key is None:
         print("API key cant be None, get your API kay at https://app.prodia.com/api")
     else:
         if prompt=="kittens on cloud":
-            print("Prompt not defined, used default 'kittens on cloud')
+            print("Prompt not defined, used default (kittens on cloud))
         url = "https://api.prodia.com/v1/job"
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
```

