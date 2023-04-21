# Comparing `tmp/bp-data-visualization-0.0.8.tar.gz` & `tmp/bp-data-visualization-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp-data-visualization-0.0.8.tar", last modified: Thu Apr 20 06:54:11 2023, max compression
+gzip compressed data, was "bp-data-visualization-0.0.9.tar", last modified: Fri Apr 21 06:13:02 2023, max compression
```

## Comparing `bp-data-visualization-0.0.8.tar` & `bp-data-visualization-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.351459 bp-data-visualization-0.0.8/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-20 06:54:11.350927 bp-data-visualization-0.0.8/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.343253 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.344205 bp-data-visualization-0.0.8/data_visualization/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-20 06:41:53.000000 bp-data-visualization-0.0.8/data_visualization/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.339534 bp-data-visualization-0.0.8/data_visualization/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.345187 bp-data-visualization-0.0.8/data_visualization/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.350168 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1959381 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-80a55e32.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-20 06:42:31.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/index.html
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-20 06:42:09.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/vite.svg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/data_visualization/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-20 06:54:11.351626 bp-data-visualization-0.0.8/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      628 2023-04-20 06:53:00.000000 bp-data-visualization-0.0.8/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.206595 bp-data-visualization-0.0.9/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.9/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.9/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      295 2023-04-21 06:13:02.206171 bp-data-visualization-0.0.9/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.9/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.193500 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      295 2023-04-21 06:13:02.000000 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-04-21 06:13:02.000000 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 06:13:02.000000 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 06:13:02.000000 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-21 06:13:02.000000 bp-data-visualization-0.0.9/bp_data_visualization.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.194271 bp-data-visualization-0.0.9/data_visualization/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-20 06:41:53.000000 bp-data-visualization-0.0.9/data_visualization/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.188899 bp-data-visualization-0.0.9/data_visualization/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.195731 bp-data-visualization-0.0.9/data_visualization/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:13:02.204808 bp-data-visualization-0.0.9/data_visualization/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1959381 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.9/data_visualization/frontend/dist/assets/index-80a55e32.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.9/data_visualization/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-20 06:42:31.000000 bp-data-visualization-0.0.9/data_visualization/frontend/dist/index.html
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-20 06:42:09.000000 bp-data-visualization-0.0.9/data_visualization/frontend/dist/vite.svg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.9/data_visualization/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 06:13:02.206721 bp-data-visualization-0.0.9/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      629 2023-04-21 06:11:02.000000 bp-data-visualization-0.0.9/setup.py
```

### Comparing `bp-data-visualization-0.0.8/LICENSE` & `bp-data-visualization-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/bp_data_visualization.egg-info/SOURCES.txt` & `bp-data-visualization-0.0.9/bp_data_visualization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/data_visualization/__init__.py` & `bp-data-visualization-0.0.9/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-80a55e32.js` & `bp-data-visualization-0.0.9/data_visualization/frontend/dist/assets/index-80a55e32.js`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/data_visualization/frontend/dist/vite.svg` & `bp-data-visualization-0.0.9/data_visualization/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/data_visualization/register.py` & `bp-data-visualization-0.0.9/data_visualization/register.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-0.0.8/setup.py` & `bp-data-visualization-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="bp-data-visualization",
-    version="0.0.8",
+    version="0.0.9",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Show data in charts",
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

