# Comparing `tmp/hstestaq-0.2.11.tar.gz` & `tmp/hstestaq-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstestaq-0.2.11.tar", last modified: Thu Apr 20 19:16:59 2023, max compression
+gzip compressed data, was "hstestaq-0.2.12.tar", last modified: Thu Apr 20 20:20:43 2023, max compression
```

## Comparing `hstestaq-0.2.11.tar` & `hstestaq-0.2.12.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.236527 hstestaq-0.2.11/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.11/MANIFEST.in
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 19:16:59.236279 hstestaq-0.2.11/PKG-INFO
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.193970 hstestaq-0.2.11/aqueduct_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.194280 hstestaq-0.2.11/aqueduct_executor/migrators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.196318 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.198401 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.200689 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.201014 hstestaq-0.2.11/aqueduct_executor/operators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.202078 hstestaq-0.2.11/aqueduct_executor/operators/airflow/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.202411 hstestaq-0.2.11/aqueduct_executor/operators/connectors/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.214595 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/athena.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/common.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/connector.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    12911 2023-04-18 17:47:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/extract.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/load.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/models.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/relational.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.215750 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.220148 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conf.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.223703 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    15880 2023-04-20 19:11:46.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/extract_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.225061 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.226429 hstestaq-0.2.11/aqueduct_executor/operators/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     8793 2023-04-03 17:36:30.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_data.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      979 2023-04-20 19:11:46.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.227879 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.230587 hstestaq-0.2.11/aqueduct_executor/operators/utils/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/enums.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/exceptions.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/execution.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.234263 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/file.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/parse.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/storage.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/timer.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.234615 hstestaq-0.2.11/bin/
--rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.11/bin/aqueduct
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.235962 hstestaq-0.2.11/hstestaq.egg-info/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/PKG-INFO
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/SOURCES.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/dependency_links.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/requires.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/top_level.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.11/requirements.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 19:16:59.236605 hstestaq-0.2.11/setup.cfg
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 19:16:47.000000 hstestaq-0.2.11/setup.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.050523 hstestaq-0.2.12/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.12/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 20:20:43.050235 hstestaq-0.2.12/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.001113 hstestaq-0.2.12/aqueduct_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.001305 hstestaq-0.2.12/aqueduct_executor/migrators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.003334 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.005206 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.007596 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.007973 hstestaq-0.2.12/aqueduct_executor/operators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.009074 hstestaq-0.2.12/aqueduct_executor/operators/airflow/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.009412 hstestaq-0.2.12/aqueduct_executor/operators/connectors/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.021884 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/athena.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/common.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/connector.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    12911 2023-04-18 17:47:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/extract.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/load.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/relational.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.023462 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.030583 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.035358 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    15880 2023-04-20 19:11:46.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.037114 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.038589 hstestaq-0.2.12/aqueduct_executor/operators/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8793 2023-04-03 17:36:30.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      984 2023-04-20 20:20:04.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.041321 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.044212 hstestaq-0.2.12/aqueduct_executor/operators/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/exceptions.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/execution.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.047794 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/file.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/parse.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/storage.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/timer.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.048381 hstestaq-0.2.12/bin/
+-rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.12/bin/aqueduct
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.049881 hstestaq-0.2.12/hstestaq.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/top_level.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.12/requirements.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 20:20:43.050616 hstestaq-0.2.12/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 20:20:28.000000 hstestaq-0.2.12/setup.py
```

### Comparing `hstestaq-0.2.11/PKG-INFO` & `hstestaq-0.2.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.11
+Version: 0.2.12
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/airflow/execute.py` & `hstestaq-0.2.12/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/airflow/spec.py` & `hstestaq-0.2.12/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/athena.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/bigquery.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/common.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/config.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/connector.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/execute.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/extract.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/gcs.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/load.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/main.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/models.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mongodb.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mysql.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/postgres.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/relational.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/snowflake.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/s3.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spec.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sql_server.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sqlite.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/utils.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conf.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/utils.py` & `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/execute.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/extract_function.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/get_extract_path.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/install_requirements.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/main.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/set_conda_version.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/spec.py` & `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/param_executor/execute.py` & `hstestaq-0.2.12/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/param_executor/spec.py` & `hstestaq-0.2.12/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_data.py` & `hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_function.py` & `hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     """
     Executes a function operator.
     """
     return run_helper(
         spec=spec, 
         read_func=read_artifacts_spark, 
         write_func=write_artifact_spark, 
-        infer_func=infer_artifact_type_spark, 
+        infer_type_func=infer_artifact_type_spark, 
         spark_session_obj=spark_session_obj,
     )
```

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/spark/utils.py` & `hstestaq-0.2.12/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/execute.py` & `hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/spec.py` & `hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/enums.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/execution.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/config.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/file.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/gcs.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/parse.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/s3.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/timer.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/aqueduct_executor/operators/utils/utils.py` & `hstestaq-0.2.12/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/bin/aqueduct` & `hstestaq-0.2.12/bin/aqueduct`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/hstestaq.egg-info/PKG-INFO` & `hstestaq-0.2.12/hstestaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.11
+Version: 0.2.12
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.11/hstestaq.egg-info/SOURCES.txt` & `hstestaq-0.2.12/hstestaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.11/setup.py` & `hstestaq-0.2.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = open("requirements.txt").read().strip().split("\n")
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="hstestaq",
-    version="0.2.11",
+    version="0.2.12",
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
     description="Prediction Infrastructure for Data Scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
```

