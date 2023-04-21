# Comparing `tmp/hsml-3.1.0rc0.tar.gz` & `tmp/hsml-3.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsml-3.1.0rc0.tar", last modified: Wed Dec 21 13:03:55 2022, max compression
+gzip compressed data, was "hsml-3.2.0rc0.tar", last modified: Wed Apr 12 12:47:02 2023, max compression
```

## Comparing `hsml-3.1.0rc0.tar` & `hsml-3.2.0rc0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/
--rw-r--r--   0     1006     1006       40 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     5174 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     3395 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.944972 hsml-3.1.0rc0/hsml/
--rw-r--r--   0     1006     1006     1016 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.944972 hsml-3.1.0rc0/hsml/client/
--rw-r--r--   0     1006     1006     3684 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/__init__.py
--rw-r--r--   0     1006     1006     1876 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/auth.py
--rw-r--r--   0     1006     1006     3946 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/base.py
--rw-r--r--   0     1006     1006     2415 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/client/exceptions.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.944972 hsml-3.1.0rc0/hsml/client/hopsworks/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     3985 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/hopsworks/base.py
--rw-r--r--   0     1006     1006     2846 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/hopsworks/external.py
--rw-r--r--   0     1006     1006     7088 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/hopsworks/internal.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.944972 hsml-3.1.0rc0/hsml/client/istio/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/istio/__init__.py
--rw-r--r--   0     1006     1006     3455 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/istio/base.py
--rw-r--r--   0     1006     1006     1663 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/istio/external.py
--rw-r--r--   0     1006     1006     6650 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/client/istio/internal.py
--rw-r--r--   0     1006     1006    10040 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/connection.py
--rw-r--r--   0     1006     1006     2594 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/constants.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/core/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/__init__.py
--rw-r--r--   0     1006     1006    15187 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/dataset_api.py
--rw-r--r--   0     1006     1006     7327 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/model_api.py
--rw-r--r--   0     1006     1006     2745 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/model_registry_api.py
--rw-r--r--   0     1006     1006     5810 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/model_serving_api.py
--rw-r--r--   0     1006     1006     1188 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/core/native_hdfs_api.py
--rw-r--r--   0     1006     1006    11463 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/core/serving_api.py
--rw-r--r--   0     1006     1006     1656 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/decorators.py
--rw-r--r--   0     1006     1006     2899 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/deployable_component.py
--rw-r--r--   0     1006     1006     2936 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/deployable_component_logs.py
--rw-r--r--   0     1006     1006    12932 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/deployment.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/engine/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/engine/__init__.py
--rw-r--r--   0     1006     1006     1536 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/engine/hopsworks_engine.py
--rw-r--r--   0     1006     1006      934 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/engine/local_engine.py
--rw-r--r--   0     1006     1006    14766 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/engine/model_engine.py
--rw-r--r--   0     1006     1006    19513 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/engine/serving_engine.py
--rw-r--r--   0     1006     1006     4387 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/inference_batcher.py
--rw-r--r--   0     1006     1006     4668 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/inference_endpoint.py
--rw-r--r--   0     1006     1006     4034 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/inference_logger.py
--rw-r--r--   0     1006     1006     4700 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/kafka_topic.py
--rw-r--r--   0     1006     1006    13554 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/model.py
--rw-r--r--   0     1006     1006     6574 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/model_registry.py
--rw-r--r--   0     1006     1006     1861 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/model_schema.py
--rw-r--r--   0     1006     1006     7689 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/model_serving.py
--rw-r--r--   0     1006     1006    14877 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/predictor.py
--rw-r--r--   0     1006     1006     5164 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/predictor_state.py
--rw-r--r--   0     1006     1006     2618 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/predictor_state_condition.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/python/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/python/__init__.py
--rw-r--r--   0     1006     1006     2247 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/python/model.py
--rw-r--r--   0     1006     1006     1151 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/python/predictor.py
--rw-r--r--   0     1006     1006     2414 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/python/signature.py
--rw-r--r--   0     1006     1006    11756 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/resources.py
--rw-r--r--   0     1006     1006     2540 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/schema.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/sklearn/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/sklearn/__init__.py
--rw-r--r--   0     1006     1006     2242 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/sklearn/model.py
--rw-r--r--   0     1006     1006      977 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/sklearn/predictor.py
--rw-r--r--   0     1006     1006     2409 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/sklearn/signature.py
--rw-r--r--   0     1006     1006     1937 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/tag.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/tensorflow/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/tensorflow/__init__.py
--rw-r--r--   0     1006     1006     2247 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/tensorflow/model.py
--rw-r--r--   0     1006     1006     1169 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/tensorflow/predictor.py
--rw-r--r--   0     1006     1006     2414 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/tensorflow/signature.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/torch/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/torch/__init__.py
--rw-r--r--   0     1006     1006     2237 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/torch/model.py
--rw-r--r--   0     1006     1006     1142 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/torch/predictor.py
--rw-r--r--   0     1006     1006     2404 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/torch/signature.py
--rw-r--r--   0     1006     1006     2968 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/transformer.py
--rw-r--r--   0     1006     1006     9632 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/util.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/utils/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/__init__.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.948972 hsml-3.1.0rc0/hsml/utils/schema/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/schema/__init__.py
--rw-r--r--   0     1006     1006      936 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/schema/column.py
--rw-r--r--   0     1006     1006     3570 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/schema/columnar_schema.py
--rw-r--r--   0     1006     1006      976 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/schema/tensor.py
--rw-r--r--   0     1006     1006     2396 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/hsml/utils/schema/tensor_schema.py
--rw-r--r--   0     1006     1006      631 2022-12-21 13:03:50.000000 hsml-3.1.0rc0/hsml/version.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.944972 hsml-3.1.0rc0/hsml.egg-info/
--rw-r--r--   0     1006     1006     5174 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/hsml.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2009 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/hsml.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/hsml.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      306 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/hsml.egg-info/requires.txt
--rw-r--r--   0     1006     1006       11 2022-12-21 13:03:55.000000 hsml-3.1.0rc0/hsml.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     2478 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/setup.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/tests/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/tests/hsml/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/tests/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2022-12-21 13:03:55.952972 hsml-3.1.0rc0/tests/hsml/core/
--rw-r--r--   0     1006     1006      605 2022-12-20 18:08:49.000000 hsml-3.1.0rc0/tests/hsml/core/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/
+-rw-r--r--   0     1006     1006       40 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     5178 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     3399 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/
+-rw-r--r--   0     1006     1006     1016 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/
+-rw-r--r--   0     1006     1006     3684 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/__init__.py
+-rw-r--r--   0     1006     1006     1876 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/auth.py
+-rw-r--r--   0     1006     1006     3946 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/base.py
+-rw-r--r--   0     1006     1006     2456 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/exceptions.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/hopsworks/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     3985 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/base.py
+-rw-r--r--   0     1006     1006     2846 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/external.py
+-rw-r--r--   0     1006     1006     7088 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/internal.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/istio/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/__init__.py
+-rw-r--r--   0     1006     1006     3455 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/base.py
+-rw-r--r--   0     1006     1006     1663 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/external.py
+-rw-r--r--   0     1006     1006     6650 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/internal.py
+-rw-r--r--   0     1006     1006    10216 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/connection.py
+-rw-r--r--   0     1006     1006     2594 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/constants.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/__init__.py
+-rw-r--r--   0     1006     1006    15187 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7327 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_api.py
+-rw-r--r--   0     1006     1006     2745 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_registry_api.py
+-rw-r--r--   0     1006     1006     5810 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_serving_api.py
+-rw-r--r--   0     1006     1006     1188 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/native_hdfs_api.py
+-rw-r--r--   0     1006     1006    11463 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/serving_api.py
+-rw-r--r--   0     1006     1006     1656 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/decorators.py
+-rw-r--r--   0     1006     1006     2899 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployable_component.py
+-rw-r--r--   0     1006     1006     2936 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployable_component_logs.py
+-rw-r--r--   0     1006     1006    13979 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployment.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/engine/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/__init__.py
+-rw-r--r--   0     1006     1006     1536 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/hopsworks_engine.py
+-rw-r--r--   0     1006     1006      934 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/local_engine.py
+-rw-r--r--   0     1006     1006    14766 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/model_engine.py
+-rw-r--r--   0     1006     1006    22555 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/serving_engine.py
+-rw-r--r--   0     1006     1006     4387 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_batcher.py
+-rw-r--r--   0     1006     1006     4668 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_endpoint.py
+-rw-r--r--   0     1006     1006     4034 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_logger.py
+-rw-r--r--   0     1006     1006     4700 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/kafka_topic.py
+-rw-r--r--   0     1006     1006    14300 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model.py
+-rw-r--r--   0     1006     1006     6574 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_registry.py
+-rw-r--r--   0     1006     1006     1861 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_schema.py
+-rw-r--r--   0     1006     1006    12706 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_serving.py
+-rw-r--r--   0     1006     1006    15504 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor.py
+-rw-r--r--   0     1006     1006     5164 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor_state.py
+-rw-r--r--   0     1006     1006     2618 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor_state_condition.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/python/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/model.py
+-rw-r--r--   0     1006     1006     1151 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/signature.py
+-rw-r--r--   0     1006     1006    11756 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/resources.py
+-rw-r--r--   0     1006     1006     2540 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/schema.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/sklearn/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/__init__.py
+-rw-r--r--   0     1006     1006     2218 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/model.py
+-rw-r--r--   0     1006     1006      977 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/predictor.py
+-rw-r--r--   0     1006     1006     2510 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/signature.py
+-rw-r--r--   0     1006     1006     1937 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tag.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/tensorflow/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/model.py
+-rw-r--r--   0     1006     1006     1169 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/signature.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/torch/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/__init__.py
+-rw-r--r--   0     1006     1006     2213 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/model.py
+-rw-r--r--   0     1006     1006     1142 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/predictor.py
+-rw-r--r--   0     1006     1006     2505 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/signature.py
+-rw-r--r--   0     1006     1006     2968 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/transformer.py
+-rw-r--r--   0     1006     1006     9842 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/util.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/utils/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/utils/schema/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/__init__.py
+-rw-r--r--   0     1006     1006      936 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/column.py
+-rw-r--r--   0     1006     1006     3570 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/columnar_schema.py
+-rw-r--r--   0     1006     1006      976 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/tensor.py
+-rw-r--r--   0     1006     1006     2396 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/tensor_schema.py
+-rw-r--r--   0     1006     1006      631 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/version.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml.egg-info/
+-rw-r--r--   0     1006     1006     5178 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2009 2023-04-12 12:47:02.000000 hsml-3.2.0rc0/hsml.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      306 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       11 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     2478 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/hsml/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/hsml/core/__init__.py
```

### Comparing `hsml-3.1.0rc0/PKG-INFO` & `hsml-3.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.1.0rc0
+Version: 3.2.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.1.0rc0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
@@ -96,15 +96,15 @@
         Start a deployment
         ```python
         deployment.start()
         ```
         
         Make predictions with a deployed model
         ```python
-        data = { "instances": model.input_example }
+        data = { "instances": [ model.input_example ] }
         
         predictions = deployment.predict(data)
         ```
         
         You can find more examples on how to use the library in [examples.hopsworks.ai](https://examples.hopsworks.ai).
         
         ## Documentation
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.1.0rc0 Summary: HSML: An
+Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc0 Summary: HSML: An
 environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api Author:
 Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
 2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
-releases/tag/3.1.0rc0 Description: # Hopsworks Model Management
+releases/tag/3.2.0rc0 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
@@ -21,23 +21,24 @@
 metrics={"accuracy": 0.94}, description="mnist model description") model.save
 ("/tmp/model_directory") # or /tmp/model_file ``` Download a model ```python
 model = mr.get_model("mnist", version=1) model_path = model.download() ```
 Delete a model ```python model.delete() ``` Get best performing model ```python
 best_model = mr.get_best_model('mnist', 'accuracy', 'max') ``` Deploy a model
 ```python deployment = model.deploy() ``` Start a deployment ```python
 deployment.start() ``` Make predictions with a deployed model ```python data =
