# Comparing `tmp/hstestaq-0.2.14.tar.gz` & `tmp/hstestaq-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstestaq-0.2.14.tar", last modified: Thu Apr 20 22:28:19 2023, max compression
+gzip compressed data, was "hstestaq-0.2.15.tar", last modified: Thu Apr 20 22:54:59 2023, max compression
```

## Comparing `hstestaq-0.2.14.tar` & `hstestaq-0.2.15.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.742406 hstestaq-0.2.14/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.14/MANIFEST.in
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:28:19.742160 hstestaq-0.2.14/PKG-INFO
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.695809 hstestaq-0.2.14/aqueduct_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.696031 hstestaq-0.2.14/aqueduct_executor/migrators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.698173 hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.700513 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.702962 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.703421 hstestaq-0.2.14/aqueduct_executor/operators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.704757 hstestaq-0.2.14/aqueduct_executor/operators/airflow/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/airflow/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/airflow/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/airflow/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/airflow/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.705190 hstestaq-0.2.14/aqueduct_executor/operators/connectors/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.718146 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/athena.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/common.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/connector.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    15014 2023-04-20 22:10:22.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/extract.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/load.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/models.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/relational.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.719448 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.724163 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/conf.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.728175 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    16021 2023-04-20 22:10:22.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/extract_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/function_executor/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.729674 hstestaq-0.2.14/aqueduct_executor/operators/param_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/param_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/param_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/param_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/param_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.731278 hstestaq-0.2.14/aqueduct_executor/operators/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.14/aqueduct_executor/operators/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2495 2023-04-20 22:27:57.000000 hstestaq-0.2.14/aqueduct_executor/operators/spark/execute_data.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      997 2023-04-20 22:10:22.000000 hstestaq-0.2.14/aqueduct_executor/operators/spark/execute_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/spark/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.732849 hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.735875 hstestaq-0.2.14/aqueduct_executor/operators/utils/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/enums.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/exceptions.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/execution.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.739253 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/file.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/parse.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/storage.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/timer.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.14/aqueduct_executor/operators/utils/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.739631 hstestaq-0.2.14/bin/
--rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.14/bin/aqueduct
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:28:19.741843 hstestaq-0.2.14/hstestaq.egg-info/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:28:19.000000 hstestaq-0.2.14/hstestaq.egg-info/PKG-INFO
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 22:28:19.000000 hstestaq-0.2.14/hstestaq.egg-info/SOURCES.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 22:28:19.000000 hstestaq-0.2.14/hstestaq.egg-info/dependency_links.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 22:28:19.000000 hstestaq-0.2.14/hstestaq.egg-info/requires.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 22:28:19.000000 hstestaq-0.2.14/hstestaq.egg-info/top_level.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.14/requirements.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 22:28:19.742484 hstestaq-0.2.14/setup.cfg
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 22:28:07.000000 hstestaq-0.2.14/setup.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.100708 hstestaq-0.2.15/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.15/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:54:59.100432 hstestaq-0.2.15/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.057498 hstestaq-0.2.15/aqueduct_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.057722 hstestaq-0.2.15/aqueduct_executor/migrators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.059924 hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.061678 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.063895 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.064261 hstestaq-0.2.15/aqueduct_executor/operators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.065531 hstestaq-0.2.15/aqueduct_executor/operators/airflow/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/airflow/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/airflow/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/airflow/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/airflow/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.065860 hstestaq-0.2.15/aqueduct_executor/operators/connectors/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.077679 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/athena.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/common.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/connector.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    15373 2023-04-20 22:54:38.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/extract.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/load.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/relational.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.078775 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.083509 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.087116 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    16527 2023-04-20 22:54:38.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/function_executor/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.088592 hstestaq-0.2.15/aqueduct_executor/operators/param_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/param_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/param_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/param_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/param_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.089718 hstestaq-0.2.15/aqueduct_executor/operators/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.15/aqueduct_executor/operators/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2669 2023-04-20 22:54:38.000000 hstestaq-0.2.15/aqueduct_executor/operators/spark/execute_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      998 2023-04-20 22:54:38.000000 hstestaq-0.2.15/aqueduct_executor/operators/spark/execute_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/spark/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.091260 hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.094039 hstestaq-0.2.15/aqueduct_executor/operators/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/exceptions.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/execution.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.097609 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/file.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/parse.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/storage.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/timer.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.15/aqueduct_executor/operators/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.097963 hstestaq-0.2.15/bin/
+-rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.15/bin/aqueduct
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:54:59.100104 hstestaq-0.2.15/hstestaq.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:54:59.000000 hstestaq-0.2.15/hstestaq.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 22:54:59.000000 hstestaq-0.2.15/hstestaq.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 22:54:59.000000 hstestaq-0.2.15/hstestaq.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 22:54:59.000000 hstestaq-0.2.15/hstestaq.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 22:54:59.000000 hstestaq-0.2.15/hstestaq.egg-info/top_level.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.15/requirements.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 22:54:59.100783 hstestaq-0.2.15/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 22:54:47.000000 hstestaq-0.2.15/setup.py
```

### Comparing `hstestaq-0.2.14/PKG-INFO` & `hstestaq-0.2.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.14
+Version: 0.2.15
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `hstestaq-0.2.15/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/airflow/execute.py` & `hstestaq-0.2.15/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/airflow/spec.py` & `hstestaq-0.2.15/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/athena.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/bigquery.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/common.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/config.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/connector.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/execute.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,24 +62,24 @@
     read_artifacts_func: Any,
     write_artifact_func: Any,
     setup_connector_func: Any,
     is_spark: bool,
     **kwargs: Any,
 ) -> None:
     """
-    Runs one of the following connector operations:
-    - authenticate
-    - extract
-    - load
-    - load-table
-    - delete-saved-objects
-    - discover
+    This function executes the spec provided. If run in a Spark environment, it uses
+    the Spark specific utils functions to read/write to storage layer and to setup connectors.
 
     Arguments:
     - spec: The spec provided for this operator.
+    - read_artifacts_func: function used to read artifacts from storage layer
+    - write_artifact_func: function used to write artifacts to storage layer
+    - setup_connector_func: function to use to setup the connectors
+    - is_spark Whether or not we are running in a Spark env.
+    The only kwarg we expect is spark_session_obj
     """
     storage = parse_storage(spec.storage_config)
     exec_state = ExecutionState(user_logs=Logs())
 
     try:
         _execute(
             spec,
```

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/extract.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/gcs.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/load.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/main.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/models.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/mongodb.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/mysql.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/postgres.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/relational.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/s3.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/snowflake.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/s3.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/spec.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/sql_server.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/sqlite.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/data/utils.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/conf.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/connectors/tests/utils.py` & `hstestaq-0.2.15/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/execute.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,39 +241,49 @@
 
 def run(spec: FunctionSpec) -> None:
     """
     Executes a function operator.
     """
     run_helper(
         spec=spec,
-        read_artifact_func=utils.read_artifacts,
+        read_artifacts_func=utils.read_artifacts,
         write_artifact_func=utils.write_artifact,
         infer_type_func=infer_artifact_type,
     )
 
 
 def run_helper(
     spec: FunctionSpec,
-    read_artifact_func: Any,
+    read_artifacts_func: Any,
     write_artifact_func: Any,
     infer_type_func: Any,
     **kwargs: Any,
 ) -> None:
     """
-    Executes a function operator.
+    Executes a function operator. If run in a Spark environment, it uses
+    the Spark specific utils functions to read/write to storage layer and to infer the type of artifact.
+
+    Arguments:
+    - spec: The spec provided for this operator.
+    - read_artifacts_func: function used to read artifacts from storage layer
+    - write_artifact_func: function used to write artifacts to storage layer
+    - infer_type_func: function used to infer type of artifacts returned by operators.
+
+    The only kwarg we expect is spark_session_obj
+
     """
     exec_state = ExecutionState(user_logs=Logs())
     storage = parse_storage(spec.storage_config)
     try:
         validate_spec(spec)
 
         # Read the input data from intermediate storage.
         inputs, _, serialization_types = time_it(
             job_name=spec.name, job_type=spec.type.value, step="Reading Inputs"
-        )(read_artifact_func)(
+        )(read_artifacts_func)(
             storage=storage,
             input_paths=spec.input_content_paths,
             input_metadata_paths=spec.input_metadata_paths,
             **kwargs,
         )
 
         # We need to check for BSON_TABLE serialization type at both the top level
