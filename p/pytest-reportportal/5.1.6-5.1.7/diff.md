# Comparing `tmp/pytest-reportportal-5.1.6.tar.gz` & `tmp/pytest-reportportal-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportportal-5.1.6.tar", last modified: Tue Mar 28 09:39:53 2023, max compression
+gzip compressed data, was "pytest-reportportal-5.1.7.tar", last modified: Fri Apr 21 13:10:27 2023, max compression
```

## Comparing `pytest-reportportal-5.1.6.tar` & `pytest-reportportal-5.1.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:39:53.000266 pytest-reportportal-5.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-03-28 09:39:53.000266 pytest-reportportal-5.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:39:52.996266 pytest-reportportal-5.1.6/pytest_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/rp_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    31887 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/pytest_reportportal/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:39:53.000266 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 09:39:52.000000 pytest-reportportal-5.1.6/pytest_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-28 09:39:53.000266 pytest-reportportal-5.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-28 09:39:49.000000 pytest-reportportal-5.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/pytest_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/rp_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31887 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/service.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 13:10:27.154582 pytest-reportportal-5.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/setup.py
```

### Comparing `pytest-reportportal-5.1.6/CONTRIBUTING.rst` & `pytest-reportportal-5.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.6/LICENSE` & `pytest-reportportal-5.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.6/PKG-INFO` & `pytest-reportportal-5.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.6
+Version: 5.1.7
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
+Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +39,14 @@
 
 
 Pytest plugin for reporting test results of the Pytest to the Report Portal.
 
 * Usage
 * Installation
 * Configuration
-* Contribution
 * Examples
 * Launching
 * Send attachment (screenshots)
 * Troubleshooting
 * Integration with GA
 * Copyright Notice
 
@@ -58,29 +58,15 @@
 
 To install pytest plugin execute next command in a terminal:
 
 .. code-block:: bash
 
     pip install pytest-reportportal
 
-**IMPORTANT!**
-The latest version **does not** support Report Portal versions below 5.0.0.
 
-Specify the last one release of the client version 1 to install or update the client for other versions of Report Portal below 5.0.0:
-
-.. code-block:: bash
-
-    pip install pytest-reportportal~=1.0
-
-
-Contribution
-~~~~~~~~~~~~~
-
-All the fixes for the agent that supports Report Portal versions below 5.0.0 should go into the v1 branch.
-The master branch will store the code base for the agent for Report Portal versions 5 and above.
 
 Look through the CONTRIBUTING.rst for contribution guidelines.
 
 Configuration
 ~~~~~~~~~~~~~
 
 Prepare the config file :code:`pytest.ini` in root directory of tests or specify
@@ -271,19 +257,19 @@
 deactivate :code:`pytest_reportportal` plugin with command like:
 
 .. code-block:: bash
 
     py.test -p no:pytest_reportportal ./tests
 
 
-Integration with GA
--------------------
+Integration with Google analytics
+---------------------------------
 ReportPortal is now supporting integrations with more than 15 test frameworks simultaneously. In order to define the most popular agents and plan the team workload accordingly, we are using Google analytics.
 
-ReportPortal collects information about agent name and its version only. This information is sent to Google analytics on the launch start. Please help us to make our work effective.
+ReportPortal collects information about agent name and its version only. This information is sent to Google Analytics on the launch start. Please help us to make our work effective.
 If you still want to switch Off Google analytics, please change env variable the way below.
 
 .. code-block:: bash
 
     export AGENT_NO_ANALYTICS=1
```

### Comparing `pytest-reportportal-5.1.6/README.rst` & `pytest-reportportal-5.1.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 Pytest plugin for reporting test results of the Pytest to the Report Portal.
 
 * Usage
 * Installation
 * Configuration
-* Contribution
 * Examples
 * Launching
 * Send attachment (screenshots)
 * Troubleshooting
 * Integration with GA
 * Copyright Notice
 
@@ -40,29 +39,15 @@
 
 To install pytest plugin execute next command in a terminal:
 
 .. code-block:: bash
 
     pip install pytest-reportportal
 
-**IMPORTANT!**
-The latest version **does not** support Report Portal versions below 5.0.0.
 
