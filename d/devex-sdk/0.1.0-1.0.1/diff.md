# Comparing `tmp/devex_sdk-0.1.0.tar.gz` & `tmp/devex_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devex_sdk-0.1.0.tar", last modified: Fri Apr  7 21:55:18 2023, max compression
+gzip compressed data, was "devex_sdk-1.0.1.tar", last modified: Thu Apr 20 23:07:02 2023, max compression
```

## Comparing `devex_sdk-0.1.0.tar` & `devex_sdk-1.0.1.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.008932 devex_sdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-07 21:55:18.004932 devex_sdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.992931 devex_sdk-0.1.0/devex_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/add.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.992931 devex_sdk-0.1.0/devex_sdk/bucketization/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/bucketization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/bucketization/bucketization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.992931 devex_sdk-0.1.0/devex_sdk/circles/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/circles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/circles/circles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.996932 devex_sdk-0.1.0/devex_sdk/data_ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.996932 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Container.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Node.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Pod.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/eks_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/nested_json_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/pandas_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.000932 devex_sdk-0.1.0/devex_sdk/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/extras/divide.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/extras/multiply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.000932 devex_sdk-0.1.0/devex_sdk/feature_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.000932 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/feature_engine/feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.000932 devex_sdk-0.1.0/devex_sdk/parity/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/parity/number_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.004932 devex_sdk-0.1.0/devex_sdk/project_inital_setup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/project_inital_setup/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/project_inital_setup/console_setup_run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/project_inital_setup/notebook_setup_run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/project_inital_setup/understanding_eks_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.004932 devex_sdk-0.1.0/devex_sdk/update_cwd/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/update_cwd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/devex_sdk/update_cwd/notebook_setup_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:17.992931 devex_sdk-0.1.0/devex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-07 21:55:17.000000 devex_sdk-0.1.0/devex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-07 21:55:17.000000 devex_sdk-0.1.0/devex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:55:17.000000 devex_sdk-0.1.0/devex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 21:55:17.000000 devex_sdk-0.1.0/devex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 21:55:17.000000 devex_sdk-0.1.0/devex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:55:18.008932 devex_sdk-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:55:18.004932 devex_sdk-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_circles.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_divide.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_eks_bucketization.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 21:55:09.000000 devex_sdk-0.1.0/tests/test_update_cwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/bucketization/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/bucketization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/bucketization/bucketization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/circles/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/circles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/circles/circles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/data_ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Container.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Pod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/eks_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/nested_json_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/pandas_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/multiply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/feature_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/parity/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/parity/number_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/project_inital_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/console_setup_run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/notebook_setup_run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/understanding_eks_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/update_cwd/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/update_cwd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/update_cwd/notebook_setup_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-20 23:06:43.000000 devex_sdk-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_circles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_eks_bucketization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_update_cwd.py
```

### Comparing `devex_sdk-0.1.0/LICENSE.txt` & `devex_sdk-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/PKG-INFO` & `devex_sdk-1.0.1/devex_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
-Name: devex_sdk
-Version: 0.1.0
+Name: devex-sdk
+Version: 1.0.1
 Summary: Dish DevEx open source SDK
 Home-page: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DevEx SDK
 
-### __Installing devex_sdk__ shortcut:
+### __Installing devex_sdk__ from PyPi (Latest Release):
+```console
+pip install devex-sdk
+```
+or
 ```console
 pip install git+https://github.com/DISHDevEx/dish-devex-sdk.git
 ```
 
