# Comparing `tmp/hstestaq-0.2.12.tar.gz` & `tmp/hstestaq-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstestaq-0.2.12.tar", last modified: Thu Apr 20 20:20:43 2023, max compression
+gzip compressed data, was "hstestaq-0.2.13.tar", last modified: Thu Apr 20 22:10:50 2023, max compression
```

## Comparing `hstestaq-0.2.12.tar` & `hstestaq-0.2.13.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.050523 hstestaq-0.2.12/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.12/MANIFEST.in
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 20:20:43.050235 hstestaq-0.2.12/PKG-INFO
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.001113 hstestaq-0.2.12/aqueduct_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.001305 hstestaq-0.2.12/aqueduct_executor/migrators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.003334 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.005206 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.007596 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.007973 hstestaq-0.2.12/aqueduct_executor/operators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.009074 hstestaq-0.2.12/aqueduct_executor/operators/airflow/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/airflow/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.009412 hstestaq-0.2.12/aqueduct_executor/operators/connectors/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.021884 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/athena.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/common.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/connector.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    12911 2023-04-18 17:47:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/extract.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/load.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/models.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/relational.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.023462 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.030583 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conf.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.035358 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    15880 2023-04-20 19:11:46.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/extract_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/function_executor/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.037114 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/param_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.038589 hstestaq-0.2.12/aqueduct_executor/operators/spark/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     8793 2023-04-03 17:36:30.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_data.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      984 2023-04-20 20:20:04.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/spark/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.041321 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.044212 hstestaq-0.2.12/aqueduct_executor/operators/utils/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/enums.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/exceptions.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/execution.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.047794 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/file.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/parse.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/storage.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/timer.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.12/aqueduct_executor/operators/utils/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.048381 hstestaq-0.2.12/bin/
--rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.12/bin/aqueduct
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 20:20:43.049881 hstestaq-0.2.12/hstestaq.egg-info/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/PKG-INFO
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/SOURCES.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/dependency_links.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/requires.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 20:20:42.000000 hstestaq-0.2.12/hstestaq.egg-info/top_level.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.12/requirements.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 20:20:43.050616 hstestaq-0.2.12/setup.cfg
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 20:20:28.000000 hstestaq-0.2.12/setup.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.692113 hstestaq-0.2.13/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.13/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:10:50.691867 hstestaq-0.2.13/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.648879 hstestaq-0.2.13/aqueduct_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.649069 hstestaq-0.2.13/aqueduct_executor/migrators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.651245 hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.653201 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.655891 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.656272 hstestaq-0.2.13/aqueduct_executor/operators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.657429 hstestaq-0.2.13/aqueduct_executor/operators/airflow/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/airflow/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/airflow/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/airflow/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/airflow/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.657803 hstestaq-0.2.13/aqueduct_executor/operators/connectors/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.669169 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/athena.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/common.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/connector.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    15014 2023-04-20 22:10:22.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/extract.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/load.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/relational.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.670444 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.674746 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.678361 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    16021 2023-04-20 22:10:22.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/function_executor/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.679980 hstestaq-0.2.13/aqueduct_executor/operators/param_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/param_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/param_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/param_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/param_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.681168 hstestaq-0.2.13/aqueduct_executor/operators/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.13/aqueduct_executor/operators/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2450 2023-04-20 22:10:22.000000 hstestaq-0.2.13/aqueduct_executor/operators/spark/execute_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      997 2023-04-20 22:10:22.000000 hstestaq-0.2.13/aqueduct_executor/operators/spark/execute_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/spark/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.682632 hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.685472 hstestaq-0.2.13/aqueduct_executor/operators/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/exceptions.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/execution.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.689231 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/file.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/parse.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/storage.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/timer.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.13/aqueduct_executor/operators/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.689591 hstestaq-0.2.13/bin/
+-rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.13/bin/aqueduct
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 22:10:50.691551 hstestaq-0.2.13/hstestaq.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 22:10:50.000000 hstestaq-0.2.13/hstestaq.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 22:10:50.000000 hstestaq-0.2.13/hstestaq.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 22:10:50.000000 hstestaq-0.2.13/hstestaq.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 22:10:50.000000 hstestaq-0.2.13/hstestaq.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 22:10:50.000000 hstestaq-0.2.13/hstestaq.egg-info/top_level.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.13/requirements.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 22:10:50.692190 hstestaq-0.2.13/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 22:10:38.000000 hstestaq-0.2.13/setup.py
```

### Comparing `hstestaq-0.2.12/PKG-INFO` & `hstestaq-0.2.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.12
+Version: 0.2.13
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `hstestaq-0.2.13/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/airflow/execute.py` & `hstestaq-0.2.13/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/airflow/spec.py` & `hstestaq-0.2.13/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/athena.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/bigquery.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/common.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/config.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/connector.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/execute.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,19 +44,57 @@
     - load-table
     - delete-saved-objects
     - discover
 
     Arguments:
     - spec: The spec provided for this operator.
     """
+    return run_helper(
+        spec=spec,
+        read_artifacts_func=utils.read_artifacts,
+        write_artifact_func=utils.write_artifact,
+        setup_connector_func=setup_connector,
+        is_spark=False,
+    )
+
+
+def run_helper(
+    spec: Spec,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    setup_connector_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
+) -> None:
+    """
+    Runs one of the following connector operations:
+    - authenticate
+    - extract
+    - load
+    - load-table
+    - delete-saved-objects
+    - discover
+
+    Arguments:
+    - spec: The spec provided for this operator.
+    """
     storage = parse_storage(spec.storage_config)
     exec_state = ExecutionState(user_logs=Logs())
 
     try:
-        _execute(spec, storage, exec_state)
+        _execute(
+            spec,
+            storage,
+            exec_state,
+            read_artifacts_func,
+            write_artifact_func,
+            setup_connector_func,
+            is_spark,
+            **kwargs,
+        )
         # Write operator execution metadata
         # Each decorator may set exec_state.status to FAILED, but if none of them did, then we are
         # certain that the operator succeeded.
         if exec_state.status == ExecutionStatus.FAILED:
             print(f"Failed with error. Full Logs:\n{exec_state.json()}")
             utils.write_exec_state(storage, spec.metadata_path, exec_state)
             sys.exit(1)
@@ -82,129 +120,183 @@
         )
         print(f"Failed with system error. Full Logs:\n{exec_state.json()}")
 
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
         sys.exit(1)
 
 
-def _execute(spec: Spec, storage: Storage, exec_state: ExecutionState) -> None:
+def _execute(
+    spec: Spec,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    setup_connector_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
+) -> None:
     if spec.type == JobType.DELETESAVEDOBJECTS:
         run_delete_saved_objects(spec, storage, exec_state)
 
     # Because constructing certain connectors (eg. Postgres) can also involve authentication,
     # we do both in `run_authenticate()`, and give a more helpful error message on failure.
     elif spec.type == JobType.AUTHENTICATE:
-        run_authenticate(spec, exec_state, is_demo=(spec.name == AQUEDUCT_DEMO_NAME))
+        run_authenticate(
+            spec,
+            exec_state,
+            is_demo=(spec.name == AQUEDUCT_DEMO_NAME),
+            setup_connector_func=setup_connector_func,
+        )
 
     else:
-        op = setup_connector(spec.connector_name, spec.connector_config)
+        op = setup_connector_func(spec.connector_name, spec.connector_config)
         if spec.type == JobType.EXTRACT:
-            run_extract(spec, op, storage, exec_state)
+            run_extract(
+                spec,
+                op,
+                storage,
+                exec_state,
+                read_artifacts_func,
+                write_artifact_func,
+                is_spark,
+                **kwargs,
+            )
         elif spec.type == JobType.LOADTABLE:
-            run_load_table(spec, op, storage)
+            run_load_table(spec, op, storage, is_spark)
         elif spec.type == JobType.LOAD:
-            run_load(spec, op, storage, exec_state)
+            run_load(spec, op, storage, exec_state, read_artifacts_func, is_spark, **kwargs)
         elif spec.type == JobType.DISCOVER:
             run_discover(spec, op, storage)
         else:
             raise Exception("Unknown job: %s" % spec.type)
 
 
 def run_authenticate(
     spec: AuthenticateSpec,
     exec_state: ExecutionState,
     is_demo: bool,
+    setup_connector_func: Any,
 ) -> None:
     @exec_state.user_fn_redirected(
         failure_tip=TIP_DEMO_CONNECTION if is_demo else TIP_INTEGRATION_CONNECTION
     )
     def _authenticate() -> None:
-        op = setup_connector(spec.connector_name, spec.connector_config)
+        op = setup_connector_func(spec.connector_name, spec.connector_config)
         op.authenticate()
 
     _authenticate()
 
 
 def run_extract(
-    spec: ExtractSpec, op: connector.DataConnector, storage: Storage, exec_state: ExecutionState
+    spec: ExtractSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
 ) -> None:
     extract_params = spec.parameters
 
     # Search for user-defined placeholders if this is a relational query, and replace them with
     # the appropriate values.
     if isinstance(extract_params, extract.RelationalParams) or isinstance(
         extract_params, extract.MongoDBParams
     ):
-        input_vals, _, _ = utils.read_artifacts(
-            storage,
-            spec.input_content_paths,
-            spec.input_metadata_paths,
+        input_vals, _, _ = read_artifacts_func(
+            storage=storage,
+            input_paths=spec.input_content_paths,
+            input_metadata_paths=spec.input_metadata_paths,
+            **kwargs,
         )
         assert all(
             isinstance(param_val, str) for param_val in input_vals
         ), "Parameter value must be a string."
         extract_params.compile(input_vals)
 
     @exec_state.user_fn_redirected(failure_tip=TIP_EXTRACT)
     def _extract() -> Any:
-        return op.extract(spec.parameters)
+        if is_spark:
+            return op.extract_spark(spec.parameters, **kwargs)  # type: ignore
+        else:
+            return op.extract(spec.parameters)
 
     output = _extract()
 
     output_artifact_type = ArtifactType.TABLE
     derived_from_bson = isinstance(extract_params, extract.MongoDBParams)
     if isinstance(extract_params, extract.S3Params):
         output_artifact_type = extract_params.artifact_type
         # If the type of the output is tuple, then it could be a multi-file S3 request so we
         # overwrite the output type to tuple.
         if isinstance(output, tuple):
             output_artifact_type = ArtifactType.TUPLE
 
     if exec_state.status != ExecutionStatus.FAILED:
-        utils.write_artifact(
+        write_artifact_func(
             storage,
             output_artifact_type,
             derived_from_bson,
             spec.output_content_path,
             spec.output_metadata_path,
             output,
             system_metadata={},
+            **kwargs,
         )
 
 
 def run_delete_saved_objects(spec: Spec, storage: Storage, exec_state: ExecutionState) -> None:
     results = {}
     assert isinstance(spec.connector_name, dict)
     for integration in spec.connector_name:
         op = setup_connector(spec.connector_name[integration], spec.connector_config[integration])
         results[integration] = op.delete(spec.integration_to_object[integration])
     utils.write_delete_saved_objects_results(storage, spec.output_content_path, results)
 
 
 def run_load(
-    spec: LoadSpec, op: connector.DataConnector, storage: Storage, exec_state: ExecutionState
+    spec: LoadSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
 ) -> None:
-    inputs, input_types, _ = utils.read_artifacts(
-        storage,
-        [spec.input_content_path],
-        [spec.input_metadata_path],
+    inputs, input_types, _ = read_artifacts_func(
+        storage=storage,
+        input_paths=[spec.input_content_path],
+        input_metadata_paths=[spec.input_metadata_path],
+        **kwargs,
     )
     if len(inputs) != 1:
         raise Exception("Expected 1 input artifact, but got %d" % len(inputs))
 
     @exec_state.user_fn_redirected(failure_tip=TIP_LOAD)
     def _load() -> None:
-        op.load(spec.parameters, inputs[0], input_types[0])
+        if is_spark:
+            op.load_spark(spec.parameters, inputs[0], input_types[0])  # type: ignore
+        else:
+            op.load(spec.parameters, inputs[0], input_types[0])
 
     _load()
 
 
-def run_load_table(spec: LoadTableSpec, op: connector.DataConnector, storage: Storage) -> None:
+def run_load_table(
+    spec: LoadTableSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    is_spark: bool,
+) -> None:
     df = utils._read_csv(storage.get(spec.csv))
-    op.load(spec.load_parameters.parameters, df, ArtifactType.TABLE)
+    if is_spark:
+        op.load_spark(spec.load_parameters.parameters, df, ArtifactType.TABLE)  # type: ignore
+    else:
+        op.load(spec.load_parameters.parameters, df, ArtifactType.TABLE)
 
 
 def run_discover(spec: DiscoverSpec, op: connector.DataConnector, storage: Storage) -> None:
     tables = op.discover()
     utils.write_discover_results(storage, spec.output_content_path, tables)
```

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/extract.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/gcs.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/load.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/main.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/models.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mongodb.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/mysql.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/postgres.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/relational.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/snowflake.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/s3.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/spec.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sql_server.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/sqlite.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/data/utils.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/conf.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/connectors/tests/utils.py` & `hstestaq-0.2.13/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/execute.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,26 +165,26 @@
             % (len(spec.output_content_paths), len(results)),
         )
 
     return [infer_type_func(res) for res in results]
 
 
 def _write_artifacts(
-    write_func: Any,
+    write_artifact_func: Any,
     results: Any,
     result_types: List[ArtifactType],
     derived_from_bson: bool,
     output_content_paths: List[str],
     output_metadata_paths: List[str],
     system_metadata: Any,
     storage: Storage,
-    **kwargs,
+    **kwargs: Any,
 ) -> None:
     for i, result in enumerate(results):
