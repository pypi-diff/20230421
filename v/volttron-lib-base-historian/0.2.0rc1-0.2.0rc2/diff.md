# Comparing `tmp/volttron_lib_base_historian-0.2.0rc1.tar.gz` & `tmp/volttron_lib_base_historian-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_base_historian-0.2.0rc1.tar", max compression
+gzip compressed data, was "volttron_lib_base_historian-0.2.0rc2.tar", max compression
```

## Comparing `volttron_lib_base_historian-0.2.0rc1.tar` & `volttron_lib_base_historian-0.2.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11928 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     2612 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/README.md
--rw-r--r--   0        0        0     1372 2023-03-26 19:37:16.842716 volttron_lib_base_historian-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1250 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/src/historian/base/__init__.py
--rw-r--r--   0        0        0    96502 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/src/historian/base/base_historian.py
--rw-r--r--   0        0        0        0 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/tests/historian/testing/__init__.py
--rw-r--r--   0        0        0    19974 2023-03-26 19:35:12.312310 volttron_lib_base_historian-0.2.0rc1/tests/historian/testing/integration_test_interface.py
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc1/setup.py
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     2612 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/README.md
+-rw-r--r--   0        0        0     1278 2023-04-20 22:06:16.756125 volttron_lib_base_historian-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1250 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/src/historian/base/__init__.py
+-rw-r--r--   0        0        0    96502 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/src/historian/base/base_historian.py
+-rw-r--r--   0        0        0        0 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/tests/historian/testing/__init__.py
+-rw-r--r--   0        0        0    20260 2023-04-20 22:03:26.515373 volttron_lib_base_historian-0.2.0rc2/tests/historian/testing/integration_test_interface.py
+-rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc2/setup.py
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc2/PKG-INFO
```

### Comparing `volttron_lib_base_historian-0.2.0rc1/LICENSE` & `volttron_lib_base_historian-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc1/README.md` & `volttron_lib_base_historian-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc1/pyproject.toml` & `volttron_lib_base_historian-0.2.0rc2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-lib-base-historian"
-version = "0.2.0rc1"
+version = "0.2.0rc2"
 description = "A base library with extension points for using with the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 keywords = []
@@ -46,12 +46,7 @@
 column_limit = 99
 split_before_logical_operator = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-# tasks
-git-changelog = ">=0.5.0"
-httpx = ">=0.16.1"
-jinja2-cli = ">=0.7.0"
-toml = ">=0.10.2"
```

### Comparing `volttron_lib_base_historian-0.2.0rc1/src/historian/base/__init__.py` & `volttron_lib_base_historian-0.2.0rc2/src/historian/base/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc1/src/historian/base/base_historian.py` & `volttron_lib_base_historian-0.2.0rc2/src/historian/base/base_historian.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc1/tests/historian/testing/integration_test_interface.py` & `volttron_lib_base_historian-0.2.0rc2/tests/historian/testing/integration_test_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,18 +346,25 @@
         # Publish messages
         fake_agent.vip.pubsub.publish('pubsub', DEVICES_ALL_TOPIC, headers, all_message)
 
         gevent.sleep(2)
 
         pattern_1 = None
         # Query the historian
-        with pytest.raises(RemoteError):
-            fake_agent.vip.rpc.call('platform.historian',
+        # Should return empty or throw RemoteError due to None
+        try:
+            return_value = fake_agent.vip.rpc.call('platform.historian',
                                     'get_topics_by_pattern',
                                     topic_pattern=pattern_1).get(timeout=10)
+            # postgresql historian handles none and return empty result
+            assert not return_value
+        except RemoteError as e:
+            # SQLiteHistorian through None type exception
+            print(f"Exception {e}")
+
 
     def test_get_version(self, historian, fake_agent):
         """
         Test the get_version api
         Expected result: Not null value
 
         :param fake_agent: instance of fake volttron agent used to query
```

### Comparing `volttron_lib_base_historian-0.2.0rc1/setup.py` & `volttron_lib_base_historian-0.2.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'volttron>=10.0.2rc0,<11.0']
 
 setup_kwargs = {
     'name': 'volttron-lib-base-historian',
-    'version': '0.2.0rc1',
+    'version': '0.2.0rc2',
     'description': 'A base library with extension points for using with the VOLTTRON platform.',
     'long_description': '[![Run Pytests](https://github.com/eclipse-volttron/volttron-lib-base-historian/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-base-historian/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-lib-base-historian.svg)](https://pypi.org/project/volttron-lib-base-historian/)\n\nVOLTTRON base historian framework that provide common functions such as caching, error handling, input validation etc. This historian cannot be used as agent as is. VOLTTRON historian agents can be created by subclassing the [BaseHistorian class](https://github.com/eclipse-volttron/volttron-lib-base-historian/blob/develop/src/historian/base/base_historian.py) in this library.\n\n## Requirements\n\n - Python >= 3.8\n\n## Installation\n\nThis library can be installed using ```pip install volttron-lib-base-historian```. However, this is not necessary. Any \nhistorian agent that uses this library will automatically install it as part of its installation. For example, \ninstalling [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) will automatically install \nvolttron-lib-base-historian into the same python environment\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/eclipse-volttron/volttron-lib-base-historian',
```

### Comparing `volttron_lib_base_historian-0.2.0rc1/PKG-INFO` & `volttron_lib_base_historian-0.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-base-historian
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: A base library with extension points for using with the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-base-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

