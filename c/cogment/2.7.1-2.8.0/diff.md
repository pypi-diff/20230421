# Comparing `tmp/cogment-2.7.1.tar.gz` & `tmp/cogment-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/ai-r/cogment/cogment-py-sdk/dist/.tmp-xpjlboug/cogment-2.7.1.tar", last modified: Mon Mar  6 17:00:18 2023, max compression
+gzip compressed data, was "/builds/ai-r/cogment/cogment-py-sdk/dist/.tmp-hbg83nvd/cogment-2.8.0.tar", last modified: Fri Apr 21 20:04:19 2023, max compression
```

## Comparing `cogment-2.7.1.tar` & `cogment-2.8.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 17:00:18.000000 cogment-2.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     8826 2023-03-06 16:59:54.000000 cogment-2.7.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-03-06 16:59:54.000000 cogment-2.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13972 2023-03-06 17:00:18.000000 cogment-2.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-03-06 16:59:54.000000 cogment-2.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/
--rw-rw-rw-   0 root         (0) root         (0)     1652 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3812 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/actor.py
--rw-rw-rw-   0 root         (0) root         (0)    19302 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/
--rw-r--r--   0 root         (0) root         (0)     1021 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/agent.proto
--rw-r--r--   0 root         (0) root         (0)     1379 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/agent_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4231 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/agent_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/common.proto
--rw-r--r--   0 root         (0) root         (0)    16049 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4537 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/datalog.proto
--rw-r--r--   0 root         (0) root         (0)    13215 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/datalog_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/datalog_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/directory.proto
--rw-r--r--   0 root         (0) root         (0)     9698 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/directory_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8131 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/directory_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/environment.proto
--rw-r--r--   0 root         (0) root         (0)     5639 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/environment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4933 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/environment_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/health.proto
--rw-r--r--   0 root         (0) root         (0)     3339 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/hooks.proto
--rw-r--r--   0 root         (0) root         (0)     1875 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/hooks_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4224 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/hooks_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/model_registry.proto
--rw-r--r--   0 root         (0) root         (0)    15133 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/model_registry_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15143 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/model_registry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/orchestrator.proto
--rw-r--r--   0 root         (0) root         (0)     8431 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/orchestrator_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13880 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/orchestrator_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7431 2023-02-28 14:19:53.000000 cogment-2.7.1/cogment/api/trial_datastore.proto
--rw-r--r--   0 root         (0) root         (0)    15895 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/trial_datastore_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11659 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment/api/trial_datastore_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    17090 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/client_service.py
--rw-rw-rw-   0 root         (0) root         (0)    20868 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7346 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/control.py
--rw-rw-rw-   0 root         (0) root         (0)     7801 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/datalog.py
--rw-rw-rw-   0 root         (0) root         (0)    10099 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/datalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)    13301 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/datastore.py
--rw-rw-rw-   0 root         (0) root         (0)    11837 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/directory.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    18786 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/env_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5587 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     7851 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/hooks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10467 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/model_registry.py
--rw-rw-rw-   0 root         (0) root         (0)    19765 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/model_registry_v2.py
--rw-rw-rw-   0 root         (0) root         (0)    17169 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/prehook.py
--rw-rw-rw-   0 root         (0) root         (0)    14365 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/session.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/trial.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-03-06 16:59:54.000000 cogment-2.7.1/cogment/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13972 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1726 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-06 17:00:18.000000 cogment-2.7.1/cogment.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-03-06 16:59:54.000000 cogment-2.7.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-03-06 17:00:18.000000 cogment-2.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6037 2023-03-06 16:59:54.000000 cogment-2.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 17:00:18.000000 cogment-2.7.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2023 2023-03-06 16:59:54.000000 cogment-2.7.1/tests/test_download_cogment.py
--rw-rw-rw-   0 root         (0) root         (0)    26016 2023-03-06 16:59:54.000000 cogment-2.7.1/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-03-06 16:59:54.000000 cogment-2.7.1/tests/test_model_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     9511 2023-04-21 20:03:55.000000 cogment-2.8.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-04-21 20:03:55.000000 cogment-2.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14657 2023-04-21 20:04:19.000000 cogment-2.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-21 20:03:55.000000 cogment-2.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/actor.py
+-rw-rw-rw-   0 root         (0) root         (0)    19336 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/agent.proto
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/agent_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/agent_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/common.proto
+-rw-r--r--   0 root         (0) root         (0)    16049 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/datalog.proto
+-rw-r--r--   0 root         (0) root         (0)    13215 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/datalog_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/datalog_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/directory.proto
+-rw-r--r--   0 root         (0) root         (0)     9698 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/directory_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8131 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/directory_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/environment.proto
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/environment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/environment_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/health.proto
+-rw-r--r--   0 root         (0) root         (0)     3339 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/hooks.proto
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/hooks_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/hooks_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/model_registry.proto
+-rw-r--r--   0 root         (0) root         (0)    15133 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/model_registry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15143 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/model_registry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/orchestrator.proto
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/orchestrator_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13880 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/orchestrator_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/trial_datastore.proto
+-rw-r--r--   0 root         (0) root         (0)    15895 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/trial_datastore_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11659 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/trial_datastore_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    17115 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/client_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    23312 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7910 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     7853 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    14369 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datastore.py
+-rw-rw-rw-   0 root         (0) root         (0)    11837 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4136 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    18791 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/env_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7840 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/hooks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10467 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/model_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    19851 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/model_registry_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21845 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/prehook.py
+-rw-rw-rw-   0 root         (0) root         (0)    14373 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/trial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14657 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-21 20:03:55.000000 cogment-2.8.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 20:04:19.000000 cogment-2.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6037 2023-04-21 20:03:55.000000 cogment-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_download_cogment.py
+-rw-rw-rw-   0 root         (0) root         (0)    26016 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_model_registry.py
```

### Comparing `cogment-2.7.1/CHANGELOG.md` & `cogment-2.8.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.0 - 2023-04-21
+
+### Added
+
+- Option to request full info (not just id and state) from 'watch_trials'
+- Ability to use the SDK without spec (cog_settings)
+- Automatic port selection for 'Context.serve_all_registered()'
+- Ability to specify an explicit host to register a service to the directory
+- Ability to specify trial properties for 'Datastore.all_trials()' and 'Datastore.get_trials()'
+- Ability to specify trial ids for 'Datastore.all_trials()'
+
+### Changed
+
+- Enable warning and error logging even if user did not define a logging handler
+- Warn user when no logging handler is defined (i.e. proper logging is disabled)
+- Better self IP address discovery functionality
+
 ## v2.7.1 - 2023-03-06
 
 ## Fixed
 
 - Deadlock in 'wait_for_newer' method of LatestModel
 
 ## v2.7.0 - 2023-02-28
```

### Comparing `cogment-2.7.1/LICENSE` & `cogment-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/PKG-INFO` & `cogment-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogment
-Version: 2.7.1
+Version: 2.8.0
 Summary: Cogment python SDK
 Author-email: Artificial Intelligence Redefined <dev+cogment@ai-r.com>
 Project-URL: Homepage, https://cogment.ai
 Project-URL: repository, https://github.com/cogment/cogment-py-sdk
 Project-URL: Reference Documentation, https://cogment.ai/docs/reference/python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -134,14 +134,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.0 - 2023-04-21
+
+### Added
+
+- Option to request full info (not just id and state) from 'watch_trials'
+- Ability to use the SDK without spec (cog_settings)
+- Automatic port selection for 'Context.serve_all_registered()'
+- Ability to specify an explicit host to register a service to the directory
+- Ability to specify trial properties for 'Datastore.all_trials()' and 'Datastore.get_trials()'
+- Ability to specify trial ids for 'Datastore.all_trials()'
+
+### Changed
+
+- Enable warning and error logging even if user did not define a logging handler
+- Warn user when no logging handler is defined (i.e. proper logging is disabled)
+- Better self IP address discovery functionality
+
 ## v2.7.1 - 2023-03-06
 
 ## Fixed
 
 - Deadlock in 'wait_for_newer' method of LatestModel
 
 ## v2.7.0 - 2023-02-28
```

### Comparing `cogment-2.7.1/README.md` & `cogment-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/__init__.py` & `cogment-2.8.0/cogment/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,7 +34,10 @@
 from cogment.datastore import DatastoreFields
 from cogment.model_registry import Model
 
 from cogment.errors import CogmentError
 
 # Necessary because of cogment CLI "cog_settings.py" generated code
 from cogment.actor import ActorClass, ActorClassList
+
+# Used in Cogment Enterprise
+from cogment.utils import make_logger
```

### Comparing `cogment-2.7.1/cogment/actor.py` & `cogment-2.8.0/cogment/actor.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 class ActorClassList:
     """Class containing the list of actor classes defined in a config file."""
 
     def __init__(self, *args):
         self._actor_classes_list = list(args)
 
-        for a_c in args:
-            setattr(self, a_c.name, a_c)
+        for actor_class_spec in args:
+            setattr(self, actor_class_spec.name, actor_class_spec)
 
     def __iter__(self):
         return iter(self._actor_classes_list)
 
     def __contains__(self, key):
         return hasattr(self, key)
 
@@ -66,23 +66,24 @@
     def get(self, key, default=None):  # Similar to dict.get()
         return getattr(self, key, default)
 
 
 class ActorSession(Session):
     """Derived class representing the session of an actor for a trial."""
 
-    def __init__(self, impl, actor_class, trial, name, impl_name, env_name, config):
+    def __init__(self, impl, actor_class_spec, trial, name, impl_name, env_name, config):
         super().__init__(trial, name, impl, impl_name, config)
-        self.class_name = actor_class.name
+        self.class_name = actor_class_spec.name
+        self.actor_class = actor_class_spec.name
         self.env_name = env_name
-        self._actor_class = actor_class
+        self._actor_class_spec = actor_class_spec
 
     def __str__(self):
         result = super().__str__()
-        result += f" --- ActorSession: class_name = {self.class_name}, config = {self.config}"
+        result += f" --- ActorSession: actor_class = {self.actor_class}, config = {self.config}"
         return result
 
     def get_active_actors(self):
         # Controller.get_actors can be used.
         # Or provide actors details in the config, or the observations.
         raise CogmentError(f"This function is deprecated for actors")
```

### Comparing `cogment-2.7.1/cogment/agent_service.py` & `cogment-2.8.0/cogment/agent_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,28 +64,28 @@
     if not init_data.actor_class:
         raise CogmentError(f"Trial [{trial_id}] - Empty actor class for actor [{init_data.actor_name}]")
 
     actor_impl = actor_impls.get(init_data.impl_name)
     if actor_impl is not None:
         # Check compatibility
         compatible = (len(actor_impl.actor_classes) == 0)
