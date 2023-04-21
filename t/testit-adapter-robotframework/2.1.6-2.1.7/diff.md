# Comparing `tmp/testit-adapter-robotframework-2.1.6.tar.gz` & `tmp/testit-adapter-robotframework-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.1.6.tar", last modified: Wed Apr 12 09:36:28 2023, max compression
+gzip compressed data, was "testit-adapter-robotframework-2.1.7.tar", last modified: Fri Apr 21 08:18:26 2023, max compression
```

## Comparing `testit-adapter-robotframework-2.1.6.tar` & `testit-adapter-robotframework-2.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:28.053650 testit-adapter-robotframework-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-12 09:36:28.053650 testit-adapter-robotframework-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:36:28.053650 testit-adapter-robotframework-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:28.049650 testit-adapter-robotframework-2.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:28.053650 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-12 09:35:58.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:28.053650 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-12 09:36:28.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 09:36:28.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:36:28.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 09:36:28.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 09:36:28.000000 testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.937446 testit-adapter-robotframework-2.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.1.6/PKG-INFO` & `testit-adapter-robotframework-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.6
+Version: 2.1.7
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.1.6/README.md` & `testit-adapter-robotframework-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.6/setup.py` & `testit-adapter-robotframework-2.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.1.6',
+    version='2.1.7',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.6']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.7']
 )
```

### Comparing `testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/TMSLibrary.py` & `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from robot.libraries.BuiltIn import BuiltIn
 
-from testit_python_commons.services import AdapterManager
+from testit_python_commons.services import TmsPluginManager
 
 from .listeners import AutotestAdapter, TestRunAdapter
 from .models import Link, Option
 
 
 def enabled(func):
     def wrapped(self, *args, **kwargs):
@@ -40,15 +40,15 @@
         built_in = BuiltIn()
         self.enabled = built_in.get_variable_value("${testit}", None) is not None
         if self.enabled:
             cli_params = ["tmsUrl", "tmsPrivateToken", "tmsProjectId",
                           "tmsConfigurationId", "tmsTestRunId", "tmsTestRunName",
                           "tmsAdapterMode", "tmsConfigFile", "tmsCertValidation", "tmsAutomaticCreationTestCases"]
             option = Option(**{param: built_in.get_variable_value(f'${{{param}}}', None) for param in cli_params})
-            self.adapter_manager = AdapterManager(option)
+            self.adapter_manager = TmsPluginManager.get_adapter_manager(option)
             pabot_index = built_in.get_variable_value('${PABOTQUEUEINDEX}', None)
             if pabot_index is not None:
                 try:
                     from pabot import PabotLib
                     pabot = PabotLib()
                     if int(pabot_index) == 0:
                         test_run_id = self.adapter_manager.get_test_run_id()
```

### Comparing `testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/listeners.py` & `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework/models.py` & `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/models.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.6
+Version: 2.1.7
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.1.6/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

