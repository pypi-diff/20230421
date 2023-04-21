# Comparing `tmp/apache-airflow-providers-trino-4.3.2rc1.tar.gz` & `tmp/apache-airflow-providers-trino-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-trino-4.3.2rc1.tar", last modified: Wed Feb  8 08:29:02 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-trino-5.0.0rc1.tar", last modified: Fri Apr 21 19:50:11 2023, max compression
```

## Comparing `apache-airflow-providers-trino-4.3.2rc1.tar` & `apache-airflow-providers-trino-5.0.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-trino-4.3.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-08 08:29:00.000000 apache-airflow-providers-trino-4.3.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-trino-4.3.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12890 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11296 2023-02-08 08:29:00.000000 apache-airflow-providers-trino-4.3.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-02-08 08:29:00.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9383 2023-01-11 12:48:26.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-11 12:48:26.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-01-11 12:48:26.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2023-01-26 14:58:03.000000 apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12890 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-08 08:29:01.000000 apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-01-13 19:37:41.000000 apache-airflow-providers-trino-4.3.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1903 2023-02-08 08:29:02.000000 apache-airflow-providers-trino-4.3.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1595 2023-02-08 08:29:00.000000 apache-airflow-providers-trino-4.3.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11750 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9383 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-04-21 10:05:41.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-trino-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/LICENSE` & `apache-airflow-providers-trino-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/MANIFEST.in` & `apache-airflow-providers-trino-5.0.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-trino-4.3.2rc1/PKG-INFO` & `apache-airflow-providers-trino-5.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 4.3.2rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/
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
@@ -51,28 +50,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``4.3.2rc1``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -134,14 +133,29 @@
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
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``GCSToPrestoOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.2
 .....
 
 Misc
 ~~~~
 * ``Deprecate 'delegate_to' param in GCP operators and update docs (#29088)``
 
@@ -386,9 +400,7 @@
    * ``More documentation update for June providers release (#16405)``
    * ``Synchronizes updated changelog after buggfix release (#16464)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/README.rst` & `apache-airflow-providers-trino-5.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``4.3.2rc1``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -98,14 +98,29 @@
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
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``GCSToPrestoOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.2
 .....
 
 Misc
 ~~~~
 * ``Deprecate 'delegate_to' param in GCP operators and update docs (#29088)``
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-trino",
         "name": "Trino",
         "description": "`Trino <https://trino.io/>`__\n",
+        "suspended": False,
         "versions": [
+            "5.0.0",
             "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.1",
             "4.0.0",
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Google Cloud Storage to Trino operator."""
 from __future__ import annotations
 
 import csv
 import json
-import warnings
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Iterable, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.google.cloud.hooks.gcs import GCSHook
 from airflow.providers.trino.hooks.trino import TrinoHook
 
@@ -45,17 +44,14 @@
     :param trino_table: trino table to upload the data
     :param trino_conn_id: destination trino connection
     :param gcp_conn_id: (Optional) The connection ID used to connect to Google Cloud and
         interact with the Google Cloud Storage service.
     :param schema_fields: The names of the columns to fill in the table. If schema_fields is
         provided, any path provided in the schema object will be
     :param schema_object: JSON file with schema fields
-    :param delegate_to: The account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
     :param impersonation_chain: Optional service account to impersonate using short-term
         credentials, or chained list of accounts required to get the access_token
         of the last account in the list, which will be impersonated in the request.
         If set as a string, the account must grant the originating account
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
@@ -74,37 +70,30 @@
         source_bucket: str,
         source_object: str,
         trino_table: str,
         trino_conn_id: str = "trino_default",
         gcp_conn_id: str = "google_cloud_default",
         schema_fields: Iterable[str] | None = None,
         schema_object: str | None = None,
-        delegate_to: str | None = None,
         impersonation_chain: str | Sequence[str] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.source_bucket = source_bucket
         self.source_object = source_object
         self.trino_table = trino_table
         self.trino_conn_id = trino_conn_id
         self.gcp_conn_id = gcp_conn_id
         self.schema_fields = schema_fields
         self.schema_object = schema_object
-        if delegate_to:
-            warnings.warn(
-                "'delegate_to' parameter is deprecated, please use 'impersonation_chain'", DeprecationWarning
-            )
-        self.delegate_to = delegate_to
         self.impersonation_chain = impersonation_chain
 
     def execute(self, context: Context) -> None:
         gcs_hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to,
             impersonation_chain=self.impersonation_chain,
         )
 
         trino_hook = TrinoHook(trino_conn_id=self.trino_conn_id)
 
         with NamedTemporaryFile("w+") as temp_file:
             self.log.info("Downloading data from %s", self.source_object)
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 4.3.2rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/
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
@@ -51,28 +50,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``4.3.2rc1``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -134,14 +133,29 @@
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
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``GCSToPrestoOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.3.2
 .....
 
 Misc
 ~~~~
 * ``Deprecate 'delegate_to' param in GCP operators and update docs (#29088)``
 
@@ -386,9 +400,7 @@
    * ``More documentation update for June providers release (#16405)``
    * ``Synchronizes updated changelog after buggfix release (#16464)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-4.3.2rc1/pyproject.toml` & `apache-airflow-providers-trino-5.0.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 target-version = ['py37', 'py38', 'py39', 'py310']
 # The build system section is needed in order to workaround the side-effect introduced by recent
 # setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
-requires = ['setuptools==63.4.3']
+requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
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

### Comparing `apache-airflow-providers-trino-4.3.2rc1/setup.cfg` & `apache-airflow-providers-trino-5.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/4.3.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-trino-4.3.2rc1/setup.py` & `apache-airflow-providers-trino-5.0.0rc1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,24 +22,31 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-trino package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.2"
+version = "5.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-trino setup."""
     setup(
         version=version,
         extras_require={
             "common.sql": ["apache-airflow-providers-common-sql"],
             "google": ["apache-airflow-providers-google"],
         },
-        packages=find_namespace_packages(include=["airflow.providers.trino", "airflow.providers.trino.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.trino",
+                "airflow.providers.trino.*",
+                "airflow.providers.trino_vendor",
+                "airflow.providers.trino_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