-        for class_name in actor_impl.actor_classes:
-            if class_name == init_data.actor_class:
+        for actor_class in actor_impl.actor_classes:
+            if actor_class == init_data.actor_class:
                 compatible = True
                 break
         if not compatible:
             raise CogmentError(f"Trial [{trial_id}] - actor [{init_data.actor_name}] class [{init_data.actor_class}] "
                                f"is not compatible with actor implementation [{init_data.impl_name}]")
     else:
         # Find a compatible actor class in the registered actors
 
         # Search for exact match first
         for init_data.impl_name, impl in actor_impls.items():
-            for class_name in impl.actor_classes:
-                if class_name == init_data.actor_class:
+            for actor_class in impl.actor_classes:
+                if actor_class == init_data.actor_class:
                     actor_impl = impl
                     break
             if actor_impl is not None:
                 break
 
         if actor_impl is None:
             raise CogmentError(f"Trial [{trial_id}] - actor [{init_data.actor_name}] class [{init_data.actor_class}] "
@@ -108,15 +108,15 @@
 
         if session._trial.ending and session._auto_ack:
             session._post_outgoing_data(_EndingAck())
 
         tick_id = data.observation.tick_id
         session._trial.tick_id = tick_id
 
-        obs_space = session._actor_class.observation_space()
+        obs_space = session._actor_class_spec.observation_space()
         obs_space.ParseFromString(data.observation.content)
 
         recv_event.observation = RecvObservation(data.observation, obs_space)
         session._post_incoming_event((tick_id, recv_event))
 
     elif data.HasField("reward"):
         logger.trace(f"Trial [{session._trial.id}] - Actor [{session.name}] received reward")
@@ -332,35 +332,35 @@
                 logger.error(error_str)
                 await context.abort(grpc.StatusCode.UNKNOWN, error_str)
 
     def _start_session(self, trial_id, init_input):
         actor_impl = get_actor_impl(trial_id, self._impls, init_input)
 
         actor_name = init_input.actor_name
-        actor_class = self._cog_settings.actor_classes.get(init_input.actor_class)
-        if actor_class is None:
+        actor_class_spec = self._cog_settings.actor_classes.get(init_input.actor_class)
+        if actor_class_spec is None:
             raise CogmentError(f"Trial [{trial_id}] - "
                                f"Unknown class [{init_input.actor_class}] for service actor [{actor_name}]")
 
         key = _trial_key(trial_id, actor_name)
         if key in self._sessions:
             raise CogmentError(f"Trial [{trial_id}] - Service actor [{actor_name}] already exists")
 
         config = None
         if init_input.HasField("config"):
-            if actor_class.config_type is None:
+            if actor_class_spec.config_type is None:
                 raise CogmentError(f"Trial [{trial_id}] - Service actor [{actor_name}] "
                                    f"received config data of unknown type (was it defined in cogment.yaml?)")
-            config = actor_class.config_type()
+            config = actor_class_spec.config_type()
             config.ParseFromString(init_input.config.content)
 
         self._prometheus_data.actors_started.labels(init_input.impl_name).inc()
 
         trial = Trial(trial_id, [], self._cog_settings)
-        new_session = ActorSession(actor_impl.impl, actor_class, trial, actor_name, init_input.impl_name,
+        new_session = ActorSession(actor_impl.impl, actor_class_spec, trial, actor_name, init_input.impl_name,
                                    init_input.env_name, config)
         new_session._prometheus_data = self._prometheus_data
         self._sessions.add(key)
 
         logger.debug(f"Trial [{trial_id}] - impl [{init_input.impl_name}] for service actor [{actor_name}] started")
 
         return new_session
```

### Comparing `cogment-2.7.1/cogment/api/agent.proto` & `cogment-2.8.0/cogment/api/agent.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/agent_pb2.py` & `cogment-2.8.0/cogment/api/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/agent_pb2_grpc.py` & `cogment-2.8.0/cogment/api/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/common.proto` & `cogment-2.8.0/cogment/api/common.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/common_pb2.py` & `cogment-2.8.0/cogment/api/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/datalog.proto` & `cogment-2.8.0/cogment/api/datalog.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/datalog_pb2.py` & `cogment-2.8.0/cogment/api/datalog_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/datalog_pb2_grpc.py` & `cogment-2.8.0/cogment/api/datalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/directory.proto` & `cogment-2.8.0/cogment/api/directory.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/directory_pb2.py` & `cogment-2.8.0/cogment/api/directory_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/directory_pb2_grpc.py` & `cogment-2.8.0/cogment/api/directory_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/environment.proto` & `cogment-2.8.0/cogment/api/environment.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/environment_pb2.py` & `cogment-2.8.0/cogment/api/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/environment_pb2_grpc.py` & `cogment-2.8.0/cogment/api/environment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/health.proto` & `cogment-2.8.0/cogment/api/health.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/health_pb2.py` & `cogment-2.8.0/cogment/api/health_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/health_pb2_grpc.py` & `cogment-2.8.0/cogment/api/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/hooks.proto` & `cogment-2.8.0/cogment/api/hooks.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/hooks_pb2.py` & `cogment-2.8.0/cogment/api/hooks_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/hooks_pb2_grpc.py` & `cogment-2.8.0/cogment/api/hooks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/model_registry.proto` & `cogment-2.8.0/cogment/api/model_registry.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/model_registry_pb2.py` & `cogment-2.8.0/cogment/api/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/model_registry_pb2_grpc.py` & `cogment-2.8.0/cogment/api/model_registry_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/orchestrator.proto` & `cogment-2.8.0/cogment/api/orchestrator.proto`

 * *Files 8% similar despite different names*

```diff
@@ -109,19 +109,24 @@
   repeated TrialInfo trial = 1;
 }
 
 message TrialListRequest {
   // Only return trials that are in the specified states.
   // If empty, every single trial will be returned.
   repeated TrialState filter = 1;
+
+  bool full_info = 2;
 }
 
 message TrialListEntry {
   string trial_id = 1;
   TrialState state = 2;
+
+  // Only present if 'full_info' is true. In which case 'trial_id' and 'state' are not set.
+  TrialInfo info = 3;
 }
 
 // ----------------------------------------------------------------------------------------------------------
 
 service ClientActorSP {
   // Expected metadata:
   //   - trial-id: The id of the trial
```

### Comparing `cogment-2.7.1/cogment/api/orchestrator_pb2.py` & `cogment-2.8.0/cogment/api/orchestrator_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from cogment.api import common_pb2 as cogment_dot_api_dot_common__pb2
 from cogment.api import environment_pb2 as cogment_dot_api_dot_environment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x63ogment/api/orchestrator.proto\x12\ncogmentAPI\x1a\x18\x63ogment/api/common.proto\x1a\x1d\x63ogment/api/environment.proto\"\xaa\x01\n\x11TrialStartRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1d.cogmentAPI.SerializedMessageH\x00\x12)\n\x06params\x18\x04 \x01(\x0b\x32\x17.cogmentAPI.TrialParamsH\x00\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x1a\n\x12trial_id_requested\x18\x03 \x01(\tB\x0c\n\nstart_data\"#\n\x0fTrialStartReply\x12\x10\n\x08trial_id\x18\x01 \x01(\t\"1\n\x15TerminateTrialRequest\x12\x18\n\x10hard_termination\x18\x01 \x01(\x08\"\x15\n\x13TerminateTrialReply\"J\n\x10TrialInfoRequest\x12\x1e\n\x16get_latest_observation\x18\x01 \x01(\x08\x12\x16\n\x0eget_actor_list\x18\x02 \x01(\x08\"\xd6\x02\n\tTrialInfo\x12\x10\n\x08trial_id\x18\x01 \x01(\t\x12\x39\n\nproperties\x18\x08 \x03(\x0b\x32%.cogmentAPI.TrialInfo.PropertiesEntry\x12%\n\x05state\x18\x02 \x01(\x0e\x32\x16.cogmentAPI.TrialState\x12\x10\n\x08\x65nv_name\x18\x03 \x01(\t\x12\x0f\n\x07tick_id\x18\x04 \x01(\x04\x12\x16\n\x0etrial_duration\x18\x05 \x01(\x06\x12\x36\n\x12latest_observation\x18\x06 \x01(\x0b\x32\x1a.cogmentAPI.ObservationSet\x12/\n\x0f\x61\x63tors_in_trial\x18\x07 \x03(\x0b\x32\x16.cogmentAPI.TrialActor\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"6\n\x0eTrialInfoReply\x12$\n\x05trial\x18\x01 \x03(\x0b\x32\x15.cogmentAPI.TrialInfo\":\n\x10TrialListRequest\x12&\n\x06\x66ilter\x18\x01 \x03(\x0e\x32\x16.cogmentAPI.TrialState\"I\n\x0eTrialListEntry\x12\x10\n\x08trial_id\x18\x01 \x01(\t\x12%\n\x05state\x18\x02 \x01(\x0e\x32\x16.cogmentAPI.TrialState2\x91\x03\n\x10TrialLifecycleSP\x12J\n\nStartTrial\x12\x1d.cogmentAPI.TrialStartRequest\x1a\x1b.cogmentAPI.TrialStartReply\"\x00\x12V\n\x0eTerminateTrial\x12!.cogmentAPI.TerminateTrialRequest\x1a\x1f.cogmentAPI.TerminateTrialReply\"\x00\x12J\n\x0cGetTrialInfo\x12\x1c.cogmentAPI.TrialInfoRequest\x1a\x1a.cogmentAPI.TrialInfoReply\"\x00\x12K\n\x0bWatchTrials\x12\x1c.cogmentAPI.TrialListRequest\x1a\x1a.cogmentAPI.TrialListEntry\"\x00\x30\x01\x12@\n\x07Version\x12\x1a.cogmentAPI.VersionRequest\x1a\x17.cogmentAPI.VersionInfo\"\x00\x32\xa4\x01\n\rClientActorSP\x12Q\n\x08RunTrial\x12\x1f.cogmentAPI.ActorRunTrialOutput\x1a\x1e.cogmentAPI.ActorRunTrialInput\"\x00(\x01\x30\x01\x12@\n\x07Version\x12\x1a.cogmentAPI.VersionRequest\x1a\x17.cogmentAPI.VersionInfo\"\x00\x42\x30Z.github.com/cogment/cogment/grpcapi/cogment/apib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x63ogment/api/orchestrator.proto\x12\ncogmentAPI\x1a\x18\x63ogment/api/common.proto\x1a\x1d\x63ogment/api/environment.proto\"\xaa\x01\n\x11TrialStartRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1d.cogmentAPI.SerializedMessageH\x00\x12)\n\x06params\x18\x04 \x01(\x0b\x32\x17.cogmentAPI.TrialParamsH\x00\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x1a\n\x12trial_id_requested\x18\x03 \x01(\tB\x0c\n\nstart_data\"#\n\x0fTrialStartReply\x12\x10\n\x08trial_id\x18\x01 \x01(\t\"1\n\x15TerminateTrialRequest\x12\x18\n\x10hard_termination\x18\x01 \x01(\x08\"\x15\n\x13TerminateTrialReply\"J\n\x10TrialInfoRequest\x12\x1e\n\x16get_latest_observation\x18\x01 \x01(\x08\x12\x16\n\x0eget_actor_list\x18\x02 \x01(\x08\"\xd6\x02\n\tTrialInfo\x12\x10\n\x08trial_id\x18\x01 \x01(\t\x12\x39\n\nproperties\x18\x08 \x03(\x0b\x32%.cogmentAPI.TrialInfo.PropertiesEntry\x12%\n\x05state\x18\x02 \x01(\x0e\x32\x16.cogmentAPI.TrialState\x12\x10\n\x08\x65nv_name\x18\x03 \x01(\t\x12\x0f\n\x07tick_id\x18\x04 \x01(\x04\x12\x16\n\x0etrial_duration\x18\x05 \x01(\x06\x12\x36\n\x12latest_observation\x18\x06 \x01(\x0b\x32\x1a.cogmentAPI.ObservationSet\x12/\n\x0f\x61\x63tors_in_trial\x18\x07 \x03(\x0b\x32\x16.cogmentAPI.TrialActor\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"6\n\x0eTrialInfoReply\x12$\n\x05trial\x18\x01 \x03(\x0b\x32\x15.cogmentAPI.TrialInfo\"M\n\x10TrialListRequest\x12&\n\x06\x66ilter\x18\x01 \x03(\x0e\x32\x16.cogmentAPI.TrialState\x12\x11\n\tfull_info\x18\x02 \x01(\x08\"n\n\x0eTrialListEntry\x12\x10\n\x08trial_id\x18\x01 \x01(\t\x12%\n\x05state\x18\x02 \x01(\x0e\x32\x16.cogmentAPI.TrialState\x12#\n\x04info\x18\x03 \x01(\x0b\x32\x15.cogmentAPI.TrialInfo2\x91\x03\n\x10TrialLifecycleSP\x12J\n\nStartTrial\x12\x1d.cogmentAPI.TrialStartRequest\x1a\x1b.cogmentAPI.TrialStartReply\"\x00\x12V\n\x0eTerminateTrial\x12!.cogmentAPI.TerminateTrialRequest\x1a\x1f.cogmentAPI.TerminateTrialReply\"\x00\x12J\n\x0cGetTrialInfo\x12\x1c.cogmentAPI.TrialInfoRequest\x1a\x1a.cogmentAPI.TrialInfoReply\"\x00\x12K\n\x0bWatchTrials\x12\x1c.cogmentAPI.TrialListRequest\x1a\x1a.cogmentAPI.TrialListEntry\"\x00\x30\x01\x12@\n\x07Version\x12\x1a.cogmentAPI.VersionRequest\x1a\x17.cogmentAPI.VersionInfo\"\x00\x32\xa4\x01\n\rClientActorSP\x12Q\n\x08RunTrial\x12\x1f.cogmentAPI.ActorRunTrialOutput\x1a\x1e.cogmentAPI.ActorRunTrialInput\"\x00(\x01\x30\x01\x12@\n\x07Version\x12\x1a.cogmentAPI.VersionRequest\x1a\x17.cogmentAPI.VersionInfo\"\x00\x42\x30Z.github.com/cogment/cogment/grpcapi/cogment/apib\x06proto3')
 
 
 
 _TRIALSTARTREQUEST = DESCRIPTOR.message_types_by_name['TrialStartRequest']
 _TRIALSTARTREPLY = DESCRIPTOR.message_types_by_name['TrialStartReply']
 _TERMINATETRIALREQUEST = DESCRIPTOR.message_types_by_name['TerminateTrialRequest']
 _TERMINATETRIALREPLY = DESCRIPTOR.message_types_by_name['TerminateTrialReply']
@@ -122,15 +122,15 @@
   _TRIALINFO._serialized_start=464
   _TRIALINFO._serialized_end=806
   _TRIALINFO_PROPERTIESENTRY._serialized_start=757
   _TRIALINFO_PROPERTIESENTRY._serialized_end=806
   _TRIALINFOREPLY._serialized_start=808
   _TRIALINFOREPLY._serialized_end=862
   _TRIALLISTREQUEST._serialized_start=864
-  _TRIALLISTREQUEST._serialized_end=922
-  _TRIALLISTENTRY._serialized_start=924
-  _TRIALLISTENTRY._serialized_end=997
-  _TRIALLIFECYCLESP._serialized_start=1000
-  _TRIALLIFECYCLESP._serialized_end=1401
-  _CLIENTACTORSP._serialized_start=1404
-  _CLIENTACTORSP._serialized_end=1568
+  _TRIALLISTREQUEST._serialized_end=941
+  _TRIALLISTENTRY._serialized_start=943
+  _TRIALLISTENTRY._serialized_end=1053
+  _TRIALLIFECYCLESP._serialized_start=1056
+  _TRIALLIFECYCLESP._serialized_end=1457
+  _CLIENTACTORSP._serialized_start=1460
+  _CLIENTACTORSP._serialized_end=1624
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cogment-2.7.1/cogment/api/orchestrator_pb2_grpc.py` & `cogment-2.8.0/cogment/api/orchestrator_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/trial_datastore.proto` & `cogment-2.8.0/cogment/api/trial_datastore.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/trial_datastore_pb2.py` & `cogment-2.8.0/cogment/api/trial_datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/api/trial_datastore_pb2_grpc.py` & `cogment-2.8.0/cogment/api/trial_datastore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/client_service.py` & `cogment-2.8.0/cogment/client_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """Internal class signaling the end of data queueing."""
     pass
 
 
 def _impl_can_serve_actor_class(impl, actor_class):
     if impl.actor_classes:
         for ac in impl.actor_classes:
-            if ac == actor_class.name:
+            if ac == actor_class:
                 return True
         return False
     else:
         return True
 
 
 def _process_normal_data(data, session):
@@ -52,15 +52,15 @@
 
         if session._trial.ending and session._auto_ack:
             session._post_outgoing_data(_EndingAck())
 
         tick_id = data.observation.tick_id
         session._trial.tick_id = tick_id
 
-        obs_space = session._actor_class.observation_space()
+        obs_space = session._actor_class_spec.observation_space()
         obs_space.ParseFromString(data.observation.content)
 
         recv_event.observation = RecvObservation(data.observation, obs_space)
         session._post_incoming_event((tick_id, recv_event))
 
     elif data.HasField("reward"):
         logger.trace(f"Trial [{session._trial.id}] - Actor [{session.name}] received reward")
@@ -294,29 +294,29 @@
                                    f"[{reply.state}] [{reply}]")
 
     def _start_session(self, impl, init_data):
         actor_name = init_data.actor_name
         if not actor_name:
             raise CogmentError(f"Trial [{self.trial_id}] - Empty actor name for client actor")
 
-        actor_class = self._cog_settings.actor_classes.get(init_data.actor_class)
-        if actor_class is None:
+        actor_class_spec = self._cog_settings.actor_classes.get(init_data.actor_class)
+        if actor_class_spec is None:
             raise CogmentError(f"Trial [{self.trial_id}] - "
                                f"Unknown class [{init_data.actor_class}] for client actor [{actor_name}]")
 
         config = None
         if init_data.HasField("config"):
-            if actor_class.config_type is None:
+            if actor_class_spec.config_type is None:
                 raise CogmentError(f"Trial [{self.trial_id}] - Client actor [{actor_name}] "
                                    f"received config data of unknown type (was it defined in cogment.yaml?)")
-            config = actor_class.config_type()
+            config = actor_class_spec.config_type()
             config.ParseFromString(init_data.config.content)
 
         trial = Trial(self.trial_id, [], self._cog_settings)
-        new_session = ActorSession(impl, actor_class, trial, actor_name, init_data.impl_name,
+        new_session = ActorSession(impl, actor_class_spec, trial, actor_name, init_data.impl_name,
                                    init_data.env_name, config)
 
         logger.debug(f"Trial [{self.trial_id}] - impl [{init_data.impl_name}] for actor [{actor_name}] started")
 
         return new_session
 
     async def run_session(self, impl, init_data):
```

### Comparing `cogment-2.7.1/cogment/context.py` & `cogment-2.8.0/cogment/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,41 @@
 import os
 from typing import Callable, Awaitable, Dict, List, Any, Tuple
 from types import ModuleType
 import asyncio
 from types import SimpleNamespace
 import socket
 import urllib.parse as urlpar
+import warnings
 
 
 _ADDITIONAL_REGISTRATION_ITEMS = {"__registration_source" : "PythonSDK-Implicit", "__version" : __version__}
 
+# (host, port): This IP address is normally not assigned, it is reserved for local benchmarking by IANA (RFC2544).
+_SPECIAL_CONNECTION_IP = ("192.19.254.254", 65535)
+
+
+def _self_ip_address():
+    sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM | socket.SOCK_NONBLOCK)
+    try:
+        sock.connect(_SPECIAL_CONNECTION_IP)
+        addr = sock.getsockname()[0]
+    except Exception as exc:
+        logger.debug(f"Failed to connect to get host ip address [{exc}]")
+        addr = None
+    finally:
+        sock.close()
+
+    if not addr or addr.startswith("127.") or addr == "0.0.0.0":
+        logger.debug(f"Could not get host address [{addr}]")
+        addr = None
+
+    logger.debug(f"Host address [{addr}]")
+    return addr
+
 
 def _make_client_channel(grpc_endpoint: ep.Endpoint):
     parsed_url = urlpar.urlparse(grpc_endpoint.url)
     if parsed_url.scheme == ep.GRPC_SCHEME:
         url = parsed_url.netloc
     else:
         raise CogmentError(f"Invalid endpoint scheme (must be 'grpc') [{grpc_endpoint.url}]")
@@ -86,88 +109,111 @@
 
 
 def _make_server(served_endpoint: ep.ServedEndpoint):
     server = grpc.aio.server()
 
     address = f"[::]:{served_endpoint.port}"
     if not served_endpoint.using_ssl():
-        server.add_insecure_port(address)
+        port = server.add_insecure_port(address)
     else:
         if served_endpoint.root_certificates:
             require_client_auth = True
             root = bytes(served_endpoint.root_certificates, "utf-8")
         else:
             require_client_auth = False
             root = None
         certs = []
         for (key, chain) in served_endpoint.private_key_certificate_chain_pairs:
             certs.append((bytes(key, "utf-8"), bytes(chain, "utf-8")))
         if not certs:
             certs = None
 
         creds = grpc.ssl_server_credentials(certs, root, require_client_auth)
-        server.add_secure_port(address, creds)
+        port = server.add_secure_port(address, creds)
+
+    if served_endpoint.port == 0:
+        logger.info(f"Serving on port [{port}]")
+    elif served_endpoint.port != port:
+        logger.warning(f"gRPC ignored requested port [{served_endpoint.port}] and is serving on port [{port}]")
 
-    return server
+    return (server, port)
 
 
 class Context:
     """Top level class for the Cogment library from which to obtain all services."""
 
     def __init__(self, user_id: str, cog_settings: ModuleType, asyncio_loop=None,
                        prometheus_registry=PROMETHEUS_REGISTRY, directory_endpoint: ep.Endpoint = None,
                        directory_auth_token: str = None):
         self._user_id = user_id
         self._actor_impls: Dict[str, SimpleNamespace] = {}
         self._env_impls: Dict[str, SimpleNamespace] = {}
         self._prehook_impl: SimpleNamespace = None
         self._datalog_impl: SimpleNamespace = None
         self._grpc_server = None  # type: Any
+        self._grpc_server_port: int = 0
         self._prometheus_registry = prometheus_registry
         self._cog_settings = cog_settings
 
         if asyncio_loop is None:
             # Make sure we are running in a asyncio.Task. Even if technically this init does not need
             # to be in a Task, the whole of the SDK expects to be running in Tasks of the same event loop.
             try:
                 self.asyncio_loop = asyncio.get_running_loop()
             except RuntimeError:
                 raise CogmentError("The Cogment SDK requires running in a Python `asyncio` Task")
         else:
             self.asyncio_loop = asyncio_loop
 
         if directory_endpoint is not None:
+            if not isinstance(directory_endpoint, ep.Endpoint):
+                CogmentError(f"Wrong argument type for 'directory_endpoint', must be a 'cogment.Endpoint' type")
             endpoint_to_use = directory_endpoint
         else:
             env_endpoint = os.environ.get("COGMENT_DIRECTORY_ENDPOINT")
             if env_endpoint is not None:
                 endpoint_to_use = ep.Endpoint(env_endpoint)
             else:
                 endpoint_to_use = None
+        logger.debug(f"Directory endpoint [{endpoint_to_use}]")
 
         if directory_auth_token is not None:
+            if type(directory_auth_token) is not str:
+                CogmentError(f"Wrong argument type for 'directory_auth_token', must be 'str' type")
+            if not endpoint_to_use:
+                logger.warning(f"Context 'directory_auth_token' argument unused because"
+                               f" the directory endpoint is not set")
             auth_token_to_use = directory_auth_token
         else:
             auth_token_to_use = os.environ.get("COGMENT_DIRECTORY_AUTHENTICATION_TOKEN")
+        logger.debug(f"Directory authorization token [{auth_token_to_use is not None and len(auth_token_to_use) > 0}]")
 
         if endpoint_to_use:
             try:
-                channel = _make_client_channel(endpoint_to_use)
+                self._directory = self.get_directory(endpoint_to_use, auth_token_to_use)
             except CogmentError as exc:
                 raise CogmentError(f"Directory endpoint: {exc}")
-
-            stub = directory_grpc_api.DirectorySPStub(channel)
-            self._directory = Directory(stub, auth_token_to_use)
         else:
+            logger.debug(f"No directory set")
             self._directory = None
 
+        if not logger.hasHandlers():
+            warnings.warn("No logging handler defined (e.g. logging.basicConfig)")
+
     def __str__(self):
-        result = f"Cogment Context: user id = {self._user_id}"
+        result = f"Cogment Context: user id = {self._user_id}, served_port = {self.served_port}"
         return result
 
+    @property
+    def served_port(self):
+        return self._grpc_server_port
+
+    def has_specs(self):
+        return (self._cog_settings is not None)
+
     def register_actor(self,
                        impl: Callable[[ActorSession], Awaitable[None]],
                        impl_name: str,
                        actor_classes: List[str] = [], properties: Dict[str, str] = {}):
 
         if self._grpc_server is not None:
             # We could accept "client" actor registration after the server is started, but it is not worth it
@@ -248,62 +294,67 @@
             try:
                 await self._directory.deregister_service(*item)
             except Exception as exc:
                 logger.debug(f"Failed to deregister service id [{item[0]}] from directory: [{exc}]")
 
         registered.clear()
 
-    async def _directory_registration(self, port, ssl):
+    async def _directory_registration(self, host, port, ssl):
         registered: List[Tuple[int, str]] = []
 
         if self._directory is None:
             logger.debug(f"No directory for implicit service registration")
             return registered
 
-        socket_addr = socket.gethostbyname(socket.gethostname())
-        logger.debug(f"Registering services available here [{socket_addr}] to Directory")
+        if host is None:
+            host = _self_ip_address()
+            if not host:
+                logger.warning(f"Could not determine this host address for directory registration")
+                return registered
 
+        logger.debug(f"Registering services available here [{host}] to Directory")
         try:
             for actor in self._actor_impls.values():
                 properties = actor.properties
                 for actor_class in actor.actor_classes:
                     properties[ep.ACTOR_CLASS_PROPERTY_NAME] = actor_class
                     res = await self._directory.register_host(
-                        ServiceType.ACTOR, socket_addr, port, ssl, properties)
+                        ServiceType.ACTOR, host, port, ssl, properties)
                     registered.append(res)
 
             for env in self._env_impls.values():
                 res = await self._directory.register_host(
-                    ServiceType.ENVIRONMENT, socket_addr, port, ssl, env.properties)
+                    ServiceType.ENVIRONMENT, host, port, ssl, env.properties)
                 registered.append(res)
 
             if self._prehook_impl is not None:
                 res = await self._directory.register_host(
-                    ServiceType.HOOK, socket_addr, port, ssl, self._prehook_impl.properties)
+                    ServiceType.HOOK, host, port, ssl, self._prehook_impl.properties)
                 registered.append(res)
 
             if self._datalog_impl is not None:
                 res = await self._directory.register_host(
-                    ServiceType.DATALOG, socket_addr, port, ssl, self._datalog_impl.properties)
+                    ServiceType.DATALOG, host, port, ssl, self._datalog_impl.properties)
                 registered.append(res)
 
         except Exception:
             await self._directory_deregistration(registered)
             raise
 
         return registered
 