-Specify the last one release of the client version 1 to install or update the client for other versions of Report Portal below 5.0.0:
-
-.. code-block:: bash
-
-    pip install pytest-reportportal~=1.0
-
-
-Contribution
-~~~~~~~~~~~~~
-
-All the fixes for the agent that supports Report Portal versions below 5.0.0 should go into the v1 branch.
-The master branch will store the code base for the agent for Report Portal versions 5 and above.
 
 Look through the CONTRIBUTING.rst for contribution guidelines.
 
 Configuration
 ~~~~~~~~~~~~~
 
 Prepare the config file :code:`pytest.ini` in root directory of tests or specify
@@ -253,19 +238,19 @@
 deactivate :code:`pytest_reportportal` plugin with command like:
 
 .. code-block:: bash
 
     py.test -p no:pytest_reportportal ./tests
 
 
-Integration with GA
--------------------
+Integration with Google analytics
+---------------------------------
 ReportPortal is now supporting integrations with more than 15 test frameworks simultaneously. In order to define the most popular agents and plan the team workload accordingly, we are using Google analytics.
 
-ReportPortal collects information about agent name and its version only. This information is sent to Google analytics on the launch start. Please help us to make our work effective.
+ReportPortal collects information about agent name and its version only. This information is sent to Google Analytics on the launch start. Please help us to make our work effective.
 If you still want to switch Off Google analytics, please change env variable the way below.
 
 .. code-block:: bash
 
     export AGENT_NO_ANALYTICS=1
```

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal/config.py` & `pytest-reportportal-5.1.7/pytest_reportportal/config.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal/plugin.py` & `pytest-reportportal-5.1.7/pytest_reportportal/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """This module contains changed pytest for report-portal."""
 
+#  Copyright (c) 2023 https://reportportal.io .
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#  https://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License
+
 import logging
-# This program is free software: you can redistribute it
-# and/or modify it under the terms of the GPL licence
 import os.path
 import time
 
 import _pytest.logging
 import dill as pickle
 import pytest
 import requests
@@ -23,14 +34,18 @@
 
 MANDATORY_PARAMETER_MISSED_PATTERN = \
     'One of the following mandatory parameters is unset: ' + \
     'rp_project: {}, ' + \
     'rp_endpoint: {}, ' + \
     'rp_uuid: {}'
 
+FAILED_LAUNCH_WAIT = 'Failed to initialize reportportal-client service. ' \
+                     + 'Waiting for Launch start timed out. ' \
+                     + 'Reporting is disabled.'
+
 
 @pytest.mark.optionalhook
 def pytest_configure_node(node):
     """Configure xdist node controller.
 
     :param node: Object of the xdist WorkerController class
     """
@@ -55,16 +70,17 @@
     """Wait for the launch startup.
 
     :param rp_client: Instance of the ReportPortalService class
     """
     timeout = time.time() + LAUNCH_WAIT_TIMEOUT
     while not rp_client.launch_id:
         if time.time() > timeout:
-            raise Exception("Launch has not started.")
+            return False
         time.sleep(1)
+    return True
 
 
 # noinspection PyProtectedMember
 def pytest_sessionstart(session):
     """Start Report Portal launch.
 
     This method is called every time on control or worker process start, it
@@ -86,15 +102,18 @@
         config._rp_enabled = False
         return
 
     if is_control(config) and not config._reporter_config.rp_launch_id:
         config.py_test_service.start_launch()
         if config.pluginmanager.hasplugin('xdist') \
                 or config.pluginmanager.hasplugin('pytest-parallel'):
-            wait_launch(session.config.py_test_service.rp)
+            if not wait_launch(session.config.py_test_service.rp):
+                log.error(FAILED_LAUNCH_WAIT)
+                config.py_test_service.rp = None
+                config._rp_enabled = False
 
 
 def pytest_collection_finish(session):
     """Collect tests if session is configured.
 
     :param session: Object of the pytest Session class
     """
```

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal/rp_logging.py` & `pytest-reportportal-5.1.7/pytest_reportportal/rp_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal/service.py` & `pytest-reportportal-5.1.7/pytest_reportportal/service.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal.egg-info/PKG-INFO` & `pytest-reportportal-5.1.7/pytest_reportportal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.6
+Version: 5.1.7
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
+Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +39,14 @@
 
 
 Pytest plugin for reporting test results of the Pytest to the Report Portal.
 
 * Usage
 * Installation
 * Configuration
