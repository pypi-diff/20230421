# Comparing `tmp/airbyte_protocol_models-1.0.0.tar.gz` & `tmp/airbyte_protocol_models-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_protocol_models-1.0.0.tar", last modified: Sun Feb 12 21:31:45 2023, max compression
+gzip compressed data, was "airbyte_protocol_models-1.0.1.tar", last modified: Mon Feb 27 15:23:17 2023, max compression
```

## Comparing `airbyte_protocol_models-1.0.0.tar` & `airbyte_protocol_models-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 21:31:45.978680 airbyte_protocol_models-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-02-12 21:26:09.000000 airbyte_protocol_models-1.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1098 2023-02-12 21:31:45.978680 airbyte_protocol_models-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 21:31:45.974680 airbyte_protocol_models-1.0.0/airbyte_protocol/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 21:31:45.978680 airbyte_protocol_models-1.0.0/airbyte_protocol/models/
--rw-r--r--   0 root         (0) root         (0)      119 2023-02-12 21:26:24.000000 airbyte_protocol_models-1.0.0/airbyte_protocol/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18672 2023-02-12 21:26:24.000000 airbyte_protocol_models-1.0.0/airbyte_protocol/models/airbyte_protocol.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-02-12 21:26:25.000000 airbyte_protocol_models-1.0.0/airbyte_protocol/models/well_known_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 21:31:45.978680 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-02-12 21:31:45.000000 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-02-12 21:31:45.000000 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-12 21:31:45.000000 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-02-12 21:31:45.000000 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-12 21:31:45.000000 airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-02-12 21:26:09.000000 airbyte_protocol_models-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-12 21:31:45.978680 airbyte_protocol_models-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1728 2023-02-12 21:26:09.000000 airbyte_protocol_models-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:23:17.547771 airbyte_protocol_models-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-02-27 15:18:32.000000 airbyte_protocol_models-1.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-02-27 15:23:17.547771 airbyte_protocol_models-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:23:17.543771 airbyte_protocol_models-1.0.1/airbyte_protocol/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:23:17.543771 airbyte_protocol_models-1.0.1/airbyte_protocol/models/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-02-27 15:18:46.000000 airbyte_protocol_models-1.0.1/airbyte_protocol/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18672 2023-02-27 15:18:46.000000 airbyte_protocol_models-1.0.1/airbyte_protocol/models/airbyte_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-02-27 15:18:47.000000 airbyte_protocol_models-1.0.1/airbyte_protocol/models/well_known_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:23:17.547771 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-02-27 15:23:17.000000 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2023-02-27 15:23:17.000000 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 15:23:17.000000 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-02-27 15:23:17.000000 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-02-27 15:23:17.000000 airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-02-27 15:18:32.000000 airbyte_protocol_models-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 15:23:17.547771 airbyte_protocol_models-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-02-27 15:18:32.000000 airbyte_protocol_models-1.0.1/setup.py
```

### Comparing `airbyte_protocol_models-1.0.0/LICENSE.txt` & `airbyte_protocol_models-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airbyte_protocol_models-1.0.0/PKG-INFO` & `airbyte_protocol_models-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte_protocol_models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Declares the Airbyte Protocol.
 Home-page: https://github.com/airbytehq/airbyte-protocol
 Author: Airbyte
 Author-email: contact@airbyte.io
 License: MIT
 Project-URL: Documentation, https://docs.airbyte.io/
 Project-URL: Source, https://github.com/airbytehq/airbyte-protocol
```

### Comparing `airbyte_protocol_models-1.0.0/airbyte_protocol/models/airbyte_protocol.py` & `airbyte_protocol_models-1.0.1/airbyte_protocol/models/airbyte_protocol.py`

 * *Files identical despite different names*

### Comparing `airbyte_protocol_models-1.0.0/airbyte_protocol/models/well_known_types.py` & `airbyte_protocol_models-1.0.1/airbyte_protocol/models/well_known_types.py`

 * *Files identical despite different names*

### Comparing `airbyte_protocol_models-1.0.0/airbyte_protocol_models.egg-info/PKG-INFO` & `airbyte_protocol_models-1.0.1/airbyte_protocol_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-protocol-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Declares the Airbyte Protocol.
 Home-page: https://github.com/airbytehq/airbyte-protocol
 Author: Airbyte
 Author-email: contact@airbyte.io
 License: MIT
 Project-URL: Documentation, https://docs.airbyte.io/
 Project-URL: Source, https://github.com/airbytehq/airbyte-protocol
```

### Comparing `airbyte_protocol_models-1.0.0/setup.py` & `airbyte_protocol_models-1.0.1/setup.py`

 * *Files identical despite different names*