-    async def serve_all_registered(self, served_endpoint: ep.ServedEndpoint, prometheus_port=None):
+    async def serve_all_registered(self, served_endpoint: ep.ServedEndpoint = ep.ServedEndpoint(),
+                                   prometheus_port=None, directory_registration_host: str = None):
         if (len(self._actor_impls) == 0 and len(self._env_impls) == 0 and
                 self._prehook_impl is None and self._datalog_impl is None):
             raise CogmentError("Nothing registered to serve!")
         if self._grpc_server is not None:
             raise CogmentError("Cannot serve the same components twice")
 
-        self._grpc_server = _make_server(served_endpoint)
+        self._grpc_server, self._grpc_server_port = _make_server(served_endpoint)
 
         if self._actor_impls:
             servicer = AgentServicer(self._actor_impls, self._cog_settings, self._prometheus_registry)
             agent_grpc_api.add_ServiceActorSPServicer_to_server(servicer, self._grpc_server)
 
         if self._env_impls:
             servicer = EnvironmentServicer(self._env_impls, self._cog_settings, self._prometheus_registry)
@@ -317,21 +368,22 @@
             servicer = DatalogServicer(self._datalog_impl.impl, self._cog_settings)
             datalog_grpc_api.add_DatalogSPServicer_to_server(servicer, self._grpc_server)
 
         if self._prometheus_registry is not None and prometheus_port is not None:
             start_prometheus_server(prometheus_port, "", self._prometheus_registry)
 
         await self._grpc_server.start()
