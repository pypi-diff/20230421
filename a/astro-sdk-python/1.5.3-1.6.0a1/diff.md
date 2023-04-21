# Comparing `tmp/astro-sdk-python-1.5.3.tar.gz` & `tmp/astro-sdk-python-1.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-sdk-python-1.5.3.tar", last modified: Wed Mar  8 22:30:42 2023, max compression
+gzip compressed data, was "astro-sdk-python-1.6.0a1.tar", last modified: Fri Apr 21 19:05:24 2023, max compression
```

## Comparing `astro-sdk-python-1.5.3.tar` & `astro-sdk-python-1.6.0a1.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-lrwxr-xr-x   0        0        0        0 2023-03-08 22:30:24.178608 astro-sdk-python-1.5.3/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     8344 2023-03-08 22:30:24.178608 astro-sdk-python-1.5.3/README.md
--rw-r--r--   0        0        0     5313 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      685 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/airflow/__init__.py
--rw-r--r--   0        0        0     1605 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/airflow/datasets.py
--rw-r--r--   0        0        0     2018 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/constants.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/custom_backend/__init__.py
--rw-r--r--   0        0        0     2187 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/custom_backend/astro_custom_backend.py
--rw-r--r--   0        0        0     3915 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/custom_backend/serializer.py
--rw-r--r--   0        0        0     1876 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/databases/aws/__init__.py
--rw-r--r--   0        0        0    18189 2023-03-08 22:30:24.194608 astro-sdk-python-1.5.3/src/astro/databases/aws/redshift.py
--rw-r--r--   0        0        0    36674 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/base.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/__init__.py
--rw-r--r--   0        0        0     7247 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/api_utils.py
--rw-r--r--   0        0        0    17479 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/delta.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/__init__.py
--rw-r--r--   0        0        0      720 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
--rw-r--r--   0        0        0      647 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
--rw-r--r--   0        0        0      913 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
--rw-r--r--   0        0        0      512 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
--rw-r--r--   0        0        0     6287 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/load_file_job.py
--rw-r--r--   0        0        0      880 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
--rw-r--r--   0        0        0     2687 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/databricks/load_options.py
--rw-r--r--   0        0        0     6181 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/duckdb.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/google/__init__.py
--rw-r--r--   0        0        0    26823 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/google/bigquery.py
--rw-r--r--   0        0        0    16827 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/mssql.py
--rw-r--r--   0        0        0    10678 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/postgres.py
--rw-r--r--   0        0        0    42201 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/snowflake.py
--rw-r--r--   0        0        0     6508 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/databases/sqlite.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/dataframes/__init__.py
--rw-r--r--   0        0        0     4116 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/dataframes/load_options.py
--rw-r--r--   0        0        0     1977 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/dataframes/pandas.py
--rw-r--r--   0        0        0     1137 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/exceptions.py
--rw-r--r--   0        0        0     1096 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/__init__.py
--rw-r--r--   0        0        0    10151 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/base.py
--rw-r--r--   0        0        0     1535 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/amazon/__init__.py
--rw-r--r--   0        0        0     3605 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/amazon/s3.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/azure/__init__.py
--rw-r--r--   0        0        0     4290 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/azure/wasb.py
--rw-r--r--   0        0        0     6355 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/base.py
--rw-r--r--   0        0        0     2374 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/ftp.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/google/__init__.py
--rw-r--r--   0        0        0     4420 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/google/gcs.py
--rw-r--r--   0        0        0     5006 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/google/gdrive.py
--rw-r--r--   0        0        0     1303 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/http.py
--rw-r--r--   0        0        0     1531 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/local.py
--rw-r--r--   0        0        0     3267 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/locations/sftp.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/operators/__init__.py
--rw-r--r--   0        0        0     1595 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/operators/files.py
--rw-r--r--   0        0        0     2576 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/__init__.py
--rw-r--r--   0        0        0     1504 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/base.py
--rw-r--r--   0        0        0     1900 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/csv.py
--rw-r--r--   0        0        0     2197 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/json.py
--rw-r--r--   0        0        0     3652 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/ndjson.py
--rw-r--r--   0        0        0     2848 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/files/types/parquet.py
--rw-r--r--   0        0        0      700 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/lineage/__init__.py
--rw-r--r--   0        0        0     4264 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/lineage/facets.py
--rw-r--r--   0        0        0     3910 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/options.py
--rw-r--r--   0        0        0     3791 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/settings.py
--rw-r--r--   0        0        0     3194 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/sql/operators/__init__.py
--rw-r--r--   0        0        0     7857 2023-03-08 22:30:24.198608 astro-sdk-python-1.5.3/src/astro/sql/operators/append.py
--rw-r--r--   0        0        0    18192 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/base_decorator.py
--rw-r--r--   0        0        0      334 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/base_operator.py
--rw-r--r--   0        0        0    11280 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/cleanup.py
--rw-r--r--   0        0        0     7870 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/data_validations/check_column.py
--rw-r--r--   0        0        0     3696 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/data_validations/check_table.py
--rw-r--r--   0        0        0    15366 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/dataframe.py
--rw-r--r--   0        0        0     1435 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/drop.py
--rw-r--r--   0        0        0     2693 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/export_file.py
--rw-r--r--   0        0        0     2715 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/export_table_to_file.py
--rw-r--r--   0        0        0     7035 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/export_to_file.py
--rw-r--r--   0        0        0    17274 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/load_file.py
--rw-r--r--   0        0        0     8824 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/merge.py
--rw-r--r--   0        0        0     9807 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/raw_sql.py
--rw-r--r--   0        0        0     7353 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/transform.py
--rw-r--r--   0        0        0      880 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/operators/upstream_task_mixin.py
--rw-r--r--   0        0        0      160 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/sql/table.py
--rw-r--r--   0        0        0     8098 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/table.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/compat/__init__.py
--rw-r--r--   0        0        0      359 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/compat/functools.py
--rw-r--r--   0        0        0      843 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/compat/typing.py
--rw-r--r--   0        0        0     2022 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/dataframe.py
--rw-r--r--   0        0        0     1581 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/load.py
--rw-r--r--   0        0        0     2790 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/path.py
--rw-r--r--   0        0        0     4025 2023-03-08 22:30:24.202608 astro-sdk-python-1.5.3/src/astro/utils/table.py
--rw-r--r--   0        0        0    13314 1970-01-01 00:00:00.000000 astro-sdk-python-1.5.3/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     8344 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/README.md
+-rw-r--r--   0        0        0     5313 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py
+-rw-r--r--   0        0        0     2018 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/constants.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/__init__.py
+-rw-r--r--   0        0        0     2187 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py
+-rw-r--r--   0        0        0     3915 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py
+-rw-r--r--   0        0        0     1876 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/__init__.py
+-rw-r--r--   0        0        0    18189 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py
+-rw-r--r--   0        0        0    37127 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/base.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/__init__.py
+-rw-r--r--   0        0        0     7247 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py
+-rw-r--r--   0        0        0    17788 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/__init__.py
+-rw-r--r--   0        0        0      720 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
+-rw-r--r--   0        0        0      647 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
+-rw-r--r--   0        0        0      913 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
+-rw-r--r--   0        0        0      512 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
+-rw-r--r--   0        0        0     6287 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py
+-rw-r--r--   0        0        0      880 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
+-rw-r--r--   0        0        0     2687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py
+-rw-r--r--   0        0        0     6181 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/__init__.py
+-rw-r--r--   0        0        0    26823 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py
+-rw-r--r--   0        0        0    17049 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py
+-rw-r--r--   0        0        0    10678 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py
+-rw-r--r--   0        0        0    42201 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py
+-rw-r--r--   0        0        0     6508 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/__init__.py
+-rw-r--r--   0        0        0     4116 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py
+-rw-r--r--   0        0        0     1977 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py
+-rw-r--r--   0        0        0     1137 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/exceptions.py
+-rw-r--r--   0        0        0     1096 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/__init__.py
+-rw-r--r--   0        0        0    10151 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/base.py
+-rw-r--r--   0        0        0     1535 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/__init__.py
+-rw-r--r--   0        0        0     3605 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/__init__.py
+-rw-r--r--   0        0        0     4290 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/wasb.py
+-rw-r--r--   0        0        0     6355 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py
+-rw-r--r--   0        0        0     2374 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/__init__.py
+-rw-r--r--   0        0        0     4420 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py
+-rw-r--r--   0        0        0     5006 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py
+-rw-r--r--   0        0        0     1303 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py
+-rw-r--r--   0        0        0     1531 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py
+-rw-r--r--   0        0        0     3267 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/sftp.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py
+-rw-r--r--   0        0        0     2576 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/base.py
+-rw-r--r--   0        0        0     1900 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py
+-rw-r--r--   0        0        0     2197 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/json.py
+-rw-r--r--   0        0        0     3652 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py
+-rw-r--r--   0        0        0     2848 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py
+-rw-r--r--   0        0        0      700 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py
+-rw-r--r--   0        0        0     4264 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py
+-rw-r--r--   0        0        0     3910 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/options.py
+-rw-r--r--   0        0        0     1117 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/query_modifier.py
+-rw-r--r--   0        0        0     3791 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/settings.py
+-rw-r--r--   0        0        0     3194 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/__init__.py
+-rw-r--r--   0        0        0     7857 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py
+-rw-r--r--   0        0        0    18379 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py
+-rw-r--r--   0        0        0      334 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_operator.py
+-rw-r--r--   0        0        0    11280 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py
+-rw-r--r--   0        0        0     7870 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py
+-rw-r--r--   0        0        0     3696 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py
+-rw-r--r--   0        0        0    15366 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py
+-rw-r--r--   0        0        0     1435 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py
+-rw-r--r--   0        0        0     2693 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py
+-rw-r--r--   0        0        0     2715 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py
+-rw-r--r--   0        0        0     7035 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py
+-rw-r--r--   0        0        0    17274 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py
+-rw-r--r--   0        0        0     8824 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py
+-rw-r--r--   0        0        0     9902 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py
+-rw-r--r--   0        0        0     7401 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py
+-rw-r--r--   0        0        0      880 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py
+-rw-r--r--   0        0        0      160 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/table.py
+-rw-r--r--   0        0        0     8098 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/table.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/__init__.py
+-rw-r--r--   0        0        0      359 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/functools.py
+-rw-r--r--   0        0        0      843 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py
+-rw-r--r--   0        0        0     2022 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py
+-rw-r--r--   0        0        0     1581 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/load.py
+-rw-r--r--   0        0        0     2790 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/path.py
+-rw-r--r--   0        0        0     4025 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/table.py
+-rw-r--r--   0        0        0    13316 1970-01-01 00:00:00.000000 astro-sdk-python-1.6.0a1/PKG-INFO
```

### Comparing `astro-sdk-python-1.5.3/README.md` & `astro-sdk-python-1.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/pyproject.toml` & `astro-sdk-python-1.6.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A decorator that allows users to run SQL queries natively in Airflow."""
 
-__version__ = "1.5.3"
+__version__ = "1.6.0a1"
 
 
 # This is needed to allow Airflow to pick up specific metadata fields it needs
 # for certain features. We recognize it's a bit unclean to define these in
 # multiple places, but at this point it's the only workaround if you'd like
 # your custom conn type to show up in the Airflow UI.
 def get_provider_info() -> dict:
```

### Comparing `astro-sdk-python-1.5.3/src/astro/airflow/datasets.py` & `astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/constants.py` & `astro-sdk-python-1.6.0a1/src/astro/constants.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/custom_backend/astro_custom_backend.py` & `astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/custom_backend/serializer.py` & `astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/aws/redshift.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/base.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 from astro.dataframes.pandas import PandasDataframe
 from astro.exceptions import DatabaseCustomError, NonExistentTableException
 from astro.files import File, resolve_file_path_pattern
 from astro.files.types import create_file_type
 from astro.files.types.base import FileType as FileTypeConstants
 from astro.options import LoadOptions
+from astro.query_modifier import QueryModifier
 from astro.settings import LOAD_FILE_ENABLE_NATIVE_FALLBACK, LOAD_TABLE_AUTODETECT_ROWS_COUNT, SCHEMA
 from astro.table import BaseTable, Metadata
 from astro.utils.compat.functools import cached_property
 
 
 class BaseDatabase(ABC):
     """
