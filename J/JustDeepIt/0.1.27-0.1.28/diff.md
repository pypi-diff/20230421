# Comparing `tmp/JustDeepIt-0.1.27.tar.gz` & `tmp/JustDeepIt-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.1.27.tar", last modified: Wed Apr 12 05:40:29 2023, max compression
+gzip compressed data, was "JustDeepIt-0.1.28.tar", last modified: Fri Apr 21 02:33:07 2023, max compression
```

## Comparing `JustDeepIt-0.1.27.tar` & `JustDeepIt-0.1.28.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.481672 JustDeepIt-0.1.27/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.481672 JustDeepIt-0.1.27/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/detectron2base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.485672 JustDeepIt-0.1.27/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55796 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.485672 JustDeepIt-0.1.27/justdeepit/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appod.py
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/justdeepit/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    23287 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/justdeepit/webapp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.968196 JustDeepIt-0.1.28/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/detectron2base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.960196 JustDeepIt-0.1.28/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.968196 JustDeepIt-0.1.28/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    56340 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.972196 JustDeepIt-0.1.28/justdeepit/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/justdeepit/webapp/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/justdeepit/webapp/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/shutdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/setup.py
```

### Comparing `JustDeepIt-0.1.27/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.1.28/JustDeepIt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.27
+Version: 0.1.28
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.27/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.1.28/JustDeepIt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/LICENSE` & `JustDeepIt-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/PKG-INFO` & `JustDeepIt-0.1.28/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.27
+Version: 0.1.28
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.27/README.md` & `JustDeepIt-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/models/instance_segment.py` & `JustDeepIt-0.1.28/justdeepit/models/instance_segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
+import glob
 import pkg_resources
+from justdeepit.utils import ImageAnnotation, ImageAnnotations
 
 class IS:
     """A class to generate model for instance segmentation
 
     The :class:`IS <justdeepit.models.IS>` class is used for generating
     deep neural network (DNN) architectures (i.e., models) for instance segmentation
     by internally calling the MMDetection or Detectron2 library.
@@ -61,15 +63,16 @@
     """  
     
     
     def __init__(self, class_label=None, model_arch=None, model_config=None, model_weight=None, workspace=None, backend='mmdetection'):
         
         self.module = None
         self.__architectures = self.__available_architectures()
-        self.__supported_formats = ('COCO',) #, 'RGB mask')
+        self.__supported_formats = ('COCO', 'VoTT') #, 'RGB mask')
+        self.__image_ext = ['.jpg', '.jpeg', '.png', '.tif', '.tiff']
         
         self.backend = backend
         self.model_arch = model_arch
         if workspace is None:
             workspace = os.path.abspath(os.getcwd())
         self.workspace = workspace
         self.module = self.__init_module(class_label, model_arch, model_config, model_weight, workspace, backend)
@@ -207,15 +210,15 @@
         The training images (``image_dpath``), annotation files (``annotation``),
         and annotation format (``annotation_format``) must be specified.
         Note that, the current version of JustDeepIt only supports COCO format.
         
         Args:
             image_dpath (str): A path to directory which contains all training images.
             annotation (str): A file path to COCO format annotation file.
-            annotation_format (str): Annotation format. Only COCO is supported in the current version.
+            annotation_format (str): Annotation format. COCO or VoTT are supported in the current version.
             optimizer (str): String to specify optimizer/solver supported by MMDetection or Detectron2.
             scheduler (str): String to specify optimization scheduler.
             batchsize (int): Batch size for each GPU.
             epoch (int): Epoch.
             score_cutoff (float): Cutoff of score for instance segmentation.
             cpu (int): Number of workers for pre-prociessing images for each GPU.
             gpu (int): Number of GPUs for model training.
