# Comparing `tmp/resoto-plugin-protector-3.3.2.tar.gz` & `tmp/resoto-plugin-protector-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.3.2.tar", last modified: Fri Apr 14 16:17:13 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.3.3.tar", last modified: Fri Apr 21 14:38:10 2023, max compression
```

## Comparing `resoto-plugin-protector-3.3.2.tar` & `resoto-plugin-protector-3.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 16:17:13.000000 resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:17:13.348073 resoto-plugin-protector-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-14 16:15:10.000000 resoto-plugin-protector-3.3.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:10.512987 resoto-plugin-protector-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-21 14:38:10.512987 resoto-plugin-protector-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:10.508987 resoto-plugin-protector-3.3.3/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:10.512987 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 14:38:10.000000 resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:38:10.512987 resoto-plugin-protector-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:10.512987 resoto-plugin-protector-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-21 14:36:24.000000 resoto-plugin-protector-3.3.3/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.3.2/PKG-INFO` & `resoto-plugin-protector-3.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Protector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.3.2/README.md` & `resoto-plugin-protector-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.2/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.3.3/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.2/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.3.3/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.2/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.3.3/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Protector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.3.2/setup.py` & `resoto-plugin-protector-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-protector",
-    version="3.3.2",
+    version="3.3.3",
     description="Resoto Protector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["protector = resoto_plugin_protector:ProtectorPlugin"]},
     include_package_data=True,
```