@@ -98,22 +99,24 @@
         return self.hook.get_sqlalchemy_engine()  # type: ignore[no-any-return]
 
     def run_sql(
         self,
         sql: str | ClauseElement = "",
         parameters: dict | None = None,
         handler: Callable | None = None,
+        query_modifier: QueryModifier = QueryModifier(),
         **kwargs,
     ) -> Any:
         """
         Return the results to running a SQL statement.
 
         Whenever possible, this method should be implemented using Airflow Hooks,
         since this will simplify the integration with Async operators.
 
+        :param query_modifier: a query modifier that informs the pre and post query queries.
         :param sql: Contains SQL query to be run against database
         :param parameters: Optional parameters to be used to render the query
         :param autocommit: Optional autocommit flag
         :param handler: function that takes in a cursor as an argument.
         """
         if parameters is None:
             parameters = {}
@@ -122,15 +125,15 @@
             warnings.warn(
                 "`sql_statement` is deprecated and will be removed in future release"
                 "Please use  `sql` param instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             sql = kwargs.get("sql_statement")  # type: ignore
-
+        sql = query_modifier.merge_pre_and_post_queries(sql)
         # We need to autocommit=True to make sure the query runs. This is done exclusively for SnowflakeDatabase's
         # truncate method to reflect changes.
         if isinstance(sql, str):
             result = self.connection.execute(
                 sqlalchemy.text(sql).execution_options(autocommit=True), parameters
             )
         else:
@@ -324,26 +327,28 @@
             )
 
     def create_table_from_select_statement(
         self,
         statement: str,
         target_table: BaseTable,
         parameters: dict | None = None,
+        query_modifier: QueryModifier = QueryModifier(),
     ) -> None:
         """
         Export the result rows of a query statement into another table.
 
+        :param query_modifier: a query modifier that informs the pre and post query queries.
         :param statement: SQL query statement
         :param target_table: Destination table where results will be recorded.
         :param parameters: (Optional) parameters to be used to render the SQL query
         """
         statement = self._create_table_statement.format(
             self.get_table_qualified_name(target_table), statement
         )