-* Contribution
 * Examples
 * Launching
 * Send attachment (screenshots)
 * Troubleshooting
 * Integration with GA
 * Copyright Notice
 
@@ -58,29 +58,15 @@
 
 To install pytest plugin execute next command in a terminal:
 
 .. code-block:: bash
 
     pip install pytest-reportportal
 
-**IMPORTANT!**
-The latest version **does not** support Report Portal versions below 5.0.0.
 
-Specify the last one release of the client version 1 to install or update the client for other versions of Report Portal below 5.0.0:
-
-.. code-block:: bash
-
-    pip install pytest-reportportal~=1.0
-
-
-Contribution
-~~~~~~~~~~~~~
-
-All the fixes for the agent that supports Report Portal versions below 5.0.0 should go into the v1 branch.
-The master branch will store the code base for the agent for Report Portal versions 5 and above.
 
 Look through the CONTRIBUTING.rst for contribution guidelines.
 
 Configuration
 ~~~~~~~~~~~~~
 
 Prepare the config file :code:`pytest.ini` in root directory of tests or specify
@@ -271,19 +257,19 @@
 deactivate :code:`pytest_reportportal` plugin with command like:
 
 .. code-block:: bash
 
     py.test -p no:pytest_reportportal ./tests
 
 
-Integration with GA
--------------------
+Integration with Google analytics
+---------------------------------
 ReportPortal is now supporting integrations with more than 15 test frameworks simultaneously. In order to define the most popular agents and plan the team workload accordingly, we are using Google analytics.
 
-ReportPortal collects information about agent name and its version only. This information is sent to Google analytics on the launch start. Please help us to make our work effective.
+ReportPortal collects information about agent name and its version only. This information is sent to Google Analytics on the launch start. Please help us to make our work effective.
 If you still want to switch Off Google analytics, please change env variable the way below.
 
 .. code-block:: bash
 
     export AGENT_NO_ANALYTICS=1
```

### Comparing `pytest-reportportal-5.1.6/pytest_reportportal.egg-info/SOURCES.txt` & `pytest-reportportal-5.1.7/pytest_reportportal.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 pytest_reportportal/__init__.py
 pytest_reportportal/config.py
+pytest_reportportal/config.pyi
 pytest_reportportal/errors.py
 pytest_reportportal/plugin.py
+pytest_reportportal/plugin.pyi
 pytest_reportportal/rp_logging.py
 pytest_reportportal/service.py
+pytest_reportportal/service.pyi
 pytest_reportportal.egg-info/PKG-INFO
 pytest_reportportal.egg-info/SOURCES.txt
 pytest_reportportal.egg-info/dependency_links.txt
 pytest_reportportal.egg-info/entry_points.txt
 pytest_reportportal.egg-info/requires.txt
 pytest_reportportal.egg-info/top_level.txt
```

### Comparing `pytest-reportportal-5.1.6/setup.py` & `pytest-reportportal-5.1.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Config for setup package pytest agent."""
 
 import os
 
 from setuptools import setup
 
 
-__version__ = '5.1.6'
+__version__ = '5.1.7'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return:      File content
@@ -20,17 +20,19 @@
 
 setup(
     name='pytest-reportportal',
     version=__version__,
     description='Agent for Reporting results of tests to the Report Portal',
     long_description=read_file('README.rst'),
     long_description_content_type='text/x-rst',
+    author='Report Portal Team',
     author_email='support@reportportal.io',
     url='https://github.com/reportportal/agent-python-pytest',
     packages=['pytest_reportportal'],
+    package_data={'pytest_reportportal': ['*.pyi']},
     install_requires=read_file('requirements.txt').splitlines(),
     license='Apache 2.0',
     keywords=['testing', 'reporting', 'reportportal', 'pytest', 'agent'],
     classifiers=[
         'Framework :: Pytest',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
```

