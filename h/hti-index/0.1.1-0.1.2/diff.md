# Comparing `tmp/hti_index-0.1.1.tar.gz` & `tmp/hti_index-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hti_index-0.1.1.tar", last modified: Fri Apr 21 06:06:55 2023, max compression
+gzip compressed data, was "hti_index-0.1.2.tar", last modified: Fri Apr 21 06:31:59 2023, max compression
```

## Comparing `hti_index-0.1.1.tar` & `hti_index-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.318132 hti_index-0.1.1/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.1/LICENSE
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:06:55.317778 hti_index-0.1.1/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.1/README.md
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.316453 hti_index-0.1.1/hti_index/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      148 2023-04-21 06:02:31.000000 hti_index-0.1.1/hti_index/__init__.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3095 2023-04-20 00:12:09.000000 hti_index-0.1.1/hti_index/component.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2696 2023-04-20 00:20:10.000000 hti_index-0.1.1/hti_index/composite.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3977 2023-04-21 06:06:46.000000 hti_index-0.1.1/hti_index/flowfreq.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     5361 2023-04-21 05:32:49.000000 hti_index-0.1.1/hti_index/indexer.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-21 06:02:13.000000 hti_index-0.1.1/hti_index/utils.py
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.317467 hti_index-0.1.1/hti_index.egg-info/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      320 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/SOURCES.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/dependency_links.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/requires.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/top_level.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-21 06:06:55.318202 hti_index-0.1.1/setup.cfg
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-21 06:06:01.000000 hti_index-0.1.1/setup.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.180386 hti_index-0.1.2/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.2/LICENSE
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:31:59.180080 hti_index-0.1.2/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.2/README.md
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.178804 hti_index-0.1.2/hti_index/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      148 2023-04-21 06:22:58.000000 hti_index-0.1.2/hti_index/__init__.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3095 2023-04-20 00:12:09.000000 hti_index-0.1.2/hti_index/component.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2696 2023-04-20 00:20:10.000000 hti_index-0.1.2/hti_index/composite.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3041 2023-04-21 06:31:46.000000 hti_index-0.1.2/hti_index/flowfreq.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     5361 2023-04-21 05:32:49.000000 hti_index-0.1.2/hti_index/indexer.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-21 06:02:13.000000 hti_index-0.1.2/hti_index/utils.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:31:59.179839 hti_index-0.1.2/hti_index.egg-info/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      320 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/SOURCES.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/dependency_links.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/requires.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-21 06:31:59.000000 hti_index-0.1.2/hti_index.egg-info/top_level.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-21 06:31:59.180450 hti_index-0.1.2/setup.cfg
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-21 06:31:54.000000 hti_index-0.1.2/setup.py
```

### Comparing `hti_index-0.1.1/PKG-INFO` & `hti_index-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti_index
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.1/README.md` & `hti_index-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.1/hti_index/component.py` & `hti_index-0.1.2/hti_index/component.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.1/hti_index/composite.py` & `hti_index-0.1.2/hti_index/composite.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.1/hti_index/indexer.py` & `hti_index-0.1.2/hti_index/indexer.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.1/hti_index/utils.py` & `hti_index-0.1.2/hti_index/utils.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.1/hti_index.egg-info/PKG-INFO` & `hti_index-0.1.2/hti_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti-index
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.1/setup.py` & `hti_index-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Description: Setup script for the qbf_index package
 from setuptools import setup, find_packages
 
 setup(
     name='hti_index',
-    version='0.1.1',
+    version='0.1.2',
     author='Mohamed Diomande',
     author_email='gdiomande7907@gmail.com',
     description='Python package for implementing a HasH Table Index', 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/diomandeee/hti_index',
     packages=find_packages(),
```