-        logger.debug(f"Context gRPC server at port [{served_endpoint.port}] for user [{self._user_id}] started")
+        logger.debug(f"Context gRPC server at port [{self._grpc_server_port}] for user [{self._user_id}] started")
 
-        directory_registered = await self._directory_registration(served_endpoint.port, served_endpoint.using_ssl())
+        directory_registered = await self._directory_registration(directory_registration_host, self._grpc_server_port,
+                                                                  served_endpoint.using_ssl())
 
         try:
             await self._grpc_server.wait_for_termination()
-            logger.debug(f"Context gRPC server at port [{served_endpoint.port}] for user [{self._user_id}] exited")
+            logger.debug(f"Context gRPC server at port [{self._grpc_server_port}] for user [{self._user_id}] exited")
 
         finally:
             await self._directory_deregistration(directory_registered)
 
     def _make_controller(self, endpoint):
         channel = _make_client_channel(endpoint)
         stub = orchestrator_grpc_api.TrialLifecycleSPStub(channel)
@@ -380,14 +432,18 @@
     # We may want to make it async to standardize with the future
     # versions of 'get_controller' and 'get_datastore'
     def get_directory(self, endpoint: ep.Endpoint, authentication_token: str = None):
         channel = _make_client_channel(endpoint)
         stub = directory_grpc_api.DirectorySPStub(channel)
         return Directory(stub, authentication_token)
 
+    # Undocumented
+    def get_context_directory(self):
+        return self._directory
+
     async def get_model_registry(self, endpoint=ep.Endpoint()):
         logger.deprecated(f"'get_model_registry' is deprecated, use 'get_model_registry_v2'")
         if self._directory is not None:
             endpoint = await self._directory.get_inquired_endpoint(endpoint, ServiceType.MODEL_REG)
 
         channel = _make_client_channel(endpoint)
         stub = model_registry_api.ModelRegistrySPStub(channel)
```

### Comparing `cogment-2.7.1/cogment/control.py` & `cogment-2.8.0/cogment/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,21 +35,29 @@
     TERMINATING = common_api.TrialState.TERMINATING
     ENDED = common_api.TrialState.ENDED
 
 
 class TrialInfo:
     """Class representing the details of a trial."""
 
-    def __init__(self, trial_id, api_state):
-        self.trial_id = trial_id
-        self.properties = {}
-        self.state = TrialState(api_state)
-        self.env_name = None
-        self.tick_id = None
-        self.duration = None
+    def __init__(self, trial_id, api_state, raw_info):
+        if raw_info is None:
+            self.trial_id = trial_id
+            self.state = TrialState(api_state)
+            self.properties = None
+            self.env_name = None
+            self.tick_id = None
+            self.duration = None
+        else:
+            self.trial_id = raw_info.trial_id
+            self.state = TrialState(raw_info.state)
+            self.properties = raw_info.properties
+            self.env_name = raw_info.env_name
+            self.tick_id = raw_info.tick_id
+            self.duration = raw_info.trial_duration
 
     def __str__(self):
         result = f"TrialInfo: trial_id = {self.trial_id}, properties = {self.properties}, env_name = {self.env_name}"
         result += f", state = {self.state}, tick_id = {self.tick_id}, duration = {self.duration}"
         return result
 
 
