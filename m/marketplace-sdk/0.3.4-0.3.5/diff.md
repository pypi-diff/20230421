# Comparing `tmp/marketplace_sdk-0.3.4.tar.gz` & `tmp/marketplace_sdk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace_sdk-0.3.4.tar", last modified: Wed Apr  5 10:34:25 2023, max compression
+gzip compressed data, was "marketplace_sdk-0.3.5.tar", last modified: Fri Apr 21 15:06:46 2023, max compression
```

## Comparing `marketplace_sdk-0.3.4.tar` & `marketplace_sdk-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-05 10:34:16.000000 marketplace_sdk-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-05 10:34:16.000000 marketplace_sdk-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-05 10:34:25.537214 marketplace_sdk-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-05 10:34:16.000000 marketplace_sdk-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/logos/MARVEL.png
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/logos/MarketPlace.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace/app/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace/app/v0_0_1/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0_0_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0_0_1/data_sink_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0_0_1/data_source_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/app/v0_0_1/transformation_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace/message_broker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/message_broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/message_broker/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/message_broker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/marketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:34:25.533214 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-05 10:34:25.000000 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-05 10:34:25.000000 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 10:34:25.000000 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-05 10:34:25.000000 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 10:34:25.000000 marketplace_sdk-0.3.4/marketplace_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-05 10:34:25.537214 marketplace_sdk-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 10:34:17.000000 marketplace_sdk-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.399979 marketplace_sdk-0.3.5/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/logos/MARVEL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/logos/MarketPlace.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_sink_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_source_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/transformation_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/message_broker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/setup.py
```

### Comparing `marketplace_sdk-0.3.4/LICENSE` & `marketplace_sdk-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/PKG-INFO` & `marketplace_sdk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace_sdk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.4/README.md` & `marketplace_sdk-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/logos/MARVEL.png` & `marketplace_sdk-0.3.5/logos/MARVEL.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/logos/MarketPlace.png` & `marketplace_sdk-0.3.5/logos/MarketPlace.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/__init__.py` & `marketplace_sdk-0.3.5/marketplace/app/__init__.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/utils.py` & `marketplace_sdk-0.3.5/marketplace/app/utils.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0/base.py` & `marketplace_sdk-0.3.5/marketplace/app/v0/base.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0/object_storage.py` & `marketplace_sdk-0.3.5/marketplace/app/v0/object_storage.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0/transformation.py` & `marketplace_sdk-0.3.5/marketplace/app/v0/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         transformation_id: transformation.TransformationId,
         update: transformation.TransformationUpdateModel,
     ) -> transformation.TransformationUpdateResponse:
         return transformation.TransformationUpdateResponse.parse_obj(
             self._client.patch(
                 self._proxy_path("updateTransformation"),
                 params={"transformation_id": transformation_id},
-                json=update,
+                json=update.json(),
             ).json()
         )
 
     def start_transformation(
         self, transformation_id: transformation.TransformationId
     ) -> transformation.TransformationStateResponse:
         update: transformation.TransformationUpdateModel = (
```

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0_0_1/__init__.py` & `marketplace_sdk-0.3.5/marketplace/app/v0_0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0_0_1/data_sink_app.py` & `marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_sink_app.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0_0_1/data_source_app.py` & `marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_source_app.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/app/v0_0_1/transformation_app.py` & `marketplace_sdk-0.3.5/marketplace/app/v0_0_1/transformation_app.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/client.py` & `marketplace_sdk-0.3.5/marketplace/client.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace/message_broker/rpc_server.py` & `marketplace_sdk-0.3.5/marketplace/message_broker/rpc_server.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/marketplace_sdk.egg-info/PKG-INFO` & `marketplace_sdk-0.3.5/marketplace_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace-sdk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.4/marketplace_sdk.egg-info/SOURCES.txt` & `marketplace_sdk-0.3.5/marketplace_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.4/setup.cfg` & `marketplace_sdk-0.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = marketplace_sdk
-version = v0.3.4
+version = v0.3.5
 description = Software Development Toolkit to communicate with the Materials MarketPlace platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/materials-marketplace/python-sdk
 author = Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 author_email = simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 license = MIT
```

