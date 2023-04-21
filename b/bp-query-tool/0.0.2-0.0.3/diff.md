# Comparing `tmp/bp_query_tool-0.0.2.tar.gz` & `tmp/bp_query_tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_query_tool-0.0.2.tar", last modified: Mon Apr 17 07:48:40 2023, max compression
+gzip compressed data, was "bp_query_tool-0.0.3.tar", last modified: Fri Apr 21 05:58:47 2023, max compression
```

## Comparing `bp_query_tool-0.0.2.tar` & `bp_query_tool-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.448578 bp_query_tool-0.0.2/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.2/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.2/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      322 2023-04-17 07:48:40.448104 bp_query_tool-0.0.2/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.432756 bp_query_tool-0.0.2/bp_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      322 2023-04-17 07:48:40.000000 bp_query_tool-0.0.2/bp_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-17 07:48:40.000000 bp_query_tool-0.0.2/bp_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-17 07:48:40.000000 bp_query_tool-0.0.2/bp_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-17 07:48:40.000000 bp_query_tool-0.0.2/bp_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-17 07:48:40.000000 bp_query_tool-0.0.2/bp_query_tool.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.433200 bp_query_tool-0.0.2/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.2/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.428955 bp_query_tool-0.0.2/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.434877 bp_query_tool-0.0.2/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.440652 bp_query_tool-0.0.2/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044744 2023-04-17 07:29:32.000000 bp_query_tool-0.0.2/query_tool/frontend/dist/assets/index-99e5fe3f.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-17 07:29:32.000000 bp_query_tool-0.0.2/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-17 07:29:52.000000 bp_query_tool-0.0.2/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-17 07:29:31.000000 bp_query_tool-0.0.2/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-17 07:48:40.447224 bp_query_tool-0.0.2/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.2/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-17 07:48:40.448776 bp_query_tool-0.0.2/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      645 2023-04-17 07:48:32.000000 bp_query_tool-0.0.2/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.873684 bp_query_tool-0.0.3/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.3/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.3/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 05:58:47.873279 bp_query_tool-0.0.3/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.864910 bp_query_tool-0.0.3/bp_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.865329 bp_query_tool-0.0.3/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.3/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.860699 bp_query_tool-0.0.3/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.866135 bp_query_tool-0.0.3/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.869004 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044744 2023-04-17 07:29:32.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-99e5fe3f.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-17 07:29:32.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-17 07:29:52.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-17 07:29:31.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.872493 bp_query_tool-0.0.3/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 05:58:47.873860 bp_query_tool-0.0.3/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-21 05:56:28.000000 bp_query_tool-0.0.3/setup.py
```

### Comparing `bp_query_tool-0.0.2/LICENSE` & `bp_query_tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/bp_query_tool.egg-info/SOURCES.txt` & `bp_query_tool-0.0.3/bp_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/__init__.py` & `bp_query_tool-0.0.3/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/frontend/dist/assets/index-99e5fe3f.js` & `bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-99e5fe3f.js`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/frontend/dist/vite.svg` & `bp_query_tool-0.0.3/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/services/dimension_service.py` & `bp_query_tool-0.0.3/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/services/entities_service.py` & `bp_query_tool-0.0.3/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/services/filters_service.py` & `bp_query_tool-0.0.3/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/services/query_tool_service.py` & `bp_query_tool-0.0.3/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/query_tool/services/register.py` & `bp_query_tool-0.0.3/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.2/setup.py` & `bp_query_tool-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="bp_query_tool",
-    version="0.0.2",
+    version="0.0.3",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
-    python_requires=">=3.9.6",
+    python_requires=">=3.8.10",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 1.20.0",
     ],
 )
```

