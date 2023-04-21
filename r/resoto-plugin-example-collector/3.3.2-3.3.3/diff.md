# Comparing `tmp/resoto-plugin-example-collector-3.3.2.tar.gz` & `tmp/resoto-plugin-example-collector-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-example-collector-3.3.2.tar", last modified: Fri Apr 14 16:12:44 2023, max compression
+gzip compressed data, was "resoto-plugin-example-collector-3.3.3.tar", last modified: Fri Apr 21 14:36:33 2023, max compression
```

## Comparing `resoto-plugin-example-collector-3.3.2.tar` & `resoto-plugin-example-collector-3.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:12:44.000000 resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:44.336150 resoto-plugin-example-collector-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 16:10:44.000000 resoto-plugin-example-collector-3.3.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 14:36:33.000000 resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:33.610098 resoto-plugin-example-collector-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 14:34:52.000000 resoto-plugin-example-collector-3.3.3/test/test_config.py
```

### Comparing `resoto-plugin-example-collector-3.3.2/PKG-INFO` & `resoto-plugin-example-collector-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Example Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector/__init__.py` & `resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/PKG-INFO` & `resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Example Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.3.2/resoto_plugin_example_collector.egg-info/SOURCES.txt` & `resoto-plugin-example-collector-3.3.3/resoto_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.3.2/setup.py` & `resoto-plugin-example-collector-3.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-example-collector",
-    version="3.3.2",
+    version="3.3.3",
     description="Resoto Example Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["example_collector = resoto_plugin_example_collector:ExampleCollectorPlugin"]},
     include_package_data=True,
```

