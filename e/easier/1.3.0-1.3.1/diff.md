# Comparing `tmp/easier-1.3.0.tar.gz` & `tmp/easier-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easier-1.3.0.tar", last modified: Wed Jan  4 17:39:09 2023, max compression
+gzip compressed data, was "easier-1.3.1.tar", last modified: Fri Apr 21 19:58:19 2023, max compression
```

## Comparing `easier-1.3.0.tar` & `easier-1.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-01-04 17:39:09.085436 easier-1.3.0/
--rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.0/CONTRIBUTORS.txt
--rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.0/LICENSE
--rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.0/MANIFEST.in
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-01-04 17:39:09.085517 easier-1.3.0/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.0/README.md
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-01-04 17:39:09.083457 easier-1.3.0/easier/
--rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.0/easier/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5093 2023-01-04 17:01:12.000000 easier-1.3.0/easier/api.py
--rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.0/easier/bernstein.py
--rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.0/easier/bigquery.py
--rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.0/easier/cli.py
--rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.0/easier/clock.py
--rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.0/easier/crypt.py
--rw-rw-r--   0 rob        (501) staff       (20)     2782 2022-11-18 14:57:08.000000 easier-1.3.0/easier/dataframe_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.0/easier/distributions.py
--rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.0/easier/duck.py
--rw-rw-r--   0 rob        (501) staff       (20)     6769 2022-11-22 15:24:41.000000 easier-1.3.0/easier/duck_model.py
--rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.0/easier/ecdf_lib.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-01-04 17:39:09.085165 easier-1.3.0/easier/filtering/
--rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.0/easier/filtering/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.0/easier/filtering/elliptic_filter.py
--rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.0/easier/filtering/tvd.py
--rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.0/easier/fit_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.0/easier/gsheet.py
--rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.0/easier/hvtools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1490 2023-01-04 17:30:31.000000 easier-1.3.0/easier/ibis_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.0/easier/item.py
--rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.0/easier/iterify.py
--rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.0/easier/memory.py
--rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.0/easier/minimodel.py
--rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.0/easier/minimodel_orig.py
--rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.0/easier/nice_dates.py
--rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.0/easier/outlier_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.0/easier/parallel.py
--rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.0/easier/param_state.py
--rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.0/easier/plotting.py
--rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.0/easier/postgres.py
--rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.0/easier/print_catcher.py
--rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.0/easier/proportion_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.0/easier/salesforce.py
--rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.0/easier/shaper.py
--rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.0/easier/timer.py
--rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.0/easier/utils.py
--rw-rw-r--   0 rob        (501) staff       (20)       22 2023-01-04 17:35:22.000000 easier-1.3.0/easier/version.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-01-04 17:39:09.084558 easier-1.3.0/easier.egg-info/
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-01-04 17:39:08.000000 easier-1.3.0/easier.egg-info/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)     1018 2023-01-04 17:39:09.000000 easier-1.3.0/easier.egg-info/SOURCES.txt
--rw-rw-r--   0 rob        (501) staff       (20)        1 2023-01-04 17:39:08.000000 easier-1.3.0/easier.egg-info/dependency_links.txt
--rw-rw-r--   0 rob        (501) staff       (20)      117 2023-01-04 17:39:08.000000 easier-1.3.0/easier.egg-info/entry_points.txt
--rw-rw-r--   0 rob        (501) staff       (20)        1 2023-01-03 21:04:26.000000 easier-1.3.0/easier.egg-info/not-zip-safe
--rw-rw-r--   0 rob        (501) staff       (20)       36 2023-01-04 17:39:08.000000 easier-1.3.0/easier.egg-info/requires.txt
--rw-rw-r--   0 rob        (501) staff       (20)        7 2023-01-04 17:39:09.000000 easier-1.3.0/easier.egg-info/top_level.txt
--rw-rw-r--   0 rob        (501) staff       (20)      504 2023-01-04 17:39:09.085927 easier-1.3.0/setup.cfg
--rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.0/setup.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-04-21 19:58:19.824477 easier-1.3.1/
+-rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.1/CONTRIBUTORS.txt
+-rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.1/LICENSE
+-rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.1/MANIFEST.in
+-rw-rw-r--   0 rob        (501) staff       (20)      448 2023-04-21 19:58:19.824534 easier-1.3.1/PKG-INFO
+-rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.1/README.md
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-04-21 19:58:19.822861 easier-1.3.1/easier/
+-rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.1/easier/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5526 2023-04-21 19:26:12.000000 easier-1.3.1/easier/api.py
+-rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.1/easier/bernstein.py
+-rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.1/easier/bigquery.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.1/easier/cli.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.1/easier/clock.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.1/easier/crypt.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5856 2023-04-21 19:26:12.000000 easier-1.3.1/easier/dataframe_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.1/easier/distributions.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.1/easier/duck.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.1/easier/duck_model.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.1/easier/ecdf_lib.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-04-21 19:58:19.824348 easier-1.3.1/easier/filtering/
+-rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.1/easier/filtering/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.1/easier/filtering/elliptic_filter.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.1/easier/filtering/tvd.py
+-rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.1/easier/fit_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.1/easier/gsheet.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.1/easier/hvtools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1966 2023-04-21 19:26:12.000000 easier-1.3.1/easier/ibis_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.1/easier/item.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.1/easier/iterify.py
+-rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.1/easier/memory.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.1/easier/minimodel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.1/easier/minimodel_orig.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.1/easier/nice_dates.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.1/easier/outlier_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.1/easier/parallel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.1/easier/param_state.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.1/easier/plotting.py
+-rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.1/easier/postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.1/easier/print_catcher.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.1/easier/proportion_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.1/easier/salesforce.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.1/easier/shaper.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.1/easier/timer.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.1/easier/utils.py
+-rw-rw-r--   0 rob        (501) staff       (20)       22 2023-04-21 19:26:44.000000 easier-1.3.1/easier/version.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-04-21 19:58:19.823930 easier-1.3.1/easier.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      448 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     1018 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)      117 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.1/easier.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       36 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2023-04-21 19:58:19.000000 easier-1.3.1/easier.egg-info/top_level.txt
+-rw-rw-r--   0 rob        (501) staff       (20)      504 2023-04-21 19:58:19.824765 easier-1.3.1/setup.cfg
+-rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.1/setup.py
```

### Comparing `easier-1.3.0/LICENSE` & `easier-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/README.md` & `easier-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/__init__.py` & `easier-1.3.1/easier/__init__.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/bernstein.py` & `easier-1.3.1/easier/bernstein.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/bigquery.py` & `easier-1.3.1/easier/bigquery.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/cli.py` & `easier-1.3.1/easier/cli.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/clock.py` & `easier-1.3.1/easier/clock.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/crypt.py` & `easier-1.3.1/easier/crypt.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/distributions.py` & `easier-1.3.1/easier/distributions.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/duck.py` & `easier-1.3.1/easier/duck.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/duck_model.py` & `easier-1.3.1/easier/duck_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 
     def head(self, n=5):
         return self.query(f'SELECT * FROM {self.table_name} LIMIT {n}')
 
     def create(self, df):
         self.drop()
         self.query(
-            f'CREATE TABLE {self.table_name} AS SELECT * FROM __df_in__',
+            f'BEGIN TRANSACTION; CREATE TABLE {self.table_name} AS SELECT * FROM __df_in__; COMMIT',
             fetch=False,
             __df_in__=df
         )
         self.exists_dict = {}
         self.duck.connection.unregister('__df_in__')
 
     def insert(self, df):
         self.ensure_writeable()
         self.query(
-            f"INSERT INTO {self.table_name} SELECT * FROM __df_in__",
+            f"BEGIN TRANSACTION INSERT INTO {self.table_name} SELECT * FROM __df_in__ COMMIT",
             fetch=False,
             __df_in__=df
         )
         self.duck.connection.unregister('__df_in__')
 
     def drop(self):
         self.ensure_writeable()