@@ -60,14 +68,17 @@
         self._lifecycle_stub = stub
         self._user_id = user_id
 
     def __str__(self):
         result = f"Controller: user id = {self._user_id}"
         return result
 
+    def has_specs(self):
+        return True  # This class does not rely on the spec
+
     async def get_actors(self, trial_id):
         req = orchestrator_api.TrialInfoRequest()
         req.get_actor_list = True
         metadata = [("trial-id", trial_id)]
         rep = await self._lifecycle_stub.GetTrialInfo(request=req, metadata=metadata)
         if len(rep.trial) == 0:
             raise CogmentError(f"Unknown trial [{trial_id}]")
@@ -83,15 +94,18 @@
     async def start_trial(self, trial_config=None, trial_id_requested=None, trial_params=None):
         req = orchestrator_api.TrialStartRequest()
         req.user_id = self._user_id
 
         if trial_config is not None:
             if trial_params is not None:
                 raise CogmentError(f"Cannot provide both a start config and start parameters")
-            req.config.content = trial_config.SerializeToString()
+            if type(trial_config) is not bytes:
+                req.config.content = trial_config.SerializeToString()
+            else:
+                req.config.content = trial_config
         elif trial_params is not None:
             req.params.CopyFrom(trial_params._raw_params)
             if trial_params._raw_params.HasField("trial_config"):
                 logger.warning(f"Trial config from trial parameters will be ignored")
 
         if trial_id_requested is not None:
             req.trial_id_requested = trial_id_requested
@@ -136,43 +150,42 @@
         elif type(trial_ids) == str:
             logger.deprecated("Using Controller.get_trial_info() with a string trial ID is deprecated.  Use a list.")
             metadata = [("trial-id", trial_ids)]
         else:
             metadata = []
             for id in trial_ids:
                 metadata.append(("trial-id", id))
-        rep = await self._lifecycle_stub.GetTrialInfo(request=req, metadata=metadata)
+        reply = await self._lifecycle_stub.GetTrialInfo(request=req, metadata=metadata)
 
         result = []
-        for reply in rep.trial:
-            info_ex = TrialInfo(reply.trial_id, reply.state)
-            info_ex.properties = reply.properties
-            info_ex.env_name = reply.env_name
-            info_ex.tick_id = reply.tick_id
-            info_ex.duration = reply.trial_duration
-
+        for info in reply.trial:
+            info_ex = TrialInfo(None, None, info)
             result.append(info_ex)
 
         return result
 
-    async def watch_trials(self, trial_state_filters=[]):
-        request = orchestrator_api.TrialListRequest()
+    async def watch_trials(self, trial_state_filters=[], full_info: bool = False):
+        request = orchestrator_api.TrialListRequest(full_info=full_info)
         for filter in trial_state_filters:
             if type(filter) != TrialState:
                 raise CogmentError(f"Unknown filter type [{type(filter)}]: must of type 'cogment.TrialState'")
             request.filter.append(filter.value)
 
         reply_itor = self._lifecycle_stub.WatchTrials(request=request)
         if not reply_itor:
             raise CogmentError(f"'watch_trials' failed to connect")
 
         try:
             async for reply in reply_itor:
-                info = TrialInfo(reply.trial_id, reply.state)
-                keep_looping = yield info
+                if reply.HasField("info"):
+                    info_ex = TrialInfo(None, None, reply.info)
+                else:
+                    info_ex = TrialInfo(reply.trial_id, reply.state, None)
+
+                keep_looping = yield info_ex
                 if keep_looping is not None and not bool(keep_looping):
                     break
 
         except grpc.aio.AioRpcError as exc:
             logger.debug(f"gRPC failed status details: [{exc.debug_error_string()}]")
             if exc.code() == grpc.StatusCode.UNAVAILABLE:
                 logger.error(f"Watch_trials Orchestrator communication lost: [{exc.details()}]")
```

### Comparing `cogment-2.7.1/cogment/datalog.py` & `cogment-2.8.0/cogment/datalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,27 +111,27 @@
     def get_actor_name(self, actor_index):
         return self._raw_params.actors[actor_index].name
 
     def get_actor(self, actor_index):
         actor = self._raw_params.actors[actor_index]
 
         actor_config = None
-        a_c = self._cog_settings.actor_classes.__getattribute__(actor.actor_class)
+        actor_class_spec = self._cog_settings.actor_classes.__getattribute__(actor.actor_class)
         if actor.HasField("config"):
-            actor_config = a_c.config_type()
+            actor_config = actor_class_spec.config_type()
             actor_config.ParseFromString(actor.config.content)
 
         actor_data = {
             "name": actor.name,
             "actor_class": actor.actor_class,
             "endpoint": actor.endpoint,
             "implementation": actor.implementation,
             "config": actor_config,
-            "action_space": a_c.action_space,
-            "observation_space": a_c.observation_space,
+            "action_space": actor_class_spec.action_space,
+            "observation_space": actor_class_spec.observation_space,
         }
 
         return actor_data
 
 
 class DatalogSession:
     """Class representing the session of a datalog for a trial."""
```

### Comparing `cogment-2.7.1/cogment/datalog_service.py` & `cogment-2.8.0/cogment/datalog_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 action_space = None
             else:
                 status = ActorStatus.ACTIVE
                 timestamp = data.timestamp
                 if self._log_params:
                     action_space = self._log_params.get_actor(actor_index)["action_space"]()
                 else:
-                    action_space = self._parameters.actors[actor_index]._actor_class.action_space()
+                    action_space = self._parameters.actors[actor_index].actor_class_spec.action_space()
                 action_space.ParseFromString(data.content)
 
             return RecvAction(actor_index, data.tick_id, status, timestamp, action_space)
 
         else:
             return None
 
@@ -161,15 +161,15 @@
             raise CogmentError(f"Wrong type of actor parameter [{type(actor)}]: must be int or str")
         if actor_index is None or actor_index < 0 or actor_index >= self._nb_actors:
             raise CogmentError(f"Invalid actor [{actor}] [{actor_index}]")
 
         if self._log_params:
             obs_space = self._log_params.get_actor(actor_index)["observation_space"]()
         else:
-            obs_space = self._parameters.actors[actor_index]._actor_class.observation_space()
+            obs_space = self._parameters.actors[actor_index].actor_class_spec.observation_space()
 
         if self._raw_sample.HasField("observations"):
             data = self._raw_sample.observations
             obs_index = data.actors_map[actor_index]
             obs_content = data.observations[obs_index]
             obs_space.ParseFromString(obs_content)
             return RecvObservation(data, obs_space)
@@ -234,16 +234,15 @@
             user_id = metadata["user-id"]
 
             request = await context.read()
 
             if not request.HasField("trial_params"):
                 raise CogmentError(f"Initial data log request for [{trial_id}] does not contain parameters.")
 
-            trial_parameters = TrialParameters(None)
-            trial_parameters._set(self._cog_settings, request.trial_params)
+            trial_parameters = TrialParameters(self._cog_settings, raw_params=request.trial_params)
 
             session = DatalogSession(self._impl, trial_id, user_id, trial_parameters)
             user_task = session._start_user_task()
 
             reader_task = asyncio.create_task(_read_sample(context, session, self._cog_settings))
 
             normal_return = await user_task
```

### Comparing `cogment-2.7.1/cogment/datastore.py` & `cogment-2.8.0/cogment/datastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,24 +48,26 @@
 
     def __init__(self, cog_settings, info: datastore_api.StoredTrialInfo):
         self.trial_id = info.trial_id
         self.trial_state = TrialState(info.last_state)
         self.user_id = info.user_id
         self.sample_count = info.samples_count
 
-        self.parameters = TrialParameters(None)
-        self.parameters._set(cog_settings, info.params)
+        self.parameters = TrialParameters(cog_settings, raw_params=info.params)
 
     def __str__(self):
         result = f"DatastoreTrialInfo:"
         result += f" trial_id = {self.trial_id}, trial_state = {self.trial_state}"
         result += f", user_id = {self.user_id}, sample_count = {self.sample_count}"
         result += f", parameters = {self.parameters}"
         return result
 
+    def has_specs(self):
+        return self.parameters.has_specs()
+
 
 class DatastoreReward:
     """Class representing an individual reward sent during this sample."""
 
     def __init__(self, reward, payloads, parameters: TrialParameters):
         self._raw_reward = reward
         self._payloads = payloads
@@ -159,49 +161,73 @@
         result += f", observation = {self.observation}, action = {self.action}"
         result += f", nb received rewards = {len(self._raw_sample.received_rewards)}"
         result += f", nb sent rewards = {len(self._raw_sample.sent_rewards)}"
         result += f", nb received messages = {len(self._raw_sample.received_messages)}"
         result += f", nb sent messages = {len(self._raw_sample.sent_messages)}"
         return result
 
+    def has_specs(self):
+        # If the trial parameters have spec, the actor's should have spec
+        return self._parameters.has_specs()
+
     @property
     def name(self):
         """Name of the actor"""
         actor_index = self._raw_sample.actor
         return self._parameters.actors[actor_index].name
 
     @property
     def observation(self):
-        """Observation space to the actor"""
+        """Observation for the actor"""
         if self._raw_sample.HasField("observation"):
             actor_index = self._raw_sample.actor
-            obs_space = self._parameters.actors[actor_index]._actor_class.observation_space()
+            obs_space = self._parameters.actors[actor_index].actor_class_spec.observation_space()
 
             obs_index = self._raw_sample.observation
             obs_content = self._payloads[obs_index]
             obs_space.ParseFromString(obs_content)
             return obs_space
         else:
             return None
 
     @property
+    def observation_serialized(self):
+        """Serialized observation for the actor"""
+        if self._raw_sample.HasField("observation"):
+            obs_index = self._raw_sample.observation
+            obs_content = self._payloads[obs_index]
+            return obs_content
+        else:
+            return None
+
+    @property
     def action(self):
-        """Action space from the actor"""
+        """Action of the actor"""
         if self._raw_sample.HasField("action"):
             actor_index = self._raw_sample.actor
-            action_space = self._parameters.actors[actor_index]._actor_class.action_space()
+            action_space = self._parameters.actors[actor_index].actor_class_spec.action_space()
 
             action_index = self._raw_sample.action
             action_content = self._payloads[action_index]
             action_space.ParseFromString(action_content)
             return action_space
         else:
             return None
 
     @property
