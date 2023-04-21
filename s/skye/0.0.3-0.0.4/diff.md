# Comparing `tmp/skye-0.0.3.tar.gz` & `tmp/skye-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skye-0.0.3.tar", last modified: Fri Apr 21 01:18:50 2023, max compression
+gzip compressed data, was "skye-0.0.4.tar", last modified: Fri Apr 21 01:26:03 2023, max compression
```

## Comparing `skye-0.0.3.tar` & `skye-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.290155 skye-0.0.3/
--rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.3/LICENSE
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:18:50.289884 skye-0.0.3/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.3/README.md
--rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-21 01:18:50.290239 skye-0.0.3/setup.cfg
--rw-r--r--   0 iosefa     (501) staff       (20)     1036 2023-04-21 01:16:21.000000 skye-0.0.3/setup.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.287733 skye-0.0.3/skye/
--rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.3/skye/__init__.py
--rw-r--r--   0 iosefa     (501) staff       (20)     9463 2023-04-21 01:17:17.000000 skye-0.0.3/skye/core.py
--rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.3/skye/utils.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.289532 skye-0.0.3/skye.egg-info/
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      209 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/SOURCES.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/dependency_links.txt
--rw-r--r--   0 iosefa     (501) staff       (20)      152 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/requires.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/top_level.txt
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.313087 skye-0.0.4/
+-rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.4/LICENSE
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:26:03.312829 skye-0.0.4/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.4/README.md
+-rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-21 01:26:03.313171 skye-0.0.4/setup.cfg
+-rw-r--r--   0 iosefa     (501) staff       (20)     1063 2023-04-21 01:25:33.000000 skye-0.0.4/setup.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.310959 skye-0.0.4/skye/
+-rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.4/skye/__init__.py
+-rw-r--r--   0 iosefa     (501) staff       (20)     9463 2023-04-21 01:17:17.000000 skye-0.0.4/skye/core.py
+-rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.4/skye/utils.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:26:03.312499 skye-0.0.4/skye.egg-info/
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      209 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/SOURCES.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/dependency_links.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)      168 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/requires.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-21 01:26:03.000000 skye-0.0.4/skye.egg-info/top_level.txt
```

### Comparing `skye-0.0.3/LICENSE` & `skye-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skye-0.0.3/PKG-INFO` & `skye-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.3
+Version: 0.0.4
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skye-0.0.3/setup.py` & `skye-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="skye",
-    version="0.0.3",
+    version="0.0.4",
     author="Iosefa Percival",
     author_email="ipercival@gmail.com",
     description="360-degree image analysis for forest ecology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iosefa/skye",
     project_urls={
@@ -17,14 +17,15 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        'ipython>=8.12.0',
         'matplotlib>=3.7.1',
         'numpy>=1.24.2',
         'opencv-python>=4.7.0.72',
         'pandas>=2.0.0',
         'Pillow>=9.5.0',
         'scikit-image>=0.20.0',
         'scikit-learn>=1.2.2',
```

### Comparing `skye-0.0.3/skye/core.py` & `skye-0.0.4/skye/core.py`

 * *Files identical despite different names*

### Comparing `skye-0.0.3/skye/utils.py` & `skye-0.0.4/skye/utils.py`

 * *Files identical despite different names*

### Comparing `skye-0.0.3/skye.egg-info/PKG-INFO` & `skye-0.0.4/skye.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.3
+Version: 0.0.4
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

