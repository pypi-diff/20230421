# Comparing `tmp/cython_bbox_fix-2023.4.20.tar.gz` & `tmp/cython_bbox_fix-2023.4.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cython_bbox_fix-2023.4.20.tar", last modified: Thu Apr 20 23:10:25 2023, max compression
+gzip compressed data, was "cython_bbox_fix-2023.4.21.tar", last modified: Thu Apr 20 23:19:09 2023, max compression
```

## Comparing `cython_bbox_fix-2023.4.20.tar` & `cython_bbox_fix-2023.4.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:10:25.385857 cython_bbox_fix-2023.4.20/
--rw-r--r--   0 y0f01wf    (503) staff       (20)     4814 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.20/LICENSE
--rw-r--r--   0 y0f01wf    (503) staff       (20)       36 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.20/MANIFEST.in
--rw-r--r--   0 y0f01wf    (503) staff       (20)     1043 2023-04-20 23:10:25.385429 cython_bbox_fix-2023.4.20/PKG-INFO
--rw-r--r--   0 y0f01wf    (503) staff       (20)      743 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.20/README.md
-drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:10:25.383802 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/
--rw-r--r--   0 y0f01wf    (503) staff       (20)     1043 2023-04-20 23:10:19.000000 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/PKG-INFO
--rw-r--r--   0 y0f01wf    (503) staff       (20)      252 2023-04-20 23:10:25.000000 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/SOURCES.txt
--rw-r--r--   0 y0f01wf    (503) staff       (20)        1 2023-04-20 23:10:19.000000 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/dependency_links.txt
--rw-r--r--   0 y0f01wf    (503) staff       (20)       13 2023-04-20 23:10:19.000000 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/requires.txt
--rw-r--r--   0 y0f01wf    (503) staff       (20)       12 2023-04-20 23:10:19.000000 cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/top_level.txt
--rw-r--r--   0 y0f01wf    (503) staff       (20)       38 2023-04-20 23:10:25.385970 cython_bbox_fix-2023.4.20/setup.cfg
--rw-r--r--   0 y0f01wf    (503) staff       (20)     1919 2023-04-20 23:02:53.000000 cython_bbox_fix-2023.4.20/setup.py
-drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:10:25.384706 cython_bbox_fix-2023.4.20/src/
--rw-r--r--   0 y0f01wf    (503) staff       (20)     1777 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.20/src/cython_bbox.pyx
+drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:19:09.698407 cython_bbox_fix-2023.4.21/
+-rw-r--r--   0 y0f01wf    (503) staff       (20)     4814 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.21/LICENSE
+-rw-r--r--   0 y0f01wf    (503) staff       (20)       36 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.21/MANIFEST.in
+-rw-r--r--   0 y0f01wf    (503) staff       (20)      985 2023-04-20 23:19:09.698003 cython_bbox_fix-2023.4.21/PKG-INFO
+-rw-r--r--   0 y0f01wf    (503) staff       (20)      743 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.21/README.md
+drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:19:09.696519 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/
+-rw-r--r--   0 y0f01wf    (503) staff       (20)      985 2023-04-20 23:19:03.000000 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/PKG-INFO
+-rw-r--r--   0 y0f01wf    (503) staff       (20)      252 2023-04-20 23:19:09.000000 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 y0f01wf    (503) staff       (20)        1 2023-04-20 23:19:03.000000 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 y0f01wf    (503) staff       (20)       13 2023-04-20 23:19:03.000000 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/requires.txt
+-rw-r--r--   0 y0f01wf    (503) staff       (20)       12 2023-04-20 23:19:03.000000 cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/top_level.txt
+-rw-r--r--   0 y0f01wf    (503) staff       (20)       38 2023-04-20 23:19:09.698515 cython_bbox_fix-2023.4.21/setup.cfg
+-rw-r--r--   0 y0f01wf    (503) staff       (20)     1845 2023-04-20 23:18:41.000000 cython_bbox_fix-2023.4.21/setup.py
+drwxr-xr-x   0 y0f01wf    (503) staff       (20)        0 2023-04-20 23:19:09.697302 cython_bbox_fix-2023.4.21/src/
+-rw-r--r--   0 y0f01wf    (503) staff       (20)     1777 2023-04-20 22:44:36.000000 cython_bbox_fix-2023.4.21/src/cython_bbox.pyx
```

### Comparing `cython_bbox_fix-2023.4.20/LICENSE` & `cython_bbox_fix-2023.4.21/LICENSE`

 * *Files identical despite different names*

### Comparing `cython_bbox_fix-2023.4.20/PKG-INFO` & `cython_bbox_fix-2023.4.21/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: cython_bbox_fix
-Version: 2023.4.20
+Version: 2023.4.21
 Summary: Standalone cython_bbox
 Home-page: https://github.com/samson-wang/cython_bbox.git
-Author: Samson Wang
-Author-email: samson.c.wang@gmail.com
 Keywords: cython_bbox_fix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cython_bbox
 
 cython_bbox is widely used in object detection tasks. To my best knowledge, it was first implemented in [Faster-RCNN](https://github.com/rbgirshick/py-faster-rcnn). Since then, almost all object detection projects use the source code directly.
```

### Comparing `cython_bbox_fix-2023.4.20/README.md` & `cython_bbox_fix-2023.4.21/README.md`

 * *Files identical despite different names*

### Comparing `cython_bbox_fix-2023.4.20/cython_bbox_fix.egg-info/PKG-INFO` & `cython_bbox_fix-2023.4.21/cython_bbox_fix.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: cython-bbox-fix
-Version: 2023.4.20
+Version: 2023.4.21
 Summary: Standalone cython_bbox
 Home-page: https://github.com/samson-wang/cython_bbox.git
-Author: Samson Wang
-Author-email: samson.c.wang@gmail.com
 Keywords: cython_bbox_fix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cython_bbox
 
 cython_bbox is widely used in object detection tasks. To my best knowledge, it was first implemented in [Faster-RCNN](https://github.com/rbgirshick/py-faster-rcnn). Since then, almost all object detection projects use the source code directly.
```

### Comparing `cython_bbox_fix-2023.4.20/setup.py` & `cython_bbox_fix-2023.4.21/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,15 @@
 
 setup(
     name='cython_bbox_fix',
     setup_requires=["setuptools>=18.0","Cython","numpy"],
     install_requires=["Cython","numpy"],
     ext_modules=ext_modules,
     cmdclass={'build': build},
-    version = '2023.4.20',
+    version = '2023.4.21',
     description = 'Standalone cython_bbox',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author = 'Samson Wang',
-    author_email = 'samson.c.wang@gmail.com',
     url = 'https://github.com/samson-wang/cython_bbox.git', 
     keywords = ['cython_bbox_fix']
 )
```

### Comparing `cython_bbox_fix-2023.4.20/src/cython_bbox.pyx` & `cython_bbox_fix-2023.4.21/src/cython_bbox.pyx`

 * *Files identical despite different names*

