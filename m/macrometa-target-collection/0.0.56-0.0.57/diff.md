# Comparing `tmp/macrometa-target-collection-0.0.56.tar.gz` & `tmp/macrometa-target-collection-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.56.tar", last modified: Wed Apr 19 05:53:07 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.57.tar", last modified: Fri Apr 21 12:20:09 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.56.tar` & `macrometa-target-collection-0.0.57.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.146036 macrometa-target-collection-0.0.56/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13889 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.651584 macrometa-target-collection-0.0.57/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13919 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.56/LICENSE` & `macrometa-target-collection-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.56/PKG-INFO` & `macrometa-target-collection-0.0.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.56
+Version: 0.0.57
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.56/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.57/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.56/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.57/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
                 logger.debug("pyC8 error occurred")
 
             state = None
             try_upsert(collection, record_batch)
         elif message_type == 'STATE':
             logger.debug('Setting state to {}'.format(o['value']))
             state = o['value']
+            emit_state(state)
         elif message_type == 'SCHEMA':
             stream = o['stream']
             schemas[stream] = o['schema']
             adjust_decimal_precision_for_schema(schemas[stream])
             validators[stream] = Draft4Validator((o['schema']))
             key_properties[stream] = o['key_properties']
         else:
```

### Comparing `macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.56
+Version: 0.0.57
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.56/pyproject.toml` & `macrometa-target-collection-0.0.57/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.56"
+version = "0.0.57"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