-{ "instances": model.input_example } predictions = deployment.predict(data) ```
-You can find more examples on how to use the library in [examples.hopsworks.ai]
-(https://examples.hopsworks.ai). ## Documentation Documentation is available at
-[Hopsworks Model Management Documentation](https://docs.hopsworks.ai/). ##
-Issues For general questions about the usage of Hopsworks Machine Learning
-please open a topic on [Hopsworks Community](https://community.hopsworks.ai/).
-Please report any issue using [Github issue tracking](https://github.com/
-logicalclocks/machine-learning-api/issues). ## Contributing If you would like
-to contribute to this library, please see the [Contribution Guidelines]
-(CONTRIBUTING.md). Keywords: Hopsworks,ML,Models,Machine Learning Models,Model
+{ "instances": [ model.input_example ] } predictions = deployment.predict(data)
+``` You can find more examples on how to use the library in
+[examples.hopsworks.ai](https://examples.hopsworks.ai). ## Documentation
+Documentation is available at [Hopsworks Model Management Documentation](https:
+//docs.hopsworks.ai/). ## Issues For general questions about the usage of
+Hopsworks Machine Learning please open a topic on [Hopsworks Community](https:/
+/community.hopsworks.ai/). Please report any issue using [Github issue
+tracking](https://github.com/logicalclocks/machine-learning-api/issues). ##
+Contributing If you would like to contribute to this library, please see the
+[Contribution Guidelines](CONTRIBUTING.md). Keywords:
+Hopsworks,ML,Models,Machine Learning Models,Model
 Registry,TensorFlow,PyTorch,Machine Learning,MLOps,DataOps Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Utilities Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Description-Content-Type: text/markdown Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `hsml-3.1.0rc0/README.md` & `hsml-3.2.0rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 Start a deployment
 ```python
 deployment.start()
 ```
 
 Make predictions with a deployed model
 ```python
-data = { "instances": model.input_example }
+data = { "instances": [ model.input_example ] }
 
 predictions = deployment.predict(data)
 ```
 
 You can find more examples on how to use the library in [examples.hopsworks.ai](https://examples.hopsworks.ai).
 
 ## Documentation
```

#### html2text {}

```diff
@@ -16,17 +16,17 @@
 metrics={"accuracy": 0.94}, description="mnist model description") model.save
 ("/tmp/model_directory") # or /tmp/model_file ``` Download a model ```python
 model = mr.get_model("mnist", version=1) model_path = model.download() ```
 Delete a model ```python model.delete() ``` Get best performing model ```python
 best_model = mr.get_best_model('mnist', 'accuracy', 'max') ``` Deploy a model
 ```python deployment = model.deploy() ``` Start a deployment ```python
 deployment.start() ``` Make predictions with a deployed model ```python data =
-{ "instances": model.input_example } predictions = deployment.predict(data) ```
-You can find more examples on how to use the library in [examples.hopsworks.ai]
-(https://examples.hopsworks.ai). ## Documentation Documentation is available at
-[Hopsworks Model Management Documentation](https://docs.hopsworks.ai/). ##
-Issues For general questions about the usage of Hopsworks Machine Learning
-please open a topic on [Hopsworks Community](https://community.hopsworks.ai/).
-Please report any issue using [Github issue tracking](https://github.com/
-logicalclocks/machine-learning-api/issues). ## Contributing If you would like
-to contribute to this library, please see the [Contribution Guidelines]
-(CONTRIBUTING.md).
+{ "instances": [ model.input_example ] } predictions = deployment.predict(data)
+``` You can find more examples on how to use the library in
+[examples.hopsworks.ai](https://examples.hopsworks.ai). ## Documentation
+Documentation is available at [Hopsworks Model Management Documentation](https:
+//docs.hopsworks.ai/). ## Issues For general questions about the usage of
+Hopsworks Machine Learning please open a topic on [Hopsworks Community](https:/
+/community.hopsworks.ai/). Please report any issue using [Github issue
+tracking](https://github.com/logicalclocks/machine-learning-api/issues). ##
+Contributing If you would like to contribute to this library, please see the
+[Contribution Guidelines](CONTRIBUTING.md).
```

### Comparing `hsml-3.1.0rc0/hsml/__init__.py` & `hsml-3.2.0rc0/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/__init__.py` & `hsml-3.2.0rc0/hsml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/auth.py` & `hsml-3.2.0rc0/hsml/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/base.py` & `hsml-3.2.0rc0/hsml/client/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/exceptions.py` & `hsml-3.2.0rc0/hsml/client/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 
 class ModelServingException(Exception):
     """Generic model serving exception"""
 
     ERROR_CODE_SERVING_NOT_FOUND = 240000
     ERROR_CODE_ILLEGAL_ARGUMENT = 240001
+    ERROR_CODE_DUPLICATED_ENTRY = 240011
 
     ERROR_CODE_DEPLOYMENT_NOT_RUNNING = 250001
 
 
 class ExternalClientError(TypeError):
     """Raised when external client cannot be initialized due to missing arguments."""
```

### Comparing `hsml-3.1.0rc0/hsml/client/hopsworks/__init__.py` & `hsml-3.2.0rc0/hsml/client/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/hopsworks/base.py` & `hsml-3.2.0rc0/hsml/client/hopsworks/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/hopsworks/external.py` & `hsml-3.2.0rc0/hsml/client/hopsworks/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/hopsworks/internal.py` & `hsml-3.2.0rc0/hsml/client/hopsworks/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/istio/__init__.py` & `hsml-3.2.0rc0/hsml/client/istio/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/istio/base.py` & `hsml-3.2.0rc0/hsml/client/istio/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/istio/external.py` & `hsml-3.2.0rc0/hsml/client/istio/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/client/istio/internal.py` & `hsml-3.2.0rc0/hsml/client/istio/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/connection.py` & `hsml-3.2.0rc0/hsml/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,24 @@
         """
         return self._model_registry_api.get(project)
 
     @connected
     def get_model_serving(self):
         """Get a reference to model serving to perform operations on. Model serving operates on top of a model registry, defaulting to the project's default model registry.
 
+        !!! example
+            ```python
+
+            import hopsworks
+
+            project = hopsworks.login()
+
+            ms = project.get_model_serving()
+            ```
+
         # Returns
             `ModelServing`. A model serving handle object to perform operations on.
         """
         return self._model_serving_api.get()
 
     @not_connected
     def connect(self):
```

### Comparing `hsml-3.1.0rc0/hsml/constants.py` & `hsml-3.2.0rc0/hsml/constants.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/__init__.py` & `hsml-3.2.0rc0/hsml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/dataset_api.py` & `hsml-3.2.0rc0/hsml/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/model_api.py` & `hsml-3.2.0rc0/hsml/core/model_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/model_registry_api.py` & `hsml-3.2.0rc0/hsml/core/model_registry_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/model_serving_api.py` & `hsml-3.2.0rc0/hsml/core/model_serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/native_hdfs_api.py` & `hsml-3.2.0rc0/hsml/core/native_hdfs_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/core/serving_api.py` & `hsml-3.2.0rc0/hsml/core/serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/decorators.py` & `hsml-3.2.0rc0/hsml/decorators.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/deployable_component.py` & `hsml-3.2.0rc0/hsml/deployable_component.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/deployable_component_logs.py` & `hsml-3.2.0rc0/hsml/deployable_component_logs.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/deployment.py` & `hsml-3.2.0rc0/hsml/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,25 @@
 class Deployment:
     """Metadata object representing a deployment in Model Serving."""
 
     def __init__(
         self, predictor, name: Optional[str] = None, description: Optional[str] = None
     ):
         self._predictor = predictor
-        self._name = name
         self._description = description
 
         if self._predictor is None:
             raise ModelServingException("A predictor is required")
         elif not isinstance(self._predictor, predictor_mod.Predictor):
             raise ValueError(
                 "The predictor provided is not an instance of the Predictor class"
             )
 
-        if self._name is None:
-            self._name = self._predictor.name
-        else:
-            self._name = self._predictor.name = name
+        if name is not None:
+            self._predictor.name = name
 
         if self._description is None:
             self._description = self._predictor.description
         else:
             self._description = self._predictor.description = description
 
         self._serving_api = serving_api.ServingApi()
@@ -142,25 +139,49 @@
         """
 
         status = self._serving_engine.get_state(self).status
         return status == PREDICTOR_STATE.STATUS_STOPPED or (
             or_created and status == PREDICTOR_STATE.STATUS_CREATED
         )
 
-    def predict(self, data: dict):
-        """Send inference requests to the deployment
+    def predict(self, data: dict = None, inputs: list = None):
+        """Send inference requests to the deployment.
+           One of data or inputs parameters must be set. If both are set, inputs will be ignored.
+
+        !!! example
+            ```python
+            # login into Hopsworks using hopsworks.login()
+
+            # get Hopsworks Model Serving handle
+            ms = project.get_model_serving()
+
+            # retrieve deployment by name
+            my_deployment = ms.get_deployment("my_deployment")
+
+            # (optional) retrieve model input example
+            my_model = project.get_model_registry()  \
+                              .get_model(my_deployment.model_name, my_deployment.model_version)
+
+            # make predictions using model inputs (single or batch)
+            predictions = my_deployment.predict(inputs=my_model.input_example)
+
+            # or using more sophisticated inference request payloads
+            data = { "instances": [ my_model.input_example ], "key2": "value2" }
+            predictions = my_deployment.predict(data)
+            ```
 
         # Arguments
-            data: Payload of the inference request.
+            data: Payload dictionary for the inference request including the model input(s)
+            inputs: Model inputs used in the inference requests
 
         # Returns
             `dict`. Inference response.
         """
 
-        return self._serving_engine.predict(self, data)
+        return self._serving_engine.predict(self, data, inputs)
 
     def download_artifact(self):
         """Download the model artifact served by the deployment"""
 
         return self._serving_engine.download_artifact(self)
 
     def get_logs(self, component="predictor", tail=10):
@@ -242,19 +263,19 @@
     def id(self):
         """Id of the deployment."""
         return self._predictor.id
 
     @property
     def name(self):
         """Name of the deployment."""
-        return self._name
+        return self._predictor.name
 
     @name.setter
     def name(self, name: str):
-        self._name = name
+        self._predictor.name = name
 
     @property
     def description(self):
         """Description of the deployment."""
         return self._description
 
     @description.setter
@@ -393,8 +414,8 @@
 
     def __repr__(self):
         desc = (
             f", description: {self._description!r}"
             if self._description is not None
             else ""
         )
-        return f"Deployment(name: {self._name!r}" + desc + ")"
+        return f"Deployment(name: {self._predictor._name!r}" + desc + ")"
```

### Comparing `hsml-3.1.0rc0/hsml/engine/__init__.py` & `hsml-3.2.0rc0/hsml/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/engine/hopsworks_engine.py` & `hsml-3.2.0rc0/hsml/engine/hopsworks_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/engine/local_engine.py` & `hsml-3.2.0rc0/hsml/engine/local_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/engine/model_engine.py` & `hsml-3.2.0rc0/hsml/engine/model_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,31 +208,29 @@
             model_query_params["jobName"] = os.environ["HOPSWORKS_JOB_NAME"]
         elif "HOPSWORKS_KERNEL_ID" in os.environ:
             model_query_params["kernelId"] = os.environ["HOPSWORKS_KERNEL_ID"]
 
         pbar = tqdm(
             [
                 {"id": 0, "desc": "Creating model folder"},
-                {"id": 1, "desc": "Uploading input_example and model_schema"},
-                {"id": 2, "desc": "Uploading model files"},
+                {"id": 1, "desc": "Uploading model files"},
+                {"id": 2, "desc": "Uploading input_example and model_schema"},
                 {"id": 3, "desc": "Registering model"},
                 {"id": 4, "desc": "Waiting for model registration"},
                 {"id": 5, "desc": "Model export complete"},
             ]
         )
 
         for step in pbar:
             try:
                 pbar.set_description("%s" % step["desc"])
                 if step["id"] == 0:
                     # Create folders
                     self._engine.mkdir(model_instance)
                 if step["id"] == 1:
-                    model_instance = self._upload_additional_resources(model_instance)
-                if step["id"] == 2:
                     # Upload Model files from local path to /Models/{model_instance._name}/{model_instance._version}
                     # check local absolute
                     if os.path.isabs(model_path) and os.path.exists(model_path):
                         self._upload_local_model(
                             model_path,
                             model_instance.version,
                             dataset_model_name_path,
@@ -253,14 +251,16 @@
                         self._copy_hopsfs_model(model_path, model_instance.version_path)
                     else:
                         raise IOError(
                             "Could not find path {} in the local filesystem or in Hopsworks File System".format(
                                 model_path
                             )
                         )
+                if step["id"] == 2:
+                    model_instance = self._upload_additional_resources(model_instance)
                 if step["id"] == 3:
                     model_instance = self._model_api.put(
                         model_instance, model_query_params
                     )
                 if step["id"] == 4:
                     model_instance = self._poll_model_available(
                         model_instance, await_registration
```

### Comparing `hsml-3.1.0rc0/hsml/engine/serving_engine.py` & `hsml-3.2.0rc0/hsml/engine/serving_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
+import os
 import time
 import uuid
-import os
 
 from tqdm.auto import tqdm
 
 from hsml import util
 
 from hsml.constants import DEPLOYMENT, PREDICTOR, PREDICTOR_STATE
 from hsml.core import serving_api, dataset_api
@@ -162,22 +162,24 @@
             _ = self._poll_deployment_status(  # wait for status
                 deployment_instance,
                 PREDICTOR_STATE.STATUS_STOPPED,
                 await_status,
                 update_progress,
             )
 
-    def predict(self, deployment_instance, data: dict):
+    def predict(self, deployment_instance, data, inputs):
+        payload = self._build_inference_payload(data, inputs)
+
         serving_tool = deployment_instance.predictor.serving_tool
         through_hopsworks = (
             serving_tool != PREDICTOR.SERVING_TOOL_KSERVE
         )  # if not KServe, send request to Hopsworks
         try:
             return self._serving_api.send_inference_request(
-                deployment_instance, data, through_hopsworks
+                deployment_instance, payload, through_hopsworks
             )
         except RestAPIError as re:
             if (
                 re.response.status_code == RestAPIError.STATUS_CODE_NOT_FOUND
                 or re.error_code
                 == ModelServingException.ERROR_CODE_DEPLOYMENT_NOT_RUNNING
             ):
@@ -186,14 +188,41 @@
                 )
 
             re.args = (
                 re.args[0] + "\n\n Check the model server logs by using `.get_logs()`",
             )
             raise re
 
+    def _build_inference_payload(self, data, inputs):
+        """Build or check the payload for an inference request. If the 'data' parameter is provided, this method ensures
+        it contains one of 'instances' or 'inputs' keys needed by the model server. Otherwise, if the 'inputs' parameter
+        is provided, this method builds the correct request payload using the 'instances' key.
+        While the 'inputs' key is only supported by default deployments, the 'instances' key is supported in all types of deployments.
+        """
+        if data is not None:  # check data
+            if not isinstance(data, dict):
+                raise ModelServingException(
+                    "Inference data must be a dictionary. Otherwise, use the inputs parameter."
+                )
+            if "instances" not in data and "inputs" not in data:
+                raise ModelServingException("Inference data is missing 'instances' key")
+        else:  # parse inputs
+            if not isinstance(inputs, list):
+                data = {"instances": [inputs]}  # wrap inputs in a list
+            else:
+                data = {"instances": inputs}  # use given inputs list by default
+                # check depth of the list: at least two levels are required for batch inference
+                # if the content is neither a list or dict, wrap it in an additional list
+                for i in inputs:
+                    if not isinstance(i, list) and not isinstance(i, dict):
+                        # if there are no two levels, wrap inputs in a list
+                        data = {"instances": [inputs]}
+                        break
+        return data
+
     def _check_status(self, deployment_instance, desired_status):
         state = deployment_instance.get_state()
         if state is None:
             return (True, None)
 
         # desired status: running
         if desired_status == PREDICTOR_STATE.STATUS_RUNNING:
@@ -353,23 +382,41 @@
             raise be
         finally:
             if os.path.exists(to_artifact_zip_path):
                 os.remove(to_artifact_zip_path)
 
         return to_artifact_version_path
 
-    def save(self, deployment_instance, await_update: int):
-        if deployment_instance.id is None:
-            # if new deployment
+    def create(self, deployment_instance):
+        try:
             self._serving_api.put(deployment_instance)
             print("Deployment created, explore it at " + deployment_instance.get_url())
+        except RestAPIError as re:
+            if re.error_code == ModelServingException.ERROR_CODE_DUPLICATED_ENTRY:
+                msg = "Deployment with the same name already exists"
+                existing_deployment = self._serving_api.get(deployment_instance.name)
+                if (
+                    existing_deployment.model_name == deployment_instance.model_name
+                    and existing_deployment.model_version
+                    == deployment_instance.model_version
+                ):  # if same name and model version, retrieve existing deployment
+                    print(msg + ". Getting existing deployment...")
+                    print("To create a new deployment choose a different name.")
+                    deployment_instance.update_from_response_json(
+                        existing_deployment.to_dict()
+                    )
+                else:  # otherwise, raise an exception
+                    print(", but it is serving a different model version.")
+                    print("Please, choose a different name.")
+                    raise re
+
+        if deployment_instance.is_stopped():
             print("Before making predictions, start the deployment by using `.start()`")
-            return
 
-        # if existing deployment
+    def update(self, deployment_instance, await_update):
         state = deployment_instance.get_state()
         if state is None:
             return
 
         if state.status == PREDICTOR_STATE.STATUS_STARTING:
             # if starting, it cannot be updated yet
             raise ModelServingException(
@@ -393,32 +440,39 @@
             return
         if state.status == PREDICTOR_STATE.STATUS_UPDATING:
             # if updating, it cannot be updated yet
             raise ModelServingException(
                 "Deployment is updating, please wait until it is running before applying changes. \n"
                 + "Check the current status by using `.get_state()` or explore the server logs using `.get_logs()`"
             )
-            return
         if state.status == PREDICTOR_STATE.STATUS_STOPPING:
             # if stopping, it cannot be updated yet
             raise ModelServingException(
                 "Deployment is stopping, please wait until it is stopped before applying changes"
             )
-            return
         if (
             state.status == PREDICTOR_STATE.STATUS_CREATED
             or state.status == PREDICTOR_STATE.STATUS_STOPPED
         ):
             # if stopped, it's fine
             self._serving_api.put(deployment_instance)
             print("Deployment updated, explore it at " + deployment_instance.get_url())
             return
 
         raise ValueError("Unknown deployment status: " + state.status)
 
+    def save(self, deployment_instance, await_update: int):
+        if deployment_instance.id is None:
+            # if new deployment
+            self.create(deployment_instance)
+            return
+
+        # if existing deployment
+        self.update(deployment_instance, await_update)
+
     def delete(self, deployment_instance, force=False):
         state = deployment_instance.get_state()
         if state is None:
             return
 
         if not force and state.status != PREDICTOR_STATE.STATUS_STOPPED:
             raise ModelServingException(
```

### Comparing `hsml-3.1.0rc0/hsml/inference_batcher.py` & `hsml-3.2.0rc0/hsml/inference_batcher.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/inference_endpoint.py` & `hsml-3.2.0rc0/hsml/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/inference_logger.py` & `hsml-3.2.0rc0/hsml/inference_logger.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/kafka_topic.py` & `hsml-3.2.0rc0/hsml/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/model.py` & `hsml-3.2.0rc0/hsml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         program=None,
         user_full_name=None,
         model_schema=None,
         training_dataset=None,
         input_example=None,
         framework=None,
         model_registry_id=None,
-        tags=None,
     ):
         self._id = id
         self._name = name
         self._version = version
 
         if description is None:
             self._description = "A collection of models for " + name
@@ -80,15 +79,23 @@
             self._shared_registry_project_name = None
 
         self._model_registry_id = model_registry_id
 
         self._model_engine = model_engine.ModelEngine()
 
     def save(self, model_path, await_registration=480):
-        """Persist this model including model files and metadata to the model registry."""
+        """Persist this model including model files and metadata to the model registry.
+
+        # Arguments
+            model_path: Local or remote (Hopsworks file system) path to the folder where the model files are located, or path to a specific model file.
+            await_registration: Awaiting time for the model to be registered in Hopsworks.
+
+        # Returns
+            `Model`. The model metadata object.
+        """
         return self._model_engine.save(
             self, model_path, await_registration=await_registration
         )
 
     def download(self):
         """Download the model files to a local folder."""
         return self._model_engine.download(self)
@@ -115,28 +122,43 @@
         resources: Optional[Union[PredictorResources, dict]] = None,
         inference_logger: Optional[Union[InferenceLogger, dict]] = None,
         inference_batcher: Optional[Union[InferenceBatcher, dict]] = None,
         transformer: Optional[Union[Transformer, dict]] = None,
     ):
         """Deploy the model.
 
+        !!! example
+            ```python
+
+            import hopsworks
+
+            project = hopsworks.login()
+
+            # get Hopsworks Model Registry handle
+            mr = project.get_model_registry()
+
+            # retrieve the trained model you want to deploy
+            my_model = mr.get_model("my_model", version=1)
+
+            my_deployment = my_model.deploy()
+            ```
         # Arguments
             name: Name of the deployment.
             description: Description of the deployment.
             artifact_version: Version number of the model artifact to deploy, `CREATE` to create a new model artifact
             or `MODEL-ONLY` to reuse the shared artifact containing only the model files.
             serving_tool: Serving tool used to deploy the model server.
             script_file: Path to a custom predictor script implementing the Predict class.
             resources: Resources to be allocated for the predictor.
             inference_logger: Inference logger configuration.
             inference_batcher: Inference batcher configuration.
             transformer: Transformer to be deployed together with the predictor.
 
         # Returns
-            `Deployment`. The deployment metadata object.
+            `Deployment`. The deployment metadata object of a new or existing deployment.
         """
 
         if name is None:
             name = self._name
 
         predictor = Predictor.for_model(
             self,
```

### Comparing `hsml-3.1.0rc0/hsml/model_registry.py` & `hsml-3.2.0rc0/hsml/model_registry.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/model_schema.py` & `hsml-3.2.0rc0/hsml/model_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/predictor.py` & `hsml-3.2.0rc0/hsml/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,16 +85,38 @@
         )
         self._transformer = util.get_obj_from_json(transformer, Transformer)
         self._validate_script_file(self._model_framework, self._script_file)
 
     def deploy(self):
         """Create a deployment for this predictor and persists it in the Model Serving.
 
+        !!! example
+            ```python
+
+            import hopsworks
+
+            project = hopsworks.login()
+
+            # get Hopsworks Model Registry handle
+            mr = project.get_model_registry()
+
+            # retrieve the trained model you want to deploy
+            my_model = mr.get_model("my_model", version=1)
+
+            # get Hopsworks Model Serving handle
+            ms = project.get_model_serving()
+
+            my_predictor = ms.create_predictor(my_model)
+            my_deployment = my_predictor.deploy()
+
+            print(my_deployment.get_state())
+            ```
+
         # Returns
-            `Deployment`. The deployment metadata object.
+            `Deployment`. The deployment metadata object of a new or existing deployment.
         """
 
         _deployment = deployment.Deployment(
             predictor=self, name=self._name, description=self._description
         )
         _deployment.save()
 
@@ -102,15 +124,14 @@
 
     def describe(self):
         """Print a description of the predictor"""
         util.pretty_print(self)
 
     def _set_state(self, state: PredictorState):
         """Set the state of the predictor"""
-
         self._state = state
 
     @classmethod
     def _validate_serving_tool(cls, serving_tool):
         if serving_tool is not None:
             if client.is_saas_connection():
                 # only kserve supported in saasy hopsworks
```

### Comparing `hsml-3.1.0rc0/hsml/predictor_state.py` & `hsml-3.2.0rc0/hsml/predictor_state.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/predictor_state_condition.py` & `hsml-3.2.0rc0/hsml/predictor_state_condition.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/python/__init__.py` & `hsml-3.2.0rc0/hsml/python/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/python/model.py` & `hsml-3.2.0rc0/hsml/sklearn/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from hsml.model import Model
 from hsml.constants import MODEL
 import humps
 
 
 class Model(Model):
-    """Metadata object representing a generic python model in the Model Registry."""
+    """Metadata object representing an sklearn model in the Model Registry."""
 
     def __init__(
         self,
         id,
         name,
         version=None,
         created=None,
@@ -35,17 +35,15 @@
         experiment_project_name=None,
         metrics=None,
         program=None,
         user_full_name=None,
         model_schema=None,
         training_dataset=None,
         input_example=None,
-        framework=None,
         model_registry_id=None,
-        tags=None,
     ):
         super().__init__(
             id,
             name,
             version=version,
             created=created,
             environment=environment,
@@ -55,18 +53,18 @@
             experiment_project_name=experiment_project_name,
             metrics=metrics,
             program=program,
             user_full_name=user_full_name,
             model_schema=model_schema,
             training_dataset=training_dataset,
             input_example=input_example,
-            framework=MODEL.FRAMEWORK_PYTHON,
+            framework=MODEL.FRAMEWORK_SKLEARN,
             model_registry_id=model_registry_id,
-            tags=tags,
         )
 
     def update_from_response_json(self, json_dict):
         json_decamelized = humps.decamelize(json_dict)
+        json_decamelized.pop("framework")
         if "type" in json_decamelized:  # backwards compatibility
             _ = json_decamelized.pop("type")
         self.__init__(**json_decamelized)
         return self
```

### Comparing `hsml-3.1.0rc0/hsml/python/predictor.py` & `hsml-3.2.0rc0/hsml/python/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/python/signature.py` & `hsml-3.2.0rc0/hsml/python/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         local file path to the directory containing the model artifacts.
 
     # Arguments
         name: Name of the model to create.
         version: Optionally version of the model to create, defaults to `None` and
             will create the model with incremented version from the last
             version in the model registry.
+        metrics: Optionally a dictionary with model evaluation metrics (e.g., accuracy, MAE)
         description: Optionally a string describing the model, defaults to empty string
             `""`.
-        input_example: Optionally an input example that represents inputs for the model, defaults to `None`.
+        input_example: Optionally an input example that represents a single input for the model, defaults to `None`.
         model_schema: Optionally a model schema for the model inputs and/or outputs.
 
     # Returns
         `Model`. The model metadata object.
     """
     model = Model(
         id=None,
```

### Comparing `hsml-3.1.0rc0/hsml/resources.py` & `hsml-3.2.0rc0/hsml/resources.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/schema.py` & `hsml-3.2.0rc0/hsml/schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/sklearn/__init__.py` & `hsml-3.2.0rc0/hsml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/sklearn/model.py` & `hsml-3.2.0rc0/hsml/tensorflow/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from hsml.model import Model
 from hsml.constants import MODEL
 import humps
 
 
 class Model(Model):
-    """Metadata object representing an sklearn model in the Model Registry."""
+    """Metadata object representing a tensorflow model in the Model Registry."""
 
     def __init__(
         self,
         id,
         name,
         version=None,
         created=None,
@@ -35,17 +35,15 @@
         experiment_project_name=None,
         metrics=None,
         program=None,
         user_full_name=None,
         model_schema=None,
         training_dataset=None,
         input_example=None,
-        framework=None,
         model_registry_id=None,
-        tags=None,
     ):
         super().__init__(
             id,
             name,
             version=version,
             created=created,
             environment=environment,
@@ -55,18 +53,18 @@
             experiment_project_name=experiment_project_name,
             metrics=metrics,
             program=program,
             user_full_name=user_full_name,
             model_schema=model_schema,
             training_dataset=training_dataset,
             input_example=input_example,
-            framework=MODEL.FRAMEWORK_SKLEARN,
+            framework=MODEL.FRAMEWORK_TENSORFLOW,
             model_registry_id=model_registry_id,
-            tags=tags,
         )
 
     def update_from_response_json(self, json_dict):
         json_decamelized = humps.decamelize(json_dict)
+        json_decamelized.pop("framework")
         if "type" in json_decamelized:  # backwards compatibility
             _ = json_decamelized.pop("type")
         self.__init__(**json_decamelized)
         return self
```

### Comparing `hsml-3.1.0rc0/hsml/sklearn/predictor.py` & `hsml-3.2.0rc0/hsml/sklearn/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/sklearn/signature.py` & `hsml-3.2.0rc0/hsml/sklearn/signature.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         local file path to the directory containing the model artifacts.
 
     # Arguments
         name: Name of the model to create.
         version: Optionally version of the model to create, defaults to `None` and
             will create the model with incremented version from the last
             version in the model registry.
+        metrics: Optionally a dictionary with model evaluation metrics (e.g., accuracy, MAE)
         description: Optionally a string describing the model, defaults to empty string
             `""`.
-        input_example: Optionally an input example that represents inputs for the model, defaults to `None`.
+        input_example: Optionally an input example that represents a single input for the model, defaults to `None`.
         model_schema: Optionally a model schema for the model inputs and/or outputs.
 
     # Returns
         `Model`. The model metadata object.
     """
     model = Model(
         id=None,
```

### Comparing `hsml-3.1.0rc0/hsml/tag.py` & `hsml-3.2.0rc0/hsml/tag.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/tensorflow/__init__.py` & `hsml-3.2.0rc0/hsml/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/tensorflow/model.py` & `hsml-3.2.0rc0/hsml/torch/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from hsml.model import Model
 from hsml.constants import MODEL
 import humps
 
 
 class Model(Model):
-    """Metadata object representing a tensorflow model in the Model Registry."""
+    """Metadata object representing a torch model in the Model Registry."""
 
     def __init__(
         self,
         id,
         name,
         version=None,
         created=None,
@@ -35,17 +35,15 @@
         experiment_project_name=None,
         metrics=None,
         program=None,
         user_full_name=None,
         model_schema=None,
         training_dataset=None,
         input_example=None,
-        framework=None,
         model_registry_id=None,
-        tags=None,
     ):
         super().__init__(
             id,
             name,
             version=version,
             created=created,
             environment=environment,
@@ -55,18 +53,18 @@
             experiment_project_name=experiment_project_name,
             metrics=metrics,
             program=program,
             user_full_name=user_full_name,
             model_schema=model_schema,
             training_dataset=training_dataset,
             input_example=input_example,
-            framework=MODEL.FRAMEWORK_TENSORFLOW,
+            framework=MODEL.FRAMEWORK_TORCH,
             model_registry_id=model_registry_id,
-            tags=tags,
         )
 
     def update_from_response_json(self, json_dict):
         json_decamelized = humps.decamelize(json_dict)
+        json_decamelized.pop("framework")
         if "type" in json_decamelized:  # backwards compatibility
             _ = json_decamelized.pop("type")
         self.__init__(**json_decamelized)
         return self
```

### Comparing `hsml-3.1.0rc0/hsml/tensorflow/predictor.py` & `hsml-3.2.0rc0/hsml/tensorflow/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/tensorflow/signature.py` & `hsml-3.2.0rc0/hsml/tensorflow/signature.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         local file path to the directory containing the model artifacts.
 
     # Arguments
         name: Name of the model to create.
         version: Optionally version of the model to create, defaults to `None` and
             will create the model with incremented version from the last
             version in the model registry.
+        metrics: Optionally a dictionary with model evaluation metrics (e.g., accuracy, MAE)
         description: Optionally a string describing the model, defaults to empty string
             `""`.
-        input_example: Optionally an input example that represents inputs for the model, defaults to `None`.
+        input_example: Optionally an input example that represents a single input for the model, defaults to `None`.
         model_schema: Optionally a model schema for the model inputs and/or outputs.
 
     # Returns
         `Model`. The model metadata object.
     """
     model = Model(
         id=None,
```

### Comparing `hsml-3.1.0rc0/hsml/torch/__init__.py` & `hsml-3.2.0rc0/hsml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/torch/model.py` & `hsml-3.2.0rc0/hsml/python/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from hsml.model import Model
 from hsml.constants import MODEL
 import humps
 
 
 class Model(Model):
-    """Metadata object representing a torch model in the Model Registry."""
+    """Metadata object representing a generic python model in the Model Registry."""
 
     def __init__(
         self,
         id,
         name,
         version=None,
         created=None,
@@ -35,17 +35,15 @@
         experiment_project_name=None,
         metrics=None,
         program=None,
         user_full_name=None,
         model_schema=None,
         training_dataset=None,
         input_example=None,
-        framework=None,
         model_registry_id=None,
-        tags=None,
     ):
         super().__init__(
             id,
             name,
             version=version,
             created=created,
             environment=environment,
@@ -55,18 +53,18 @@
             experiment_project_name=experiment_project_name,
             metrics=metrics,
             program=program,
             user_full_name=user_full_name,
             model_schema=model_schema,
             training_dataset=training_dataset,
             input_example=input_example,
-            framework=MODEL.FRAMEWORK_TORCH,
+            framework=MODEL.FRAMEWORK_PYTHON,
             model_registry_id=model_registry_id,
-            tags=tags,
         )
 
     def update_from_response_json(self, json_dict):
         json_decamelized = humps.decamelize(json_dict)
+        json_decamelized.pop("framework")
         if "type" in json_decamelized:  # backwards compatibility
             _ = json_decamelized.pop("type")
         self.__init__(**json_decamelized)
         return self
```

### Comparing `hsml-3.1.0rc0/hsml/torch/predictor.py` & `hsml-3.2.0rc0/hsml/torch/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/torch/signature.py` & `hsml-3.2.0rc0/hsml/torch/signature.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         local file path to the directory containing the model artifacts.
 
     # Arguments
         name: Name of the model to create.
         version: Optionally version of the model to create, defaults to `None` and
             will create the model with incremented version from the last
             version in the model registry.
+        metrics: Optionally a dictionary with model evaluation metrics (e.g., accuracy, MAE)
         description: Optionally a string describing the model, defaults to empty string
             `""`.
-        input_example: Optionally an input example that represents inputs for the model, defaults to `None`.
+        input_example: Optionally an input example that represents a single input for the model, defaults to `None`.
         model_schema: Optionally a model schema for the model inputs and/or outputs.
 
     # Returns
         `Model`. The model metadata object.
     """
     model = Model(
         id=None,
```

### Comparing `hsml-3.1.0rc0/hsml/transformer.py` & `hsml-3.2.0rc0/hsml/transformer.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/util.py` & `hsml-3.2.0rc0/hsml/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,62 +98,65 @@
 
 
 # Model registry
 
 # - schema and types
 
 
-def _is_numpy_scalar(x):
-    return np.isscalar(x) or x is None
-
-
 def set_model_class(model):
-    _ = model.pop("href")
+    if "href" in model:
+        _ = model.pop("href")
     if "type" in model:  # backwards compatibility
         _ = model.pop("type")
+    if "tags" in model:
+        _ = model.pop("tags")  # tags are always retrieved from backend
 
     if "framework" not in model:
         return BaseModel(**model)
-    if model["framework"] == MODEL.FRAMEWORK_TENSORFLOW:
+
+    framework = model.pop("framework")
+    if framework == MODEL.FRAMEWORK_TENSORFLOW:
         return TFModel(**model)
-    if model["framework"] == MODEL.FRAMEWORK_TORCH:
+    if framework == MODEL.FRAMEWORK_TORCH:
         return TorchModel(**model)
-    if model["framework"] == MODEL.FRAMEWORK_SKLEARN:
+    if framework == MODEL.FRAMEWORK_SKLEARN:
         return SkLearnModel(**model)
-    elif model["framework"] == MODEL.FRAMEWORK_PYTHON:
+    elif framework == MODEL.FRAMEWORK_PYTHON:
         return PyModel(**model)
 
 
-def _handle_tensor_input(input_tensor):
-    return input_tensor.tolist()
-
-
 def input_example_to_json(input_example):
     if isinstance(input_example, np.ndarray):
         if input_example.size > 0:
             return _handle_tensor_input(input_example)
         else:
             raise ValueError(
                 "input_example of type {} can not be empty".format(type(input_example))
             )
+    elif isinstance(input_example, dict):
+        return _handle_dict_input(input_example)
     else:
         return _handle_dataframe_input(input_example)
 
 
+def _handle_tensor_input(input_tensor):
+    return input_tensor.tolist()
+
+
 def _handle_dataframe_input(input_ex):
     if isinstance(input_ex, pd.DataFrame):
         if not input_ex.empty:
             return input_ex.iloc[0].tolist()
         else:
             raise ValueError(
                 "input_example of type {} can not be empty".format(type(input_ex))
             )
     elif isinstance(input_ex, pd.Series):
         if not input_ex.empty:
-            return input_ex.iloc[0]
+            return input_ex.tolist()
         else:
             raise ValueError(
                 "input_example of type {} can not be empty".format(type(input_ex))
             )
     elif isinstance(input_ex, list):
         if len(input_ex) > 0:
             return input_ex
@@ -163,14 +166,18 @@
             )
     else:
         raise TypeError(
             "{} is not a supported input example type".format(type(input_ex))
         )
 
 
+def _handle_dict_input(input_ex):
+    return input_ex
+
+
 # - artifacts
 
 
 def compress(archive_out_path, archive_name, path_to_archive):
     if os.path.isdir(path_to_archive):
         return shutil.make_archive(
             os.path.join(archive_out_path, archive_name), "gztar", path_to_archive
```

### Comparing `hsml-3.1.0rc0/hsml/utils/__init__.py` & `hsml-3.2.0rc0/hsml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/utils/schema/__init__.py` & `hsml-3.2.0rc0/hsml/utils/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/utils/schema/column.py` & `hsml-3.2.0rc0/hsml/utils/schema/column.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/utils/schema/columnar_schema.py` & `hsml-3.2.0rc0/hsml/utils/schema/columnar_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/utils/schema/tensor.py` & `hsml-3.2.0rc0/hsml/utils/schema/tensor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/utils/schema/tensor_schema.py` & `hsml-3.2.0rc0/hsml/utils/schema/tensor_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/hsml/version.py` & `hsml-3.2.0rc0/hsml/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.1.0rc0"
+__version__ = "3.2.0rc0"
```

### Comparing `hsml-3.1.0rc0/hsml.egg-info/PKG-INFO` & `hsml-3.2.0rc0/hsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.1.0rc0
+Version: 3.2.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.1.0rc0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
@@ -96,15 +96,15 @@
         Start a deployment
         ```python
         deployment.start()
         ```
         
         Make predictions with a deployed model
         ```python
-        data = { "instances": model.input_example }
+        data = { "instances": [ model.input_example ] }
         
         predictions = deployment.predict(data)
         ```
         
         You can find more examples on how to use the library in [examples.hopsworks.ai](https://examples.hopsworks.ai).
         
         ## Documentation
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.1.0rc0 Summary: HSML: An
+Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc0 Summary: HSML: An
 environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api Author:
 Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
 2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
-releases/tag/3.1.0rc0 Description: # Hopsworks Model Management
+releases/tag/3.2.0rc0 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
@@ -21,23 +21,24 @@
 metrics={"accuracy": 0.94}, description="mnist model description") model.save
 ("/tmp/model_directory") # or /tmp/model_file ``` Download a model ```python
 model = mr.get_model("mnist", version=1) model_path = model.download() ```
 Delete a model ```python model.delete() ``` Get best performing model ```python
 best_model = mr.get_best_model('mnist', 'accuracy', 'max') ``` Deploy a model
 ```python deployment = model.deploy() ``` Start a deployment ```python
 deployment.start() ``` Make predictions with a deployed model ```python data =
-{ "instances": model.input_example } predictions = deployment.predict(data) ```
-You can find more examples on how to use the library in [examples.hopsworks.ai]
-(https://examples.hopsworks.ai). ## Documentation Documentation is available at
-[Hopsworks Model Management Documentation](https://docs.hopsworks.ai/). ##
-Issues For general questions about the usage of Hopsworks Machine Learning
-please open a topic on [Hopsworks Community](https://community.hopsworks.ai/).
-Please report any issue using [Github issue tracking](https://github.com/
-logicalclocks/machine-learning-api/issues). ## Contributing If you would like
-to contribute to this library, please see the [Contribution Guidelines]
-(CONTRIBUTING.md). Keywords: Hopsworks,ML,Models,Machine Learning Models,Model
+{ "instances": [ model.input_example ] } predictions = deployment.predict(data)
+``` You can find more examples on how to use the library in
+[examples.hopsworks.ai](https://examples.hopsworks.ai). ## Documentation
+Documentation is available at [Hopsworks Model Management Documentation](https:
+//docs.hopsworks.ai/). ## Issues For general questions about the usage of
+Hopsworks Machine Learning please open a topic on [Hopsworks Community](https:/
+/community.hopsworks.ai/). Please report any issue using [Github issue
+tracking](https://github.com/logicalclocks/machine-learning-api/issues). ##
+Contributing If you would like to contribute to this library, please see the
+[Contribution Guidelines](CONTRIBUTING.md). Keywords:
+Hopsworks,ML,Models,Machine Learning Models,Model
 Registry,TensorFlow,PyTorch,Machine Learning,MLOps,DataOps Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Utilities Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Description-Content-Type: text/markdown Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `hsml-3.1.0rc0/hsml.egg-info/SOURCES.txt` & `hsml-3.2.0rc0/hsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/setup.py` & `hsml-3.2.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/tests/__init__.py` & `hsml-3.2.0rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/tests/hsml/__init__.py` & `hsml-3.2.0rc0/tests/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.1.0rc0/tests/hsml/core/__init__.py` & `hsml-3.2.0rc0/tests/hsml/core/__init__.py`

 * *Files identical despite different names*

