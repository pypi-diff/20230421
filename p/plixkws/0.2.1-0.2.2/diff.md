# Comparing `tmp/plixkws-0.2.1.tar.gz` & `tmp/plixkws-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plixkws-0.2.1.tar", last modified: Fri Apr 21 19:50:15 2023, max compression
+gzip compressed data, was "plixkws-0.2.2.tar", last modified: Fri Apr 21 19:50:56 2023, max compression
```

## Comparing `plixkws-0.2.1.tar` & `plixkws-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:50:15.415238 plixkws-0.2.1/
--rw-rw-rw-   0        0        0    11558 2023-04-20 10:09:41.000000 plixkws-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3893 2023-04-21 19:50:15.415238 plixkws-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3405 2023-04-20 11:51:09.000000 plixkws-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 19:50:15.395075 plixkws-0.2.1/plixkws/
--rw-rw-rw-   0        0        0     1374 2023-04-20 10:08:27.000000 plixkws-0.2.1/plixkws/backbone.py
--rw-rw-rw-   0        0        0     1470 2023-04-21 19:48:17.000000 plixkws-0.2.1/plixkws/model.py
--rw-rw-rw-   0        0        0     2099 2023-04-20 10:08:27.000000 plixkws-0.2.1/plixkws/protonet.py
--rw-rw-rw-   0        0        0     1536 2023-04-20 10:08:27.000000 plixkws-0.2.1/plixkws/util.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:50:15.415238 plixkws-0.2.1/plixkws.egg-info/
--rw-rw-rw-   0        0        0     3893 2023-04-21 19:50:15.000000 plixkws-0.2.1/plixkws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-21 19:50:15.000000 plixkws-0.2.1/plixkws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:50:15.000000 plixkws-0.2.1/plixkws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-21 19:50:15.000000 plixkws-0.2.1/plixkws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 19:50:15.000000 plixkws-0.2.1/plixkws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 19:50:15.415238 plixkws-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-04-21 19:50:09.000000 plixkws-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:50:56.175931 plixkws-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-20 10:09:41.000000 plixkws-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3893 2023-04-21 19:50:56.175931 plixkws-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3405 2023-04-20 11:51:09.000000 plixkws-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:50:56.154569 plixkws-0.2.2/plixkws/
+-rw-rw-rw-   0        0        0     1374 2023-04-20 10:08:27.000000 plixkws-0.2.2/plixkws/backbone.py
+-rw-rw-rw-   0        0        0     1470 2023-04-21 19:48:17.000000 plixkws-0.2.2/plixkws/model.py
+-rw-rw-rw-   0        0        0     2099 2023-04-20 10:08:27.000000 plixkws-0.2.2/plixkws/protonet.py
+-rw-rw-rw-   0        0        0     1536 2023-04-20 10:08:27.000000 plixkws-0.2.2/plixkws/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:50:56.175931 plixkws-0.2.2/plixkws.egg-info/
+-rw-rw-rw-   0        0        0     3893 2023-04-21 19:50:55.000000 plixkws-0.2.2/plixkws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-21 19:50:56.000000 plixkws-0.2.2/plixkws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:50:55.000000 plixkws-0.2.2/plixkws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-21 19:50:55.000000 plixkws-0.2.2/plixkws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 19:50:55.000000 plixkws-0.2.2/plixkws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:50:56.178668 plixkws-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-04-21 19:50:47.000000 plixkws-0.2.2/setup.py
```

### Comparing `plixkws-0.2.1/LICENSE` & `plixkws-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/PKG-INFO` & `plixkws-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plixkws
-Version: 0.2.1
+Version: 0.2.2
 Summary: Plug-and-Play Multilingual Few-shot Spoken Words Recognition
 Home-page: https://github.com/FewshotML/plix
 Download-URL: https://pypi.org/project/plixkws/
 Author: Aaqib Saeed
 Author-email: plix-kws@proton.me
 License: Apache-2.0
 Keywords: Keyword Spotting,Few-shot Learning,Deep Neural Network,Audio,Speech
```

### Comparing `plixkws-0.2.1/README.md` & `plixkws-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/plixkws/backbone.py` & `plixkws-0.2.2/plixkws/backbone.py`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/plixkws/model.py` & `plixkws-0.2.2/plixkws/model.py`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/plixkws/protonet.py` & `plixkws-0.2.2/plixkws/protonet.py`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/plixkws/util.py` & `plixkws-0.2.2/plixkws/util.py`

 * *Files identical despite different names*

### Comparing `plixkws-0.2.1/plixkws.egg-info/PKG-INFO` & `plixkws-0.2.2/plixkws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plixkws
-Version: 0.2.1
+Version: 0.2.2
 Summary: Plug-and-Play Multilingual Few-shot Spoken Words Recognition
 Home-page: https://github.com/FewshotML/plix
 Download-URL: https://pypi.org/project/plixkws/
 Author: Aaqib Saeed
 Author-email: plix-kws@proton.me
 License: Apache-2.0
 Keywords: Keyword Spotting,Few-shot Learning,Deep Neural Network,Audio,Speech
```

### Comparing `plixkws-0.2.1/setup.py` & `plixkws-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name="plixkws",
-    version="0.2.1",
+    version="0.2.2",
     description="Plug-and-Play Multilingual Few-shot Spoken Words Recognition",
     long_description_content_type="text/markdown",
     long_description=README,
     license="Apache-2.0",
     packages=['plixkws'],
     author="Aaqib Saeed",
     author_email="plix-kws@proton.me",
```

