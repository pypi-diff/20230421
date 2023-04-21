# Comparing `tmp/apache-airflow-providers-mysql-4.0.2rc1.tar.gz` & `tmp/apache-airflow-providers-mysql-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-mysql-4.0.2rc1.tar", last modified: Fri Mar  3 13:47:10 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-mysql-5.0.0rc1.tar", last modified: Fri Apr 21 19:49:45 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-4.0.2rc1.tar` & `apache-airflow-providers-mysql-5.0.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-4.0.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-03 13:47:08.000000 apache-airflow-providers-mysql-4.0.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-4.0.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14276 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12613 2023-03-03 13:47:08.000000 apache-airflow-providers-mysql-4.0.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-03 13:47:08.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11365 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14276 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      343 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-03 13:47:09.000000 apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-4.0.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-03-03 13:47:10.000000 apache-airflow-providers-mysql-4.0.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1772 2023-03-03 13:47:08.000000 apache-airflow-providers-mysql-4.0.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14468 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12786 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-04-14 10:21:56.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14468 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-mysql-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/LICENSE` & `apache-airflow-providers-mysql-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/MANIFEST.in` & `apache-airflow-providers-mysql-5.0.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/PKG-INFO` & `apache-airflow-providers-mysql-5.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 4.0.2rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
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
@@ -30,14 +29,15 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: vertica
+Provides-Extra: mysql-connector-python
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
@@ -54,28 +54,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``4.0.2rc1``
+Release: ``5.0.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -87,15 +87,14 @@
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.3.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``mysql-connector-python``               ``>=8.0.11``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -131,26 +130,38 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
-The version of MySQL server has to be 5.6.4+. The exact version upper bound depends
-on the version of ``mysqlclient`` package. For example, ``mysqlclient`` 1.3.12 can only be
-used with MySQL server 5.6.4 through 5.7.
-
 .. NOTE TO CONTRIBUTORS:
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  If you are using mysql-connector-python please note that starting this release it is an extra option.
+  The library will not be installed by default.
+
+* ``Remove mysql-connector-python (#30487)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.2
 .....
 
 Misc
 ~~~~
 
 * ``Use MariaDB client binaries in arm64 image for support MySQL backend (#29519)``
@@ -414,9 +425,7 @@
 Updated documentation and readme files.
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/README.rst` & `apache-airflow-providers-mysql-5.0.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``4.0.2rc1``
+Release: ``5.0.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -48,15 +48,14 @@
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.3.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``mysql-connector-python``               ``>=8.0.11``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -92,26 +91,38 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
-The version of MySQL server has to be 5.6.4+. The exact version upper bound depends
-on the version of ``mysqlclient`` package. For example, ``mysqlclient`` 1.3.12 can only be
-used with MySQL server 5.6.4 through 5.7.
-
 .. NOTE TO CONTRIBUTORS:
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  If you are using mysql-connector-python please note that starting this release it is an extra option.
+  The library will not be installed by default.
+
+* ``Remove mysql-connector-python (#30487)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.2
 .....
 
 Misc
 ~~~~
 
 * ``Use MariaDB client binaries in arm64 image for support MySQL backend (#29519)``
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mysql",
         "name": "MySQL",
         "description": "`MySQL <https://www.mysql.com/products/>`__\n",
+        "suspended": False,
         "versions": [
+            "5.0.0",
             "4.0.2",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
             "3.2.0",
@@ -48,15 +50,14 @@
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
             "apache-airflow>=2.3.0",
             "apache-airflow-providers-common-sql>=1.3.1",
-            "mysql-connector-python>=8.0.11",
             "mysqlclient>=1.3.6",
         ],
         "integrations": [
             {
                 "integration-name": "MySQL",
                 "external-doc-url": "https://www.mysql.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-mysql/operators.rst"],
@@ -89,8 +90,11 @@
                 "target-integration-name": "MySQL",
                 "python-module": "airflow.providers.mysql.transfers.trino_to_mysql",
             },
         ],
         "connection-types": [
             {"hook-class-name": "airflow.providers.mysql.hooks.mysql.MySqlHook", "connection-type": "mysql"}
         ],
+        "additional-extras": [
+            {"name": "mysql-connector-python", "dependencies": ["mysql-connector-python>=8.0.11"]}
+        ],
     }
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module allows to connect to a MySQL database."""
 from __future__ import annotations
 
 import json
+import logging
 from typing import TYPE_CHECKING, Any, Union
 
+from airflow.exceptions import AirflowOptionalProviderFeatureException
 from airflow.models import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
+logger = logging.getLogger(__name__)
+
 if TYPE_CHECKING:
-    from mysql.connector.abstracts import MySQLConnectionAbstract
+    try:
+        from mysql.connector.abstracts import MySQLConnectionAbstract
+    except ModuleNotFoundError:
+        logger.warning("The package 'mysql-connector-python' is not installed. Import skipped")
     from MySQLdb.connections import Connection as MySQLdbConnection
 
 MySQLConnectionTypes = Union["MySQLdbConnection", "MySQLConnectionAbstract"]
 
 
 class MySqlHook(DbApiHook):
     """
@@ -177,15 +184,22 @@
         if client_name == "mysqlclient":
             import MySQLdb
 
             conn_config = self._get_conn_config_mysql_client(conn)
             return MySQLdb.connect(**conn_config)
 
         if client_name == "mysql-connector-python":
-            import mysql.connector
+            try:
+                import mysql.connector
+            except ModuleNotFoundError:
+                raise AirflowOptionalProviderFeatureException(
+                    "The pip package 'mysql-connector-python' is not installed, therefore the connection "
+                    "wasn't established. Please, consider using default driver or pip install the package "
+                    "'mysql-connector-python'. Warning! It might cause dependency conflicts."
+                )
 
             conn_config = self._get_conn_config_mysql_connector_python(conn)
             return mysql.connector.connect(**conn_config)
 
         raise ValueError("Unknown MySQL client name provided!")
 
     def bulk_load(self, table: str, tmp_file: str) -> None:
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/__init__.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 4.0.2rc1
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
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
@@ -30,14 +29,15 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: vertica
+Provides-Extra: mysql-connector-python
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
@@ -54,28 +54,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``4.0.2rc1``
+Release: ``5.0.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -87,15 +87,14 @@
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.3.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``mysql-connector-python``               ``>=8.0.11``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -131,26 +130,38 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
-The version of MySQL server has to be 5.6.4+. The exact version upper bound depends
-on the version of ``mysqlclient`` package. For example, ``mysqlclient`` 1.3.12 can only be
-used with MySQL server 5.6.4 through 5.7.
-
 .. NOTE TO CONTRIBUTORS:
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  If you are using mysql-connector-python please note that starting this release it is an extra option.
+  The library will not be installed by default.
+
+* ``Remove mysql-connector-python (#30487)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.2
 .....
 
 Misc
 ~~~~
 
 * ``Use MariaDB client binaries in arm64 image for support MySQL backend (#29519)``
@@ -414,9 +425,7 @@
 Updated documentation and readme files.
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/pyproject.toml` & `apache-airflow-providers-mysql-5.0.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/setup.cfg` & `apache-airflow-providers-mysql-5.0.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/4.0.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -44,15 +44,14 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.3.0.dev0
-	mysql-connector-python>=8.0.11
 	mysqlclient>=1.3.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-mysql-4.0.2rc1/setup.py` & `apache-airflow-providers-mysql-5.0.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,27 +22,35 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mysql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.0.2"
+version = "5.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mysql setup."""
     setup(
         version=version,
         extras_require={
             "amazon": ["apache-airflow-providers-amazon"],
             "common.sql": ["apache-airflow-providers-common-sql"],
             "presto": ["apache-airflow-providers-presto"],
             "trino": ["apache-airflow-providers-trino"],
             "vertica": ["apache-airflow-providers-vertica"],
+            "mysql-connector-python": ["mysql-connector-python>=8.0.11"],
         },
-        packages=find_namespace_packages(include=["airflow.providers.mysql", "airflow.providers.mysql.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.mysql",
+                "airflow.providers.mysql.*",
+                "airflow.providers.mysql_vendor",
+                "airflow.providers.mysql_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

