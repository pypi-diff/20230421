# Comparing `tmp/apache-airflow-providers-apache-beam-4.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-beam-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-beam-4.3.0rc1.tar", last modified: Sat Feb 18 20:35:03 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.0.0rc1.tar", last modified: Fri Apr 21 19:47:56 2023, max compression
```

## Comparing `apache-airflow-providers-apache-beam-4.3.0rc1.tar` & `apache-airflow-providers-apache-beam-5.0.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-apache-beam-4.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-18 20:35:02.000000 apache-airflow-providers-apache-beam-4.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-apache-beam-4.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14109 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12524 2023-02-18 20:35:02.000000 apache-airflow-providers-apache-beam-4.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-02-18 20:35:02.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14199 2023-02-17 14:47:51.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/hooks/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33377 2023-01-26 14:58:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/operators/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14109 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-11 18:49:53.000000 apache-airflow-providers-apache-beam-4.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1879 2023-02-18 20:35:03.000000 apache-airflow-providers-apache-beam-4.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1571 2023-02-18 20:35:02.000000 apache-airflow-providers-apache-beam-4.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12986 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14199 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-04-21 10:05:41.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-apache-beam-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/LICENSE` & `apache-airflow-providers-apache-beam-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-beam-5.0.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/PKG-INFO` & `apache-airflow-providers-apache-beam-5.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 4.3.0rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -50,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``4.3.0rc1``
+Release: ``5.0.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -130,14 +129,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS and Dataflow hooks' param ``delegate_to`` is removed from all Beam operators.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Get rid of state in Apache Beam provider hook (#29503)``
@@ -397,9 +411,7 @@
 * ``Corrections in docs and tools after releasing provider RCs (#14082)``
 * ``Remove WARNINGs from BeamHook (#14554)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/README.rst` & `apache-airflow-providers-apache-beam-5.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``4.3.0rc1``
+Release: ``5.0.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -95,14 +95,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS and Dataflow hooks' param ``delegate_to`` is removed from all Beam operators.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Get rid of state in Apache Beam provider hook (#29503)``
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/__init__.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/get_provider_info.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-beam",
         "name": "Apache Beam",
         "description": "`Apache Beam <https://beam.apache.org/>`__.\n",
+        "suspended": False,
         "versions": [
+            "5.0.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
             "4.0.0",
             "3.4.0",
             "3.3.0",
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/hooks/__init__.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/hooks/beam.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/operators/__init__.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/airflow/providers/apache/beam/operators/beam.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/beam.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 """This module contains Apache Beam operators."""
 from __future__ import annotations
 
 import copy
 import os
 import stat
 import tempfile
-import warnings
 from abc import ABC, ABCMeta, abstractmethod
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import ExitStack
 from functools import partial
 from typing import TYPE_CHECKING, Callable, Sequence
 
 from airflow import AirflowException
@@ -53,15 +52,14 @@
     :class:`~airflow.providers.apache.beam.operators.beam.BeamRunJavaPipelineOperator` and
     :class:`~airflow.providers.apache.beam.operators.beam.BeamRunGoPipelineOperator`.
     """
 
     dataflow_hook: DataflowHook | None
     dataflow_config: DataflowConfiguration
     gcp_conn_id: str
-    delegate_to: str | None
     dataflow_support_impersonation: bool = True
 
     def _set_dataflow(
         self,
         pipeline_options: dict,
         job_name_variable_key: str | None = None,
     ) -> tuple[str, dict, Callable[[str], None]]:
@@ -73,15 +71,14 @@
         )
         process_line_callback = self.__get_dataflow_process_callback()
         return dataflow_job_name, pipeline_options, process_line_callback
 
     def __set_dataflow_hook(self) -> DataflowHook:
         self.dataflow_hook = DataflowHook(
             gcp_conn_id=self.dataflow_config.gcp_conn_id or self.gcp_conn_id,
-            delegate_to=self.dataflow_config.delegate_to or self.delegate_to,
             poll_sleep=self.dataflow_config.poll_sleep,
             impersonation_chain=self.dataflow_config.impersonation_chain,
             drain_pipeline=self.dataflow_config.drain_pipeline,
             cancel_timeout=self.dataflow_config.cancel_timeout,
             wait_until_finished=self.dataflow_config.wait_until_finished,
         )
         return self.dataflow_hook
@@ -142,43 +139,33 @@
           If the value is ``['A', 'B']`` and the key is ``key`` then the ``--key=A --key=B`` options
           will be left
         * Other value types will be replaced with the Python textual representation.
 
         When defining labels (labels option), you can also provide a dictionary.
     :param gcp_conn_id: Optional.
         The connection ID to use connecting to Google Cloud Storage if python file is on GCS.
-    :param delegate_to:  Optional.
-        The account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
     :param dataflow_config: Dataflow configuration, used when runner type is set to DataflowRunner,
         (optional) defaults to None.
     """
 
     def __init__(
         self,
         *,
         runner: str = "DirectRunner",
         default_pipeline_options: dict | None = None,
         pipeline_options: dict | None = None,
         gcp_conn_id: str = "google_cloud_default",
-        delegate_to: str | None = None,
         dataflow_config: DataflowConfiguration | dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.runner = runner
         self.default_pipeline_options = default_pipeline_options or {}
         self.pipeline_options = pipeline_options or {}
         self.gcp_conn_id = gcp_conn_id
-        if delegate_to:
-            warnings.warn(
-                "'delegate_to' parameter is deprecated, please use 'impersonation_chain'", DeprecationWarning
-            )
-        self.delegate_to = delegate_to
         if isinstance(dataflow_config, dict):
             self.dataflow_config = DataflowConfiguration(**dataflow_config)
         else:
             self.dataflow_config = dataflow_config or DataflowConfiguration()
         self.beam_hook: BeamHook | None = None
         self.dataflow_hook: DataflowHook | None = None
         self.dataflow_job_id: str | None = None
@@ -269,24 +256,22 @@
         default_pipeline_options: dict | None = None,
         pipeline_options: dict | None = None,
         py_interpreter: str = "python3",
         py_options: list[str] | None = None,
         py_requirements: list[str] | None = None,
         py_system_site_packages: bool = False,
         gcp_conn_id: str = "google_cloud_default",
-        delegate_to: str | None = None,
         dataflow_config: DataflowConfiguration | dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(
             runner=runner,
             default_pipeline_options=default_pipeline_options,
             pipeline_options=pipeline_options,
             gcp_conn_id=gcp_conn_id,
-            delegate_to=delegate_to,
             dataflow_config=dataflow_config,
             **kwargs,
         )
 
         self.py_file = py_file
         self.py_options = py_options or []
         self.py_interpreter = py_interpreter
@@ -306,15 +291,15 @@
         ) = self._init_pipeline_options(format_pipeline_options=True, job_name_variable_key="job_name")
 
         if not self.beam_hook:
             raise AirflowException("Beam hook is not defined.")
 
         with ExitStack() as exit_stack:
             if self.py_file.lower().startswith("gs://"):
-                gcs_hook = GCSHook(self.gcp_conn_id, self.delegate_to)
+                gcs_hook = GCSHook(gcp_conn_id=self.gcp_conn_id)
                 tmp_gcs_file = exit_stack.enter_context(gcs_hook.provide_file(object_url=self.py_file))
                 self.py_file = tmp_gcs_file.name
 
             if is_dataflow and self.dataflow_hook:
                 with self.dataflow_hook.provide_authorized_gcloud():
                     self.beam_hook.start_python_pipeline(
                         variables=snake_case_pipeline_options,
@@ -407,24 +392,22 @@
         *,
         jar: str,
         runner: str = "DirectRunner",
         job_class: str | None = None,
         default_pipeline_options: dict | None = None,
         pipeline_options: dict | None = None,
         gcp_conn_id: str = "google_cloud_default",
-        delegate_to: str | None = None,
         dataflow_config: DataflowConfiguration | dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(
             runner=runner,
             default_pipeline_options=default_pipeline_options,
             pipeline_options=pipeline_options,
             gcp_conn_id=gcp_conn_id,
-            delegate_to=delegate_to,
             dataflow_config=dataflow_config,
             **kwargs,
         )
         self.jar = jar
         self.job_class = job_class
 
     def execute(self, context: Context):
@@ -437,15 +420,15 @@
         ) = self._init_pipeline_options()
 
         if not self.beam_hook:
             raise AirflowException("Beam hook is not defined.")
 
         with ExitStack() as exit_stack:
             if self.jar.lower().startswith("gs://"):
-                gcs_hook = GCSHook(self.gcp_conn_id, self.delegate_to)
+                gcs_hook = GCSHook(self.gcp_conn_id)
                 tmp_gcs_file = exit_stack.enter_context(gcs_hook.provide_file(object_url=self.jar))
                 self.jar = tmp_gcs_file.name
 
             if is_dataflow and self.dataflow_hook:
                 is_running = False
                 if self.dataflow_config.check_if_running != CheckJobRunning.IgnoreJob:
                     is_running = (
@@ -564,24 +547,22 @@
         go_file: str = "",
         launcher_binary: str = "",
         worker_binary: str = "",
         runner: str = "DirectRunner",
         default_pipeline_options: dict | None = None,
         pipeline_options: dict | None = None,
         gcp_conn_id: str = "google_cloud_default",
-        delegate_to: str | None = None,
         dataflow_config: DataflowConfiguration | dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(
             runner=runner,
             default_pipeline_options=default_pipeline_options,
             pipeline_options=pipeline_options,
             gcp_conn_id=gcp_conn_id,
-            delegate_to=delegate_to,
             dataflow_config=dataflow_config,
             **kwargs,
         )
 
         if self.dataflow_config.impersonation_chain:
             self.log.info(
                 "Impersonation chain parameter is not supported for Apache Beam GO SDK and will be skipped "
@@ -616,15 +597,15 @@
             _GoFile(file=self.go_file)
             if self.go_file
             else _GoBinary(launcher=self.launcher_binary, worker=self.worker_binary)
         )
 
         with ExitStack() as exit_stack:
             if go_artifact.is_located_on_gcs():
-                gcs_hook = GCSHook(self.gcp_conn_id, self.delegate_to)
+                gcs_hook = GCSHook(self.gcp_conn_id)
                 tmp_dir = exit_stack.enter_context(tempfile.TemporaryDirectory(prefix="apache-beam-go"))
                 go_artifact.download_from_gcs(gcs_hook=gcs_hook, tmp_dir=tmp_dir)
 
             if is_dataflow and self.dataflow_hook:
                 with self.dataflow_hook.provide_authorized_gcloud():
                     go_artifact.start_pipeline(
                         beam_hook=self.beam_hook,
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO` & `apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 4.3.0rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -50,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``4.3.0rc1``
+Release: ``5.0.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -130,14 +129,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS and Dataflow hooks' param ``delegate_to`` is removed from all Beam operators.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Get rid of state in Apache Beam provider hook (#29503)``
@@ -397,9 +411,7 @@
 * ``Corrections in docs and tools after releasing provider RCs (#14082)``
 * ``Remove WARNINGs from BeamHook (#14554)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/pyproject.toml` & `apache-airflow-providers-apache-beam-5.0.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
-
+    "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi"
 ]
 
 # TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
 target-version = "py37"
@@ -63,14 +63,46 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+[tool.pytest.ini_options]
+# * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
+# * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
+# * And we focus on use native pytest capabilities rather than adopt another frameworks.
+addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
+norecursedirs = [
+    ".eggs",
+    "airflow",
+    "tests/dags_with_system_exit",
+    "tests/test_utils",
+    "tests/dags_corrupted",
+    "tests/dags",
+    "tests/system/providers/google/cloud/dataproc/resources",
+    "tests/system/providers/google/cloud/gcs/resources",
+]
+log_level = "INFO"
+filterwarnings = [
+    "error::pytest.PytestCollectionWarning",
+    "ignore::DeprecationWarning:flask_appbuilder.filemanager",
+    "ignore::DeprecationWarning:flask_appbuilder.widgets",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
+    "ignore::DeprecationWarning:flask_sqlalchemy",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
+    "ignore::DeprecationWarning:apispec.utils",
+]
+python_files = [
+    "*.py",
+]
+testpaths = [
+    "tests",
+]
+
 [tool.ruff.isort]
 known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
 # TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
 known-third-party = [
@@ -101,14 +133,18 @@
 "airflow/models/sqla_models.py" = ["F401"]
 
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
+# The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
+# when __future__.annotations is used so we need to skip them from upgrading
+"airflow/serialization/pydantic/*.py" = ["I002"]
+
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
 "provider_packages/*" = ["D"]
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/setup.cfg` & `apache-airflow-providers-apache-beam-5.0.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/4.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-beam-4.3.0rc1/setup.py` & `apache-airflow-providers-apache-beam-5.0.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-beam package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.0"
+version = "5.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-beam setup."""
     setup(
         version=version,
         extras_require={"google": ["apache-airflow-providers-google", "apache-beam[gcp]"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.beam", "airflow.providers.apache.beam.*"]
+            include=[
+                "airflow.providers.apache.beam",
+                "airflow.providers.apache.beam.*",
+                "airflow.providers.apache.beam_vendor",
+                "airflow.providers.apache.beam_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