@@ -223,15 +226,26 @@
         Examples:
             >>> from justdeepit.models import IS 
             >>> 
             >>> model = IS('./class_label.txt', model_arch='maskrcnn')
             >>> model.train('./train_images', './annotations.coco.json', 'COCO')
         """
         annotation_format = self.__norm_format(annotation_format)
-        if annotation_format != 'coco':
+        if annotation_format == 'coco':
+            pass
+        elif annotation_format == 'vott':
+            anns = ImageAnnotations()
+            for fpath in glob.glob(os.path.join(image_dpath, '*')):
+                fname, fext = os.path.splitext(os.path.basename(fpath))
+                if fext.lower() in self.__image_ext:
+                    anns.append(ImageAnnotation(fpath, annotation))
+            if len(anns) > 0:
+                annotation = os.path.join(self.workspace, 'train_image_annotation.coco.json')
+                anns.format('coco', annotation)
+        else:
             raise NotImplementedError('JustDeepIt does not support {} format for training instance segmentation model.'.format(annotation_format))
         
         self.module.train(image_dpath, annotation,
                           optimizer, scheduler,
                           batchsize=batchsize, epoch=epoch, score_cutoff=score_cutoff,
                           cpu=cpu, gpu=gpu)
```

### Comparing `JustDeepIt-0.1.27/justdeepit/models/object_detect.py` & `JustDeepIt-0.1.28/justdeepit/models/object_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     
     def __init__(self, class_label=None,
                  model_arch=None, model_config=None, model_weight=None,
                  workspace=None, backend='mmdetection'):
         
         self.module = None
         self.__architectures = self.__available_architectures()
-        self.__supported_formats = ('COCO', 'Pascal VOC')
+        self.__supported_formats = ('COCO', 'Pascal VOC', 'VoTT')
         self.__image_ext = ['.jpg', '.jpeg', '.png', '.tif', '.tiff']
         
         self.backend = backend
         self.model_arch = model_arch
         if workspace is None:
             workspace = os.path.abspath(os.getcwd())
         self.workspace = workspace
@@ -214,17 +214,17 @@
         
         The :func:`train <justdeepit.models.OD.train>` is used for training a model.
         The training images (``image_dpath``), annotation files (``annotation``),
         and annotation format (``annotation_format``) must be specified.
         
         Args:
             image_dpath (str): A path to directory which contains all training images.
-            annotation (str): A path to a file (COCO format) or folder
+            annotation (str): A path to a file (COCO, VoTT format) or folder
                     (Pascal VOC format, each file should have an extension :file:`.xml`).
-            annotation_format (str): Annotation format. COCO or Pascal VOC are supported.
+            annotation_format (str): Annotation format. COCO, VoTT, and Pascal VOC are supported.
             optimizer (str): String to specify optimizer supported by MMDetection.
             scheduler (str): String to specify optimization scheduler.
             batchsize (int): Batch size for each GPU.
             epoch (int): Epoch.
             score_cutoff (float): Cutoff of score for object detection.
             cpu (int): Number of workers for pre-prociessing images for each GPU.
             gpu (int): Number of GPUs for model training.
@@ -251,14 +251,23 @@
                 if fext.lower() in self.__image_ext:
                     ann_fpath = os.path.join(annotation, fname + '.xml')
                     if os.path.exists(ann_fpath):
                         anns.append(ImageAnnotation(fpath, ann_fpath))
             if len(anns) > 0:
                 annotation = os.path.join(self.workspace, 'train_image_annotation.coco.json')
                 anns.format('coco', annotation)
+        elif annotation_format == 'vott':
+            anns = ImageAnnotations()
+            for fpath in glob.glob(os.path.join(image_dpath, '*')):
+                fname, fext = os.path.splitext(os.path.basename(fpath))
+                if fext.lower() in self.__image_ext:
+                    anns.append(ImageAnnotation(fpath, annotation))
+            if len(anns) > 0:
+                annotation = os.path.join(self.workspace, 'train_image_annotation.coco.json')
+                anns.format('coco', annotation)
         else:
             raise NotImplementedError('JustDeepIt does not support {} format for training object detection model.'.format(annotation_format))
         
         self.module.train(image_dpath, annotation,
                           optimizer, scheduler,
                           batchsize, epoch, score_cutoff,
                           cpu=cpu, gpu=gpu)
```

### Comparing `JustDeepIt-0.1.27/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.1.28/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/models/utils/detectron2base.py` & `JustDeepIt-0.1.28/justdeepit/models/utils/detectron2base.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.1.28/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.1.28/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/models/utils/unet.py` & `JustDeepIt-0.1.28/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.1.28/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.1.28/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/utils.py` & `JustDeepIt-0.1.28/justdeepit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,39 +354,49 @@
 
         
     def __set_regions_from_vott(self, vott):
         regions = []
         vott_data = None
         with open(vott, 'r') as jsonfh:
             vott_data = json.load(jsonfh)
+        
+        # find image and annotaiton from the multi-entry VoTT annotation
+        vott_regions = None
+        for vott_image_id, vott_image_meta in vott_data['assets'].items():
+            if vott_image_meta['asset']['name'] == os.path.basename(self.image_path):
+                vott_regions = vott_image_meta['regions']
+                break
+
+        if vott_regions is not None:
+            for vott_region in vott_regions:
+                bbox_xy = [[int(np.floor(vott_region['boundingBox']['left'])),
+                            int(np.floor(vott_region['boundingBox']['top']))],
+                           [int(np.floor(vott_region['boundingBox']['left'])) + \
+                                    int(np.floor(vott_region['boundingBox']['width'])),
+                            int(np.floor(vott_region['boundingBox']['top'])) + \
+                                    int(np.floor(vott_region['boundingBox']['height']))]]
+                polygon_xy = [[int(np.floor(p['x'])), int(np.floor(p['y']))] for p in vott_region['points']]
+    
+                bbox_xy = self.__exif_transpose(bbox_xy, self.image.shape[0:2], self.exif_orientation)
+                polygon_xy = self.__exif_transpose(polygon_xy, self.image.shape[0:2], self.exif_orientation)
 
-        for vott_region in vott_data['regions']:
-            bbox_xy = [[int(np.floor(vott_region['boundingBox']['left'])),
-                        int(np.floor(vott_region['boundingBox']['top']))],
-                       [int(np.floor(vott_region['boundingBox']['left'])) + int(np.floor(vott_region['boundingBox']['width'])),
-                        int(np.floor(vott_region['boundingBox']['top'])) + int(np.floor(vott_region['boundingBox']['height']))]]
-            polygon_xy = [[int(np.floor(p['x'])), int(np.floor(p['y']))] for p in vott_region['points']]
-
-            bbox_xy = self.__exif_transpose(bbox_xy, self.image.shape[0:2], self.exif_orientation)
-            polygon_xy = self.__exif_transpose(polygon_xy, self.image.shape[0:2], self.exif_orientation)
-
-            if bbox_xy[0][0] > bbox_xy[1][0]:
-                bbox_xy[0][0], bbox_xy[1][0] = bbox_xy[1][0], bbox_xy[0][0]
-            if bbox_xy[0][1] > bbox_xy[1][1]:
-                bbox_xy[0][1], bbox_xy[1][1] = bbox_xy[1][1], bbox_xy[0][1]
+                if bbox_xy[0][0] > bbox_xy[1][0]:
+                    bbox_xy[0][0], bbox_xy[1][0] = bbox_xy[1][0], bbox_xy[0][0]
+                if bbox_xy[0][1] > bbox_xy[1][1]:
+                    bbox_xy[0][1], bbox_xy[1][1] = bbox_xy[1][1], bbox_xy[0][1]
             
-            for vott_tag in vott_region['tags']:
-                region = {
-                    'id' : vott_region['id'] + '_' + vott_tag,
-                    'class': vott_tag,
-                    'bbox': [bbox_xy[0][0], bbox_xy[0][1], bbox_xy[1][0], bbox_xy[1][1]],
-                    'contour' : np.array(polygon_xy),
-                    'score': np.nan,
-                }
-                regions.append(region)
+                for vott_tag in vott_region['tags']:
+                    region = {
+                        'id' : vott_region['id'] + '_' + vott_tag,
+                        'class': vott_tag,
+                        'bbox': [bbox_xy[0][0], bbox_xy[0][1], bbox_xy[1][0], bbox_xy[1][1]],
+                        'contour' : np.array(polygon_xy),
+                        'score': np.nan,
+                    }
+                    regions.append(region)
         
         return regions
     
 
     def __exif_transpose(self, points, image_size, exif_orientation):
         """Transpose coordinates according to EXIF orientation