-        self.run_sql(statement, parameters)
+        self.run_sql(sql=statement, parameters=parameters, query_modifier=query_modifier)
 
     def drop_table(self, table: BaseTable) -> None:
         """
         Delete a SQL table, if it exists.
 
         :param table: The table to be deleted.
         """
```

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/api_utils.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/delta.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from astro.constants import DEFAULT_CHUNK_SIZE, ColumnCapitalization, LoadExistStrategy, MergeConflictStrategy
 from astro.databases.base import BaseDatabase
 from astro.databases.databricks.load_file.load_file_job import load_file_to_delta
 from astro.databases.databricks.load_options import DeltaLoadOptions
 from astro.dataframes.pandas import PandasDataframe
 from astro.files import File
 from astro.options import LoadOptions
+from astro.query_modifier import QueryModifier
 from astro.table import BaseTable, Metadata
 
 
 class DeltaDatabase(BaseDatabase):
     LOAD_OPTIONS_CLASS_NAME = ("DeltaLoadOptions",)
     _create_table_statement: str = "CREATE TABLE IF NOT EXISTS {} USING DELTA AS {} "
 
@@ -158,26 +159,28 @@
         return ""
 
     def create_table_from_select_statement(
         self,
         statement: str,
         target_table: BaseTable,
         parameters: dict | None = None,
+        query_modifier=QueryModifier(),
     ) -> None:
         """
         Create a Delta table from a SQL SELECT statement.
 
         :param statement: Statement that will return a table
         :param target_table: The table which the result of the SQL statement will be placed
         :param parameters: Parameters to pass to databricks
         :return: None
         """
         statement = self._create_table_statement.format(
             self.get_table_qualified_name(target_table), statement
         )
+        statement = query_modifier.merge_pre_and_post_queries(statement)
         self.run_sql(sql=statement, parameters=parameters)
 
     def parameterize_variable(self, variable: str) -> str:
         """
         Parameterize a variable in a way that the Databricks SQL API can recognize.
         :param variable: Variable to parameterize
         :return: The number of rows in the table
@@ -192,28 +195,31 @@
         return result.asDict()["count(1)"]
 
     def run_sql(
         self,
         sql: str | ClauseElement = "",
         parameters: dict | None = None,
         handler: Callable | None = None,
+        query_modifier: QueryModifier = QueryModifier(),
         **kwargs,
     ) -> Any:
         """
         Run SQL against a delta table using spark SQL.
 
+        :param query_modifier:
         :param sql: SQL Query to run on delta table
         :param parameters: parameters to pass to delta
         :param handler: function that takes in a databricks cursor as an argument.
         :param kwargs:
         :return: None if there is no handler, otherwise return result of handler function
         """
         hook = DatabricksSqlHook(
             databricks_conn_id=self.conn_id,
         )
+        sql = query_modifier.merge_pre_and_post_queries(sql)
         return hook.run(sql, parameters=parameters, handler=handler)
 
     def table_exists(self, table: BaseTable) -> bool:
         """
         Queries databricks to check if a table exists.
 
         Since the databricks SQL API returns an exception if the table does not exist
```

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/load_file_job.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_file/load_file_python_code_generator.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/databricks/load_options.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/duckdb.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/google/bigquery.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/mssql.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from airflow.providers.microsoft.mssql.hooks.mssql import MsSqlHook
 from pymssql._pymssql import ProgrammingError
 from sqlalchemy.sql import ClauseElement
 
 from astro.constants import DEFAULT_CHUNK_SIZE, LoadExistStrategy, MergeConflictStrategy
 from astro.databases.base import BaseDatabase
 from astro.options import LoadOptions