```

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/extract_function.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/get_extract_path.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/install_requirements.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/main.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/set_conda_version.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/function_executor/spec.py` & `hstestaq-0.2.15/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/param_executor/execute.py` & `hstestaq-0.2.15/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/param_executor/spec.py` & `hstestaq-0.2.15/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/spark/execute_data.py` & `hstestaq-0.2.15/aqueduct_executor/operators/spark/execute_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,28 +20,34 @@
     - load
     - load-table
     - delete-saved-objects
     - discover
 
     Arguments:
     - spec: The spec provided for this operator.
+    - spark_session_obj: The SparkSession
     """
     return run_helper(
         spec=spec,
         read_artifacts_func=read_artifacts_spark,
         write_artifact_func=write_artifact_spark,
         setup_connector_func=setup_connector_spark,
         is_spark=True,
         spark_session_obj=spark_session_obj,
     )
 
 
 def setup_connector_spark(
     connector_name: common.Name, connector_config: config.Config
 ) -> connector.DataConnector:
+    """
+    Sets up the Spark Connectors. We currently support the following resources with Spark:
+    - S3
+    - Snowflake
+    """
     # prevent isort from moving around type: ignore comments which will cause mypy issues.
     # isort: off
     if connector_name == common.Name.SNOWFLAKE:
         try:
             from pyspark.sql import SparkSession
             from snowflake import sqlalchemy
         except:
```

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/spark/execute_function.py` & `hstestaq-0.2.15/aqueduct_executor/operators/spark/execute_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
 def run(spec: FunctionSpec, spark_session_obj: SparkSession) -> None:
     """
     Executes a function operator.
     """
     return run_helper(
         spec=spec,
-        read_artifact_func=read_artifacts_spark,
+        read_artifacts_func=read_artifacts_spark,
         write_artifact_func=write_artifact_spark,
         infer_type_func=infer_artifact_type_spark,
         spark_session_obj=spark_session_obj,
     )
```

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/spark/utils.py` & `hstestaq-0.2.15/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/execute.py` & `hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/system_metric_executor/spec.py` & `hstestaq-0.2.15/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/enums.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/execution.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/config.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/file.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/gcs.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/parse.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/storage/s3.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/timer.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/aqueduct_executor/operators/utils/utils.py` & `hstestaq-0.2.15/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/bin/aqueduct` & `hstestaq-0.2.15/bin/aqueduct`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/hstestaq.egg-info/PKG-INFO` & `hstestaq-0.2.15/hstestaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.14
+Version: 0.2.15
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.14/hstestaq.egg-info/SOURCES.txt` & `hstestaq-0.2.15/hstestaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.14/setup.py` & `hstestaq-0.2.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = open("requirements.txt").read().strip().split("\n")
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="hstestaq",
-    version="0.2.14",
+    version="0.2.15",
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
     description="Prediction Infrastructure for Data Scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
```

