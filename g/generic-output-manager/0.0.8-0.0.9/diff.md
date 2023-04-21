# Comparing `tmp/generic-output-manager-0.0.8.tar.gz` & `tmp/generic-output-manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/generic-output-manager-0.0.8.tar", last modified: Wed Mar 29 09:27:31 2023, max compression
+gzip compressed data, was "dist/generic-output-manager-0.0.9.tar", last modified: Fri Apr 21 10:16:46 2023, max compression
```

## Comparing `generic-output-manager-0.0.8.tar` & `generic-output-manager-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.825339 generic-output-manager-0.0.8/generic_output_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-29 09:27:31.000000 generic-output-manager-0.0.8/generic_output_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      699 2023-03-29 09:27:31.000000 generic-output-manager-0.0.8/generic_output_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 09:27:31.000000 generic-output-manager-0.0.8/generic_output_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-29 09:27:31.000000 generic-output-manager-0.0.8/generic_output_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-29 09:27:31.000000 generic-output-manager-0.0.8/generic_output_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/genericoutput/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/genericoutput/assets/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/gasset.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/html.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/log.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/assets/picture.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/genericoutput/metadata/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/metadata/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:27:31.826339 generic-output-manager-0.0.8/genericoutput/storages/
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/storages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/storages/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/storages/minio.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/genericoutput/storages/storage.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-03-29 09:27:31.827339 generic-output-manager-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-03-29 09:27:23.000000 generic-output-manager-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.466862 generic-output-manager-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-21 10:16:46.466862 generic-output-manager-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.465862 generic-output-manager-0.0.9/generic_output_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-21 10:16:46.000000 generic-output-manager-0.0.9/generic_output_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-21 10:16:46.000000 generic-output-manager-0.0.9/generic_output_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 10:16:46.000000 generic-output-manager-0.0.9/generic_output_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-21 10:16:46.000000 generic-output-manager-0.0.9/generic_output_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-21 10:16:46.000000 generic-output-manager-0.0.9/generic_output_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.465862 generic-output-manager-0.0.9/genericoutput/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.465862 generic-output-manager-0.0.9/genericoutput/assets/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/gasset.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/assets/picture.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.465862 generic-output-manager-0.0.9/genericoutput/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/metadata/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:16:46.466862 generic-output-manager-0.0.9/genericoutput/storages/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/storages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/storages/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/storages/minio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/genericoutput/storages/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-21 10:16:46.466862 generic-output-manager-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-04-21 10:16:35.000000 generic-output-manager-0.0.9/setup.py
```

### Comparing `generic-output-manager-0.0.8/generic_output_manager.egg-info/SOURCES.txt` & `generic-output-manager-0.0.9/generic_output_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/assets/file.py` & `generic-output-manager-0.0.9/genericoutput/assets/file.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/assets/gasset.py` & `generic-output-manager-0.0.9/genericoutput/assets/gasset.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/assets/log.py` & `generic-output-manager-0.0.9/genericoutput/assets/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return "json"
     elif "bool" in t:
         return "boolean"
     else:
         return "invalid"
 
 class Log(GAsset):
-    def __init__(self, name, value, title=None, description=None, var=None, messageType="file"):
+    def __init__(self, name, value, title=None, description=None, var=None, messageType="log"):
         super().__init__(name=name, title=title, description=description, var=var, messageType=messageType)
         self.set_value(value)
 
     def to_json(self):
         
         result = super().to_json()
         result['path'] = None
```

### Comparing `generic-output-manager-0.0.8/genericoutput/metadata/metadata.py` & `generic-output-manager-0.0.9/genericoutput/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/notifier.py` & `generic-output-manager-0.0.9/genericoutput/notifier.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/storages/filesystem.py` & `generic-output-manager-0.0.9/genericoutput/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/storages/minio.py` & `generic-output-manager-0.0.9/genericoutput/storages/minio.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/genericoutput/storages/storage.py` & `generic-output-manager-0.0.9/genericoutput/storages/storage.py`

 * *Files identical despite different names*

### Comparing `generic-output-manager-0.0.8/setup.py` & `generic-output-manager-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="generic-output-manager",
-    version="0.0.8",
+    version="0.0.9",
     author="Alida research team",
     author_email="engineering-alida-lab@eng.it",
     description="",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

