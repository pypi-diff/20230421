# Comparing `tmp/arlas-permissions_api-23.0.5.tar.gz` & `tmp/arlas-permissions_api-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arlas-permissions_api-23.0.5.tar", last modified: Sun Mar  5 17:04:20 2023, max compression
+gzip compressed data, was "dist/arlas-permissions_api-24.0.0.tar", last modified: Fri Apr 21 08:29:49 2023, max compression
```

## Comparing `arlas-permissions_api-23.0.5.tar` & `arlas-permissions_api-24.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/
--rw-r--r--   0 container  (1000) container  (1000)      345 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)     2472 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/README.md
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/
--rw-r--r--   0 container  (1000) container  (1000)      345 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)      732 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/SOURCES.txt
--rw-r--r--   0 container  (1000) container  (1000)        1 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/dependency_links.txt
--rw-r--r--   0 container  (1000) container  (1000)       48 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/requires.txt
--rw-r--r--   0 container  (1000) container  (1000)       34 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/top_level.txt
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/
--rw-r--r--   0 container  (1000) container  (1000)      568 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)    24169 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/api_client.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/apis/
--rw-r--r--   0 container  (1000) container  (1000)      111 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/apis/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)     5643 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/apis/authorize_api.py
--rw-r--r--   0 container  (1000) container  (1000)     6827 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/configuration.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/
--rw-r--r--   0 container  (1000) container  (1000)      350 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)     3984 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/error.py
--rw-r--r--   0 container  (1000) container  (1000)     3518 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/resource.py
--rw-r--r--   0 container  (1000) container  (1000)    12809 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/arlas_permissions_api_python/rest.py
--rw-r--r--   0 container  (1000) container  (1000)       38 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/setup.cfg
--rw-r--r--   0 container  (1000) container  (1000)      956 2023-03-05 17:04:18.000000 arlas-permissions_api-23.0.5/setup.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-03-05 17:04:20.000000 arlas-permissions_api-23.0.5/test/
--rw-r--r--   0 container  (1000) container  (1000)        0 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/test/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)      898 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/test/test_authorize_api.py
--rw-r--r--   0 container  (1000) container  (1000)      875 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/test/test_error.py
--rw-r--r--   0 container  (1000) container  (1000)      899 2023-03-05 17:04:11.000000 arlas-permissions_api-23.0.5/test/test_resource.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/
+-rw-r--r--   0 container  (1000) container  (1000)      345 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)     2472 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/README.md
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/
+-rw-r--r--   0 container  (1000) container  (1000)      345 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)      732 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/SOURCES.txt
+-rw-r--r--   0 container  (1000) container  (1000)        1 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/dependency_links.txt
+-rw-r--r--   0 container  (1000) container  (1000)       48 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/requires.txt
+-rw-r--r--   0 container  (1000) container  (1000)       34 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/top_level.txt
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/
+-rw-r--r--   0 container  (1000) container  (1000)      568 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)    24169 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/api_client.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/apis/
+-rw-r--r--   0 container  (1000) container  (1000)      111 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/apis/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)     5643 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/apis/authorize_api.py
+-rw-r--r--   0 container  (1000) container  (1000)     6827 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/configuration.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/
+-rw-r--r--   0 container  (1000) container  (1000)      350 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)     3984 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/error.py
+-rw-r--r--   0 container  (1000) container  (1000)     3518 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/resource.py
+-rw-r--r--   0 container  (1000) container  (1000)    12809 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/arlas_permissions_api_python/rest.py
+-rw-r--r--   0 container  (1000) container  (1000)       38 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/setup.cfg
+-rw-r--r--   0 container  (1000) container  (1000)      956 2023-04-21 08:29:46.000000 arlas-permissions_api-24.0.0/setup.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-21 08:29:49.000000 arlas-permissions_api-24.0.0/test/
+-rw-r--r--   0 container  (1000) container  (1000)        0 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/test/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)      898 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/test/test_authorize_api.py
+-rw-r--r--   0 container  (1000) container  (1000)      875 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/test/test_error.py
+-rw-r--r--   0 container  (1000) container  (1000)      899 2023-04-21 08:29:39.000000 arlas-permissions_api-24.0.0/test/test_resource.py
```

### Comparing `arlas-permissions_api-23.0.5/README.md` & `arlas-permissions_api-24.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # arlas-permissions-api-python
 permissions REST services
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 23.0.5
+- API version: 24.0.0
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [http://www.gisaia.com/](http://www.gisaia.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api.egg-info/SOURCES.txt` & `arlas-permissions_api-24.0.0/arlas_permissions_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/__init__.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/api_client.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import os
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/apis/authorize_api.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/apis/authorize_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/configuration.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
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

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/error.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/models/resource.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/models/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-permissions_api-23.0.5/arlas_permissions_api_python/rest.py` & `arlas-permissions_api-24.0.0/arlas_permissions_api_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-permissions_api-23.0.5/setup.py` & `arlas-permissions_api-24.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "arlas-permissions_api"
-VERSION = "23.0.5"
+VERSION = "24.0.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `arlas-permissions_api-23.0.5/test/test_authorize_api.py` & `arlas-permissions_api-24.0.0/test/test_authorize_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-permissions_api-23.0.5/test/test_error.py` & `arlas-permissions_api-24.0.0/test/test_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-permissions_api-23.0.5/test/test_resource.py` & `arlas-permissions_api-24.0.0/test/test_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS permissions API
 
     permissions REST services
 
-    OpenAPI spec version: 23.0.5
+    OpenAPI spec version: 24.0.0
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