+from astro.query_modifier import QueryModifier
 from astro.settings import MSSQL_SCHEMA
 from astro.table import BaseTable, Metadata
 from astro.utils.compat.functools import cached_property
 
 DEFAULT_CONN_ID = MsSqlHook.default_conn_name
 
 
@@ -140,14 +141,15 @@
         return any(query in sql.lower() for query in self._queries_requiring_autocommit)
 
     def run_sql(
         self,
         sql: str | ClauseElement = "",
         parameters: dict | None = None,
         handler: Callable | None = None,
+        query_modifier: QueryModifier = QueryModifier(),
         **kwargs,
     ) -> Any:
         """
         Return the results to running a SQL statement.
         Whenever possible, this method should be implemented using Airflow Hooks,
         since this will simplify the integration with Async operators.
 
@@ -163,14 +165,15 @@
                 "`sql_statement` is deprecated and will be removed in future release"
                 "Please use  `sql` param instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             sql = kwargs.get("sql_statement")  # type: ignore
 
+        sql = query_modifier.merge_pre_and_post_queries(sql)
         autocommit = kwargs.get("autocommit", False)
 
         # We need to set autocommit=True for specific queries
         if isinstance(sql, str):
             if (autocommit is True) or self.is_autocommit_required(sql):
                 self.connection.execute(sqlalchemy.text(sql).execution_options(autocommit=True), parameters)
             else:
@@ -196,14 +199,15 @@
             self.run_sql(statement, autocommit=True)
 
     def create_table_from_select_statement(
         self,
         statement: str,
         target_table: BaseTable,
         parameters: dict | None = None,
+        query_modifier: QueryModifier = QueryModifier(),
     ) -> None:
         """
         Export the result rows of a query statement into another table.
 
         :param statement: SQL query statement
         :param target_table: Destination table where results will be recorded.
         :param parameters: (Optional) parameters to be used to render the SQL query