@@ -133,14 +133,16 @@
         self.file_name = file_name
         self._read_only = read_only
         self._force_index_join = force_index_join
         self._connection = None
 
         if overwrite and os.path.isfile(self.file_name):
             os.unlink(self.file_name)
+        if overwrite and os.path.isfile(f'{self.file_name}.wal'):
+            os.unlink(f'{self.file_name}.wal')
 
         if overwrite and read_only:
             raise ValueError("It doesn't make sense to set read_only and overwrite at the same time")
 
         self.reset_connection()
         self.tables = Tables(self)
```

### Comparing `easier-1.3.0/easier/ecdf_lib.py` & `easier-1.3.1/easier/ecdf_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/filtering/elliptic_filter.py` & `easier-1.3.1/easier/filtering/elliptic_filter.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/filtering/tvd.py` & `easier-1.3.1/easier/filtering/tvd.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/fit_lib.py` & `easier-1.3.1/easier/fit_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/gsheet.py` & `easier-1.3.1/easier/gsheet.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/hvtools.py` & `easier-1.3.1/easier/hvtools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/ibis_tools.py` & `easier-1.3.1/easier/ibis_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import contextlib
 import os
 import weakref
+import StringIO
 
 
 def _get_duck_connection(file_name, overwrite=False, read_only=False):
     """
     A function to get a connection to the local database
     Args:
         reset: if set to True, will blow away any existing database file
     """
     import ibis
