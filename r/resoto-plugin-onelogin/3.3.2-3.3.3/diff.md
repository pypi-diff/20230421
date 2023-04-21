# Comparing `tmp/resoto-plugin-onelogin-3.3.2.tar.gz` & `tmp/resoto-plugin-onelogin-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onelogin-3.3.2.tar", last modified: Fri Apr 14 16:14:45 2023, max compression
+gzip compressed data, was "resoto-plugin-onelogin-3.3.3.tar", last modified: Fri Apr 21 14:33:44 2023, max compression
```

## Comparing `resoto-plugin-onelogin-3.3.2.tar` & `resoto-plugin-onelogin-3.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:45.406439 resoto-plugin-onelogin-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 16:14:45.406439 resoto-plugin-onelogin-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:45.402439 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:45.402439 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:14:45.000000 resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:14:45.406439 resoto-plugin-onelogin-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:45.406439 resoto-plugin-onelogin-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-14 16:12:31.000000 resoto-plugin-onelogin-3.3.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:33:44.000000 resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:44.517791 resoto-plugin-onelogin-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-21 14:32:01.000000 resoto-plugin-onelogin-3.3.3/test/test_config.py
```

### Comparing `resoto-plugin-onelogin-3.3.2/PKG-INFO` & `resoto-plugin-onelogin-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto OneLogin Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin/__init__.py` & `resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onelogin-3.3.2/resoto_plugin_onelogin.egg-info/PKG-INFO` & `resoto-plugin-onelogin-3.3.3/resoto_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto OneLogin Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onelogin-3.3.2/setup.py` & `resoto-plugin-onelogin-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-onelogin",
-    version="3.3.2",
+    version="3.3.3",
     description="Resoto OneLogin Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["onelogin = resoto_plugin_onelogin:OneLoginPlugin"]},
     include_package_data=True,
```

