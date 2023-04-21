# Comparing `tmp/apache-airflow-providers-microsoft-azure-5.3.1rc2.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-5.3.1rc2.tar", last modified: Wed Apr 12 17:49:36 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-6.0.0rc1.tar", last modified: Fri Apr 21 19:49:40 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2.tar` & `apache-airflow-providers-microsoft-azure-6.0.0rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:36.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-12 17:49:30.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25056 2023-04-12 17:49:36.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23435 2023-04-12 17:49:30.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16620 2023-04-12 17:49:30.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6056 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    12985 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    11484 2023-04-12 16:51:16.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5611 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     5957 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5293 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4765 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8863 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 17:49:36.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25056 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-12 17:49:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2359 2023-04-12 17:49:36.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-04-12 17:49:30.000000 apache-airflow-providers-microsoft-azure-5.3.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    25473 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23852 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16641 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6056 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    12985 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    11484 2023-04-13 08:25:21.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2023-04-19 10:00:26.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 10:05:41.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8863 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25473 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/LICENSE` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 5.3.1rc2
+Version: 6.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.1rc2``
+Release: ``6.0.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -149,14 +149,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``AzureBlobStorageToGCSOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+Misc
+~~~~
+
+* ``Merge WasbBlobAsyncSensor to WasbBlobSensor (#30488)``
+
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
@@ -181,14 +198,15 @@
 ~~~~~~~~~
 
 * ``Fix ADF job failure during deferral (#30248)``
 * ``Fix AzureDataLakeStorageV2Hook 'account_url' with Active Directory authentication (#29980) (#29981)``
 
 Misc
 ~~~~
+
 * ``merge AzureDataFactoryPipelineRunStatusAsyncSensor to AzureDataFactoryPipelineRunStatusSensor (#30250)``
 * ``Expose missing params in AzureSynapseHook API docs (#30099)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``organize azure provider.yaml (#30155)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/README.rst` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.1rc2``
+Release: ``6.0.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -113,14 +113,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``AzureBlobStorageToGCSOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+Misc
+~~~~
+
+* ``Merge WasbBlobAsyncSensor to WasbBlobSensor (#30488)``
+
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
@@ -145,14 +162,15 @@
 ~~~~~~~~~
 
 * ``Fix ADF job failure during deferral (#30248)``
 * ``Fix AzureDataLakeStorageV2Hook 'account_url' with Active Directory authentication (#29980) (#29981)``
 
 Misc
 ~~~~
+
 * ``merge AzureDataFactoryPipelineRunStatusAsyncSensor to AzureDataFactoryPipelineRunStatusSensor (#30250)``
 * ``Expose missing params in AzureSynapseHook API docs (#30099)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``organize azure provider.yaml (#30155)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
         "suspended": False,
         "versions": [
+            "6.0.0",
             "5.3.1",
             "5.3.0",
             "5.2.1",
             "5.2.0",
             "5.1.0",
             "5.0.2",
             "5.0.1",
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.exceptions import AirflowException
 from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
 from airflow.providers.microsoft.azure.triggers.wasb import WasbBlobSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
@@ -34,85 +35,64 @@
     Waits for a blob to arrive on Azure Blob Storage.
 
     :param container_name: Name of the container.
     :param blob_name: Name of the blob.
     :param wasb_conn_id: Reference to the :ref:`wasb connection <howto/connection:wasb>`.
     :param check_options: Optional keyword arguments that
         `WasbHook.check_for_blob()` takes.
+    :param deferrable: Run sensor in the deferrable mode.
+    :param public_read: whether an anonymous public read access should be used. Default is False
     """
 
     template_fields: Sequence[str] = ("container_name", "blob_name")
 
     def __init__(
         self,
         *,
         container_name: str,
         blob_name: str,
         wasb_conn_id: str = "wasb_default",
         check_options: dict | None = None,
+        public_read: bool = False,
+        deferrable: bool = False,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if check_options is None:
             check_options = {}
         self.wasb_conn_id = wasb_conn_id
         self.container_name = container_name
         self.blob_name = blob_name
         self.check_options = check_options
+        self.public_read = public_read
+        self.deferrable = deferrable
 
     def poke(self, context: Context):
         self.log.info("Poking for blob: %s\n in wasb://%s", self.blob_name, self.container_name)
         hook = WasbHook(wasb_conn_id=self.wasb_conn_id)
         return hook.check_for_blob(self.container_name, self.blob_name, **self.check_options)
 
-
-class WasbBlobAsyncSensor(WasbBlobSensor):
-    """
-    Polls asynchronously for the existence of a blob in a WASB container.
-
-    :param container_name: name of the container in which the blob should be searched for
-    :param blob_name: name of the blob to check existence for
-    :param wasb_conn_id: the connection identifier for connecting to Azure WASB
-    :param poke_interval:  polling period in seconds to check for the status
-    :param public_read: whether an anonymous public read access should be used. Default is False
-    :param timeout: Time, in seconds before the task times out and fails.
-    """
-
-    def __init__(
-        self,
-        *,
-        container_name: str,
-        blob_name: str,
-        wasb_conn_id: str = "wasb_default",
-        public_read: bool = False,
-        poke_interval: float = 5.0,
-        **kwargs: Any,
-    ):
-        self.container_name = container_name
-        self.blob_name = blob_name
-        self.poke_interval = poke_interval
-        super().__init__(container_name=container_name, blob_name=blob_name, **kwargs)
-        self.wasb_conn_id = wasb_conn_id
-        self.public_read = public_read
-
     def execute(self, context: Context) -> None:
-        """Defers trigger class to poll for state of the job run until it reaches
-        a failure state or success state
+        """Defers trigger class to poll for state of the job run until
+        it reaches a failure state or success state
         """
-        self.defer(
-            timeout=timedelta(seconds=self.timeout),
-            trigger=WasbBlobSensorTrigger(
-                container_name=self.container_name,
-                blob_name=self.blob_name,
-                wasb_conn_id=self.wasb_conn_id,
-                public_read=self.public_read,
-                poke_interval=self.poke_interval,
-            ),
-            method_name="execute_complete",
-        )
+        if not self.deferrable:
+            super().execute(context=context)
+        else:
+            self.defer(
+                timeout=timedelta(seconds=self.timeout),
+                trigger=WasbBlobSensorTrigger(
+                    container_name=self.container_name,
+                    blob_name=self.blob_name,
+                    wasb_conn_id=self.wasb_conn_id,
+                    public_read=self.public_read,
+                    poke_interval=self.poke_interval,
+                ),
+                method_name="execute_complete",
+            )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
@@ -120,14 +100,38 @@
             if event["status"] == "error":
                 raise AirflowException(event["message"])
             self.log.info(event["message"])
         else:
             raise AirflowException("Did not receive valid event from the triggerer")
 
 
+class WasbBlobAsyncSensor(WasbBlobSensor):
+    """
+    Polls asynchronously for the existence of a blob in a WASB container.
+
+    :param container_name: name of the container in which the blob should be searched for
+    :param blob_name: name of the blob to check existence for
+    :param wasb_conn_id: the connection identifier for connecting to Azure WASB
+    :param poke_interval:  polling period in seconds to check for the status
+    :param public_read: whether an anonymous public read access should be used. Default is False
+    :param timeout: Time, in seconds before the task times out and fails.
+    """
+
+    def __init__(self, **kwargs: Any) -> None:
+        warnings.warn(
+            "Class `WasbBlobAsyncSensor` is deprecated and "
+            "will be removed in a future release. "
+            "Please use `WasbBlobSensor` and "
+            "set `deferrable` attribute to `True` instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init__(**kwargs, deferrable=True)
+
+
 class WasbPrefixSensor(BaseSensorOperator):
     """
     Waits for blobs matching a prefix to arrive on Azure Blob Storage.
 
     :param container_name: Name of the container.
     :param prefix: Prefix of the blob.
     :param wasb_conn_id: Reference to the wasb connection.
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import tempfile
-import warnings
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.google.cloud.hooks.gcs import GCSHook
 from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
 
 if TYPE_CHECKING:
@@ -42,17 +41,14 @@
     :param blob_name: Name of the blob
     :param file_path: Path to the file to download
     :param container_name: Name of the container
     :param bucket_name: The bucket to upload to
     :param object_name: The object name to set when uploading the file
     :param filename: The local file path to the file to be uploaded
     :param gzip: Option to compress local file or file data for upload
-    :param delegate_to: The account to impersonate using domain-wide delegation of authority,
-        if any. For this to work, the service account making the request must have
-        domain-wide delegation enabled.
     :param impersonation_chain: Optional service account to impersonate using short-term
         credentials, or chained list of accounts required to get the access_token
         of the last account in the list, which will be impersonated in the request.
         If set as a string, the account must grant the originating account
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
@@ -67,33 +63,27 @@
         blob_name: str,
         file_path: str,
         container_name: str,
         bucket_name: str,
         object_name: str,
         filename: str,
         gzip: bool,
-        delegate_to: str | None,
         impersonation_chain: str | Sequence[str] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.wasb_conn_id = wasb_conn_id
         self.gcp_conn_id = gcp_conn_id
         self.blob_name = blob_name
         self.file_path = file_path
         self.container_name = container_name
         self.bucket_name = bucket_name
         self.object_name = object_name
         self.filename = filename
         self.gzip = gzip
-        if delegate_to:
-            warnings.warn(
-                "'delegate_to' parameter is deprecated, please use 'impersonation_chain'", DeprecationWarning
-            )
-        self.delegate_to = delegate_to
         self.impersonation_chain = impersonation_chain
 
     template_fields: Sequence[str] = (
         "blob_name",
         "file_path",
         "container_name",
         "bucket_name",
@@ -101,15 +91,14 @@
         "filename",
     )
 
     def execute(self, context: Context) -> str:
         azure_hook = WasbHook(wasb_conn_id=self.wasb_conn_id)
         gcs_hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to,
             impersonation_chain=self.impersonation_chain,
         )
 
         with tempfile.NamedTemporaryFile() as temp_file:
             self.log.info("Downloading data from blob: %s", self.blob_name)
             azure_hook.get_file(
                 file_path=temp_file.name,
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 5.3.1rc2
+Version: 6.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.1rc2``
+Release: ``6.0.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -149,14 +149,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+......
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. warning::
+  In this version of the provider, deprecated GCS hook's param ``delegate_to`` is removed from ``AzureBlobStorageToGCSOperator``.
+  Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
+
+* ``remove delegate_to from GCP operators and hooks (#30748)``
+
+Misc
+~~~~
+
+* ``Merge WasbBlobAsyncSensor to WasbBlobSensor (#30488)``
+
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
@@ -181,14 +198,15 @@
 ~~~~~~~~~
 
 * ``Fix ADF job failure during deferral (#30248)``
 * ``Fix AzureDataLakeStorageV2Hook 'account_url' with Active Directory authentication (#29980) (#29981)``
 
 Misc
 ~~~~
+
 * ``merge AzureDataFactoryPipelineRunStatusAsyncSensor to AzureDataFactoryPipelineRunStatusSensor (#30250)``
 * ``Expose missing params in AzureSynapseHook API docs (#30099)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``organize azure provider.yaml (#30155)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -69,10 +69,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.azure.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.azure
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.1rc2/setup.py` & `apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.3.1"
+version = "6.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
```

