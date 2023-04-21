# Comparing `tmp/bp_data_fabric-0.0.7.tar.gz` & `tmp/bp_data_fabric-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.7.tar", last modified: Thu Apr 20 09:47:40 2023, max compression
+gzip compressed data, was "bp_data_fabric-0.0.8.tar", last modified: Fri Apr 21 06:21:07 2023, max compression
```

## Comparing `bp_data_fabric-0.0.7.tar` & `bp_data_fabric-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.726180 bp_data_fabric-0.0.7/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.7/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-20 09:47:40.725901 bp_data_fabric-0.0.7/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.7/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.724706 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.725445 bp_data_fabric-0.0.7/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.7/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.7/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-20 09:47:40.726269 bp_data_fabric-0.0.7/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-20 09:47:33.000000 bp_data_fabric-0.0.7/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.798644 bp_data_fabric-0.0.8/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.8/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:21:07.798195 bp_data_fabric-0.0.8/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.8/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.796044 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-21 06:21:07.000000 bp_data_fabric-0.0.8/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:21:07.797237 bp_data_fabric-0.0.8/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.8/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.8/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 06:21:07.798844 bp_data_fabric-0.0.8/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      603 2023-04-21 06:14:22.000000 bp_data_fabric-0.0.8/setup.py
```

### Comparing `bp_data_fabric-0.0.7/LICENSE` & `bp_data_fabric-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.7/data_fabric/__init__.py` & `bp_data_fabric-0.0.8/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.7/data_fabric/components.py` & `bp_data_fabric-0.0.8/data_fabric/components.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.7/setup.py` & `bp_data_fabric-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="0.0.7",
+    version="0.0.8",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",
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

