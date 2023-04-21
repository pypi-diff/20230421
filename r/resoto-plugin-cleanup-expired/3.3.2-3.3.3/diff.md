# Comparing `tmp/resoto-plugin-cleanup-expired-3.3.2.tar.gz` & `tmp/resoto-plugin-cleanup-expired-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-expired-3.3.2.tar", last modified: Fri Apr 14 16:14:13 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-expired-3.3.3.tar", last modified: Fri Apr 21 14:34:03 2023, max compression
```

## Comparing `resoto-plugin-cleanup-expired-3.3.2.tar` & `resoto-plugin-cleanup-expired-3.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 16:14:13.000000 resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.347086 resoto-plugin-cleanup-expired-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 16:12:34.000000 resoto-plugin-cleanup-expired-3.3.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 14:34:03.000000 resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:03.699092 resoto-plugin-cleanup-expired-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-21 14:31:52.000000 resoto-plugin-cleanup-expired-3.3.3/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-expired-3.3.2/PKG-INFO` & `resoto-plugin-cleanup-expired-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Expired Resource Cleanup Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.3.2/README.md` & `resoto-plugin-cleanup-expired-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired/__init__.py` & `resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/PKG-INFO` & `resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto Expired Resource Cleanup Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.3.2/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-expired-3.3.3/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.3.2/setup.py` & `resoto-plugin-cleanup-expired-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-expired",
-    version="3.3.2",
+    version="3.3.3",
     description="Resoto Expired Resource Cleanup Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["cleanup_expired = resoto_plugin_cleanup_expired:CleanupExpiredPlugin"]},
     include_package_data=True,
```