-### __Installing devex_sdk__ versioned:
+### __Installing devex_sdk__ from local build (beta testing):
 1. Navigate into the root _devex_sdk_ directory.
 ```console
 $ cd dish-devex-sdk
 ```
 2. Run the following command to create the wheel file
  
 ```console
@@ -48,14 +52,23 @@
 ```console
 >>> from devex_sdk import *
 >>> multiply(2,3)
 6
 ```
 
 ## __History__
-View verion history and release notes in [HISTORY](HISTORY.md). 
+View version history and release notes in [HISTORY](https://github.com/DISHDevEx/dish-devex-sdk/blob/main/HISTORY.md). 
 
 ## __Contributing__
-Learn how about [CONTRIBUTING](CONTRIBUTING.md) to devex_sdk.
+Learn how about [CONTRIBUTING](https://github.com/DISHDevEx/dish-devex-sdk/blob/main/CONTRIBUTING.md) to devex_sdk.
+
+## __Releases on GitHub__
+View all [DevEx SDK releases](https://github.com/DISHDevEx/dish-devex-sdk/releases) on GitHub.
+
+## __Releases on PyPi__
+View all [DevEx SDK release](https://pypi.org/project/devex-sdk/#history) history on PyPi.
+
 
-## Data Ingestion Framework
-Learn about the components and how to use [Data Ingestion](devex_sdk/data_ingestion/DATA_INGESTION.md)
+## Python Packages in DevEx SDK
+- [Data Ingestion](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/data_ingestion)
+- [Feature Engine](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/feature_engine)
+- [Bucketization](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/bucketization)
```

### Comparing `devex_sdk-0.1.0/README.md` & `devex_sdk-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # DevEx SDK
 
-### __Installing devex_sdk__ shortcut:
+### __Installing devex_sdk__ from PyPi (Latest Release):
+```console
+pip install devex-sdk
+```
+or
 ```console
 pip install git+https://github.com/DISHDevEx/dish-devex-sdk.git
 ```
 
-### __Installing devex_sdk__ versioned:
+### __Installing devex_sdk__ from local build (beta testing):
 1. Navigate into the root _devex_sdk_ directory.
 ```console
 $ cd dish-devex-sdk
 ```
 2. Run the following command to create the wheel file
  
 ```console
@@ -38,14 +42,23 @@
 ```console
 >>> from devex_sdk import *
 >>> multiply(2,3)
 6
 ```
 
 ## __History__
-View verion history and release notes in [HISTORY](HISTORY.md). 
+View version history and release notes in [HISTORY](https://github.com/DISHDevEx/dish-devex-sdk/blob/main/HISTORY.md). 
 
 ## __Contributing__
-Learn how about [CONTRIBUTING](CONTRIBUTING.md) to devex_sdk.
+Learn how about [CONTRIBUTING](https://github.com/DISHDevEx/dish-devex-sdk/blob/main/CONTRIBUTING.md) to devex_sdk.
+
+## __Releases on GitHub__
+View all [DevEx SDK releases](https://github.com/DISHDevEx/dish-devex-sdk/releases) on GitHub.
+
+## __Releases on PyPi__
+View all [DevEx SDK release](https://pypi.org/project/devex-sdk/#history) history on PyPi.
+
 
-## Data Ingestion Framework
-Learn about the components and how to use [Data Ingestion](devex_sdk/data_ingestion/DATA_INGESTION.md)
+## Python Packages in DevEx SDK
+- [Data Ingestion](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/data_ingestion)
+- [Feature Engine](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/feature_engine)
+- [Bucketization](https://github.com/DISHDevEx/dish-devex-sdk/tree/main/devex_sdk/bucketization)
```

### Comparing `devex_sdk-0.1.0/devex_sdk/__init__.py` & `devex_sdk-1.0.1/devex_sdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 from .update_cwd import update_cwd_to_root
 
 from .data_ingestion import EKS_Connector
 from .data_ingestion import Spark_Data_Connector
 from .data_ingestion import Nested_Json_Connector
 from .data_ingestion import Spark_Utils
 from .data_ingestion import eks_performance_logs_schema
+from .data_ingestion import GzConnector
 
 from .project_inital_setup import setup_runner
 
 from .feature_engine import get_features
