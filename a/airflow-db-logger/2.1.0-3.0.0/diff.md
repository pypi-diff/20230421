# Comparing `tmp/airflow_db_logger-2.1.0.tar.gz` & `tmp/airflow_db_logger-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_db_logger-2.1.0.tar", last modified: Wed Apr 19 20:14:46 2023, max compression
+gzip compressed data, was "airflow_db_logger-3.0.0.tar", last modified: Fri Apr 21 19:23:41 2023, max compression
```

## Comparing `airflow_db_logger-2.1.0.tar` & `airflow_db_logger-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5623 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/airflow_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17091 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/shell_logging_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger/writers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3807 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/local.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/airflow_db_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/airlfow_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4865 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4174 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2562 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/shell_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/airflow_db_logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 19:23:41.000000 airflow_db_logger-3.0.0/airflow_db_logger.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-21 19:23:41.413793 airflow_db_logger-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-21 19:23:28.000000 airflow_db_logger-3.0.0/setup.py
```

### Comparing `airflow_db_logger-2.1.0/airflow_db_logger/airflow_utils.py` & `airflow_db_logger-3.0.0/airflow_db_logger/airflow_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import airflow
 from datetime import datetime
 from airflow import settings
 from airflow.operators.python import PythonOperator
 from sqlalchemy.orm import Session, Query
 
-from airflow_db_logger.config import DBLoggerSession
-from airflow_db_logger.data import TaskExecutionLogRecord, DagFileProcessingLogRecord, LoggerModelBase
+from airflow_db_logger.db import db_logger_session
+from airflow_db_logger.data import DBLoggerLogRecord, DagFileProcessingLogRecord, LoggerModelBase
 
 
 def create_clean_old_logs_task(
     task_id: str,
     before: datetime,
     after: datetime = None,
     dag: airflow.DAG = None,
@@ -25,16 +25,16 @@
         query: Query = session.query(cls)
         query = query.filter(cls.timestamp <= before)
         query = query.filter(cls.timestamp > after)
         return query
 
     def clean_airflow_logs(*args, **kwargs):
         logging.info(f"Cleaning up logs from {after} to {before}")
-        session: Session = DBLoggerSession()
-        task_logs = create_select_query(session, TaskExecutionLogRecord)
+        session: Session = db_logger_session()
+        task_logs = create_select_query(session, DBLoggerLogRecord)
         processor_logs = create_select_query(session, DagFileProcessingLogRecord)
 
         task_logs.delete()
         processor_logs.delete()
 
         session.commit()
```

### Comparing `airflow_db_logger-2.1.0/airflow_db_logger/utils.py` & `airflow_db_logger-3.0.0/airflow_db_logger/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,30 @@
 
     if first_only:
         return None
 
     return lst
 
 
+def deep_merge_dicts(target: dict, *args):
+    assert isinstance(target, dict), "Target must be a dict"
+    for src in args:
+        assert isinstance(src, dict), "All merge items must be dicts"
+
+        for key in src.keys():
+            if key not in target:
+                target[key] = src[key]
+                continue
+            if isinstance(src[key], dict) and isinstance(target[key], dict):
+                target[key] = deep_merge_dicts({}, target[key], src[key])
+            else:
+                target[key] = src[key]
+    return target
+
+
 class style:
     GRAY = lambda x: colorize(str(x), "\033[90m")  # noqa: E731
     LIGHT_GRAY = lambda x: colorize(str(x), "\033[37m")  # noqa: E731
     BLACK = lambda x: colorize(str(x), "\033[30m")  # noqa: E731
     RED = lambda x: colorize(str(x), "\033[31m")  # noqa: E731
     GREEN = lambda x: colorize(str(x), "\033[32m")  # noqa: E731
     YELLOW = lambda x: colorize(str(x), "\033[33m")  # noqa: E731
```

### Comparing `airflow_db_logger-2.1.0/airflow_db_logger.egg-info/SOURCES.txt` & `airflow_db_logger-3.0.0/airflow_db_logger.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 MANIFEST.in
 README.md
 README.rst
 setup.cfg
 setup.py
 airflow_db_logger/__init__.py
 airflow_db_logger/airflow_utils.py
+airflow_db_logger/airlfow_config.py
 airflow_db_logger/config.py
-airflow_db_logger/consts.py
 airflow_db_logger/data.py
+airflow_db_logger/db.py
 airflow_db_logger/exceptions.py
 airflow_db_logger/handlers.py
+airflow_db_logger/log.py
+airflow_db_logger/logging_config.py
 airflow_db_logger/operators.py
 airflow_db_logger/shell_logging_config.py
+airflow_db_logger/storage.py
 airflow_db_logger/utils.py
 airflow_db_logger.egg-info/PKG-INFO
 airflow_db_logger.egg-info/SOURCES.txt
 airflow_db_logger.egg-info/dependency_links.txt
-airflow_db_logger.egg-info/requires.txt
-airflow_db_logger.egg-info/top_level.txt
-airflow_db_logger/writers/gcs.py
-airflow_db_logger/writers/local.py
-airflow_db_logger/writers/shell.py
+airflow_db_logger.egg-info/top_level.txt
```

### Comparing `airflow_db_logger-2.1.0/setup.py` & `airflow_db_logger-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     version=get_version(),
     description="An airflow logger that stores its results in a database given an SQLAlchemy connection.",
     long_description="Please see readme.md @ https://github.com/LamaAni/AirflowDBLogger",
     classifiers=[],
     author="Zav Shotan",
     author_email="",
     url="https://github.com/LamaAni/AirflowDBLogger",
-    packages=["airflow_db_logger", "airflow_db_logger/writers"],
+    packages=["airflow_db_logger"],
     platforms="any",
     license="docs/LICENSE",
-    install_requires=[
-        "zthreading>=0.1.15",
-    ],
+    install_requires=[],
     python_requires=">=3.6",
     include_package_data=True,
 )
```

