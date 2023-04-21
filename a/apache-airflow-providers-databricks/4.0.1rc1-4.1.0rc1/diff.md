# Comparing `tmp/apache-airflow-providers-databricks-4.0.1rc1.tar.gz` & `tmp/apache-airflow-providers-databricks-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-databricks-4.0.1rc1.tar", last modified: Sun Apr  2 05:47:26 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-databricks-4.1.0rc1.tar", last modified: Fri Apr 21 19:48:16 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.0.1rc1.tar` & `apache-airflow-providers-databricks-4.1.0rc1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.0.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:24.000000 apache-airflow-providers-databricks-4.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.0.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18455 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16889 2023-04-02 05:47:24.000000 apache-airflow-providers-databricks-4.0.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-04-02 05:47:24.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31391 2023-03-10 19:31:58.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16679 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18455 2023-04-02 05:47:25.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:25.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:25.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-databricks-4.0.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1981 2023-04-02 05:47:26.000000 apache-airflow-providers-databricks-4.0.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1555 2023-04-02 05:47:24.000000 apache-airflow-providers-databricks-4.0.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17221 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-04-15 10:20:41.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31391 2023-03-10 19:31:58.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    16679 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2811 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-databricks-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/LICENSE` & `apache-airflow-providers-databricks-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/MANIFEST.in` & `apache-airflow-providers-databricks-4.1.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/PKG-INFO` & `apache-airflow-providers-databricks-4.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.0.1rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -132,14 +132,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add delete inactive run functionality to databricks provider (#30646)``
+* ``Databricks SQL sensor (#30477)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``DatabricksSubmitRunOperator to support taskflow (#29840)``
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/README.rst` & `apache-airflow-providers-databricks-4.1.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -98,14 +98,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add delete inactive run functionality to databricks provider (#30646)``
+* ``Databricks SQL sensor (#30477)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``DatabricksSubmitRunOperator to support taskflow (#29840)``
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
@@ -117,14 +119,20 @@
         ],
         "triggers": [
             {
                 "integration-name": "Databricks",
                 "python-modules": ["airflow.providers.databricks.triggers.databricks"],
             }
         ],
+        "sensors": [
+            {
+                "integration-name": "Databricks",
+                "python-modules": ["airflow.providers.databricks.sensors.databricks_sql"],
+            }
+        ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.databricks.hooks.databricks.DatabricksHook",
                 "connection-type": "databricks",
             }
         ],
         "extra-links": ["airflow.providers.databricks.operators.databricks.DatabricksJobRunLink"],
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 START_CLUSTER_ENDPOINT = ("POST", "api/2.0/clusters/start")
 TERMINATE_CLUSTER_ENDPOINT = ("POST", "api/2.0/clusters/delete")
 
 RUN_NOW_ENDPOINT = ("POST", "api/2.1/jobs/run-now")
 SUBMIT_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/submit")
 GET_RUN_ENDPOINT = ("GET", "api/2.1/jobs/runs/get")
 CANCEL_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel")
+DELETE_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/delete")
 OUTPUT_RUNS_JOB_ENDPOINT = ("GET", "api/2.1/jobs/runs/get-output")
 
 INSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/install")
 UNINSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/uninstall")
 
 LIST_JOBS_ENDPOINT = ("GET", "api/2.1/jobs/list")
 
@@ -347,14 +348,23 @@
         Cancels the run.
 
         :param run_id: id of the run
         """
         json = {"run_id": run_id}
         self._do_api_call(CANCEL_RUN_ENDPOINT, json)
 
+    def delete_run(self, run_id: int) -> None:
+        """
+        Deletes a non-active run.
+
+        :param run_id: id of the run
+        """
+        json = {"run_id": run_id}
+        self._do_api_call(DELETE_RUN_ENDPOINT, json)
+
     def restart_cluster(self, json: dict) -> None:
         """
         Restarts the cluster.
 
         :param json: json dictionary containing cluster specification.
         """
         self._do_api_call(RESTART_CLUSTER_ENDPOINT, json)
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.0.1rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -132,14 +132,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add delete inactive run functionality to databricks provider (#30646)``
+* ``Databricks SQL sensor (#30477)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``DatabricksSubmitRunOperator to support taskflow (#29840)``
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 airflow/providers/databricks/hooks/databricks.py
 airflow/providers/databricks/hooks/databricks_base.py
 airflow/providers/databricks/hooks/databricks_sql.py
 airflow/providers/databricks/operators/__init__.py
 airflow/providers/databricks/operators/databricks.py
 airflow/providers/databricks/operators/databricks_repos.py
 airflow/providers/databricks/operators/databricks_sql.py
+airflow/providers/databricks/sensors/__init__.py
+airflow/providers/databricks/sensors/databricks_sql.py
 airflow/providers/databricks/triggers/__init__.py
 airflow/providers/databricks/triggers/databricks.py
 airflow/providers/databricks/utils/__init__.py
 airflow/providers/databricks/utils/databricks.py
 apache_airflow_providers_databricks.egg-info/PKG-INFO
 apache_airflow_providers_databricks.egg-info/SOURCES.txt
 apache_airflow_providers_databricks.egg-info/dependency_links.txt
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/pyproject.toml` & `apache-airflow-providers-databricks-4.1.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -135,18 +135,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/setup.cfg` & `apache-airflow-providers-databricks-4.1.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.0.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-databricks-4.0.1rc1/setup.py` & `apache-airflow-providers-databricks-4.1.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-databricks package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.0.1"
+version = "4.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-databricks setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.databricks", "airflow.providers.databricks.*"]
+            include=[
+                "airflow.providers.databricks",
+                "airflow.providers.databricks.*",
+                "airflow.providers.databricks_vendor",
+                "airflow.providers.databricks_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