-        write_func(
+        write_artifact_func(
             storage,
             result_types[i],
             derived_from_bson,
             output_content_paths[i],
             output_metadata_paths[i],
             result,
             system_metadata=system_metadata,
@@ -241,37 +241,43 @@
 
 def run(spec: FunctionSpec) -> None:
     """
     Executes a function operator.
     """
     run_helper(
         spec=spec,
-        read_func=utils.read_artifacts,
-        write_func=utils.write_artifact, 
+        read_artifact_func=utils.read_artifacts,
+        write_artifact_func=utils.write_artifact,
         infer_type_func=infer_artifact_type,
     )
 
 
-def run_helper(spec: FunctionSpec, read_func: Any, write_func: Any, infer_type_func: Any, **kwargs) -> None:
+def run_helper(
+    spec: FunctionSpec,
+    read_artifact_func: Any,
+    write_artifact_func: Any,
+    infer_type_func: Any,
+    **kwargs: Any,
+) -> None:
     """
     Executes a function operator.
     """
     exec_state = ExecutionState(user_logs=Logs())
     storage = parse_storage(spec.storage_config)
     try:
         validate_spec(spec)
 
         # Read the input data from intermediate storage.
         inputs, _, serialization_types = time_it(
             job_name=spec.name, job_type=spec.type.value, step="Reading Inputs"
-        )(read_func)(
-            storage=storage, 
-            input_paths=spec.input_content_paths, 
-            input_metadata_paths=spec.input_metadata_paths, 
-            **kwargs
+        )(read_artifact_func)(
+            storage=storage,
+            input_paths=spec.input_content_paths,
+            input_metadata_paths=spec.input_metadata_paths,
+            **kwargs,
         )
 
         # We need to check for BSON_TABLE serialization type at both the top level
         # and within any serialized pickled collection (if it exists).
         derived_from_bson = SerializationType.BSON_TABLE in serialization_types
         if not derived_from_bson:
             for i, serialization_type in enumerate(serialization_types):
@@ -292,15 +298,17 @@
         if exec_state.status == ExecutionStatus.FAILED:
             # user failure
             utils.write_exec_state(storage, spec.metadata_path, exec_state)
             sys.exit(1)
 
         print("Function invoked successfully!")
 
-        result_types = _validate_result_count_and_infer_type(spec=spec, results=results, infer_type_func=infer_type_func)
+        result_types = _validate_result_count_and_infer_type(
+            spec=spec, results=results, infer_type_func=infer_type_func
+        )
 
         # Perform type checking on the function output.
         if spec.operator_type == OperatorType.METRIC:
             assert len(results) == 1, "Metric operator can only have a single output."
             result = results[0]
 
             if not (
@@ -333,15 +341,15 @@
                     tip=TIP_NOT_BOOL,
                 )
 
             # If the check returned a value we interpret to mean 'false', we exit here, but
             # not before recording the output artifact value (which will be False).
             if not check_passed:
                 print(f"Check Operator did not pass.")
-                write_func(
+                write_artifact_func(
                     storage=storage,
                     artifact_type=ArtifactType.BOOL,
                     derived_from_bson=derived_from_bson,  # derived_from_bson doesn't apply to bool artifact
                     output_path=spec.output_content_paths[0],
                     output_metadata_path=spec.output_metadata_paths[0],
                     content=check_passed,
                     system_metadata=system_metadata,
@@ -376,15 +384,15 @@
                         tip="Expected type %s for the %d-th output of function, but it is of type %s."
                         % (expected_output_type, i, result_types[i]),
                     )
 
         time_it(job_name=spec.name, job_type=spec.type.value, step="Writing Outputs")(
             _write_artifacts
         )(
-            write_func=write_func,
+            write_artifact_func=write_artifact_func,
             results=results,
             result_types=result_types,
             derived_from_bson=derived_from_bson,
             output_content_paths=spec.output_content_paths,
             output_metadata_paths=spec.output_metadata_paths,
             system_metadata=system_metadata,
             storage=storage,
@@ -411,15 +419,14 @@
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
         sys.exit(1)
     finally:
         # Perform any cleanup
         cleanup(spec)
 
 
-
 def run_with_setup(spec: FunctionSpec) -> None:
     """
     Performs the setup needed for a Function operator and then executes it.
     """
     # Generate a unique function extract path if one does not exist already
     if not spec.function_extract_path:
         fn_extract_path = os.path.join(os.getcwd(), str(uuid.uuid4()))
```

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/extract_function.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/get_extract_path.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/install_requirements.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/main.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/set_conda_version.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/function_executor/spec.py` & `hstestaq-0.2.13/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/param_executor/execute.py` & `hstestaq-0.2.13/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/param_executor/spec.py` & `hstestaq-0.2.13/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/spark/execute_function.py` & `hstestaq-0.2.13/aqueduct_executor/operators/spark/execute_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
+
 from aqueduct.utils.type_inference import infer_artifact_type
 from aqueduct_executor.operators.function_executor.execute import run_helper
 from aqueduct_executor.operators.function_executor.spec import FunctionSpec
 from aqueduct_executor.operators.spark.utils import read_artifacts_spark, write_artifact_spark
 from aqueduct_executor.operators.utils.enums import ArtifactType
-
-
 from pyspark.sql import SparkSession, dataframe
 
 
 def infer_artifact_type_spark(value: Any) -> Any:
     if isinstance(value, dataframe.DataFrame):
         return ArtifactType.TABLE
     else:
@@ -17,13 +16,13 @@
 
 
 def run(spec: FunctionSpec, spark_session_obj: SparkSession) -> None:
     """
     Executes a function operator.
     """
     return run_helper(
-        spec=spec, 
-        read_func=read_artifacts_spark, 
-        write_func=write_artifact_spark, 
-        infer_type_func=infer_artifact_type_spark, 
+        spec=spec,
+        read_artifact_func=read_artifacts_spark,
+        write_artifact_func=write_artifact_spark,
+        infer_type_func=infer_artifact_type_spark,
         spark_session_obj=spark_session_obj,
     )
```

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/spark/utils.py` & `hstestaq-0.2.13/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/execute.py` & `hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/system_metric_executor/spec.py` & `hstestaq-0.2.13/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/enums.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/execution.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/config.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/file.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/gcs.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/parse.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/storage/s3.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/timer.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/aqueduct_executor/operators/utils/utils.py` & `hstestaq-0.2.13/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/bin/aqueduct` & `hstestaq-0.2.13/bin/aqueduct`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/hstestaq.egg-info/PKG-INFO` & `hstestaq-0.2.13/hstestaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.2.12
+Version: 0.2.13
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `hstestaq-0.2.12/hstestaq.egg-info/SOURCES.txt` & `hstestaq-0.2.13/hstestaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hstestaq-0.2.12/setup.py` & `hstestaq-0.2.13/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = open("requirements.txt").read().strip().split("\n")
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="hstestaq",
-    version="0.2.12",
+    version="0.2.13",
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
     description="Prediction Infrastructure for Data Scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
```

