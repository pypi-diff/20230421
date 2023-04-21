# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.1.0rc1.tar", last modified: Fri Mar  3 13:46:48 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar", last modified: Fri Apr 21 19:48:19 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1.tar` & `apache-airflow-providers-dbt-cloud-3.1.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-03 13:46:47.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9605 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8028 2023-03-03 13:46:47.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-03-03 13:46:46.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24217 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12832 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4841 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9605 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1895 2023-03-03 13:46:48.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1539 2023-03-03 13:46:46.000000 apache-airflow-providers-dbt-cloud-3.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12832 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5341 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.0rc1
+Version: 3.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.0rc1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -132,14 +131,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.1.1
+.....
+
+Misc
+~~~~
+
+* ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
+* ``Move typing imports behind TYPE_CHECKING in DbtCloudHook (#29989)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``adding trigger info to provider yaml (#29950)``
+
 3.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add 'DbtCloudJobRunAsyncSensor' (#29695)``
@@ -269,9 +282,7 @@
 
 * ``Fix mistakenly added install_requires for all providers (#22382)``
 
 1.0.1
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/README.rst` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.0rc1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -97,14 +97,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.1.1
+.....
+
+Misc
+~~~~
+
+* ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
+* ``Move typing imports behind TYPE_CHECKING in DbtCloudHook (#29989)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``adding trigger info to provider yaml (#29950)``
+
 3.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add 'DbtCloudJobRunAsyncSensor' (#29695)``
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-dbt-cloud",
         "name": "dbt Cloud",
         "description": "`dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.1",
             "2.3.0",
             "2.2.0",
             "2.1.0",
             "2.0.1",
@@ -54,14 +56,17 @@
         ],
         "sensors": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.sensors.dbt"]}
         ],
         "hooks": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.hooks.dbt"]}
         ],
+        "triggers": [
+            {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.triggers.dbt"]}
+        ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.dbt.cloud.hooks.dbt.DbtCloudHook",
                 "connection-type": "dbt_cloud",
             }
         ],
         "extra-links": ["airflow.providers.dbt.cloud.operators.dbt.DbtCloudRunJobOperatorLink"],
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,32 @@
 from __future__ import annotations
 
 import json
 import time
 from enum import Enum
 from functools import wraps
 from inspect import signature
-from typing import Any, Callable, Sequence, Set, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Sequence, Set, TypeVar, cast
 
 import aiohttp
 from aiohttp import ClientResponseError
 from asgiref.sync import sync_to_async
-from requests import PreparedRequest, Session
 from requests.auth import AuthBase
-from requests.models import Response
+from requests.sessions import Session
 
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
-from airflow.models import Connection
 from airflow.providers.http.hooks.http import HttpHook
 from airflow.typing_compat import TypedDict
 
+if TYPE_CHECKING:
+    from requests.models import PreparedRequest, Response
+
+    from airflow.models import Connection
+
 
 def fallback_to_default_account(func: Callable) -> Callable:
     """
     Decorator which provides a fallback value for ``account_id``. If the ``account_id`` is None or not passed
     to the decorated function, the value will be taken from the configured dbt Cloud Airflow Connection.
     """
     sig = signature(func)
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.0rc1
+Version: 3.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.0rc1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -132,14 +131,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.1.1
+.....
+
+Misc
+~~~~
+
+* ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
+* ``Move typing imports behind TYPE_CHECKING in DbtCloudHook (#29989)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``adding trigger info to provider yaml (#29950)``
+
 3.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add 'DbtCloudJobRunAsyncSensor' (#29695)``
@@ -269,9 +282,7 @@
 
 * ``Fix mistakenly added install_requires for all providers (#22382)``
 
 1.0.1
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.0rc1/setup.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-dbt-cloud package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.0"
+version = "3.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-dbt-cloud setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.dbt.cloud", "airflow.providers.dbt.cloud.*"]
+            include=[
+                "airflow.providers.dbt.cloud",
+                "airflow.providers.dbt.cloud.*",
+                "airflow.providers.dbt.cloud_vendor",
+                "airflow.providers.dbt.cloud_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