+    def action_serialized(self):
+        """Serialized action of the actor"""
+        if self._raw_sample.HasField("action"):
+            action_index = self._raw_sample.action
+            action_content = self._payloads[action_index]
+            return action_content
+        else:
+            return None
+
+    @property
     def reward(self):
         """Aggregated reward received by the actor"""
         if self._raw_sample.HasField("reward"):
             return self._raw_sample.reward
         else:
             return 0.0
 
@@ -245,58 +271,64 @@
         utc_time = datetime.datetime.utcfromtimestamp(self.timestamp * _REV_NANO)
         result = f"DatastoreSample:"
         result += f" trial_id = {self.trial_id}, trial_state = {self.trial_state}"
         result += f", tick_id = {self.tick_id}, timestamp = {self.timestamp} UTC[{utc_time}]"
         result += f", nb actors = {len(self.actors_data)}"
         return result
 
+    def has_specs(self):
+        return self._parameters.has_specs()
+
 
 class Datastore:
     """Class representing the session of a datalog for a trial."""
 
     def __init__(self, stub, cog_settings):
         self._datastore_stub = stub
         self._cog_settings = cog_settings
-        self._timeout = 0
 
     def __str__(self):
         result = f"Datastore"
         return result
 
-    async def all_trials(self, bundle_size=1, wait_for_trials=0):
+    def has_specs(self):
+        return (self._cog_settings is not None)
+
+    async def all_trials(self, bundle_size=1, wait_for_trials=0, properties={}, ids=[]):
         request = datastore_api.RetrieveTrialsRequest()
         request.timeout = int(wait_for_trials * 1000)
         request.trials_count = bundle_size
         request.trial_handle = ""
+        request.properties.update(properties)
+        request.trial_ids.extend(ids)
 
         while True:
             reply = await self._datastore_stub.RetrieveTrials(request)
 
-            for rep_info in reply.trial_infos:
-                info = DatastoreTrialInfo(self._cog_settings, rep_info)
+            for reply_info in reply.trial_infos:
+                info = DatastoreTrialInfo(self._cog_settings, reply_info)
                 yield info
 
             if len(reply.trial_infos) < bundle_size:
                 break
             if reply.next_trial_handle:
                 request.trial_handle = reply.next_trial_handle
             else:
                 break
 
-    async def get_trials(self, ids):
+    async def get_trials(self, ids=[], properties={}):
         request = datastore_api.RetrieveTrialsRequest()
-        request.timeout = self._timeout
-        for id in ids:
-            request.trial_ids.append(id)
+        request.properties.update(properties)
+        request.trial_ids.extend(ids)
 
         reply = await self._datastore_stub.RetrieveTrials(request)
 
         trial_infos = []
-        for rep_info in reply.trial_infos:
-            info = DatastoreTrialInfo(self._cog_settings, rep_info)
+        for reply_info in reply.trial_infos:
+            info = DatastoreTrialInfo(self._cog_settings, reply_info)
             trial_infos.append(info)
 
         return trial_infos
 
     async def delete_trials(self, ids):
         if not ids:
             raise CogmentError("At least one trial ID must be provided to delete")
```

### Comparing `cogment-2.7.1/cogment/directory.py` & `cogment-2.8.0/cogment/directory.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/endpoints.py` & `cogment-2.8.0/cogment/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             logger.error(f"Failed loading file from CWD: {os.getcwd()}")
             raise
 
 
 class ServedEndpoint:
     """Class representing a local Cogment endpoint where others can connect."""
 
-    def __init__(self, port: int):
+    def __init__(self, port: int = 0):
         if type(port) == str:
             logger.deprecated(f"'ServedEndpoint' port should be an integer, not a string")  # type: ignore
             self.port = int(port)
         else:
             self.port = port
         self.private_key_certificate_chain_pairs: List[Tuple[str, str]] = None
         self.root_certificates: str = None
```

### Comparing `cogment-2.7.1/cogment/env_service.py` & `cogment-2.8.0/cogment/env_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             if index in act_set.unavailable_actors:
                 status = ActorStatus.UNAVAILABLE
                 timestamp = 0
                 action = None
             else:
                 status = ActorStatus.ACTIVE
                 timestamp = act_set.timestamp
-                action = actor.actor_class.action_space()
+                action = actor.actor_class_spec.action_space()
                 action.ParseFromString(act_set.actions[index])
 
             recv_event.actions.append(RecvAction(index, act_set.tick_id, status, timestamp, action))
 
         session._post_incoming_event((tick_id, recv_event))
 
     elif data.HasField("message"):
```

### Comparing `cogment-2.7.1/cogment/environment.py` & `cogment-2.8.0/cogment/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,32 +92,32 @@
                     if "." not in target:
                         if actor.name == target:
                             if new_obs[actor_index] is not None:
                                 raise CogmentError(f"Duplicate actor [{actor.name}] in observations list")
                             new_obs[actor_index] = obs
                             break  # Names are unique in trial
                     else:
-                        class_name, actor_name = target.split(".")
-                        if class_name == actor.actor_class.name:
+                        actor_class, actor_name = target.split(".")
+                        if actor_class == actor.actor_class_spec.name:
                             if actor_name == actor.name or actor_name == "*":
                                 if new_obs[actor_index] is not None:
