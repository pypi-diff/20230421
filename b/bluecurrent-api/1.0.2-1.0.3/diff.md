# Comparing `tmp/bluecurrent-api-1.0.2.tar.gz` & `tmp/bluecurrent-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecurrent-api-1.0.2.tar", last modified: Fri Feb  3 15:28:09 2023, max compression
+gzip compressed data, was "bluecurrent-api-1.0.3.tar", last modified: Fri Apr 21 09:43:28 2023, max compression
```

## Comparing `bluecurrent-api-1.0.2.tar` & `bluecurrent-api-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 15:28:09.173317 bluecurrent-api-1.0.2/
--rw-rw-rw-   0        0        0     1073 2022-09-09 13:33:12.000000 bluecurrent-api-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3805 2023-02-03 15:28:09.173317 bluecurrent-api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3230 2022-11-18 13:49:58.000000 bluecurrent-api-1.0.2/README.md
--rw-rw-rw-   0        0        0      735 2023-02-03 15:27:55.000000 bluecurrent-api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-03 15:28:09.173317 bluecurrent-api-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-03 15:28:09.146316 bluecurrent-api-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-03 15:28:09.154315 bluecurrent-api-1.0.2/src/bluecurrent_api/
--rw-rw-rw-   0        0        0       56 2022-10-03 11:18:14.000000 bluecurrent-api-1.0.2/src/bluecurrent_api/__init__.py
--rw-rw-rw-   0        0        0     4436 2023-02-03 15:06:22.000000 bluecurrent-api-1.0.2/src/bluecurrent_api/client.py
--rw-rw-rw-   0        0        0      670 2022-11-18 12:50:41.000000 bluecurrent-api-1.0.2/src/bluecurrent_api/exceptions.py
--rw-rw-rw-   0        0        0     6328 2023-02-03 15:07:49.000000 bluecurrent-api-1.0.2/src/bluecurrent_api/utils.py
--rw-rw-rw-   0        0        0     8503 2023-02-03 15:15:37.000000 bluecurrent-api-1.0.2/src/bluecurrent_api/websocket.py
-drwxrwxrwx   0        0        0        0 2023-02-03 15:28:09.171316 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/
--rw-rw-rw-   0        0        0     3805 2023-02-03 15:28:09.000000 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-02-03 15:28:09.000000 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 15:28:09.000000 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-02-03 15:28:09.000000 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-03 15:28:09.000000 bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.551419 bluecurrent-api-1.0.3/
+-rw-rw-rw-   0        0        0     1073 2022-09-09 13:33:12.000000 bluecurrent-api-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3805 2023-04-21 09:43:28.550406 bluecurrent-api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3230 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/README.md
+-rw-rw-rw-   0        0        0      762 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:43:28.551419 bluecurrent-api-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.502407 bluecurrent-api-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.511405 bluecurrent-api-1.0.3/src/bluecurrent_api/
+-rw-rw-rw-   0        0        0       56 2022-10-03 11:18:14.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/__init__.py
+-rw-rw-rw-   0        0        0     4436 2023-02-03 15:06:22.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/client.py
+-rw-rw-rw-   0        0        0      670 2022-11-18 12:50:41.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/exceptions.py
+-rw-rw-rw-   0        0        0     6328 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/utils.py
+-rw-rw-rw-   0        0        0     8507 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.542409 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/
+-rw-rw-rw-   0        0        0     3805 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.548405 bluecurrent-api-1.0.3/tests/
+-rw-rw-rw-   0        0        0     2873 2022-11-18 12:50:41.000000 bluecurrent-api-1.0.3/tests/test_client.py
+-rw-rw-rw-   0        0        0     9452 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/tests/test_utils.py
+-rw-rw-rw-   0        0        0    15803 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/tests/test_websocket.py
```

### Comparing `bluecurrent-api-1.0.2/LICENSE` & `bluecurrent-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.2/PKG-INFO` & `bluecurrent-api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecurrent-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper for the Blue Current websocket api
 Author-email: Floris272 <florispuijk@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bluecurrent/HomeAssistantAPI
 Project-URL: Bug Tracker, https://github.com/bluecurrent/HomeAssistantAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluecurrent-api-1.0.2/README.md` & `bluecurrent-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.2/pyproject.toml` & `bluecurrent-api-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "bluecurrent-api"
-version = "1.0.2"
-authors = [
-  { name="Floris272", email="florispuijk@outlook.com" },
-]
-description = "A wrapper for the Blue Current websocket api"
-readme = "README.md"
-license = {text = "MIT"}
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "websockets >= 10.0",
-    "asyncio >= 3.4.3",
-    "pytz >= 2021.3"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/bluecurrent/HomeAssistantAPI"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "bluecurrent-api"
+version = "1.0.3"
+authors = [
+  { name="Floris272", email="florispuijk@outlook.com" },
+]
+description = "A wrapper for the Blue Current websocket api"
+readme = "README.md"
+license = {text = "MIT"}
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "websockets >= 10.0",
+    "asyncio >= 3.4.3",
+    "pytz >= 2021.3"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/bluecurrent/HomeAssistantAPI"
 "Bug Tracker" = "https://github.com/bluecurrent/HomeAssistantAPI/issues"
```

### Comparing `bluecurrent-api-1.0.2/src/bluecurrent_api/client.py` & `bluecurrent-api-1.0.3/src/bluecurrent_api/client.py`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.2/src/bluecurrent_api/exceptions.py` & `bluecurrent-api-1.0.3/src/bluecurrent_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.2/src/bluecurrent_api/utils.py` & `bluecurrent-api-1.0.3/src/bluecurrent_api/utils.py`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.2/src/bluecurrent_api/websocket.py` & `bluecurrent-api-1.0.3/src/bluecurrent_api/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     handle_grid,
     handle_setting_change,
     handle_session_messages,
     get_dummy_message,
     get_exception
 )
 
-URL = "wss://bo.bluecurrent.nl/haserver"
+URL = "wss://motown.bluecurrent.nl/haserver"
 BUTTONS = ("START_SESSION", "STOP_SESSION", "SOFT_RESET", "REBOOT")
 
 class Websocket:
     """Class for handling requests and responses for the BlueCurrent Websocket Api."""
     _connection = None
     _has_connection = False
     auth_token = None
```

### Comparing `bluecurrent-api-1.0.2/src/bluecurrent_api.egg-info/PKG-INFO` & `bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecurrent-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper for the Blue Current websocket api
 Author-email: Floris272 <florispuijk@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bluecurrent/HomeAssistantAPI
 Project-URL: Bug Tracker, https://github.com/bluecurrent/HomeAssistantAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

