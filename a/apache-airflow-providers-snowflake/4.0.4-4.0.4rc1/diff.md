# Comparing `tmp/apache-airflow-providers-snowflake-4.0.4.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.0.4.tar", last modified: Sat Feb 18 20:30:03 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.0.4rc1.tar", last modified: Sat Feb 18 20:36:16 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.0.4.tar` & `apache-airflow-providers-snowflake-4.0.4rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-snowflake-4.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-18 20:30:01.000000 apache-airflow-providers-snowflake-4.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-snowflake-4.0.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)    17504 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15902 2023-02-18 20:30:01.000000 apache-airflow-providers-snowflake-4.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-02-18 20:30:01.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-02-02 18:37:35.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/hooks/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15295 2023-02-02 18:37:35.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-02-11 18:49:53.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5973 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/utils/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17504 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1079 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      217 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-11 18:49:53.000000 apache-airflow-providers-snowflake-4.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1946 2023-02-18 20:30:03.000000 apache-airflow-providers-snowflake-4.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1631 2023-02-18 20:30:01.000000 apache-airflow-providers-snowflake-4.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-02-18 20:36:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    17510 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15905 2023-02-18 20:36:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-02-18 20:36:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17835 2023-02-02 18:37:35.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/hooks/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15295 2023-02-02 18:37:35.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-02-11 18:49:53.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5973 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-01-11 12:48:26.000000 apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/utils/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17510 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-02-11 18:49:53.000000 apache-airflow-providers-snowflake-4.0.4rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-02-18 20:36:16.000000 apache-airflow-providers-snowflake-4.0.4rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-02-18 20:36:15.000000 apache-airflow-providers-snowflake-4.0.4rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.0.4/LICENSE` & `apache-airflow-providers-snowflake-4.0.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/MANIFEST.in` & `apache-airflow-providers-snowflake-4.0.4rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/PKG-INFO` & `apache-airflow-providers-snowflake-4.0.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.0.4
+Version: 4.0.4rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.0.4/
@@ -51,15 +51,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.4``
+Release: ``4.0.4rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.4/README.rst` & `apache-airflow-providers-snowflake-4.0.4rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.4``
+Release: ``4.0.4rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.0.4rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.0.4
+Version: 4.0.4rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.0.4/
@@ -51,15 +51,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.4``
+Release: ``4.0.4rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.4/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.0.4rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/pyproject.toml` & `apache-airflow-providers-snowflake-4.0.4rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.4/setup.cfg` & `apache-airflow-providers-snowflake-4.0.4rc1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.3.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.3.0.dev0
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.0.4/setup.py` & `apache-airflow-providers-snowflake-4.0.4rc1/setup.py`

 * *Files identical despite different names*