```

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/app.py` & `JustDeepIt-0.1.28/justdeepit/webapp/app.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/appbase.py` & `JustDeepIt-0.1.28/justdeepit/webapp/appbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,24 @@
     
     def check_training_images(self, image_dpath, annotation_path, annotation_format, class_label='NA'):
         images = []
         
         if self.__norm_str(annotation_format) == 'coco':
             with open(annotation_path, 'r') as infh:
                 image_records = json.load(infh)
-                for f in image_records['images']:
-                    if os.path.exists(os.path.join(image_dpath, os.path.basename(f['file_name']))):
-                        images.append(f)
+            for f in image_records['images']:
+                if os.path.exists(os.path.join(image_dpath, os.path.basename(f['file_name']))):
+                    images.append(f)
+        
+        elif self.__norm_str(annotation_format) == 'vott':
+            with open(annotation_path, 'r') as infh:
+                image_records = json.load(infh)
+            for fid, f in image_records['assets'].items():
+                if os.path.exists(os.path.join(image_dpath, os.path.basename(f['asset']['name']))):
+                    images.append(f)
         
         elif (self.__norm_str(annotation_format) == 'mask') or ('voc' in self.__norm_str(annotation_format)):
             fdict = {}
             for f in glob.glob(os.path.join(image_dpath, '*')):
                 fname = os.path.splitext(os.path.basename(f))[0]
                 if os.path.splitext(f)[1].lower() in self.image_ext:
                     if fname not in fdict:
```

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/appis.py` & `JustDeepIt-0.1.28/justdeepit/webapp/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/appod.py` & `JustDeepIt-0.1.28/justdeepit/webapp/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/appsod.py` & `JustDeepIt-0.1.28/justdeepit/webapp/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.js` & `JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.map` & `JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/styles.css` & `JustDeepIt-0.1.28/justdeepit/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js` & `JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js.map` & `JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/static/utils.js` & `JustDeepIt-0.1.28/justdeepit/webapp/static/utils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -468,15 +468,15 @@
                 closedIcon: '&#x0229E;',
                 showEmptyFolder: true,
                 autoOpen: 0,
                 selectable: true,
                 data: dirtree,
             });
             if (selectType === 'any') {
-                if ($('#module-training-annotation_format').val() === 'COCO') {
+                if ($('#module-training-annotation_format').val() === 'COCO' || $('#module-training-annotation_format').val() === 'VoTT') {
                     selectType = 'file';
                 } else {
                     selectType = 'folder';
                 }
             }
             $('#filetree-required-filetype').val(selectType);
             if (selectType === 'file') {
```

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/templates/index.html` & `JustDeepIt-0.1.28/justdeepit/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/templates/module.html` & `JustDeepIt-0.1.28/justdeepit/webapp/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/justdeepit/webapp/templates/shutdown.html` & `JustDeepIt-0.1.28/justdeepit/webapp/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.27/setup.py` & `JustDeepIt-0.1.28/setup.py`

 * *Files identical despite different names*

