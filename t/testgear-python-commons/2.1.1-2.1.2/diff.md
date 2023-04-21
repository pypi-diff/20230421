# Comparing `tmp/testgear-python-commons-2.1.1.tar.gz` & `tmp/testgear-python-commons-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-python-commons-2.1.1.tar", last modified: Fri Mar 31 06:29:43 2023, max compression
+gzip compressed data, was "testgear-python-commons-2.1.2.tar", last modified: Fri Apr 21 14:54:27 2023, max compression
```

## Comparing `testgear-python-commons-2.1.1.tar` & `testgear-python-commons-2.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.510933 testgear-python-commons-2.1.1/
--rw-rw-rw-   0        0        0      604 2023-03-31 06:29:43.510933 testgear-python-commons-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-03-27 12:00:18.000000 testgear-python-commons-2.1.1/README.md
--rw-rw-rw-   0        0        0      113 2023-03-27 12:00:18.000000 testgear-python-commons-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 06:29:43.510933 testgear-python-commons-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.481038 testgear-python-commons-2.1.1/src/
--rw-rw-rw-   0        0        0      882 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.481038 testgear-python-commons-2.1.1/src/testgear_python_commons/
--rw-rw-rw-   0        0        0        0 2022-10-10 11:17:51.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/__init__.py
--rw-rw-rw-   0        0        0     7755 2023-03-31 06:05:19.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/app_properties.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.495291 testgear-python-commons-2.1.1/src/testgear_python_commons/client/
--rw-rw-rw-   0        0        0      176 2023-03-31 06:07:11.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/client/__init__.py
--rw-rw-rw-   0        0        0     5302 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/client/api_client.py
--rw-rw-rw-   0        0        0     2012 2023-03-31 06:06:58.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/client/client_configuration.py
--rw-rw-rw-   0        0        0    10044 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/client/converter.py
--rw-rw-rw-   0        0        0     4613 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/decorators.py
--rw-rw-rw-   0        0        0     4086 2023-03-31 06:04:54.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/dynamic_methods.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.495291 testgear-python-commons-2.1.1/src/testgear_python_commons/models/
--rw-rw-rw-   0        0        0       97 2023-03-31 06:06:33.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/models/__init__.py
--rw-rw-rw-   0        0        0       91 2022-10-10 11:17:51.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/models/adapter_mode.py
--rw-rw-rw-   0        0        0      180 2022-10-10 11:17:51.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/models/link_type.py
--rw-rw-rw-   0        0        0      116 2022-11-01 10:54:32.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/models/outcome_type.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.510933 testgear-python-commons-2.1.1/src/testgear_python_commons/services/
--rw-rw-rw-   0        0        0      387 2023-03-31 06:06:12.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/__init__.py
--rw-rw-rw-   0        0        0     2159 2023-03-31 06:06:04.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/adapter_manager.py
--rw-rw-rw-   0        0        0     1265 2023-03-31 06:05:58.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/adapter_manager_configuration.py
--rw-rw-rw-   0        0        0     1601 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/logger.py
--rw-rw-rw-   0        0        0     1717 2023-03-31 06:05:40.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/plugin_manager.py
--rw-rw-rw-   0        0        0    11721 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/services/utils.py
--rw-rw-rw-   0        0        0     5279 2023-03-31 06:28:55.000000 testgear-python-commons-2.1.1/src/testgear_python_commons/step.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:29:43.495291 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/
--rw-rw-rw-   0        0        0      604 2023-03-31 06:29:43.000000 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-03-31 06:29:43.000000 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:29:43.000000 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-03-31 06:29:43.000000 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-03-31 06:29:43.000000 testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/
+-rw-rw-rw-   0        0        0      563 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/README.md
+-rw-rw-rw-   0        0        0      113 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-21 13:52:57.000000 testgear-python-commons-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/
+-rw-rw-rw-   0        0        0      882 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/testgear_python_commons/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/__init__.py
+-rw-rw-rw-   0        0        0     7773 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/app_properties.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/client/
+-rw-rw-rw-   0        0        0      176 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/__init__.py
+-rw-rw-rw-   0        0        0     5302 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/api_client.py
+-rw-rw-rw-   0        0        0     2012 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/client_configuration.py
+-rw-rw-rw-   0        0        0    10032 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/converter.py
+-rw-rw-rw-   0        0        0     4715 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/decorators.py
+-rw-rw-rw-   0        0        0     4144 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/dynamic_methods.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/models/
+-rw-rw-rw-   0        0        0       97 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/adapter_mode.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/link_type.py
+-rw-rw-rw-   0        0        0      116 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/outcome_type.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/services/
+-rw-rw-rw-   0        0        0      387 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager.py
+-rw-rw-rw-   0        0        0     1265 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager_configuration.py
+-rw-rw-rw-   0        0        0     1601 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/logger.py
+-rw-rw-rw-   0        0        0     1717 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/plugin_manager.py
+-rw-rw-rw-   0        0        0    13482 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/utils.py
+-rw-rw-rw-   0        0        0     5281 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/step.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-04-21 14:54:27.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/top_level.txt
```

### Comparing `testgear-python-commons-2.1.1/PKG-INFO` & `testgear-python-commons-2.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: testgear-python-commons
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python commons for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `testgear-python-commons-2.1.1/setup.py` & `testgear-python-commons-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testgear-python-commons',
-    version='2.1.1',
+    version='2.1.2',
     description='Python commons for Test Gear',
     url='https://github.com/testgear-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@test-gear.io',
     license='Apache-2.0',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `testgear-python-commons-2.1.1/src/testgear.py` & `testgear-python-commons-2.1.2/src/testgear.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from testgear_python_commons.decorators import (
+    className,
     description,
     displayName,
-    nameSpace,
-    className,
     externalID,
     externalId,
     labels,
     link,
     links,
+    nameSpace,
     title,
     workItemID,
     workItemIds
 )
 from testgear_python_commons.dynamic_methods import (
     addAttachments,
     addLink,
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/app_properties.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/app_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,16 @@
         if f'{cls.__env_prefix}_ADAPTER_MODE' in os.environ.keys():
             env_properties['adaptermode'] = os.environ.get(f'{cls.__env_prefix}_ADAPTER_MODE')
 
         if f'{cls.__env_prefix}_CERT_VALIDATION' in os.environ.keys():
             env_properties['certvalidation'] = os.environ.get(f'{cls.__env_prefix}_CERT_VALIDATION')
 
         if f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES' in os.environ.keys():
-            env_properties['automaticcreationtestcases'] = os.environ.get(f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
+            env_properties['automaticcreationtestcases'] = os.environ.get(
+                f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
 
         return env_properties
 
     @staticmethod
     def __check_properties(properties: dict):
         adapter_mode = properties.get('adaptermode')
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/client/api_client.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/client/api_client.py`

 * *Files identical despite different names*

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/client/client_configuration.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/client/converter.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/client/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from testgear_api_client.models import (
-    AutoTestStepModel,
-    AvailableTestResultOutcome,
     AttachmentPutModelAutoTestStepResultsModel,
     AutoTestPostModel,
     AutoTestPutModel,
     AutoTestResultsForTestRunModel,
+    AutoTestStepModel,
+    AvailableTestResultOutcome,
     LinkPostModel,
     LinkPutModel,
     LinkType,
     TestRunV2PostShortModel
 )
+
 from testgear_python_commons.services.logger import adapter_logger
 
 
 class Converter:
     @classmethod
     @adapter_logger
     def test_run_to_test_run_short_model(cls, project_id, name):
@@ -263,16 +264,15 @@
             outcome: str,
             description: str = None,
             duration: str = None,
             parameters: list = None,
             attachments: list = None,
             started_on: str = None,
             completed_on: str = None,
-            step_results: list = None
-            ):
+            step_results: list = None):
         return AttachmentPutModelAutoTestStepResultsModel(
             title=title,
             outcome=AvailableTestResultOutcome(outcome),
             description=description,
             duration=duration,
             parameters=parameters,
             attachments=attachments,
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/decorators.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+import types
 from functools import wraps
 
 from testgear_python_commons.services.logger import adapter_logger
 from testgear_python_commons.services.utils import Utils
 
 
 def inner(function):
@@ -11,17 +13,19 @@
             function.test_properties = {}
 
             for key, value in kwargs.items():
                 if hasattr(function,
                            'callspec') and key not in function.callspec.params:
                     function.test_properties[key] = str(value)
         function(*args, **kwargs)
-        return function
 
-    return wrapper
+    if isinstance(function, types.FunctionType):
+        return wrapper
+
+    return function
 
 
 @Utils.deprecated('Use "workItemIds" instead.')
 @adapter_logger
 def workItemID(*test_workitems_id: int or str):  # noqa: N802
     def outer(function):
         function.test_workitems_id = []
@@ -141,13 +145,13 @@
                     function.test_links.append(
                         {'url': link['url'],
                          'title': link['title'] if 'title' in link else None,
                          'type': link['type'] if 'type' in link else None,
                          'description': link['description'] if 'description' in link else None}
                     )
                 else:
-                    print(f'Link ({link}) can\'t be processed!')
+                    logging.warning(f'Link ({link}) can\'t be processed!')
         else:
-            print(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
+            logging.warning(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
         return inner(function)
 
     return outer
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/dynamic_methods.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/dynamic_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from testgear_python_commons.services import TmsPluginManager
 from testgear_python_commons.services.logger import adapter_logger
 from testgear_python_commons.services.utils import Utils
 from testgear_python_commons.step import Step
 
 
 @Utils.deprecated('Use "addLinks" instead.')
@@ -35,17 +37,17 @@
             )
         elif links and (isinstance(links, list) or isinstance(links, tuple)):
             for link in links:
                 if isinstance(link, dict) and 'url' in link:
                     TmsPluginManager.get_plugin_manager().hook \
                         .add_link(link=link)
                 else:
-                    print(f'Link ({link}) can\'t be processed!')
+                    logging.warning(f'Link ({link}) can\'t be processed!')
         else:
-            print("Links can't be processed!\nPlease, set 'url' or 'links'!")
+            logging.warning("Links can't be processed!\nPlease, set 'url' or 'links'!")
 
 
 @Utils.deprecated('Use "addMessage" instead.')
 @adapter_logger
 def message(test_message: str):
     if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
         TmsPluginManager.get_plugin_manager().hook \
@@ -79,15 +81,15 @@
                 name)
         else:
             if isinstance(data, str):
                 Step.add_attachments([data])
             elif isinstance(data, tuple) or isinstance(data, list):
                 Step.add_attachments(data)
             else:
-                print(f'File ({data}) not found!')
+                logging.warning(f'File ({data}) not found!')
     else:
         if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
             Step.create_attachment(str(data), name)
             TmsPluginManager.get_plugin_manager().hook \
                 .create_attachment(
                 body=str(data),
                 name=name)
@@ -95,8 +97,8 @@
             if isinstance(data, str):
                 TmsPluginManager.get_plugin_manager().hook \
                     .add_attachments(attach_paths=[data])
             elif isinstance(data, tuple) or isinstance(data, list):
                 TmsPluginManager.get_plugin_manager().hook \
                     .add_attachments(attach_paths=data)
             else:
-                print(f'({data}) is not path!')
+                logging.warning(f'({data}) is not path!')
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/services/adapter_manager.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import uuid
 
 from testgear_python_commons.client.api_client import ApiClientWorker
 from testgear_python_commons.client.client_configuration import ClientConfiguration
-from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
 from testgear_python_commons.models.adapter_mode import AdapterMode
+from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
 from testgear_python_commons.services.logger import adapter_logger
 
 
 class AdapterManager:
     def __init__(
             self,
             adapter_configuration: AdapterManagerConfiguration,
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/services/adapter_manager_configuration.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/services/logger.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/services/logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-
 from functools import wraps
 
 from testgear_python_commons.services.plugin_manager import TmsPluginManager
 
 
 def adapter_logger(function):
     @wraps(function)
@@ -27,14 +26,15 @@
             message += f' with result: {result}'
 
         logger.debug(message)
 
         return result
     return wrapper
 
+
 def get_function_parameters(function, *args, **kwargs):
     parameters = {}
     args_default_values = inspect.getfullargspec(function).defaults
 
     if args or args_default_values:
         all_keys = inspect.getfullargspec(function).args
         all_args = list(args)
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/services/plugin_manager.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons/step.py` & `testgear-python-commons-2.1.2/src/testgear_python_commons/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 
 from testgear_python_commons.services import (
     TmsPluginManager,
     Utils
 )
 
+
 class Step:
     step_stack = []
     steps_data = []
     steps_data_results = []
     attachments = []
 
     def __init__(self, *args, **kwargs):
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/PKG-INFO` & `testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: testgear-python-commons
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python commons for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `testgear-python-commons-2.1.1/src/testgear_python_commons.egg-info/SOURCES.txt` & `testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