```

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/postgres.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/snowflake.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/databases/sqlite.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/dataframes/load_options.py` & `astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/dataframes/pandas.py` & `astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/exceptions.py` & `astro-sdk-python-1.6.0a1/src/astro/exceptions.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/amazon/s3.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/azure/wasb.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/wasb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/ftp.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/google/gcs.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/google/gdrive.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/http.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/local.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/locations/sftp.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/sftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/operators/files.py` & `astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/csv.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/json.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/json.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/ndjson.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/files/types/parquet.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/lineage/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/lineage/facets.py` & `astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/options.py` & `astro-sdk-python-1.6.0a1/src/astro/options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/settings.py` & `astro-sdk-python-1.6.0a1/src/astro/settings.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/append.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/base_decorator.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from airflow.models import BaseOperator
 from airflow.models.xcom_arg import XComArg
 from sqlalchemy.sql.functions import Function
 
 from astro.airflow.datasets import kwargs_with_datasets
 from astro.databases import create_database
 from astro.databases.base import BaseDatabase
+from astro.query_modifier import QueryModifier
 from astro.sql.operators.upstream_task_mixin import UpstreamTaskMixin
 from astro.table import BaseTable, Table
 from astro.utils.compat.functools import cached_property
 from astro.utils.compat.typing import Context
 from astro.utils.table import find_first_table
 
 
@@ -33,14 +34,15 @@
         parameters: dict | None = None,
         handler: Function | None = None,
         database: str | None = None,
         schema: str | None = None,
         response_limit: int = -1,
         response_size: int = -1,
         sql: str = "",
+        query_modifier: QueryModifier = QueryModifier(),
         **kwargs: Any,
     ):
         self.kwargs = kwargs or {}
         self.op_kwargs: dict = self.kwargs.get("op_kwargs") or {}
         self.output_table: BaseTable = self.op_kwargs.pop("output_table", Table())
         self.handler = self.op_kwargs.pop("handler", handler)
         self.conn_id = self.op_kwargs.pop("conn_id", conn_id)
@@ -49,14 +51,15 @@
         self.parameters = parameters or {}
         self.database = self.op_kwargs.pop("database", database)
         self.schema = self.op_kwargs.pop("schema", schema)
         self.response_limit = self.op_kwargs.pop("response_limit", response_limit)
         self.response_size = self.op_kwargs.pop("response_size", response_size)
 
         self.op_args: dict[str, Table | pd.DataFrame] = {}
+        self.query_modifier = self.op_kwargs.pop("query_modifier", query_modifier)
 
         # We purposely do NOT render upstream_tasks otherwise we could have a case where a user
         # has 10 dataframes as upstream tasks and it crashes the worker
         upstream_tasks = self.op_kwargs.pop("upstream_tasks", [])
         super().__init__(
             upstream_tasks=upstream_tasks,
             **kwargs_with_datasets(kwargs=kwargs, output_datasets=self.output_table),
```

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/cleanup.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/data_validations/check_column.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/data_validations/check_table.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/dataframe.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/drop.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/export_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/export_table_to_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/export_to_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/load_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/merge.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/raw_sql.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,20 @@
         self.results_format = results_format
         self.fail_on_empty = fail_on_empty
 
     def execute(self, context: Context) -> Any:
         super().execute(context)
 
         self.handler = self.get_handler()