+
     ibis.options.sql.default_limit = None
     if os.path.isfile(file_name) and overwrite:
         os.unlink(file_name)
     conn = ibis.duckdb.connect(file_name, read_only=read_only)
     return conn
 
 
 def _get_pg_connection(url=None):
     import ibis
+
     ibis.options.sql.default_limit = None
     from .postgres import pg_creds_from_env
+
     if url is None:
         url = pg_creds_from_env()
     conn = ibis.postgres.connect(url=url)
     return conn
 
 
 @contextlib.contextmanager
@@ -43,14 +47,38 @@
     finally:
         connection.con.dispose()
         del connection
 
 
 @contextlib.contextmanager
 def ibis_duck_connection(file_name, overwrite=False, read_only=False):
-    connection = _get_duck_connection(file_name, overwrite=overwrite, read_only=read_only)
+    connection = _get_duck_connection(
+        file_name, overwrite=overwrite, read_only=read_only
+    )
     try:
         proxy_conn = weakref.proxy(connection)
         yield proxy_conn
     finally:
         connection.con.dispose()
         del connection
+
+
+def get_sql(expr):
+    """
+    Returns the SQL for an ibis expression as a string
+    """
+    import ibis
+
+    buff = StringIO()
+    ibis.show_sql(expr, file=buff)
+    return buff.getvalue()
+
+
+def sql_to_frame(conn, sql):
+    """
+    Returns a pandas dataframe from a SQL query on an ibis connection
+    """
+    import pandas as pd
+
+    res = conn.raw_sql(sql)
+    df = pd.DataFrame(res.fetchall(), columns=res._metadata.keys)
+    return df
```

### Comparing `easier-1.3.0/easier/item.py` & `easier-1.3.1/easier/item.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/iterify.py` & `easier-1.3.1/easier/iterify.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/minimodel.py` & `easier-1.3.1/easier/minimodel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/minimodel_orig.py` & `easier-1.3.1/easier/minimodel_orig.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/nice_dates.py` & `easier-1.3.1/easier/nice_dates.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/outlier_tools.py` & `easier-1.3.1/easier/outlier_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/parallel.py` & `easier-1.3.1/easier/parallel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/param_state.py` & `easier-1.3.1/easier/param_state.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/plotting.py` & `easier-1.3.1/easier/plotting.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/postgres.py` & `easier-1.3.1/easier/postgres.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/print_catcher.py` & `easier-1.3.1/easier/print_catcher.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/proportion_lib.py` & `easier-1.3.1/easier/proportion_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/salesforce.py` & `easier-1.3.1/easier/salesforce.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/shaper.py` & `easier-1.3.1/easier/shaper.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/timer.py` & `easier-1.3.1/easier/timer.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier/utils.py` & `easier-1.3.1/easier/utils.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/easier.egg-info/SOURCES.txt` & `easier-1.3.1/easier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easier-1.3.0/setup.py` & `easier-1.3.1/setup.py`

 * *Files identical despite different names*

