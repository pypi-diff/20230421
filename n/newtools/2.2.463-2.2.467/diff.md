# Comparing `tmp/newtools-2.2.463.tar.gz` & `tmp/newtools-2.2.467.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newtools-2.2.463.tar", last modified: Wed Apr 19 13:33:43 2023, max compression
+gzip compressed data, was "dist/newtools-2.2.467.tar", last modified: Fri Apr 21 09:46:06 2023, max compression
```

## Comparing `newtools-2.2.463.tar` & `newtools-2.2.467.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-19 13:31:44.000000 newtools-2.2.463/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-19 13:33:43.000000 newtools-2.2.463/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 13:31:44.000000 newtools-2.2.463/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/aws/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9641 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/load_partitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/s3_location.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/db/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6912 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/athena.py
--rw-rw-rw-   0 root         (0) root         (0)    39426 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/cached_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12954 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/sql_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/doggo/
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13397 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/doggo.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     9277 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/lock.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/log/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9531 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/json_persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/optional_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/queue/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/queue/task_queue.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-19 13:31:45.000000 newtools-2.2.463/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-19 13:33:43.000000 newtools-2.2.463/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2296 2023-04-19 13:31:45.000000 newtools-2.2.463/setup.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-19 13:33:37.000000 newtools-2.2.463/version.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-21 09:44:16.000000 newtools-2.2.467/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-21 09:46:06.000000 newtools-2.2.467/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-21 09:44:16.000000 newtools-2.2.467/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/aws/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9641 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/load_partitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/s3_location.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/db/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6912 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/athena.py
+-rw-rw-rw-   0 root         (0) root         (0)    39431 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/cached_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    12954 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/sql_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/doggo/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13397 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/doggo.py
+-rw-rw-rw-   0 root         (0) root         (0)    19227 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9277 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/lock.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/log/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9531 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/json_persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/optional_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/queue/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/queue/task_queue.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-21 09:44:16.000000 newtools-2.2.467/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-21 09:46:06.000000 newtools-2.2.467/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2023-04-21 09:44:16.000000 newtools-2.2.467/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-21 09:46:04.000000 newtools-2.2.467/version.txt
```

### Comparing `newtools-2.2.463/PKG-INFO` & `newtools-2.2.467/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.463
+Version: 2.2.467
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.463/README.md` & `newtools-2.2.467/README.md`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/__init__.py` & `newtools-2.2.467/newtools/__init__.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/aws/load_partitions.py` & `newtools-2.2.467/newtools/aws/load_partitions.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/aws/s3_location.py` & `newtools-2.2.467/newtools/aws/s3_location.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/db/athena.py` & `newtools-2.2.467/newtools/db/athena.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/db/cached_query.py` & `newtools-2.2.467/newtools/db/cached_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -977,15 +977,15 @@
         :param df: the dataframe to format
         :param index_cols: the columns to set as the index
         """
         col_name = df.columns[-1]
         if index_cols:
             return df.set_index(index_cols).to_dict()[col_name]
         else:
-            return {'total': df.loc[0, col_name]}
+            return {'total': int(df.loc[0, col_name])}
 
     @staticmethod
     def validate_ctas_params(
         parameters: dict
     ) -> None:
         """
         Function to check the required parameters for CTAS are specified in the parameters.
```

### Comparing `newtools-2.2.463/newtools/db/sql_client.py` & `newtools-2.2.467/newtools/db/sql_client.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/doggo/csv.py` & `newtools-2.2.467/newtools/doggo/csv.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/doggo/doggo.py` & `newtools-2.2.467/newtools/doggo/doggo.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/doggo/fs.py` & `newtools-2.2.467/newtools/doggo/fs.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/doggo/lock.py` & `newtools-2.2.467/newtools/doggo/lock.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/log/json_persistent_field_logger.py` & `newtools-2.2.467/newtools/log/json_persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/log/log.py` & `newtools-2.2.467/newtools/log/log.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/log/persistent_field_logger.py` & `newtools-2.2.467/newtools/log/persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/optional_imports.py` & `newtools-2.2.467/newtools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools/queue/task_queue.py` & `newtools-2.2.467/newtools/queue/task_queue.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/newtools.egg-info/PKG-INFO` & `newtools-2.2.467/newtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.463
+Version: 2.2.467
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.463/newtools.egg-info/SOURCES.txt` & `newtools-2.2.467/newtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newtools-2.2.463/setup.py` & `newtools-2.2.467/setup.py`

 * *Files identical despite different names*