-        result = self.database_impl.run_sql(sql=self.sql, parameters=self.parameters, handler=self.handler)
+        result = self.database_impl.run_sql(
+            sql=self.sql,
+            parameters=self.parameters,
+            handler=self.handler,
+            query_modifier=self.query_modifier,
+        )
         if self.response_size == -1 and not settings.IS_CUSTOM_XCOM_BACKEND:
             logging.warning(
                 "Using `run_raw_sql` without `response_size` can result in excessive amount of data being recorded "
                 "to the Airflow metadata database, leading to issues to the orchestration of tasks. It is possible to "
                 "avoid this problem by either setting `response_size` to a small integer or by using a custom XCom "
                 "backend."
             )
```

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/transform.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         super().execute(context)
         self.database_impl.create_schema_if_needed(self.output_table.metadata.schema)
         self.database_impl.drop_table(self.output_table)
         self.database_impl.create_table_from_select_statement(
             statement=self.sql,
             target_table=self.output_table,
             parameters=self.parameters,
+            query_modifier=self.query_modifier,
         )
         # TODO: remove pushing to XCom once we update the airflow version.
         context["ti"].xcom_push(
             key="output_table_row_count", value=str(self.database_impl.row_count(self.output_table))
         )
         context["ti"].xcom_push(key="output_table_conn_id", value=str(self.output_table.conn_id))
         return self.output_table
```

### Comparing `astro-sdk-python-1.5.3/src/astro/sql/operators/upstream_task_mixin.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/table.py` & `astro-sdk-python-1.6.0a1/src/astro/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/utils/compat/typing.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/utils/dataframe.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/utils/load.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/load.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/utils/path.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/path.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/src/astro/utils/table.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.5.3/PKG-INFO` & `astro-sdk-python-1.6.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-sdk-python
-Version: 1.5.3
+Version: 1.6.0a1
 Summary: Astro SDK allows rapid and clean development of {Extract, Load, Transform} workflows using Python and SQL, powered by Apache Airflow.
 Keywords: airflow,provider,astronomer,sql,decorator,task flow,elt,etl,dag
 Author-email: Astronomer <humans@astronomer.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

