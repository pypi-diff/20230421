# Comparing `tmp/testit-python-commons-2.1.6.tar.gz` & `tmp/testit-python-commons-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-python-commons-2.1.6.tar", last modified: Wed Apr 12 09:36:34 2023, max compression
+gzip compressed data, was "testit-python-commons-2.1.7.tar", last modified: Fri Apr 21 08:18:33 2023, max compression
```

## Comparing `testit-python-commons-2.1.6.tar` & `testit-python-commons-2.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/outcome_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.373439 testit-python-commons-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 08:18:33.369439 testit-python-commons-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:33.373439 testit-python-commons-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.365439 testit-python-commons-2.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.365439 testit-python-commons-2.1.7/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.369439 testit-python-commons-2.1.7/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.369439 testit-python-commons-2.1.7/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/models/outcome_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.369439 testit-python-commons-2.1.7/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-21 08:17:56.000000 testit-python-commons-2.1.7/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:33.365439 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 08:18:33.000000 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-21 08:18:33.000000 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:33.000000 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 08:18:33.000000 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 08:18:33.000000 testit-python-commons-2.1.7/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit-python-commons-2.1.6/PKG-INFO` & `testit-python-commons-2.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.6/setup.py` & `testit-python-commons-2.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='2.1.6',
+    version='2.1.7',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-python-commons-2.1.6/src/testit.py` & `testit-python-commons-2.1.7/src/testit.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/app_properties.py` & `testit-python-commons-2.1.7/src/testit_python_commons/app_properties.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/client/api_client.py` & `testit-python-commons-2.1.7/src/testit_python_commons/client/api_client.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/client/client_configuration.py` & `testit-python-commons-2.1.7/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/client/converter.py` & `testit-python-commons-2.1.7/src/testit_python_commons/client/converter.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/decorators.py` & `testit-python-commons-2.1.7/src/testit_python_commons/decorators.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/dynamic_methods.py` & `testit-python-commons-2.1.7/src/testit_python_commons/dynamic_methods.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager.py` & `testit-python-commons-2.1.7/src/testit_python_commons/services/adapter_manager.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit-python-commons-2.1.7/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/services/logger.py` & `testit-python-commons-2.1.7/src/testit_python_commons/services/logger.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/services/plugin_manager.py` & `testit-python-commons-2.1.7/src/testit_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/services/utils.py` & `testit-python-commons-2.1.7/src/testit_python_commons/services/utils.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons/step.py` & `testit-python-commons-2.1.7/src/testit_python_commons/step.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons.egg-info/PKG-INFO` & `testit-python-commons-2.1.7/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.6/src/testit_python_commons.egg-info/SOURCES.txt` & `testit-python-commons-2.1.7/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