-
```

### Comparing `devex_sdk-0.1.0/devex_sdk/bucketization/bucketization.py` & `devex_sdk-1.0.1/devex_sdk/bucketization/bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/circles/circles.py` & `devex_sdk-1.0.1/devex_sdk/circles/circles.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Cluster.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Container.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Container.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Node.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Node.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/Pod.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Pod.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/PodNet.json` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/eks_connector.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/eks_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/nested_json_connector.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/nested_json_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/pandas_data_connector.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/pandas_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_config.ini` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_config.ini`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_data_connector.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/data_ingestion/spark_utils.py` & `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_utils.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json` & `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/feature_engine/feature_extractor.py` & `devex_sdk-1.0.1/devex_sdk/feature_engine/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/project_inital_setup/understanding_eks_setup.py` & `devex_sdk-1.0.1/devex_sdk/project_inital_setup/understanding_eks_setup.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk/update_cwd/notebook_setup_path.py` & `devex_sdk-1.0.1/devex_sdk/update_cwd/notebook_setup_path.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/devex_sdk.egg-info/SOURCES.txt` & `devex_sdk-1.0.1/devex_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 devex_sdk.egg-info/top_level.txt
 devex_sdk/bucketization/__init__.py
 devex_sdk/bucketization/bucketization.py
 devex_sdk/circles/__init__.py
 devex_sdk/circles/circles.py
 devex_sdk/data_ingestion/__init__.py
 devex_sdk/data_ingestion/eks_connector.py
+devex_sdk/data_ingestion/gz_connector.py
 devex_sdk/data_ingestion/nested_json_connector.py
 devex_sdk/data_ingestion/pandas_data_connector.py
 devex_sdk/data_ingestion/spark_config.ini
 devex_sdk/data_ingestion/spark_data_connector.py
 devex_sdk/data_ingestion/spark_utils.py
 devex_sdk/data_ingestion/container_insights_schema/Cluster.json
 devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
@@ -58,12 +59,13 @@
 devex_sdk/update_cwd/notebook_setup_path.py
 tests/test_add.py
 tests/test_circles.py
 tests/test_counts.py
 tests/test_dataframe_creation.py
 tests/test_divide.py
 tests/test_eks_bucketization.py
+tests/test_gz_connector.py
 tests/test_multiply.py
 tests/test_parity.py
 tests/test_schema.py
 tests/test_subtract.py
 tests/test_update_cwd.py
```

### Comparing `devex_sdk-0.1.0/setup.py` & `devex_sdk-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,39 +6,45 @@
 
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name = 'devex_sdk',
-    version = '0.1.0',
-    description = 'Dish DevEx open source SDK',
-    url = 'https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk',
-    author_email = 'devex@dish.com',
+    name='devex_sdk',
+    version='v1.0.1',
+    description='Dish DevEx open source SDK',
+    url='https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk',
+    author_email='devex@dish.com',
     license='Dish Wireless',
     packages=find_packages(
         include=['devex_sdk',
                  'devex_sdk.extras',
                  'devex_sdk.circles',
                  'devex_sdk.parity',
                  'devex_sdk.bucketization',
                  'devex_sdk.update_cwd',
                  'devex_sdk.data_ingestion',
                  'devex_sdk.data_ingestion.container_insights_schema',
                  'devex_sdk.project_inital_setup',
                  'devex_sdk.feature_engine.eks_feature_store',
                  'devex_sdk.feature_engine',
-                 ]),
+                 'devex_sdk.data_ingestion.gz_connector',
+                 'devex_sdk.utilities'
+        ]
+    ),
     include_package_data=True,
-    install_requires = [
+    install_requires=[
         'pyspark',
         'pandas',
         'numpy',
         'tqdm',
         'pyspark',
         'configparser',
         'dask',
+        'boto3',
+        'fastparquet',
+        'pyarrow',
         ],
     long_description=long_description,
     long_description_content_type='text/markdown'
     )
```

### Comparing `devex_sdk-0.1.0/tests/test_counts.py` & `devex_sdk-1.0.1/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/tests/test_dataframe_creation.py` & `devex_sdk-1.0.1/tests/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/tests/test_eks_bucketization.py` & `devex_sdk-1.0.1/tests/test_eks_bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-0.1.0/tests/test_schema.py` & `devex_sdk-1.0.1/tests/test_schema.py`

 * *Files identical despite different names*

