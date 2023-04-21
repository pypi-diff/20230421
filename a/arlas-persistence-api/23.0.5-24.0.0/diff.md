# Comparing `tmp/arlas-persistence_api-23.0.5.tar.gz` & `tmp/arlas-persistence_api-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arlas-persistence_api-23.0.5.tar", last modified: Sun Mar  5 14:09:31 2023, max compression
+gzip compressed data, was "dist/arlas-persistence_api-24.0.0.tar", last modified: Fri Apr 21 09:27:56 2023, max compression
```

## Comparing `arlas-persistence_api-23.0.5.tar` & `arlas-persistence_api-24.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/
--rw-r--r--   0 container  (1000) container  (1000)      345 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)     4274 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/README.md
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/
--rw-r--r--   0 container  (1000) container  (1000)      345 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)      950 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/SOURCES.txt
--rw-r--r--   0 container  (1000) container  (1000)        1 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/dependency_links.txt
--rw-r--r--   0 container  (1000) container  (1000)       48 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/requires.txt
--rw-r--r--   0 container  (1000) container  (1000)       34 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/top_level.txt
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/
--rw-r--r--   0 container  (1000) container  (1000)      687 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)    24169 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/api_client.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/apis/
--rw-r--r--   0 container  (1000) container  (1000)      107 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/apis/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)    52058 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/apis/persist_api.py
--rw-r--r--   0 container  (1000) container  (1000)     6827 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/configuration.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/
--rw-r--r--   0 container  (1000) container  (1000)      452 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)     4663 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/data_resource.py
--rw-r--r--   0 container  (1000) container  (1000)    10877 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/data_with_links.py
--rw-r--r--   0 container  (1000) container  (1000)     3984 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/error.py
--rw-r--r--   0 container  (1000) container  (1000)     2872 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/exists.py
--rw-r--r--   0 container  (1000) container  (1000)     4776 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/link.py
--rw-r--r--   0 container  (1000) container  (1000)    12809 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/arlas_persistence_api_python/rest.py
--rw-r--r--   0 container  (1000) container  (1000)       38 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/setup.cfg
--rw-r--r--   0 container  (1000) container  (1000)      956 2023-03-05 14:09:30.000000 arlas-persistence_api-23.0.5/setup.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 14:09:31.000000 arlas-persistence_api-23.0.5/test/
--rw-r--r--   0 container  (1000) container  (1000)        0 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/test/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)      933 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/test/test_data_resource.py
--rw-r--r--   0 container  (1000) container  (1000)      943 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/test/test_data_with_links.py
--rw-r--r--   0 container  (1000) container  (1000)      875 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/test/test_error.py
--rw-r--r--   0 container  (1000) container  (1000)      883 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/test/test_exists.py
--rw-r--r--   0 container  (1000) container  (1000)      867 2023-03-05 14:09:20.000000 arlas-persistence_api-23.0.5/test/test_link.py
--rw-r--r--   0 container  (1000) container  (1000)     2287 2023-03-05 14:09:21.000000 arlas-persistence_api-23.0.5/test/test_persist_api.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/
+-rw-r--r--   0 container  (1000) container  (1000)      345 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)     4274 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/README.md
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/
+-rw-r--r--   0 container  (1000) container  (1000)      345 2023-04-21 09:27:55.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)      950 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/SOURCES.txt
+-rw-r--r--   0 container  (1000) container  (1000)        1 2023-04-21 09:27:55.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/dependency_links.txt
+-rw-r--r--   0 container  (1000) container  (1000)       48 2023-04-21 09:27:55.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/requires.txt
+-rw-r--r--   0 container  (1000) container  (1000)       34 2023-04-21 09:27:55.000000 arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/top_level.txt
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/
+-rw-r--r--   0 container  (1000) container  (1000)      687 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)    24169 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/api_client.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/apis/
+-rw-r--r--   0 container  (1000) container  (1000)      107 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/apis/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)    52058 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/apis/persist_api.py
+-rw-r--r--   0 container  (1000) container  (1000)     6827 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/configuration.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/
+-rw-r--r--   0 container  (1000) container  (1000)      452 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)     4663 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/data_resource.py
+-rw-r--r--   0 container  (1000) container  (1000)    10877 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/data_with_links.py
+-rw-r--r--   0 container  (1000) container  (1000)     3984 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/error.py
+-rw-r--r--   0 container  (1000) container  (1000)     2872 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/exists.py
+-rw-r--r--   0 container  (1000) container  (1000)     4776 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/link.py
+-rw-r--r--   0 container  (1000) container  (1000)    12809 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/arlas_persistence_api_python/rest.py
+-rw-r--r--   0 container  (1000) container  (1000)       38 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/setup.cfg
+-rw-r--r--   0 container  (1000) container  (1000)      956 2023-04-21 09:27:54.000000 arlas-persistence_api-24.0.0/setup.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 09:27:56.000000 arlas-persistence_api-24.0.0/test/
+-rw-r--r--   0 container  (1000) container  (1000)        0 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)      933 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_data_resource.py
+-rw-r--r--   0 container  (1000) container  (1000)      943 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_data_with_links.py
+-rw-r--r--   0 container  (1000) container  (1000)      875 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_error.py
+-rw-r--r--   0 container  (1000) container  (1000)      883 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_exists.py
+-rw-r--r--   0 container  (1000) container  (1000)      867 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_link.py
+-rw-r--r--   0 container  (1000) container  (1000)     2287 2023-04-21 09:27:43.000000 arlas-persistence_api-24.0.0/test/test_persist_api.py
```

### Comparing `arlas-persistence_api-23.0.5/README.md` & `arlas-persistence_api-24.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # arlas-persistence-api-python
 persistence REST services
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 23.0.5
+- API version: 24.0.0
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [http://www.gisaia.com/](http://www.gisaia.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api.egg-info/SOURCES.txt` & `arlas-persistence_api-24.0.0/arlas_persistence_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/__init__.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/api_client.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import os
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/apis/persist_api.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/apis/persist_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/configuration.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -215,10 +215,10 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.0.5\n"\
+               "Version of the API: 24.0.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/data_resource.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/data_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/data_with_links.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/data_with_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/error.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/exists.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/exists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/models/link.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-persistence_api-23.0.5/arlas_persistence_api_python/rest.py` & `arlas-persistence_api-24.0.0/arlas_persistence_api_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/setup.py` & `arlas-persistence_api-24.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "arlas-persistence_api"
-VERSION = "23.0.5"
+VERSION = "24.0.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `arlas-persistence_api-23.0.5/test/test_data_resource.py` & `arlas-persistence_api-24.0.0/test/test_data_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/test/test_data_with_links.py` & `arlas-persistence_api-24.0.0/test/test_data_with_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/test/test_error.py` & `arlas-persistence_api-24.0.0/test/test_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/test/test_exists.py` & `arlas-persistence_api-24.0.0/test/test_exists.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/test/test_link.py` & `arlas-persistence_api-24.0.0/test/test_link.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-persistence_api-23.0.5/test/test_persist_api.py` & `arlas-persistence_api-24.0.0/test/test_persist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS persistence API
 
     persistence REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