-                                    raise CogmentError(f"Duplicate actor [{class_name}.{actor.name}] "
+                                    raise CogmentError(f"Duplicate actor [{actor_class}.{actor.name}] "
                                                        f"in observations list")
                                 new_obs[actor_index] = obs
 
         for actor_index, actor in enumerate(self._trial.actors):
             if new_obs[actor_index] is None:
                 raise CogmentError(f"Actor [{actor.name}] is missing an observation")
 
         package = env_api.ObservationSet()
         package.tick_id = tick_id
         package.timestamp = timestamp
 
         seen_observations = {}
-        for actor_index, actor in enumerate(self._trial.actors):
+        for actor_index, _ in enumerate(self._trial.actors):
             actor_obs = new_obs[actor_index]
             obs_id = id(actor_obs)
             obs_key = seen_observations.get(obs_id)
             if obs_key is None:
                 obs_key = len(package.observations)
 
                 package.observations.append(actor_obs.SerializeToString())
```

### Comparing `cogment-2.7.1/cogment/errors.py` & `cogment-2.8.0/cogment/errors.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/generate.py` & `cogment-2.8.0/cogment/generate.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/hooks_service.py` & `cogment-2.8.0/cogment/hooks_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             session.environment_endpoint = None
             session.environment_name = None
             session.environment_implementation = None
 
         session.actors = []
         for actor in proto_params.actors:
             if actor.HasField("config"):
-                a_c = self._cog_settings.actor_classes.__getattribute__(actor.actor_class)
-                actor_config = a_c.config_type()
+                actor_class_spec = getattr(self._cog_settings.actor_classes, actor.actor_class)
+                actor_config = actor_class_spec.config_type()
                 actor_config.ParseFromString(actor.config.content)
             else:
                 actor_config = None
             actor_name = actor.name
             actor_class = actor.actor_class
             actor_endpoint = actor.endpoint
             actor_implementation = actor.implementation
@@ -133,16 +133,15 @@
             metadata = dict(context.invocation_metadata())
             logger.debug(f"Received metadata: [{metadata}]")
             trial_id = metadata["trial-id"]
             user_id = metadata["user-id"]
 
             trial = Trial(trial_id, [], self._cog_settings)
 
-            trial_parameters = TrialParameters(None)
-            trial_parameters._set(self._cog_settings, request.params)
+            trial_parameters = TrialParameters(self._cog_settings, raw_params=request.params)
 
             session = PrehookSession(trial, user_id, trial_parameters)
             self._decode(session, request.params)
 
             try:
                 await self._impl(session)
                 session.validate()
```

### Comparing `cogment-2.7.1/cogment/model_registry.py` & `cogment-2.8.0/cogment/model_registry.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/model_registry_v2.py` & `cogment-2.8.0/cogment/model_registry_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,17 @@
     def __init__(self, stub, endpoint_url):
         self._model_registry_stub = stub
         self._endpoint_url = endpoint_url
 
     def __str__(self):
         return "ModelRegistry"
 
+    def has_specs(self):
+        return True  # This class does not rely on the spec
+
     async def store_model(self,
             name: str, model: bytes, iteration_properties: Dict[str, str] = None) -> ModelIterationInfo:
         return await self._send_model(name, model, iteration_properties, True)
 
     async def publish_model(self,
             name: str, model: bytes, iteration_properties: Dict[str, str] = None) -> ModelIterationInfo:
         return await self._send_model(name, model, iteration_properties, False)
```

### Comparing `cogment-2.7.1/cogment/parameters.py` & `cogment-2.8.0/cogment/parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,73 +17,118 @@
 from cogment.errors import CogmentError
 from cogment.utils import logger
 
 
 class ActorParameters:
     """Class wrapping the trial api parameters for an actor"""
 
-    def __init__(self, cog_settings, class_name, **kwargs):
-        # Done not to waste resources for internal use with a '_set' call
-        if cog_settings is not None:
-            self._cog_settings = cog_settings
-            self._raw_params = common_api.ActorParams()
+    _METHODS = ["has_specs"]
 
-            if class_name is None:
-                raise CogmentError(f"Required attribute 'class_name' missing")
+    def __init__(self, cog_settings, class_name=None, **kwargs):
+        self._cog_settings = cog_settings
+
+        if "raw_params" in kwargs:
+            self._raw_params = kwargs["raw_params"]
+            return
+
+        self._raw_params = common_api.ActorParams()
+
+        if class_name is not None:
             if type(class_name) is not str:
                 raise CogmentError(f"Wrong type for 'class_name' [{type(class_name)}]")
             self._raw_params.actor_class = class_name
-
-            # Provide an easy way for users to set parameter attributes on construction
-            for name, value in kwargs.items():
-                if name[0] == "_" or name not in dir(self):
-                    raise CogmentError(f"Unknown attribute [{name}]")
-                setattr(self, name, value)
-
-    def _set(self, cog_settings, raw_params):
-        self._cog_settings = cog_settings
-        self._raw_params = raw_params
+        else:
+            if "actor_class" not in kwargs:
+                raise CogmentError(f"Required attribute 'actor_class' missing")
+            self._raw_params.actor_class = kwargs["actor_class"]
+
+        # Provide an easy way for users to set parameter attributes on construction
+        for name, value in kwargs.items():
+            if name[0] == "_" or name in self._METHODS or name not in dir(self):
+                raise CogmentError(f"Unknown attribute [{name}]")
+            setattr(self, name, value)
 
     def __str__(self):
         result = f"ActorParameters: {self._raw_params}"
         return result
 
+    def has_specs(self):
+        return (self._cog_settings is not None)
+
     # ----------------- properties -------------------
 
     @property
     def config(self):
         """Config sent to actor on trial start"""
         if self._raw_params.HasField("config"):
-            config_instance = self._actor_class.config_type()
+            if self._cog_settings is None:
+                raise CogmentError(f"Unknown type to return (no 'cog_settings')")
+
+            config_instance = self.actor_class_spec.config_type()
             config_instance.ParseFromString(self._raw_params.config.content)
         else:
             config_instance = None
 
         return config_instance
 
     @config.setter
     def config(self, val):
         if val is None:
             self._raw_params.ClearField("config")
-        elif type(val) is self._actor_class.config_type:
+        else:
+            if self._cog_settings is not None:
+                if type(val) is not self.actor_class_spec.config_type:
+                    raise CogmentError(f"Wrong type [{type(val)}]")
+
             self._raw_params.config.content = val.SerializeToString()
+
+    @property
+    def config_serialized(self):
+        """Config sent to actor on trial start in raw serialized format"""
+        if self._raw_params.HasField("config"):
+            return self._raw_params.config.content
         else:
-            raise CogmentError(f"Wrong type [{type(val)}]")
+            return None
+
+    @config_serialized.setter
+    def config_serialized(self, val: bytes):
+        if val is None:
+            self._raw_params.ClearField("config")
+        else:
+            self._raw_params.config.content = val
 
     @property
     def class_name(self):
         """Name of the actor class"""
         return self._raw_params.actor_class
 
     @class_name.setter
     def class_name(self, val):
         # We could make a setter, but we would have to sync with the config and default_action: not worth it.
         raise CogmentError(f"Cannot change class name of existing instance of ActorParameters")
 
     @property
+    def actor_class(self):
+        """Class of the actor (defined in spec)"""
+        return self._raw_params.actor_class
+
+    @actor_class.setter
+    def actor_class(self, val):
+        if self._cog_settings is not None:
+            # We could make a setter, but we would have to sync with the config and default_action: not worth it.
+            raise CogmentError(f"Cannot change actor class of existing instance of ActorParameters")
+
+        if val is None or len(val) == 0:
+            raise CogmentError(f"Cannot reset required actor class")
+        elif type(val) is str:
+            self._raw_params.actor_class = val
+        else:
+            raise CogmentError(f"Wrong type [{type(val)}]")
+
+    @property
     def name(self):
         """Name of the actor"""
         return self._raw_params.name
 
     @name.setter
     def name(self, val):
         if val is None:
@@ -159,81 +204,121 @@
         else:
             raise CogmentError(f"Wrong type [{type(val)}]")
 
     @property
     def default_action(self):
         """The default action space for optional actors not connected"""
         if self._raw_params.HasField("default_action"):
-            action_space = self._actor_class.action_space()
+            if self._cog_settings is None:
+                raise CogmentError(f"Unknown type to return (no 'cog_settings')")
+
+            action_space = self.actor_class_spec.action_space()
             action_space.ParseFromString(self._raw_params.default_action.content)
         else:
             action_space = None
 
         return action_space
 
     @default_action.setter
     def default_action(self, val):
         if val is None:
             self._raw_params.ClearField("default_action")
-        elif type(val) is self._actor_class.action_space:
+        else:
+            if self._cog_settings is not None:
+                if type(val) is not self.actor_class_spec.action_space:
+                    raise CogmentError(f"Wrong type [{type(val)}]")
+
             self._raw_params.default_action.content = val.SerializeToString()
+
+    @property
+    def default_action_serialized(self):
+        """The default action space for optional actors not connected, in raw serialized format"""
+        if self._raw_params.HasField("default_action"):
+            return self._raw_params.default_action.content
         else:
-            raise CogmentError(f"Wrong type [{type(val)}]")
+            return None
+
+    @default_action_serialized.setter
+    def default_action_serialized(self, val: bytes):
+        if val is None:
+            self._raw_params.ClearField("default_action")
+        else:
+            self._raw_params.default_action.content = val
 
     @property
-    def _actor_class(self):
-        return getattr(self._cog_settings.actor_classes, self._raw_params.actor_class)
+    def actor_class_spec(self):
+        if self._cog_settings is not None:
+            return self._cog_settings.actor_classes[self._raw_params.actor_class]
+        else:
+            raise CogmentError(f"Unknown actor class spec (no 'cog_settings' available)")
 
 
 class _ActorsList:
     """List like object to manage actor parameters"""
 
     def __init__(self, cog_settings, raw_params):
         self._cog_settings = cog_settings
         self._raw_params = raw_params
 
+        # dict(actor name : actor index)
+        # This is not perfect, if the name of actors change, this will become
+        # out of date. And creating a back reference is not an option here.
+        # We also don't want to do a search for every call as it would be very
+        # inefficient for current use case in enterprise.
+        self._actor_indexes = None
+
     def __str__(self):
         result = f"Actors Parameters: {self._raw_params.actors}"
         return result
 
     def __len__(self):
         return len(self._raw_params.actors)
 
     def __getitem__(self, key):
         if type(key) is int:
-            actor_params = ActorParameters(None, None)
-            actor_params._set(self._cog_settings, self._raw_params.actors[key])
+            actor_params = ActorParameters(self._cog_settings, raw_params=self._raw_params.actors[key])
+
         elif type(key) is slice:
             actor_params = []
             actors = self._raw_params.actors
             for actual_index in range(len(actors))[key]:
-                params = ActorParameters(None, None)
-                params._set(self._cog_settings, actors[actual_index])
+                params = ActorParameters(self._cog_settings, raw_params=actors[actual_index])
                 actor_params.append(params)
+
+        elif type(key) is str:
+            if self._actor_indexes is None:
+                self._actor_indexes = {actor.name : index for index, actor in enumerate(self._raw_params.actors)}
+
+            actor_index = self._actor_indexes.get(key)
+            if actor_index is None:
+                raise CogmentError(f"Unknown actor name [{key}]")
+            actor_params = ActorParameters(self._cog_settings, raw_params=self._raw_params.actors[actor_index])
+
         else:
             raise CogmentError(f"Wrong key type [{type(key)}]")
 
         return actor_params
 
     def __setitem__(self, key, val):
         if type(key) is int and type(val) is ActorParameters:
             self._raw_params.actors[key].CopyFrom(val._raw_params)
+            self._actor_indexes = None
         elif type(key) is slice:
             # Complicated for very little gain
             raise CogmentError(f"Slices are not valid for setting")
         else:
             raise CogmentError(f"Wrong type [{type(key)}] [{type(val)}]")
 
     def __delitem__(self, key):
         del self._raw_params.actors[key]
+        self._actor_indexes = None
 
     def __iter__(self):
         for raw_actor in self._raw_params.actors:
-            actor_params = ActorParameters(None, None)
-            actor_params._set(self._cog_settings, raw_actor)
+            actor_params = ActorParameters(self._cog_settings, raw_params=raw_actor)
             yield actor_params
 
     def append(self, val):
         if type(val) is ActorParameters:
             self._raw_params.actors.append(val._raw_params)
         else:
             raise CogmentError(f"Wrong type [{type(val)}]")
@@ -245,40 +330,40 @@
                 raise CogmentError(f"Wrong type [{type(actor)}]")
             raw_list.append(actor._raw_params)
 
         self._raw_params.actors.extend(raw_list)
 
     def clear(self):
         self._raw_params.ClearField("actors")
+        self._actor_indexes = None
 
 
 class TrialParameters:
     """Class wrapping the api parameters of a trial"""
 
-    _SERIALIZATION_TYPE = 2
-    _METHODS = ["get_serialization_type", "serialize", "deserialize"]
+    _SERIALIZATION_TYPE = 3
+    _METHODS = ["get_serialization_type", "serialize", "deserialize", "has_specs"]
 
     def __init__(self, cog_settings, **kwargs):
-        # Done not to waste resources for internal use with a '_set' call
-        if cog_settings is not None:
-            self._cog_settings = cog_settings
-            self._raw_params = common_api.TrialParams()
+        self._cog_settings = cog_settings
+
+        if "raw_params" in kwargs:
+            self._raw_params = kwargs["raw_params"]
             self._actors = _ActorsList(cog_settings, self._raw_params)
+            return
 
-            # Provide an easy way for users to set parameter attributes on construction
-            for name, value in kwargs.items():
-                # TODO: We could also protect the methods
-                if name[0] == "_" or name in self._METHODS or name not in dir(self):
-                    raise CogmentError(f"Unknown attribute [{name}]")
-                setattr(self, name, value)
+        self._raw_params = common_api.TrialParams()
+        self._actors = _ActorsList(cog_settings, self._raw_params)
 
-    def _set(self, cog_settings, raw_params):
-        self._cog_settings = cog_settings
-        self._raw_params = raw_params
-        self._actors = _ActorsList(cog_settings, raw_params)
+        # Provide an easy way for users to set parameter attributes on construction
+        for name, value in kwargs.items():
+            # TODO: We could also protect the methods
+            if name[0] == "_" or name in self._METHODS or name not in dir(self):
+                raise CogmentError(f"Unknown attribute [{name}]")
+            setattr(self, name, value)
 
     def __str__(self):
         result = f"TrialParameters: {self._raw_params}"
         return result
 
     # Type of serialized data being produced and consumed by this class.
     # This is dependent on all the underlying protobuf messages used to
@@ -298,38 +383,58 @@
 
         params = common_api.TrialParams()
         params.ParseFromString(raw_string)
 
         self._raw_params = params
         self._actors = _ActorsList(self._cog_settings, params)
 
+    def has_specs(self):
+        return (self._cog_settings is not None)
+
     # ----------------- properties -------------------
 
     # Trial
     @property
     def config(self):
         """Config for initial trial setup by pre-trial hooks"""
         if self._raw_params.HasField("trial_config"):
+            if self._cog_settings is None:
+                raise CogmentError(f"Unknown type to return (no 'cog_settings')")
+
             config_instance = self._cog_settings.trial.config_type()
             config_instance.ParseFromString(self._raw_params.trial_config.content)
         else:
             config_instance = None
 
         return config_instance
 
     @config.setter
     def config(self, val):
         if val is None:
             self._raw_params.ClearField("trial_config")
+        else:
+            if self._cog_settings is not None and not isinstance(val, self._cog_settings.trial.config_type):
+                raise CogmentError(f"Wrong type [{type(val)}]")
 
-        elif isinstance(val, self._cog_settings.trial.config_type):
             self._raw_params.trial_config.content = val.SerializeToString()
 
+    @property
+    def config_serialized(self):
+        """Config for initial trial setup by pre-trial hooks in raw serialized format"""
+        if self._raw_params.HasField("trial_config"):
+            return self._raw_params.trial_config.content
         else:
-            raise CogmentError(f"Wrong type [{type(val)}]")
+            return None
+
+    @config_serialized.setter
+    def config_serialized(self, val: bytes):
+        if val is None:
+            self._raw_params.ClearField("trial_config")
+        else:
+            self._raw_params.trial_config.content = val
 
     @property
     def properties(self):
         """User properties associated with the trial"""
         return self._raw_params.properties
 
     @properties.setter
@@ -415,31 +520,48 @@
             self._raw_params.datalog.exclude_fields.extend(raw_fields)
 
     # Environment
     @property
     def environment_config(self):
         """Config sent to environment on trial start"""
         if(self._raw_params.environment.HasField("config")):
+            if self._cog_settings is None:
+                raise CogmentError(f"Unknown type to return (no 'cog_settings')")
+
             config_instance = self._cog_settings.environment.config_type()
             config_instance.ParseFromString(self._raw_params.environment.config.content)
         else:
             config_instance = None
 
         return config_instance
 
     @environment_config.setter
     def environment_config(self, val):
         if val is None:
             self._raw_params.environment.ClearField("config")
+        else:
+            if self._cog_settings is not None and not isinstance(val, self._cog_settings.environment.config_type):
+                raise CogmentError(f"Wrong type [{type(val)}]")
 
-        elif isinstance(val, self._cog_settings.environment.config_type):
             self._raw_params.environment.config.content = val.SerializeToString()
 
+    @property
+    def environment_config_serialized(self):
+        """Config sent to environment on trial start in raw serialized format"""
+        if(self._raw_params.environment.HasField("config")):
+            return self._raw_params.environment.config.content
         else:
-            raise CogmentError(f"Wrong type [{type(val)}]")
+            return None
+
+    @environment_config_serialized.setter
+    def environment_config_serialized(self, val: bytes):
+        if val is None:
+            self._raw_params.environment.ClearField("config")
+        else:
+            self._raw_params.environment.config.content = val
 
     @property
     def environment_name(self):
         """Name of the environment"""
         return self._raw_params.environment.name
 
     @environment_name.setter
@@ -483,13 +605,16 @@
     @property
     def actors(self):
         """Parameters for all actors of the trial"""
         return self._actors
 
     @actors.setter
     def actors(self, val):
-        for param in val:
-            if type(param) is not ActorParameters:
-                raise CogmentError(f"Wrong type for actor parameter [{type(param)}]")
+        if val is None:
+            self._actors.clear()
+        else:
+            for param in val:
+                if type(param) is not ActorParameters:
+                    raise CogmentError(f"Wrong type for actor parameter [{type(param)}]")
 
-        self._actors.clear()
-        self._actors.extend(val)
+            self._actors.clear()
+            self._actors.extend(val)
```

### Comparing `cogment-2.7.1/cogment/prehook.py` & `cogment-2.8.0/cogment/prehook.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/cogment/session.py` & `cogment-2.8.0/cogment/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     """Internal class to signal acknowledgement of the ending."""
     pass
 
 
 class ActorInfo:
     """Class representing the information of an actor."""
 
-    def __init__(self, name, class_name):
+    def __init__(self, name, actor_class):
         self.actor_name = name
-        self.actor_class_name = class_name
+        self.actor_class_name = actor_class
 
     def __str__(self):
         result = f"ActorInfo: actor_name = {self.actor_name}, actor_class_name = {self.actor_class_name}"
         return result
 
 
 class RecvObservation:
@@ -200,15 +200,15 @@
         self._started = False
         self._last_tick_delivered = -1
         self._last_event_delivered = False
         self._user_task = None  # Task used to call user implementation
         self._auto_ack = True
 
         # Pre-compute since it will be used regularly
-        self._active_actors = [ActorInfo(actor.name, actor.actor_class.name) for actor in trial.actors]
+        self._active_actors = [ActorInfo(actor.name, actor.actor_class_spec.name) for actor in trial.actors]
 
     def __str__(self):
         result = f"Session: name = {self.name}, impl_name = {self.impl_name}, config = {self.config}"
         result += f", trial = {self._trial}"
         return result
 
     def _start(self, auto_done_sending):
@@ -231,15 +231,15 @@
             return True
 
         except asyncio.CancelledError as exc:
             logger.debug(f"[{self.name}] implementation coroutine cancelled: [{exc}]")
             return False
 
         except Exception:
-            logger.exception(f"An exception occured in user implementation of [{self.name}]")
+            logger.exception(f"An exception occurred in user implementation of [{self.name}]")
             raise
 
     def _start_user_task(self):
         self._user_task = asyncio.create_task(self._run())
         return self._user_task
 
     def _post_incoming_event(self, event_tuple):
```

### Comparing `cogment-2.7.1/cogment/trial.py` & `cogment-2.8.0/cogment/trial.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 
 
 class Trial:
     """Internal class maintaining the information of a trial."""
 
     class Actor:
         """Internal class maintaining the information of an actor in a trial."""
-        def __init__(self, name, actor_class):
+        def __init__(self, name, actor_class_spec):
             self.name = name
-            self.actor_class = actor_class
+            self.actor_class_spec = actor_class_spec
 
     def __init__(self, id, actors_in_trial, cog_settings):
         self.id = id
         self.ended = False
         self.ending = False
         self.ending_ack = False
         self.cog_settings = cog_settings
         self.tick_id = -1
 
         self.actors = []
         for actor in actors_in_trial:
             if actor.actor_class not in self.cog_settings.actor_classes:
                 raise CogmentError(f"class [{actor.actor_class}] of actor [{actor.name}] cannot be found.")
-            actor_class = self.cog_settings.actor_classes[actor.actor_class]
-            new_actor = self.Actor(name=actor.name, actor_class=actor_class)
+            actor_class_spec = self.cog_settings.actor_classes[actor.actor_class]
+            new_actor = self.Actor(name=actor.name, actor_class_spec=actor_class_spec)
             self.actors.append(new_actor)
 
     def __str__(self):
         result = f"Trial: id = {self.id}, tick_id = {self.tick_id}, ended = {self.ended}"
         result += f", actors = "
         for actor in self.actors:
-            result += f"{{name = {actor.name}, class = {actor.actor_class.name}}},"
+            result += f"{{name = {actor.name}, class = {actor.actor_class_spec.name}}},"
         return result
```

### Comparing `cogment-2.7.1/cogment/utils.py` & `cogment-2.8.0/cogment/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,30 +32,39 @@
 def _logger_deprecated(self, msg):
     """Log deprecation as warning but only once"""
     if msg not in self.DEPRECATED_LOGGED:
         self.warning(msg)
         self.DEPRECATED_LOGGED.add(msg)
 
 
-# `logger` type is set to `Any` to stop pylint from complaining
-# about: '"Logger" has no attribute "deprecated"'. Similarly for "trace".
-logger: typing.Any = logging.getLogger("cogment.sdk")
-setattr(logger, "TRACE", 5)  # We don't want a new global level name (i.e. with 'logging.addLevelName')
-setattr(logger, "trace", types.MethodType(_logger_trace, logger))
-setattr(logger, "DEPRECATED_LOGGED", set())
-setattr(logger, "deprecated", types.MethodType(_logger_deprecated, logger))
-
-_COGMENT_LOG_LEVEL = os.environ.get("COGMENT_LOG_LEVEL", "INFO").upper()
-if _COGMENT_LOG_LEVEL == "OFF":
-    logger.setLevel(logging.CRITICAL)
-elif _COGMENT_LOG_LEVEL == "TRACE":
-    logger.setLevel(logger.TRACE)
-else:
-    logger.setLevel(_COGMENT_LOG_LEVEL)
-logger.addHandler(logging.NullHandler())
+def make_logger(name, env_name=None, default_level="INFO"):
+    # `logger` type is set to `Any` to stop pylint from complaining
+    # about: '"Logger" has no attribute "deprecated"'. Similarly for "trace".
+    logger: typing.Any = logging.getLogger(name)
+    setattr(logger, "TRACE", 5)  # We don't want a new global level name (i.e. with 'logging.addLevelName')
+    setattr(logger, "trace", types.MethodType(_logger_trace, logger))
+    setattr(logger, "DEPRECATED_LOGGED", set())
+    setattr(logger, "deprecated", types.MethodType(_logger_deprecated, logger))
+
+    if env_name is not None:
+        log_level = os.environ.get(env_name, default_level).upper()
+    else:
+        log_level = default_level.upper()
+
+    if log_level == "OFF":
+        logger.setLevel(logging.CRITICAL)
+    elif log_level == "TRACE":
+        logger.setLevel(logger.TRACE)
+    else:
+        logger.setLevel(log_level)
+
+    return logger
+
+
+logger = make_logger("cogment.sdk", "COGMENT_LOG_LEVEL")
 
 
 # Timeout (in seconds) for the init data to come from the Orchestrator before we consider a failure.
 INIT_TIMEOUT = 30
 
 
 def list_versions():
```

### Comparing `cogment-2.7.1/cogment/version.py` & `cogment-2.8.0/cogment/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # no import: add a comment to please linters
 
-__version__ = "2.7.1"
+__version__ = "2.8.0"
```

### Comparing `cogment-2.7.1/cogment.egg-info/PKG-INFO` & `cogment-2.8.0/cogment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogment
-Version: 2.7.1
+Version: 2.8.0
 Summary: Cogment python SDK
 Author-email: Artificial Intelligence Redefined <dev+cogment@ai-r.com>
 Project-URL: Homepage, https://cogment.ai
 Project-URL: repository, https://github.com/cogment/cogment-py-sdk
 Project-URL: Reference Documentation, https://cogment.ai/docs/reference/python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -134,14 +134,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.0 - 2023-04-21
+
+### Added
+
+- Option to request full info (not just id and state) from 'watch_trials'
+- Ability to use the SDK without spec (cog_settings)
+- Automatic port selection for 'Context.serve_all_registered()'
+- Ability to specify an explicit host to register a service to the directory
+- Ability to specify trial properties for 'Datastore.all_trials()' and 'Datastore.get_trials()'
+- Ability to specify trial ids for 'Datastore.all_trials()'
+
+### Changed
+
+- Enable warning and error logging even if user did not define a logging handler
+- Warn user when no logging handler is defined (i.e. proper logging is disabled)
+- Better self IP address discovery functionality
+
 ## v2.7.1 - 2023-03-06
 
 ## Fixed
 
 - Deadlock in 'wait_for_newer' method of LatestModel
 
 ## v2.7.0 - 2023-02-28
```

### Comparing `cogment-2.7.1/cogment.egg-info/SOURCES.txt` & `cogment-2.8.0/cogment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/pyproject.toml` & `cogment-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/setup.py` & `cogment-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/tests/test_download_cogment.py` & `cogment-2.8.0/tests/test_download_cogment.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/tests/test_integration.py` & `cogment-2.8.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cogment-2.7.1/tests/test_model_registry.py` & `cogment-2.8.0/tests/test_model_registry.py`

 * *Files identical despite different names*

