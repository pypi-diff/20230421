# Comparing `tmp/apache-airflow-providers-sqlite-3.3.1rc3.tar.gz` & `tmp/apache-airflow-providers-sqlite-3.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.3.1rc3.tar", last modified: Sat Nov 26 10:30:14 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.3.2rc1.tar", last modified: Fri Apr 21 19:50:07 2023, max compression
```

## Comparing `apache-airflow-providers-sqlite-3.3.1rc3.tar` & `apache-airflow-providers-sqlite-3.3.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-sqlite-3.3.1rc3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-26 10:30:12.000000 apache-airflow-providers-sqlite-3.3.1rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-sqlite-3.3.1rc3/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11712 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10138 2022-11-26 10:30:12.000000 apache-airflow-providers-sqlite-3.3.1rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2489 2022-11-26 10:30:12.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1653 2022-10-26 03:21:46.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/hooks/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2147 2022-10-26 03:21:46.000000 apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/operators/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11712 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       98 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-sqlite-3.3.1rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1849 2022-11-26 10:30:14.000000 apache-airflow-providers-sqlite-3.3.1rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1517 2022-11-26 10:30:12.000000 apache-airflow-providers-sqlite-3.3.1rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-sqlite-3.3.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:50:05.000000 apache-airflow-providers-sqlite-3.3.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-sqlite-3.3.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11950 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-04-21 19:50:05.000000 apache-airflow-providers-sqlite-3.3.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-21 19:50:05.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-13 08:25:21.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/hooks/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/operators/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11950 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-sqlite-3.3.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-21 19:50:07.000000 apache-airflow-providers-sqlite-3.3.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-04-21 19:50:05.000000 apache-airflow-providers-sqlite-3.3.2rc1/setup.py
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/LICENSE` & `apache-airflow-providers-sqlite-3.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/MANIFEST.in` & `apache-airflow-providers-sqlite-3.3.2rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/PKG-INFO` & `apache-airflow-providers-sqlite-3.3.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.3.1rc3
+Version: 3.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/
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
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.3.1rc3``
+Release: ``3.3.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -129,14 +128,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.2
+.....
+
+Misc
+~~~~
+
+* ``Use connection URI in SqliteHook (#28721)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
@@ -334,9 +345,7 @@
 
 * ``Add example DAG & how-to guide for sqlite (#13196)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/README.rst` & `apache-airflow-providers-sqlite-3.3.2rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.3.1rc3``
+Release: ``3.3.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -94,14 +94,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.2
+.....
+
+Misc
+~~~~
+
+* ``Use connection URI in SqliteHook (#28721)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/__init__.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/get_provider_info.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sqlite",
         "name": "SQLite",
         "description": "`SQLite <https://www.sqlite.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.3",
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/hooks/__init__.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/hooks/sqlite.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/hooks/sqlite.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import sqlite3
+from urllib.parse import unquote
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 
 class SqliteHook(DbApiHook):
     """Interact with SQLite."""
 
@@ -29,17 +30,27 @@
     default_conn_name = "sqlite_default"
     conn_type = "sqlite"
     hook_name = "Sqlite"
     placeholder = "?"
 
     def get_conn(self) -> sqlite3.dbapi2.Connection:
         """Returns a sqlite connection object"""
-        conn_id = getattr(self, self.conn_name_attr)
-        airflow_conn = self.get_connection(conn_id)
-        conn = sqlite3.connect(airflow_conn.host)
+        sqlalchemy_uri = self.get_uri()
+        # The sqlite3 connection does not use the sqlite scheme.
+        # See https://docs.sqlalchemy.org/en/14/dialects/sqlite.html#uri-connections for details.
+        sqlite_uri = sqlalchemy_uri.replace("sqlite:///", "file:")
+        conn = sqlite3.connect(sqlite_uri, uri=True)
         return conn
 
     def get_uri(self) -> str:
         """Override DbApiHook get_uri method for get_sqlalchemy_engine()"""
         conn_id = getattr(self, self.conn_name_attr)
         airflow_conn = self.get_connection(conn_id)
-        return f"sqlite:///{airflow_conn.host}"
+        if airflow_conn.conn_type is None:
+            airflow_conn.conn_type = self.conn_type
+        airflow_uri = unquote(airflow_conn.get_uri())
+        # For sqlite, there is no schema in the connection URI. So we need to drop the trailing slash.
+        airflow_sqlite_uri = airflow_uri.replace("/?", "?")
+        # The sqlite connection has one more slash for path specification.
+        # See https://docs.sqlalchemy.org/en/14/dialects/sqlite.html#connect-strings for details.
+        sqlalchemy_uri = airflow_sqlite_uri.replace("sqlite://", "sqlite:///")
+        return sqlalchemy_uri
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/operators/__init__.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/airflow/providers/sqlite/operators/sqlite.py` & `apache-airflow-providers-sqlite-3.3.2rc1/airflow/providers/sqlite/operators/sqlite.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/PKG-INFO` & `apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.3.1rc3
+Version: 3.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/
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
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.3.1rc3``
+Release: ``3.3.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -129,14 +128,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.2
+.....
+
+Misc
+~~~~
+
+* ``Use connection URI in SqliteHook (#28721)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
@@ -334,9 +345,7 @@
 
 * ``Add example DAG & how-to guide for sqlite (#13196)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/apache_airflow_providers_sqlite.egg-info/SOURCES.txt` & `apache-airflow-providers-sqlite-3.3.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.3.1rc3/setup.cfg` & `apache-airflow-providers-sqlite-3.3.2rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.3.2/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -52,10 +52,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.sqlite.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.sqlite
 
 [egg_info]
-tag_build = rc3
+tag_build = rc1
 tag_date = 0
```

