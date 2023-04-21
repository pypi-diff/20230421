# Comparing `tmp/petals-1.1.3.tar.gz` & `tmp/petals-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petals-1.1.3.tar", last modified: Wed Mar  1 09:02:08 2023, max compression
+gzip compressed data, was "petals-1.1.4.tar", last modified: Fri Apr 21 01:40:09 2023, max compression
```

## Comparing `petals-1.1.3.tar` & `petals-1.1.4.tar`

### file list

```diff
@@ -1,77 +1,75 @@
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.184064 petals-1.1.3/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2023-03-01 09:01:22.000000 petals-1.1.3/LICENSE
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    10738 2023-03-01 09:02:08.184064 petals-1.1.3/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9567 2023-03-01 09:01:22.000000 petals-1.1.3/README.md
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      297 2023-03-01 09:01:22.000000 petals-1.1.3/pyproject.toml
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1558 2023-03-01 09:02:08.184064 petals-1.1.3/setup.cfg
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.176064 petals-1.1.3/src/
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.176064 petals-1.1.3/src/petals/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      140 2023-03-01 09:01:31.000000 petals-1.1.3/src/petals/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/bloom/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/bloom/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2528 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/bloom/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4795 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/bloom/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3877 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/bloom/modeling_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/cli/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/cli/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4596 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/cli/convert_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2121 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/cli/inference_one_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/cli/run_dht.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13383 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/cli/run_server.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/client/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      484 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14981 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/inference_session.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/remote_forward_backward.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15928 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/remote_generation.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11806 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/remote_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4368 2023-03-01 09:01:22.000000 petals-1.1.3/src/petals/client/remote_sequential.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/client/routing/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/client/routing/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4464 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/client/routing/sequence_info.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    17130 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/client/routing/sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/client/routing/spending_policy.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12394 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/client/sequential_autograd.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      537 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/constants.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1116 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/data_structures.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6945 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/dht_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/server/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9337 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/backend.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/block_selection.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1684 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/block_utils.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    24633 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/handler.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8655 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/memory_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7808 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/reachability.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    26677 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/server.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/task_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/task_prioritizer.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6627 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/server/throughput.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals/utils/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/asyncio.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6181 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/convert_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3091 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/disk_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5591 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/generation_algorithms.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/generation_constraints.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15072 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/linear8bitlt_patch.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1242 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/logging.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/misc.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      914 2023-03-01 09:01:23.000000 petals-1.1.3/src/petals/utils/version.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.180065 petals-1.1.3/src/petals.egg-info/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    10738 2023-03-01 09:02:08.000000 petals-1.1.3/src/petals.egg-info/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2019 2023-03-01 09:02:08.000000 petals-1.1.3/src/petals.egg-info/SOURCES.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-03-01 09:02:08.000000 petals-1.1.3/src/petals.egg-info/dependency_links.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      320 2023-03-01 09:02:08.000000 petals-1.1.3/src/petals.egg-info/requires.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-03-01 09:02:08.000000 petals-1.1.3/src/petals.egg-info/top_level.txt
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-03-01 09:02:08.184064 petals-1.1.3/tests/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      752 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_aux_functions.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1809 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_block_exact_match.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3151 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_chained_calls.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7789 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_full_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3966 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_linear8bitlt.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_priority_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5811 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_remote_sequential.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1923 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1797 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_server_stats.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1910 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_tensor_parallel.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      419 2023-03-01 09:01:23.000000 petals-1.1.3/tests/test_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2023-04-21 01:39:52.000000 petals-1.1.4/LICENSE
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11712 2023-04-21 01:40:09.579757 petals-1.1.4/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    10540 2023-04-21 01:39:52.000000 petals-1.1.4/README.md
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-21 01:39:52.000000 petals-1.1.4/pyproject.toml
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1586 2023-04-21 01:40:09.579757 petals-1.1.4/setup.cfg
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.571757 petals-1.1.4/src/
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      140 2023-04-21 01:39:57.000000 petals-1.1.4/src/petals/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/bloom/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2672 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5146 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3877 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/modeling_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/cli/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4718 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/convert_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2121 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/inference_one_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/run_dht.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13616 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/run_server.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/client/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      484 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14981 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/inference_session.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_forward_backward.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15928 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_generation.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12364 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4340 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_sequential.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/client/routing/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4464 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/sequence_info.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    16884 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/spending_policy.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12394 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/sequential_autograd.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      537 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/constants.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1116 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/data_structures.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7030 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/dht_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/server/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9337 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/backend.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/block_selection.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1704 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/block_utils.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    24633 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/handler.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8655 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/memory_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7808 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/reachability.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    26298 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/server.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/task_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/task_prioritizer.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6627 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/throughput.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/src/petals/utils/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/asyncio.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6171 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/convert_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3091 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/disk_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5591 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/generation_algorithms.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/generation_constraints.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1242 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/logging.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/misc.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      914 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/version.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals.egg-info/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11712 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1953 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      347 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/requires.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/top_level.txt
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/tests/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      731 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_aux_functions.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3654 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_block_exact_match.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3151 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_chained_calls.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7789 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_full_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_priority_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5773 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_remote_sequential.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1797 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_server_stats.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1910 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_tensor_parallel.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      419 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_utils.py
```

### Comparing `petals-1.1.3/LICENSE` & `petals-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/PKG-INFO` & `petals-1.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,11 @@
-Metadata-Version: 2.1
-Name: petals
-Version: 1.1.3
-Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
-Home-page: https://github.com/bigscience-workshop/petals
-Author: Petals Developers
-Author-email: petals-dev@googlegroups.com
-Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
     <img src="https://i.imgur.com/7eR7Pan.png" width="400"><br>
     Run 100B+ language models at home, BitTorrent-style.<br>
-    Fine-tuning and inference up to 10x faster than offloading<br><br>
+    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading<br><br>
     <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a><br>
 </p>
 
 Generate text using distributed 176B-parameter [BLOOM](https://huggingface.co/bigscience/bloom) or [BLOOMZ](https://huggingface.co/bigscience/bloomz) and fine-tune them for your own tasks:
 
 ```python
 from petals import DistributedBloomForCausalLM
@@ -58,27 +31,27 @@
     🚀 &nbsp;<b><a href="https://colab.research.google.com/drive/1Ervk6HPNS6AYVr3xVdQnY5a-TjjmLCdQ?usp=sharing">Try now in Colab</a></b>
 </p>
 
 🔏 Your data will be processed by other people in the public swarm. Learn more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety). For sensitive data, you can set up a [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
 
 ### Connect your GPU and increase Petals capacity
 
-Run this in an [Anaconda](https://www.anaconda.com) env (requires Linux and Python 3.7+):
+Run our [Docker](https://www.docker.com) image (works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)):
 
 ```bash
-conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install -U petals
-python -m petals.cli.run_server bigscience/bloom-petals
+sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm \
+    learningathome/petals:main python -m petals.cli.run_server bigscience/bloom-petals --port 31330
 ```
 
-Or use our [Docker](https://www.docker.com) image (works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)):
+Or run these commands in an [Anaconda](https://www.anaconda.com) env (requires Linux and Python 3.7+):
 
 ```bash
-sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm \
-    learningathome/petals:main python -m petals.cli.run_server bigscience/bloom-petals --port 31330
+conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
+pip install -U petals
+python -m petals.cli.run_server bigscience/bloom-petals
 ```
 
 📚 See [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to configure the server to use multiple GPUs, address common issues, etc.
 
 You can also host [BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of BLOOM fine-tuned to follow human instructions in the zero-shot regime — just replace `bloom-petals` with `bloomz-petals`.
 
 🔒 Hosting a server does not allow others to run custom code on your computer. Learn more about security [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
@@ -106,84 +79,129 @@
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
 
 📋 If you build an app running BLOOM with Petals, make sure it follows the BLOOM's [terms of use](https://huggingface.co/bigscience/bloom).
 
 ## How does it work?
 
 - Petals runs large language models like [BLOOM-176B](https://huggingface.co/bigscience/bloom) **collaboratively** — you load a small part of the model, then team up with people serving the other parts to run inference or fine-tuning.
-- Inference runs at ≈ 1 sec per step (token) — 10x faster than possible with offloading, enough for chatbots and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
-- Beyond classic language model APIs — you can employ any fine-tuning and sampling methods by executing custom paths through the model or accessing its hidden states. You get the comforts of an API with the flexibility of PyTorch.
+- Single-batch inference runs at ≈ 1 sec per step (token) — [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
+- Beyond classic language model APIs — you can employ any fine-tuning and sampling methods, execute custom paths through the model, or see its hidden states. You get the comforts of an API with the flexibility of PyTorch.
 
 <p align="center">
     <img src="https://i.imgur.com/RTYF3yW.png" width="800">
 </p>
 
 <p align="center">
     📚 &nbsp;<b><a href="https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions">See FAQ</a></b>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
     📜 &nbsp;<b><a href="https://arxiv.org/pdf/2209.01188.pdf">Read paper</a></b>
 </p>
 
 ## Installation
 
-Here's how to install Petals with conda:
+Here's how to install Petals with [Anaconda](https://www.anaconda.com/products/distribution) on Linux:
 
 ```bash
 conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
 pip install -U petals
 ```
 
-This script uses Anaconda to install CUDA-enabled PyTorch.
-If you don't have anaconda, you can get it from [here](https://www.anaconda.com/products/distribution).
-If you don't want anaconda, you can install PyTorch [any other way](https://pytorch.org/get-started/locally/).
-If you want to run models with 8-bit weights, please install **PyTorch with CUDA 11** or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
-
-__System requirements:__ Petals only supports Linux for now. If you don't have a Linux machine, consider running Petals in Docker (see our [image](https://hub.docker.com/r/learningathome/petals)) or, in case of Windows, in WSL2 ([read more](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)). CPU is enough to run a client, but you probably need a GPU to run a server efficiently.
-
-## 🛠️ Development
-
-Petals uses pytest with a few plugins. To install them, run:
-
-```bash
-conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-git clone https://github.com/bigscience-workshop/petals.git && cd petals
-pip install -e .[dev]
-```
-
-To run minimalistic tests, you need to make a local swarm with a small model and some servers. You may find more information about how local swarms work and how to run them in [this tutorial](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm).
+If you don't use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/get-started/locally/). If you want to run models with 8-bit weights, please install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
 
-```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main
+See the instructions for macOS and Windows, the full requirements, and troubleshooting advice in our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-client).
 
-python -m petals.cli.run_server $MODEL_NAME --block_indices 0:12 \
-  --identity tests/test.id --host_maddrs /ip4/127.0.0.1/tcp/31337 --new_swarm  &> server1.log &
-sleep 5  # wait for the first server to initialize DHT
+## Benchmarks
 
-python -m petals.cli.run_server $MODEL_NAME --block_indices 12:24 \
-  --initial_peers SEE_THE_OUTPUT_OF_THE_1ST_PEER &> server2.log &
-
-tail -f server1.log server2.log  # view logs for both servers
-```
-
-Then launch pytest:
-
-```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main REF_NAME=bigscience/bloom-560m
-export INITIAL_PEERS=/ip4/127.0.0.1/tcp/31337/p2p/QmS9KwZptnVdB9FFV7uGgaTq4sEKBwcYeKZDfSpyKDUd1g
-PYTHONPATH=. pytest tests --durations=0 --durations-min=1.0 -v
-```
+<table align="center">
+  <tr>
+    <th colspan="2">Network</th>
+    <th colspan="2">Single-batch inference<br>(steps/s)</th>
+    <th colspan="2">Parallel forward<br>(tokens/s)</th>
+  </tr>
+  <tr>
+    <th rowspan="2">Bandwidth</th>
+    <th rowspan="2">Round-trip<br>latency</th>
+    <th colspan="2">Sequence length</th>
+    <th colspan="2">Batch size</th>
+  </tr>
+  <tr align="center">
+    <td>128</td>
+    <td>2048</td>
+    <td>1</td>
+    <td>64</td>
+  </tr>
+  <tr>
+    <th colspan="6">Offloading, max. possible speed on 1x A100 <sup>1</sup></th>
+  </tr>
+  <tr align="center">
+    <td>256 Gbit/s</td>
+    <td></td>
+    <td>0.18</td>
+    <td>0.18</td>
+    <td>2.7</td>
+    <td>170.3</td>
+  </tr>
+  <tr align="center">
+    <td>128 Gbit/s</td>
+    <td></td>
+    <td>0.09</td>
+    <td>0.09</td>
+    <td>2.4</td>
+    <td>152.8</td>
+  </tr>
+  <tr>
+    <th colspan="6">Petals on 14 heterogeneous servers across Europe and North America <sup>2</sup></th>
+  </tr>
+  <tr align="center">
+    <td colspan="2">Real world</td>
+    <td>0.83</td>
+    <td>0.79</td>
+    <td>32.6</td>
+    <td>179.4</td>
+  </tr>
+  <tr>
+    <th colspan="6">Petals on 3 servers, with one A100 each <sup>3</sup></th>
+  </tr>
+  <tr align="center">
+    <td>1 Gbit/s</td>
+    <td>&lt; 5 ms</td>
+    <td>1.71</td>
+    <td>1.54</td>
+    <td>70.0</td>
+    <td>253.6</td>
+  </tr>
+  <tr align="center">
+    <td>100 Mbit/s</td>
+    <td>&lt; 5 ms</td>
+    <td>1.66</td>
+    <td>1.49</td>
+    <td>56.4</td>
+    <td>182.0</td>
+  </tr>
+  <tr align="center">
+    <td>100 Mbit/s</td>
+    <td>100 ms</td>
+    <td>1.23</td>
+    <td>1.11</td>
+    <td>19.7</td>
+    <td>112.2</td>
+  </tr>
+</table>
+
+<sup>1</sup> **An upper bound for offloading performance.** We base our offloading numbers on the best possible hardware setup for offloading: CPU RAM offloading via PCIe 4.0 with 16 PCIe lanes per GPU and PCIe switches for pairs of GPUs. We assume zero latency for the upper bound estimation. In 8-bit, the model uses 1 GB of memory per billion parameters. PCIe 4.0 with 16 lanes has a throughput of 256 Gbit/s, so offloading 176B parameters takes 5.5 seconds. The throughput is twice as slow (128 Gbit/s) if we have two GPUs behind the same PCIe switch.
+
+<sup>2</sup> **A real-world distributed setting** with 14 servers holding 2× RTX 3060, 4× 2080Ti, 2× 3090, 2× A4000, and 4× A5000 GPUs. These are personal servers and servers from university labs, spread across Europe and North America and connected to the Internet at speeds of 100–1000 Mbit/s. 4 servers operate from under firewalls.
 
-After you're done, you can terminate the servers and ensure that no zombie processes are left with `pkill -f petals.cli.run_server && pkill -f p2p`.
+<sup>3</sup> **An optimistic setup** that requires least communication. The client nodes have 8 CPU cores and no GPU.
 
-The automated tests use a more complex server configuration that can be found [here](https://github.com/bigscience-workshop/petals/blob/main/.github/workflows/run-tests.yaml).
+We provide more evaluations and discuss these results in more detail in **Section 3.3** of our [paper](https://arxiv.org/pdf/2209.01188.pdf).
 
-### Code style
+## 🛠️ Contributing
 
-We use [black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html) and [isort](https://pycqa.github.io/isort/) for all pull requests.
-Before committing your code, simply run `black . && isort .` and you will be fine.
+Please see our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#contributing) on contributing.
 
 ## 📜 Citation
 
 Alexander Borzunov, Dmitry Baranchuk, Tim Dettmers, Max Ryabinin, Younes Belkada, Artem Chumachenko, Pavel Samygin, and Colin Raffel.
 [Petals: Collaborative Inference and Fine-tuning of Large Models.](https://arxiv.org/abs/2209.01188)
 _arXiv preprint arXiv:2209.01188,_ 2022.
```

#### html2text {}

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1 Name: petals Version: 1.1.3 Summary: Easy way to
-efficiently run 100B+ language models without high-end GPUs Home-page: https://
-github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
-petals-dev@googlegroups.com Project-URL: Bug Tracker, https://github.com/
-bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE
                        [https://i.imgur.com/7eR7Pan.png]
              Run 100B+ language models at home, BitTorrent-style.
-          Fine-tuning and inference up to 10x faster than offloading
+          Fine-tuning and inference up_to_10x_faster than offloading
 
             [https://img.shields.io/pypi/v/petals.svg?color=green]
 Generate text using distributed 176B-parameter [BLOOM](https://huggingface.co/
 bigscience/bloom) or [BLOOMZ](https://huggingface.co/bigscience/bloomz) and
 fine-tune them for your own tasks: ```python from petals import
 DistributedBloomForCausalLM model = DistributedBloomForCausalLM.from_pretrained
 ("bigscience/bloom-petals", tuning_mode="ptune", pre_seq_len=16) # Embeddings &
@@ -34,33 +18,33 @@
 ```
                             ð  Try_now_in_Colab
 ð Your data will be processed by other people in the public swarm. Learn
 more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/
 Security,-privacy,-and-AI-safety). For sensitive data, you can set up a
 [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
 own-swarm) among people you trust. ### Connect your GPU and increase Petals
-capacity Run this in an [Anaconda](https://www.anaconda.com) env (requires
-Linux and Python 3.7+): ```bash conda install pytorch pytorch-cuda=11.7 -
-c pytorch -c nvidia pip install -U petals python -m petals.cli.run_server
-bigscience/bloom-petals ``` Or use our [Docker](https://www.docker.com) image
-(works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-
-us/windows/ai/directml/gpu-cuda-in-wsl)): ```bash sudo docker run -p 31330:
-31330 --ipc host --gpus all --volume petals-cache:/cache --rm \ learningathome/
-petals:main python -m petals.cli.run_server bigscience/bloom-petals --port
-31330 ``` ð See [FAQ](https://github.com/bigscience-workshop/petals/wiki/
-FAQ:-Frequently-asked-questions#running-a-server) to learn how to configure the
-server to use multiple GPUs, address common issues, etc. You can also host
-[BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of BLOOM fine-
-tuned to follow human instructions in the zero-shot regime â just replace
-`bloom-petals` with `bloomz-petals`. ð Hosting a server does not allow
-others to run custom code on your computer. Learn more about security [here]
-(https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-
-safety). ð¬ If you have any issues or feedback, let us know on [our Discord
-server](https://discord.gg/D9MwApKgWa)! ### Check out tutorials, examples, and
-more Basic tutorials: - Getting started: [tutorial](https://
+capacity Run our [Docker](https://www.docker.com) image (works on Linux, macOS,
+and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/
+gpu-cuda-in-wsl)): ```bash sudo docker run -p 31330:31330 --ipc host --gpus all
+--volume petals-cache:/cache --rm \ learningathome/petals:main python -
+m petals.cli.run_server bigscience/bloom-petals --port 31330 ``` Or run these
+commands in an [Anaconda](https://www.anaconda.com) env (requires Linux and
+Python 3.7+): ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
+c nvidia pip install -U petals python -m petals.cli.run_server bigscience/
+bloom-petals ``` ð See [FAQ](https://github.com/bigscience-workshop/petals/
+wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to
+configure the server to use multiple GPUs, address common issues, etc. You can
+also host [BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of
+BLOOM fine-tuned to follow human instructions in the zero-shot regime â just
+replace `bloom-petals` with `bloomz-petals`. ð Hosting a server does not
+allow others to run custom code on your computer. Learn more about security
+[here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-
+and-AI-safety). ð¬ If you have any issues or feedback, let us know on [our
+Discord server](https://discord.gg/D9MwApKgWa)! ### Check out tutorials,
+examples, and more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1Ervk6HPNS6AYVr3xVdQnY5a-TjjmLCdQ?usp=sharing)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-personachat.ipynb) - Prompt-tune BLOOM for text semantic
 classification: [tutorial](https://colab.research.google.com/github/bigscience-
 workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb) Useful tools and
 advanced guides: - [Chatbot web app](http://chat.petals.ml) (connects to Petals
@@ -73,67 +57,69 @@
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ð If you build an app running
 BLOOM with Petals, make sure it follows the BLOOM's [terms of use](https://
 huggingface.co/bigscience/bloom). ## How does it work? - Petals runs large
 language models like [BLOOM-176B](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
-people serving the other parts to run inference or fine-tuning. - Inference
-runs at â 1 sec per step (token) â 10x faster than possible with
-offloading, enough for chatbots and other interactive apps. Parallel inference
-reaches hundreds of tokens/sec. - Beyond classic language model APIs â you
-can employ any fine-tuning and sampling methods by executing custom paths
-through the model or accessing its hidden states. You get the comforts of an
-API with the flexibility of PyTorch.
+people serving the other parts to run inference or fine-tuning. - Single-batch
+inference runs at â 1 sec per step (token) â [up to 10x faster](https://
+github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for
+[chatbots](http://chat.petals.ml) and other interactive apps. Parallel
+inference reaches hundreds of tokens/sec. - Beyond classic language model APIs
+â you can employ any fine-tuning and sampling methods, execute custom paths
+through the model, or see its hidden states. You get the comforts of an API
+with the flexibility of PyTorch.
                        [https://i.imgur.com/RTYF3yW.png]
                    ð  See_FAQ            ð  Read_paper
-## Installation Here's how to install Petals with conda: ```bash conda install
-pytorch pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` This
-script uses Anaconda to install CUDA-enabled PyTorch. If you don't have
-anaconda, you can get it from [here](https://www.anaconda.com/products/
-distribution). If you don't want anaconda, you can install PyTorch [any other
-way](https://pytorch.org/get-started/locally/). If you want to run models with
-8-bit weights, please install **PyTorch with CUDA 11** or newer for compatility
-with [bitsandbytes](https://github.com/timDettmers/bitsandbytes). __System
-requirements:__ Petals only supports Linux for now. If you don't have a Linux
-machine, consider running Petals in Docker (see our [image](https://
-hub.docker.com/r/learningathome/petals)) or, in case of Windows, in WSL2 ([read
-more](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)).
-CPU is enough to run a client, but you probably need a GPU to run a server
-efficiently. ## ð ï¸ Development Petals uses pytest with a few plugins. To
-install them, run: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
-c nvidia git clone https://github.com/bigscience-workshop/petals.git && cd
-petals pip install -e .[dev] ``` To run minimalistic tests, you need to make a
-local swarm with a small model and some servers. You may find more information
-about how local swarms work and how to run them in [this tutorial](https://
-github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm). ```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main python -
-m petals.cli.run_server $MODEL_NAME --block_indices 0:12 \ --identity tests/
-test.id --host_maddrs /ip4/127.0.0.1/tcp/31337 --new_swarm &> server1.log &
-sleep 5 # wait for the first server to initialize DHT python -
-m petals.cli.run_server $MODEL_NAME --block_indices 12:24 \ --initial_peers
-SEE_THE_OUTPUT_OF_THE_1ST_PEER &> server2.log & tail -f server1.log server2.log
-# view logs for both servers ``` Then launch pytest: ```bash export
-MODEL_NAME=bloom-testing/test-bloomd-560m-main REF_NAME=bigscience/bloom-560m
-export INITIAL_PEERS=/ip4/127.0.0.1/tcp/31337/p2p/
-QmS9KwZptnVdB9FFV7uGgaTq4sEKBwcYeKZDfSpyKDUd1g PYTHONPATH=. pytest tests --
-durations=0 --durations-min=1.0 -v ``` After you're done, you can terminate the
-servers and ensure that no zombie processes are left with `pkill -
-f petals.cli.run_server && pkill -f p2p`. The automated tests use a more
-complex server configuration that can be found [here](https://github.com/
-bigscience-workshop/petals/blob/main/.github/workflows/run-tests.yaml). ###
-Code style We use [black](https://black.readthedocs.io/en/stable/
-the_black_code_style/current_style.html) and [isort](https://pycqa.github.io/
-isort/) for all pull requests. Before committing your code, simply run `black .
-&& isort .` and you will be fine. ## ð Citation Alexander Borzunov, Dmitry
-Baranchuk, Tim Dettmers, Max Ryabinin, Younes Belkada, Artem Chumachenko, Pavel
-Samygin, and Colin Raffel. [Petals: Collaborative Inference and Fine-tuning of
-Large Models.](https://arxiv.org/abs/2209.01188) _arXiv preprint arXiv:
-2209.01188,_ 2022. ```bibtex @article{borzunov2022petals, title = {Petals:
-Collaborative Inference and Fine-tuning of Large Models}, author = {Borzunov,
-Alexander and Baranchuk, Dmitry and Dettmers, Tim and Ryabinin, Max and
-Belkada, Younes and Chumachenko, Artem and Samygin, Pavel and Raffel, Colin},
-journal = {arXiv preprint arXiv:2209.01188}, year = {2022}, url = {https://
-arxiv.org/abs/2209.01188} } ``` -----------------------------------------------
----------------------------------
+## Installation Here's how to install Petals with [Anaconda](https://
+www.anaconda.com/products/distribution) on Linux: ```bash conda install pytorch
+pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` If you don't
+use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/
+get-started/locally/). If you want to run models with 8-bit weights, please
+install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes]
+(https://github.com/timDettmers/bitsandbytes). See the instructions for macOS
+and Windows, the full requirements, and troubleshooting advice in our [FAQ]
+(https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-
+questions#running-a-client). ## Benchmarks
+     Network               Single-batch inference Parallel forward
+                           (steps/s)              (tokens/s)
+     Bandwidth  Round-trip Sequence length        Batch size
+                latency    128           2048       1              64
+     Offloading, max. possible speed on 1x A100 1
+     256 Gbit/s            0.18          0.18     2.7           170.3
+     128 Gbit/s            0.09          0.09     2.4           152.8
+     Petals on 14 heterogeneous servers across Europe and North America 2
+             Real world    0.83          0.79     32.6          179.4
+     Petals on 3 servers, with one A100 each 3
+      1 Gbit/s     < 5 ms  1.71          1.54     70.0          253.6
+     100 Mbit/s    < 5 ms  1.66          1.49     56.4          182.0
+     100 Mbit/s    100 ms  1.23          1.11     19.7          112.2
+1 **An upper bound for offloading performance.** We base our offloading numbers
+on the best possible hardware setup for offloading: CPU RAM offloading via PCIe
+4.0 with 16 PCIe lanes per GPU and PCIe switches for pairs of GPUs. We assume
+zero latency for the upper bound estimation. In 8-bit, the model uses 1 GB of
+memory per billion parameters. PCIe 4.0 with 16 lanes has a throughput of 256
+Gbit/s, so offloading 176B parameters takes 5.5 seconds. The throughput is
+twice as slow (128 Gbit/s) if we have two GPUs behind the same PCIe switch. 2
+**A real-world distributed setting** with 14 servers holding 2Ã RTX 3060, 4Ã
+2080Ti, 2Ã 3090, 2Ã A4000, and 4Ã A5000 GPUs. These are personal servers and
+servers from university labs, spread across Europe and North America and
+connected to the Internet at speeds of 100â1000 Mbit/s. 4 servers operate
+from under firewalls. 3 **An optimistic setup** that requires least
+communication. The client nodes have 8 CPU cores and no GPU. We provide more
+evaluations and discuss these results in more detail in **Section 3.3** of our
+[paper](https://arxiv.org/pdf/2209.01188.pdf). ## ð ï¸ Contributing Please
+see our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-
+Frequently-asked-questions#contributing) on contributing. ## ð Citation
+Alexander Borzunov, Dmitry Baranchuk, Tim Dettmers, Max Ryabinin, Younes
+Belkada, Artem Chumachenko, Pavel Samygin, and Colin Raffel. [Petals:
+Collaborative Inference and Fine-tuning of Large Models.](https://arxiv.org/
+abs/2209.01188) _arXiv preprint arXiv:2209.01188,_ 2022. ```bibtex @article
+{borzunov2022petals, title = {Petals: Collaborative Inference and Fine-tuning
+of Large Models}, author = {Borzunov, Alexander and Baranchuk, Dmitry and
+Dettmers, Tim and Ryabinin, Max and Belkada, Younes and Chumachenko, Artem and
+Samygin, Pavel and Raffel, Colin}, journal = {arXiv preprint arXiv:2209.01188},
+year = {2022}, url = {https://arxiv.org/abs/2209.01188} } ``` -----------------
+---------------------------------------------------------------
           This project is a part of the BigScience research workshop.
                       [https://petals.ml/bigscience.png]
```

### Comparing `petals-1.1.3/setup.cfg` & `petals-1.1.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = petals
 version = attr: petals.__version__
 author = Petals Developers
-author_email = petals-dev@googlegroups.com
+author_email = petals-devs@googlegroups.com
 description = Easy way to efficiently run 100B+ language models without high-end GPUs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bigscience-workshop/petals
 project_urls = 
 	Bug Tracker = https://github.com/bigscience-workshop/petals/issues
 classifiers = 
@@ -28,20 +28,20 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	torch>=1.12
-	bitsandbytes==0.34.0
-	accelerate==0.15.0
-	huggingface-hub==0.11.1
-	transformers==4.25.1
+	bitsandbytes==0.38.0.post2
+	accelerate>=0.15.0,<1.0.0
+	huggingface-hub>=0.11.1,<1.0.0
+	transformers>=4.25.1,<5.0.0
 	speedtest-cli==2.1.3
-	hivemind==1.1.5
+	hivemind==1.1.7
 	tensor_parallel==1.0.23
 	humanfriendly
 	async-timeout>=4.0.2
 	cpufeature>=0.2.0
 	packaging>=20.9
 
 [options.extras_require]
```

### Comparing `petals-1.1.3/src/petals/bloom/block.py` & `petals-1.1.4/src/petals/bloom/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 See commit history for authorship.
 """
 import os
 from typing import Optional, Tuple
 
 import torch.nn.quantized.dynamic.modules.linear
 import transformers
+from packaging import version
 from transformers.models.bloom.modeling_bloom import BloomBlock, _expand_mask, _make_causal_mask, build_alibi_tensor
 
 if not os.getenv("PETALS_IGNORE_DEPENDENCY_VERSION"):
-    assert transformers.__version__.startswith("4.25."), "Please install transformers 4.25.1"
+    assert (
+        version.parse("4.25.1") <= version.parse(transformers.__version__) < version.parse("5.0.0")
+    ), "Please install a proper transformers version: pip install transformers>=4.25.1,<5.0.0"
 
 
 class WrappedBloomBlock(BloomBlock):
     def forward(
         self,
         hidden_states: torch.Tensor,
         *args,
```

### Comparing `petals-1.1.3/src/petals/bloom/from_pretrained.py` & `petals-1.1.4/src/petals/bloom/from_pretrained.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from __future__ import annotations
 
 import itertools
 import time
 from typing import Optional, OrderedDict, Union
 
 import torch
+from accelerate import init_empty_weights
+from accelerate.utils import set_module_tensor_to_device
 from hivemind.utils.logging import get_logger
 from transformers.modeling_utils import WEIGHTS_NAME
 from transformers.models.bloom.configuration_bloom import BloomConfig
 from transformers.utils import get_file_from_repo
 
 from petals.bloom.block import WrappedBloomBlock
 from petals.server.block_utils import get_block_size
@@ -34,40 +36,44 @@
     config: Optional[BloomConfig] = None,
     torch_dtype: Union[torch.dtype, str] = "auto",
     use_auth_token: Optional[str] = None,
     cache_dir: Optional[str] = None,
     max_disk_space: Optional[int] = None,
 ) -> WrappedBloomBlock:
     """Load one BLOOM block from a converted model. See convert_model.py (or README.md) on how to convert it."""
+    assert torch_dtype in DTYPE_MAP.values(), f"torch_dtype must be one of {list(DTYPE_MAP.values())}"
 
     if config is None:
         config = BloomConfig.from_pretrained(converted_model_name_or_path, use_auth_token=use_auth_token)
     if cache_dir is None:
         cache_dir = DEFAULT_CACHE_DIR
 
-    block = WrappedBloomBlock(config)
+    with init_empty_weights():
+        block = WrappedBloomBlock(config)
+
     state_dict = _load_state_dict(
         converted_model_name_or_path,
         block_index,
         config,
         use_auth_token=use_auth_token,
         cache_dir=cache_dir,
         max_disk_space=max_disk_space,
     )
 
-    if torch_dtype == "auto":
-        with torch.no_grad():
-            for name, param in block.named_parameters():
-                assert name in state_dict, f"{name} not in state dict"
-                param.data = param.data.to(state_dict[name].dtype)
-    else:
-        assert torch_dtype in DTYPE_MAP.values(), f"torch_dtype must be one of {list(DTYPE_MAP.values())}"
-        block = block.to(dtype=torch_dtype)
-
+    # dummy load, check that keys match
     report = block.load_state_dict(state_dict, strict=True)
+    assert not report.missing_keys, f"Some block weights are missing: {report.missing_keys}"
+
+    for param_name, _ in block.named_parameters():
+        assert param_name in state_dict, f"{param_name} not in state dict"
+        param = state_dict[param_name]
+        if torch_dtype != "auto" and not str(param.dtype).startswith(("torch.uint", "torch.int", "torch.bool")):
+            param = param.to(torch_dtype)
+        set_module_tensor_to_device(block, param_name, "cpu", value=param)
+
     logger.info(f"Loaded {converted_model_name_or_path} block {block_index}, {report}")
     return block
 
 
 def _load_state_dict(
     pretrained_model_name_or_path: str,
     block_index: int,
```

### Comparing `petals-1.1.3/src/petals/bloom/modeling_utils.py` & `petals-1.1.4/src/petals/bloom/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/cli/convert_model.py` & `petals-1.1.4/src/petals/cli/convert_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 import psutil
 import torch.backends.quantized
 import torch.nn as nn
 import transformers
 from hivemind.utils.logging import get_logger
-from huggingface_hub import Repository
+from huggingface_hub import HfApi, Repository
 from tqdm.auto import tqdm
 from transformers.models.bloom.modeling_bloom import BloomModel
 
 from petals.bloom.from_pretrained import BLOCK_BRANCH_PREFIX, CLIENT_BRANCH
 from petals.client import DistributedBloomConfig
 
 logger = get_logger(__name__)
@@ -62,14 +62,16 @@
         config.vocab_size = args.resize_token_embeddings
 
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         args.model, use_auth_token=args.use_auth_token, revision=args.revision
     )
     os.makedirs(args.output_path, exist_ok=True)
 
+    api = HfApi(token=args.use_auth_token)
+    api.create_repo(args.output_repo, repo_type="model", exist_ok=True)
     repo = Repository(args.output_path, clone_from=args.output_repo, use_auth_token=args.use_auth_token)
     repo.git_pull()
 
     transformer_blocks = model.h
     logger.info(
         f"Saving transformer blocks to {args.output_repo}@{args.block_branch_prefix}0"
         f" - {args.output_repo}@{args.block_branch_prefix}{len(transformer_blocks)}"
```

### Comparing `petals-1.1.3/src/petals/cli/inference_one_block.py` & `petals-1.1.4/src/petals/cli/inference_one_block.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/cli/run_dht.py` & `petals-1.1.4/src/petals/cli/run_dht.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/cli/run_server.py` & `petals-1.1.4/src/petals/cli/run_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
                         help="Do not look for libp2p relays to become reachable if we are behind NAT/firewall")
 
     parser.add_argument('--host_maddrs', nargs='+', required=False,
                         help='Multiaddrs to listen for external connections from other peers')
     parser.add_argument('--announce_maddrs', nargs='+', required=False,
                         help='Visible multiaddrs the host announces for external connections from other peers')
 
+    parser.add_argument('--daemon_startup_timeout', type=float, default=60,
+                        help='Timeout for the libp2p daemon connecting to initial peers')
+
     parser.add_argument('--compression', type=str, default='NONE', required=False, help='Tensor compression communication')
 
     parser.add_argument('--num_handlers', type=int, default=8, required=False,
                         help='server will use this many processes to handle incoming requests')
     parser.add_argument('--min_batch_size', type=int, default=1,
                         help='Minimum required batch size for all operations (in total tokens)')
     parser.add_argument('--max_batch_size', type=int, default=2048,
@@ -163,14 +166,16 @@
     announce_maddrs = args.pop("announce_maddrs")
     public_ip = args.pop("public_ip")
     if public_ip is not None:
         assert announce_maddrs is None, "You can't use --public_ip and --announce_maddrs at the same time"
         assert port != 0, "Please specify a fixed non-zero --port when you use --public_ip (e.g., --port 31337)"
         announce_maddrs = [f"/ip4/{public_ip}/tcp/{port}"]
 
+    args["startup_timeout"] = args.pop("daemon_startup_timeout")
+
     if args.pop("increase_file_limit"):
         increase_file_limit()
 
     compression_type = args.pop("compression").upper()
     compression = getattr(CompressionType, compression_type)
 
     attn_cache_size = args.pop("attn_cache_size")
```

### Comparing `petals-1.1.3/src/petals/client/inference_session.py` & `petals-1.1.4/src/petals/client/inference_session.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/client/remote_forward_backward.py` & `petals-1.1.4/src/petals/client/remote_forward_backward.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/client/remote_generation.py` & `petals-1.1.4/src/petals/client/remote_generation.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/client/remote_model.py` & `petals-1.1.4/src/petals/client/remote_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     A bloom config that contains information about DHT peers.
     To create a distributed model, one must provide dht_prefix and either initial_peers or dht.
     """
 
     initial_peers: List[str] = PUBLIC_INITIAL_PEERS  # a list of initial peers for hivemind DHT
     dht_prefix: str  # a prefix for all dht keys that correspond to this model (usually equal to model name)
-    daemon_startup_timeout: int = 30
+    daemon_startup_timeout: int = 60  # timeout for the libp2p daemon connecting to initial peers
     dht: Optional[hivemind.DHT] = None  # a running DHT instance, e.g. when using the same DHT for multiple models
     request_timeout: int = 3 * 60  # a number of seconds for waiting result from each node
     max_retries: Optional[int] = None  # max number retries before the client raises an exception (default: inf)
     allowed_servers: Optional[
         Collection[Union[str, hivemind.PeerID]]
     ] = None  # if defined, send requests only to these servers
 
@@ -67,28 +67,41 @@
         possibly_patched_register_parameter = nn.Module.register_parameter
         nn.Module.register_parameter = original_register_parameter
         yield
     finally:
         nn.Module.register_parameter = possibly_patched_register_parameter
 
 
-class _LowCPUMemoryMixin:
+class _FromPretrainedDefaultsMixin:
     @classmethod
-    def from_pretrained(cls, *args, low_cpu_mem_usage: Optional[bool] = None, **kwargs):
+    def from_pretrained(
+        cls,
+        *args,
+        low_cpu_mem_usage: Optional[bool] = None,
+        torch_dtype: Optional[Union[str, torch.dtype]] = None,
+        **kwargs,
+    ):
         if low_cpu_mem_usage is None:
             low_cpu_mem_usage = True
-        return super().from_pretrained(*args, low_cpu_mem_usage=low_cpu_mem_usage, **kwargs)
+        if torch_dtype is None:
+            # torch_dtype=None gives torch.float32 in transformers>=4.26.0. In contrast,
+            # torch_dtype="auto" attempts to (1) use config.torch_dtype (if exists), (2) use dtype of the weights.
+            torch_dtype = "auto"
+        return super().from_pretrained(*args, low_cpu_mem_usage=low_cpu_mem_usage, torch_dtype=torch_dtype, **kwargs)
 
     from_pretrained.__doc__ = BloomPreTrainedModel.from_pretrained.__doc__.replace(
         "low_cpu_mem_usage(`bool`, *optional*)",
         "low_cpu_mem_usage(`bool`, *optional*, defaults to `True` in Petals)",
+    ).replace(
+        "torch_dtype (`str` or `torch.dtype`, *optional*)",
+        'torch_dtype (`str` or `torch.dtype`, *optional*, defaults to `"auto"` in Petals)',
     )
 
 
-class DistributedBloomModel(_LowCPUMemoryMixin, BloomModel):
+class DistributedBloomModel(_FromPretrainedDefaultsMixin, BloomModel):
     """BloomModel, but all transformer layers are hosted by the swarm"""
 
     _keys_to_ignore_on_load_missing = BloomModel._keys_to_ignore_on_load_missing + [
         r"^(intermediate_)?prompt_embeddings\.weight$",
     ]
 
     config_class = DistributedBloomConfig
@@ -98,27 +111,23 @@
         assert config.initial_peers or config.dht, "Please specify initial_peers=list(...) or dht=hivemind.DHT(...)"
 
         n_layer, config.n_layer = config.n_layer, 0  # temporarily set n_layer to 0 to prevent layer initialization
         super().__init__(config)
         assert len(self.h) == 0
         config.n_layer = n_layer
 
-        dht = (
-            config.dht
-            if config.dht is not None
-            else hivemind.DHT(
+        dht = config.dht
+        if dht is None:
+            dht = hivemind.DHT(
                 initial_peers=config.initial_peers,
                 client_mode=True,
                 num_workers=n_layer,
                 startup_timeout=config.daemon_startup_timeout,
                 start=True,
-                use_relay=True,
-                use_auto_relay=True,
             )
-        )
         assert isinstance(dht, hivemind.DHT) and dht.is_alive(), "dht must be a running hivemind.DHT instance"
         self.h = RemoteSequential(
             config,
             dht,
             config.dht_prefix,
         )
 
@@ -218,15 +227,15 @@
             last_hidden_state=hidden_states,
             past_key_values=None,
             hidden_states=None,
             attentions=None,
         )
 
 
-class DistributedBloomForCausalLM(_LowCPUMemoryMixin, RemoteGenerationMixin, BloomForCausalLM):
+class DistributedBloomForCausalLM(_FromPretrainedDefaultsMixin, RemoteGenerationMixin, BloomForCausalLM):
     """DistributedBloomForCausalLM, but all transformer layers are hosted by the swarm"""
 
     _keys_to_ignore_on_load_missing = (
         BloomForCausalLM._keys_to_ignore_on_load_missing
         + DistributedBloomModel._keys_to_ignore_on_load_missing
         + [r"^lm_head.word_embeddings\.weight$"]  # Missing since they are shared with input embeddings
     )
@@ -256,15 +265,15 @@
 
     def set_output_embeddings(self, new_lm_head: nn.Linear):
         with torch.no_grad():
             self.lm_head.word_embeddings.weight[...] = new_lm_head.weight
             self.lm_head.bias[...] = new_lm_head.bias
 
 
-class DistributedBloomForSequenceClassification(_LowCPUMemoryMixin, BloomForSequenceClassification):
+class DistributedBloomForSequenceClassification(_FromPretrainedDefaultsMixin, BloomForSequenceClassification):
     _keys_to_ignore_on_load_missing = (
         BloomForSequenceClassification._keys_to_ignore_on_load_missing
         + DistributedBloomModel._keys_to_ignore_on_load_missing
     )
 
     config_class = DistributedBloomConfig
```

### Comparing `petals-1.1.3/src/petals/client/remote_sequential.py` & `petals-1.1.4/src/petals/client/remote_sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             self.sequence_manager = RemoteSequenceManager(
                 dht,
                 block_uids,
                 self.p2p,
                 request_timeout=config.request_timeout,
                 max_retries=config.max_retries,
                 allowed_servers=config.allowed_servers,
-                start=True,
                 **kwargs,
             )
             self.is_subsequence = False
         else:
             logger.debug(f"Reusing sequence manager with {len(sequence_manager)} modules")
             if kwargs:
                 logger.warning(f"Parameters {kwargs} are ignored because sequence_manager is explicitly provided")
```

### Comparing `petals-1.1.3/src/petals/client/routing/sequence_info.py` & `petals-1.1.4/src/petals/client/routing/sequence_info.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/client/routing/sequence_manager.py` & `petals-1.1.4/src/petals/client/routing/sequence_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 import threading
 import time
 from typing import Any, Collection, Dict, List, Optional, Sequence, Union
 from weakref import WeakMethod
 
 import numpy as np
-from hivemind import DHT, P2P, MSGPackSerializer, PeerID
+from hivemind import DHT, P2P, MSGPackSerializer, PeerID, get_dht_time
 from hivemind.dht.node import Blacklist
 from hivemind.moe.client.remote_expert_worker import RemoteExpertWorker
 from hivemind.p2p import P2PHandlerError
 from hivemind.proto import runtime_pb2
 from hivemind.utils.logging import get_logger
 
 import petals.dht_utils
@@ -62,67 +62,60 @@
         min_backoff: float = 1,
         max_backoff: float = 15 * 60,
         ban_timeout: float = 15,
         sequence_info: Optional[RemoteSequenceInfo] = None,
         rpc_info: Optional[dict] = None,
         allowed_servers: Optional[Collection[Union[str, hivemind.PeerID]]] = None,
         banned_peers: Optional[Blacklist] = None,
-        *,  # dear dev, if you add more parameters to this class, please make sure to handle them in __getitem__ (below)
-        start: bool,
+        # dear dev, if you add more parameters to this class, please make sure to handle them in __getitem__ (below)
     ):
         assert len(block_uids) > 0, "Sequences must contain at least one block"
         self.dht, self.p2p = dht, p2p
         self.request_timeout, self.max_retries = request_timeout, max_retries
         self.ban_timeout, self.min_backoff, self.max_backoff = ban_timeout, min_backoff, max_backoff
         self.lock_changes = threading.Lock()
         self._thread = _SequenceManagerUpdateThread(update_period, WeakMethod(self._update))
+        self._thread_start_lock = threading.Lock()
         self.policy = NoSpendingPolicy()
         self._rpc_info = rpc_info
 
         if allowed_servers is not None:
             allowed_servers = {
                 PeerID.from_base58(peer_id) if isinstance(peer_id, str) else peer_id for peer_id in allowed_servers
             }
         self.allowed_servers = allowed_servers
         self.banned_peers = Blacklist(base_time=ban_timeout, backoff_rate=2.0) if banned_peers is None else banned_peers
 
         if sequence_info is None:
             self.sequence_info = RemoteSequenceInfo.make_empty(block_uids)
-            self.update(wait=False)
+
+            # Pre-fetch module infos in DHT in parallel with .from_pretrained(), then use cached records
+            # in the first _update() instead of the latest ones. This makes the first .update() faster.
+            petals.dht_utils.get_remote_module_infos(self.dht, self.block_uids, latest=True, return_future=True)
+            self._need_latest_infos = False
         else:
             self.sequence_info = sequence_info
             assert block_uids == sequence_info.block_uids
             self._thread.ready.set()  # no need to await the first dht fetch
-
-        if start:
-            self.run_in_background()
-
-    def run_in_background(self, await_ready: bool = True, timeout: Optional[float] = None) -> None:
-        """
-        Starts the updater thread in a background. if await_ready, this method will wait until sequence manager
-        is ready to process incoming requests or for :timeout: seconds max.
-        """
-        self._thread.start()
-        if await_ready:
-            self._thread.ready.wait(timeout)
+            self._need_latest_infos = True
 
     def make_sequence(
         self, start_index: int = 0, end_index: Optional[int] = None, mode: str = "random"
     ) -> List[RemoteSpanInfo]:
         """
         Form a sequence of remote servers that collectively serve all consecutive layers
 
         :param start_index: optional index of the first module in a sequence, default = the first of block_uids
         :param end_index: optional index of the last module (non-inclusive), default = after last of block uids
         :param mode: either random or fastest
         """
-        if not self.is_alive():
-            logger.error("Using a sequence manager that is not running: it has either crashed or never started")
+        with self._thread_start_lock:
+            if not self.is_alive():
+                self._thread.start()
         if not self.ready.is_set():
-            logger.warning("Remote SequenceManager is still searching for routes, waiting for it to become ready")
             self.update(wait=True)  # this will await an existing update or trigger a new one (if not updating)
 
         end_index = end_index if end_index is not None else len(self)
         span_sequence = []
         current_index = start_index
         while current_index < end_index:
             candidate_spans = self.sequence_info.spans_containing_block[current_index]
@@ -159,31 +152,32 @@
             ban_timeout=self.ban_timeout,
             min_backoff=self.min_backoff,
             max_backoff=self.max_backoff,
             sequence_info=self.sequence_info[ix],
             rpc_info=self._rpc_info,
             allowed_servers=self.allowed_servers,
             banned_peers=self.banned_peers,
-            start=True,
         )
 
     def update(self, *, wait: bool):
         """Run an asynchronous update in background as soon as possible"""
         self.ready.clear()  # TODO this should be a separate event
         self._thread.trigger.set()
         if wait:
             self.ready.wait()
 
     def _update(self):
         """Perform an immediate and synchronous refresh, may take time"""
         for attempt_no in itertools.count():
             try:
                 new_block_infos = petals.dht_utils.get_remote_module_infos(
-                    self.dht, self.block_uids, expiration_time=float("inf")
+                    self.dht, self.block_uids, latest=self._need_latest_infos
                 )
+                self._need_latest_infos = True  # All future _update() should use latest infos
+
                 for block_info in new_block_infos:
                     if not block_info:
                         continue
 
                     # Apply whitelist, if defined
                     if self.allowed_servers is not None:
                         block_info.servers = {
@@ -255,14 +249,18 @@
     def block_uids(self):
         return self.sequence_info.block_uids
 
     @property
     def rpc_info(self):
         """Return the rpc_info queried from one of the servers that hold the first block"""
         if self._rpc_info is None:
+            with self._thread_start_lock:
+                if not self.is_alive():
+                    self._thread.start()
+
             for attempt_no in itertools.count():
                 peer_id = None
                 try:
                     if not self.ready.is_set():
                         self.update(wait=True)
 
                     active_servers = [
@@ -316,49 +314,44 @@
 
 class _SequenceManagerUpdateThread(threading.Thread):
     def __init__(self, update_period: float, ref_update_manager: WeakMethod):
         super().__init__(daemon=True)
         self.ref_update_manager = ref_update_manager
         self.ready = threading.Event()
         self.trigger = threading.Event()
-        self.last_update_time = -float("inf")
         self.update_period = update_period
         self.should_shutdown = False
 
     def run(self) -> None:
         while not self.should_shutdown:
-            self.trigger.wait(max(0.0, min(self.update_period, time.perf_counter() - self.last_update_time)))
-
-            if self.should_shutdown:
-                logger.debug(f"{self.__class__.__name__} is shutting down")
-                break
-
             update_manager = self.ref_update_manager()
             if update_manager is None:
                 logger.debug(f"{self.__class__.__name__} exited because the sequence manager no longer exists")
                 break
 
             try:
                 self.trigger.clear()
                 update_manager()
             except Exception as e:
                 logger.exception(e)
             finally:
                 del update_manager
 
+            self.trigger.wait(self.update_period)
+
         logger.debug(f"{self.__class__.__name__} thread exited")
 
     def shutdown(self, timeout: Optional[float] = None):
         self.should_shutdown = True
         self.trigger.set()
-        self.join(timeout)
+        if self.is_alive():
+            self.join(timeout)
 
     def __del__(self):
-        if self.is_alive():
-            self.shutdown()
+        self.shutdown()
 
 
 def maybe_log_traceback(exc: Exception):
     traceback_level = logging.DEBUG if str(exc) or isinstance(exc, asyncio.TimeoutError) else logging.WARNING
     logger.log(traceback_level, "See detailed traceback below:", exc_info=True)
```

### Comparing `petals-1.1.3/src/petals/client/routing/spending_policy.py` & `petals-1.1.4/src/petals/client/routing/spending_policy.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/client/sequential_autograd.py` & `petals-1.1.4/src/petals/client/sequential_autograd.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/constants.py` & `petals-1.1.4/src/petals/constants.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/data_structures.py` & `petals-1.1.4/src/petals/data_structures.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/dht_utils.py` & `petals-1.1.4/src/petals/dht_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     start: int,
     stop: int,
     config: petals.client.DistributedBloomConfig,
     dht_prefix: Optional[str] = None,
 ) -> petals.client.RemoteSequential:
     uids = [f"{config.dht_prefix}{UID_DELIMITER}{i}" for i in range(start, stop)]
     p2p = await dht.replicate_p2p()
-    manager = petals.client.RemoteSequenceManager(dht, uids, p2p, start=True)
+    manager = petals.client.RemoteSequenceManager(dht, uids, p2p)
     return petals.client.RemoteSequential(config, dht, dht_prefix, p2p, manager)
 
 
 def get_remote_module(
     dht: DHT,
     uid_or_uids: Union[ModuleUID, List[ModuleUID]],
     config: petals.client.DistributedBloomConfig,
@@ -120,38 +120,43 @@
     uid_or_uids: Union[ModuleUID, List[ModuleUID]],
     config: petals.client.DistributedBloomConfig,
     dht_prefix: Optional[str] = None,
 ) -> Union[petals.client.RemoteTransformerBlock, List[petals.client.RemoteTransformerBlock]]:
     single_uid = isinstance(uid_or_uids, ModuleUID)
     uids = [uid_or_uids] if single_uid else uid_or_uids
     p2p = await dht.replicate_p2p()
-    managers = (petals.client.RemoteSequenceManager(dht, [uid], p2p, start=True) for uid in uids)
+    managers = (petals.client.RemoteSequenceManager(dht, [uid], p2p) for uid in uids)
     modules = [
         petals.client.RemoteTransformerBlock(config, dht, dht_prefix=dht_prefix, p2p=p2p, sequence_manager=m)
         for m in managers
     ]
     return modules[0] if single_uid else modules
 
 
 def get_remote_module_infos(
-    dht: DHT, uid_or_uids: Union[ModuleUID, Sequence[ModuleUID]], expiration_time: Optional[DHTExpiration] = None
-) -> List[Optional[RemoteModuleInfo]]:
-    single_uid = isinstance(uid_or_uids, ModuleUID)
-    uids = [uid_or_uids] if single_uid else uid_or_uids
-    infos = dht.run_coroutine(
-        partial(_get_remote_module_infos, uids=uids, expiration_time=expiration_time),
-        return_future=False,
+    dht: DHT,
+    uids: Sequence[ModuleUID],
+    expiration_time: Optional[DHTExpiration] = None,
+    *,
+    latest: bool = False,
+    return_future: bool = False,
+) -> Union[List[Optional[RemoteModuleInfo]], MPFuture]:
+    return dht.run_coroutine(
+        partial(_get_remote_module_infos, uids=uids, expiration_time=expiration_time, latest=latest),
+        return_future=return_future,
     )
-    return infos[0] if single_uid else infos
 
 
 async def _get_remote_module_infos(
-    dht: DHT, node: DHTNode, uids: List[ModuleUID], expiration_time: Optional[DHTExpiration]
+    dht: DHT, node: DHTNode, uids: List[ModuleUID], expiration_time: Optional[DHTExpiration], latest: bool
 ) -> List[Optional[RemoteModuleInfo]]:
-    if expiration_time is None:
+    if latest:
+        assert expiration_time is None, "You should define either `expiration_time` or `latest`, not both"
+        expiration_time = math.inf
+    elif expiration_time is None:
         expiration_time = get_dht_time()
     num_workers = len(uids) if dht.num_workers is None else min(len(uids), dht.num_workers)
     found: Dict[ModuleUID, DHTValue] = await node.get_many(uids, expiration_time, num_workers=num_workers)
 
     modules: List[Optional[RemoteModuleInfo]] = [None] * len(uids)
     for i, uid in enumerate(uids):
         metadata = found[uid]
```

### Comparing `petals-1.1.3/src/petals/server/backend.py` & `petals-1.1.4/src/petals/server/backend.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/block_selection.py` & `petals-1.1.4/src/petals/server/block_selection.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/block_utils.py` & `petals-1.1.4/src/petals/server/block_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     eps: float = 0.01,  # eps accounts for ~1% of metainfo for tensor descriptions, quantization tables, etc.
 ) -> int:
     if location == "memory":
         assert (
             dtype is not None and load_in_8bit is not None
         ), 'get_block_size(..., location="memory") requires to specify dtype and load_in_8bit for calculations'
 
-    with init_empty_weights():
+    with init_empty_weights(include_buffers=True):
         block = WrappedBloomBlock(config)
         n_params = sum(param.numel() for param in block.parameters())
 
     if location == "memory" and load_in_8bit:
         # Note: We may need a larger eps here for models of size < 1B
         return n_params * (1 + eps)
```

### Comparing `petals-1.1.3/src/petals/server/handler.py` & `petals-1.1.4/src/petals/server/handler.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/memory_cache.py` & `petals-1.1.4/src/petals/server/memory_cache.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/reachability.py` & `petals-1.1.4/src/petals/server/reachability.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/server.py` & `petals-1.1.4/src/petals/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,20 +159,14 @@
         self.tensor_parallel_devices = tuple(map(torch.device, tensor_parallel_devices))
         if len(self.tensor_parallel_devices) > 1:
             logger.info(f"Model weights will be split between {', '.join(tensor_parallel_devices)}")
             check_device_balance(self.tensor_parallel_devices)
 
         if load_in_8bit is None:
             load_in_8bit = device.type == "cuda"
-            if load_in_8bit and len(self.tensor_parallel_devices) > 1:
-                load_in_8bit = False
-                logger.warning(
-                    "Tensor parallelism doesn't work properly with 8-bit weights yet, loading weights in 16-bit. "
-                    "You can explicitly set `--load_in_8bit True` to override this"
-                )
         self.load_in_8bit = load_in_8bit
         logger.info(f"Model weights will be loaded in {get_dtype_name(torch_dtype, load_in_8bit)} format")
 
         assert num_blocks is None or block_indices is None, "Please specify num_blocks or block_indices, not both"
         if num_blocks is None and block_indices is None:
             num_blocks = self._choose_num_blocks()
         if block_indices is not None:
@@ -326,22 +320,22 @@
     def _choose_blocks(self) -> List[int]:
         if self.strict_block_indices is not None:
             return self.strict_block_indices
 
         # If multiple servers (e.g., launched on the same machine by a script) get to this line at the same time,
         # this delay decreases the probability of a race condition while choosing the best blocks to serve.
         time.sleep(random.random() * 2 * self.mean_block_selection_delay)
-        module_infos = get_remote_module_infos(self.dht, self.module_uids, expiration_time=np.inf)
+        module_infos = get_remote_module_infos(self.dht, self.module_uids, latest=True)
         return block_selection.choose_best_blocks(self.num_blocks, module_infos)
 
     def _should_choose_other_blocks(self) -> bool:
         if self.strict_block_indices is not None:
             return False
 
-        module_infos = get_remote_module_infos(self.dht, self.module_uids, expiration_time=np.inf)
+        module_infos = get_remote_module_infos(self.dht, self.module_uids, latest=True)
         return block_selection.should_choose_other_blocks(self.dht.peer_id, module_infos, self.balance_quality)
 
     def shutdown(self):
         self.stop.set()
 
         if self.reachability_protocol is not None:
             self.reachability_protocol.shutdown()
```

### Comparing `petals-1.1.3/src/petals/server/task_pool.py` & `petals-1.1.4/src/petals/server/task_pool.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/task_prioritizer.py` & `petals-1.1.4/src/petals/server/task_prioritizer.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/server/throughput.py` & `petals-1.1.4/src/petals/server/throughput.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/asyncio.py` & `petals-1.1.4/src/petals/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/convert_block.py` & `petals-1.1.4/src/petals/utils/convert_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tools for converting transformer blocks, applying quantization and/or tensor parallelism
 """
+import os
 import re
 from typing import Sequence
 
 import tensor_parallel as tp
 import torch
 import torch.nn as nn
 from hivemind.utils.logging import get_logger, use_hivemind_log_handler
@@ -71,25 +72,24 @@
             Input model or `torch.nn.Module` as the function is run recursively.
         threshold (`float`, *optional*):
             `int8_threshold` for outlier detection as described in the formentioned paper. This parameters is set to
             `6.0` as described by the paper.
     """
 
     # Import bitsandbytes only when necessary, so Petals runs on platforms not supported by bitsandbytes
+    os.environ["BITSANDBYTES_NOWELCOME"] = "1"
     import bitsandbytes as bnb
 
-    from petals.utils.linear8bitlt_patch import CustomLinear8bitLt
-
     for n, module in model.named_children():
         if len(list(module.children())) > 0:
             replace_8bit_linear(module, threshold)
 
         if isinstance(module, torch.nn.Linear) and n not in ["lm_head", "score"]:
             assert module.weight.device.type == "cpu", f"expected linear layers on CPU, got {module.weight.device}"
-            model._modules[n] = CustomLinear8bitLt(
+            model._modules[n] = bnb.nn.Linear8bitLt(
                 module.in_features,
                 module.out_features,
                 module.bias is not None,
                 has_fp16_weights=False,
                 threshold=threshold,
             )
             model._modules[n].weight = bnb.nn.Int8Params(
```

### Comparing `petals-1.1.3/src/petals/utils/disk_cache.py` & `petals-1.1.4/src/petals/utils/disk_cache.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/generation_algorithms.py` & `petals-1.1.4/src/petals/utils/generation_algorithms.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/generation_constraints.py` & `petals-1.1.4/src/petals/utils/generation_constraints.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/logging.py` & `petals-1.1.4/src/petals/utils/logging.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals/utils/version.py` & `petals-1.1.4/src/petals/utils/version.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/src/petals.egg-info/PKG-INFO` & `petals-1.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 1.1.3
+Version: 1.1.4
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
-Author-email: petals-dev@googlegroups.com
+Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
     <img src="https://i.imgur.com/7eR7Pan.png" width="400"><br>
     Run 100B+ language models at home, BitTorrent-style.<br>
-    Fine-tuning and inference up to 10x faster than offloading<br><br>
+    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading<br><br>
     <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a><br>
 </p>
 
 Generate text using distributed 176B-parameter [BLOOM](https://huggingface.co/bigscience/bloom) or [BLOOMZ](https://huggingface.co/bigscience/bloomz) and fine-tune them for your own tasks:
 
 ```python
 from petals import DistributedBloomForCausalLM
@@ -58,27 +58,27 @@
     🚀 &nbsp;<b><a href="https://colab.research.google.com/drive/1Ervk6HPNS6AYVr3xVdQnY5a-TjjmLCdQ?usp=sharing">Try now in Colab</a></b>
 </p>
 
 🔏 Your data will be processed by other people in the public swarm. Learn more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety). For sensitive data, you can set up a [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
 
 ### Connect your GPU and increase Petals capacity
 
-Run this in an [Anaconda](https://www.anaconda.com) env (requires Linux and Python 3.7+):
+Run our [Docker](https://www.docker.com) image (works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)):
 
 ```bash
-conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install -U petals
-python -m petals.cli.run_server bigscience/bloom-petals
+sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm \
+    learningathome/petals:main python -m petals.cli.run_server bigscience/bloom-petals --port 31330
 ```
 
-Or use our [Docker](https://www.docker.com) image (works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)):
+Or run these commands in an [Anaconda](https://www.anaconda.com) env (requires Linux and Python 3.7+):
 
 ```bash
-sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm \
-    learningathome/petals:main python -m petals.cli.run_server bigscience/bloom-petals --port 31330
+conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
+pip install -U petals
+python -m petals.cli.run_server bigscience/bloom-petals
 ```
 
 📚 See [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to configure the server to use multiple GPUs, address common issues, etc.
 
 You can also host [BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of BLOOM fine-tuned to follow human instructions in the zero-shot regime — just replace `bloom-petals` with `bloomz-petals`.
 
 🔒 Hosting a server does not allow others to run custom code on your computer. Learn more about security [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
@@ -106,84 +106,129 @@
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
 
 📋 If you build an app running BLOOM with Petals, make sure it follows the BLOOM's [terms of use](https://huggingface.co/bigscience/bloom).
 
 ## How does it work?
 
 - Petals runs large language models like [BLOOM-176B](https://huggingface.co/bigscience/bloom) **collaboratively** — you load a small part of the model, then team up with people serving the other parts to run inference or fine-tuning.
-- Inference runs at ≈ 1 sec per step (token) — 10x faster than possible with offloading, enough for chatbots and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
-- Beyond classic language model APIs — you can employ any fine-tuning and sampling methods by executing custom paths through the model or accessing its hidden states. You get the comforts of an API with the flexibility of PyTorch.
+- Single-batch inference runs at ≈ 1 sec per step (token) — [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
+- Beyond classic language model APIs — you can employ any fine-tuning and sampling methods, execute custom paths through the model, or see its hidden states. You get the comforts of an API with the flexibility of PyTorch.
 
 <p align="center">
     <img src="https://i.imgur.com/RTYF3yW.png" width="800">
 </p>
 
 <p align="center">
     📚 &nbsp;<b><a href="https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions">See FAQ</a></b>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
     📜 &nbsp;<b><a href="https://arxiv.org/pdf/2209.01188.pdf">Read paper</a></b>
 </p>
 
 ## Installation
 
-Here's how to install Petals with conda:
+Here's how to install Petals with [Anaconda](https://www.anaconda.com/products/distribution) on Linux:
 
 ```bash
 conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
 pip install -U petals
 ```
 
-This script uses Anaconda to install CUDA-enabled PyTorch.
-If you don't have anaconda, you can get it from [here](https://www.anaconda.com/products/distribution).
-If you don't want anaconda, you can install PyTorch [any other way](https://pytorch.org/get-started/locally/).
-If you want to run models with 8-bit weights, please install **PyTorch with CUDA 11** or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
+If you don't use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/get-started/locally/). If you want to run models with 8-bit weights, please install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
 
-__System requirements:__ Petals only supports Linux for now. If you don't have a Linux machine, consider running Petals in Docker (see our [image](https://hub.docker.com/r/learningathome/petals)) or, in case of Windows, in WSL2 ([read more](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)). CPU is enough to run a client, but you probably need a GPU to run a server efficiently.
+See the instructions for macOS and Windows, the full requirements, and troubleshooting advice in our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-client).
 
-## 🛠️ Development
+## Benchmarks
 
-Petals uses pytest with a few plugins. To install them, run:
-
-```bash
-conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-git clone https://github.com/bigscience-workshop/petals.git && cd petals
-pip install -e .[dev]
-```
-
-To run minimalistic tests, you need to make a local swarm with a small model and some servers. You may find more information about how local swarms work and how to run them in [this tutorial](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm).
-
-```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main
-
-python -m petals.cli.run_server $MODEL_NAME --block_indices 0:12 \
-  --identity tests/test.id --host_maddrs /ip4/127.0.0.1/tcp/31337 --new_swarm  &> server1.log &
-sleep 5  # wait for the first server to initialize DHT
-
-python -m petals.cli.run_server $MODEL_NAME --block_indices 12:24 \
-  --initial_peers SEE_THE_OUTPUT_OF_THE_1ST_PEER &> server2.log &
-
-tail -f server1.log server2.log  # view logs for both servers
-```
-
-Then launch pytest:
-
-```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main REF_NAME=bigscience/bloom-560m
-export INITIAL_PEERS=/ip4/127.0.0.1/tcp/31337/p2p/QmS9KwZptnVdB9FFV7uGgaTq4sEKBwcYeKZDfSpyKDUd1g
-PYTHONPATH=. pytest tests --durations=0 --durations-min=1.0 -v
-```
+<table align="center">
+  <tr>
+    <th colspan="2">Network</th>
+    <th colspan="2">Single-batch inference<br>(steps/s)</th>
+    <th colspan="2">Parallel forward<br>(tokens/s)</th>
+  </tr>
+  <tr>
+    <th rowspan="2">Bandwidth</th>
+    <th rowspan="2">Round-trip<br>latency</th>
+    <th colspan="2">Sequence length</th>
+    <th colspan="2">Batch size</th>
+  </tr>
+  <tr align="center">
+    <td>128</td>
+    <td>2048</td>
+    <td>1</td>
+    <td>64</td>
+  </tr>
+  <tr>
+    <th colspan="6">Offloading, max. possible speed on 1x A100 <sup>1</sup></th>
+  </tr>
+  <tr align="center">
+    <td>256 Gbit/s</td>
+    <td></td>
+    <td>0.18</td>
+    <td>0.18</td>
+    <td>2.7</td>
+    <td>170.3</td>
+  </tr>
+  <tr align="center">
+    <td>128 Gbit/s</td>
+    <td></td>
+    <td>0.09</td>
+    <td>0.09</td>
+    <td>2.4</td>
+    <td>152.8</td>
+  </tr>
+  <tr>
+    <th colspan="6">Petals on 14 heterogeneous servers across Europe and North America <sup>2</sup></th>
+  </tr>
+  <tr align="center">
+    <td colspan="2">Real world</td>
+    <td>0.83</td>
+    <td>0.79</td>
+    <td>32.6</td>
+    <td>179.4</td>
+  </tr>
+  <tr>
+    <th colspan="6">Petals on 3 servers, with one A100 each <sup>3</sup></th>
+  </tr>
+  <tr align="center">
+    <td>1 Gbit/s</td>
+    <td>&lt; 5 ms</td>
+    <td>1.71</td>
+    <td>1.54</td>
+    <td>70.0</td>
+    <td>253.6</td>
+  </tr>
+  <tr align="center">
+    <td>100 Mbit/s</td>
+    <td>&lt; 5 ms</td>
+    <td>1.66</td>
+    <td>1.49</td>
+    <td>56.4</td>
+    <td>182.0</td>
+  </tr>
+  <tr align="center">
+    <td>100 Mbit/s</td>
+    <td>100 ms</td>
+    <td>1.23</td>
+    <td>1.11</td>
+    <td>19.7</td>
+    <td>112.2</td>
+  </tr>
+</table>
+
+<sup>1</sup> **An upper bound for offloading performance.** We base our offloading numbers on the best possible hardware setup for offloading: CPU RAM offloading via PCIe 4.0 with 16 PCIe lanes per GPU and PCIe switches for pairs of GPUs. We assume zero latency for the upper bound estimation. In 8-bit, the model uses 1 GB of memory per billion parameters. PCIe 4.0 with 16 lanes has a throughput of 256 Gbit/s, so offloading 176B parameters takes 5.5 seconds. The throughput is twice as slow (128 Gbit/s) if we have two GPUs behind the same PCIe switch.
+
+<sup>2</sup> **A real-world distributed setting** with 14 servers holding 2× RTX 3060, 4× 2080Ti, 2× 3090, 2× A4000, and 4× A5000 GPUs. These are personal servers and servers from university labs, spread across Europe and North America and connected to the Internet at speeds of 100–1000 Mbit/s. 4 servers operate from under firewalls.
 
-After you're done, you can terminate the servers and ensure that no zombie processes are left with `pkill -f petals.cli.run_server && pkill -f p2p`.
+<sup>3</sup> **An optimistic setup** that requires least communication. The client nodes have 8 CPU cores and no GPU.
 
-The automated tests use a more complex server configuration that can be found [here](https://github.com/bigscience-workshop/petals/blob/main/.github/workflows/run-tests.yaml).
+We provide more evaluations and discuss these results in more detail in **Section 3.3** of our [paper](https://arxiv.org/pdf/2209.01188.pdf).
 
-### Code style
+## 🛠️ Contributing
 
-We use [black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html) and [isort](https://pycqa.github.io/isort/) for all pull requests.
-Before committing your code, simply run `black . && isort .` and you will be fine.
+Please see our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#contributing) on contributing.
 
 ## 📜 Citation
 
 Alexander Borzunov, Dmitry Baranchuk, Tim Dettmers, Max Ryabinin, Younes Belkada, Artem Chumachenko, Pavel Samygin, and Colin Raffel.
 [Petals: Collaborative Inference and Fine-tuning of Large Models.](https://arxiv.org/abs/2209.01188)
 _arXiv preprint arXiv:2209.01188,_ 2022.
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: petals Version: 1.1.3 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 1.1.4 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
-petals-dev@googlegroups.com Project-URL: Bug Tracker, https://github.com/
+petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Provides-Extra: dev License-File: LICENSE
                        [https://i.imgur.com/7eR7Pan.png]
              Run 100B+ language models at home, BitTorrent-style.
-          Fine-tuning and inference up to 10x faster than offloading
+          Fine-tuning and inference up_to_10x_faster than offloading
 
             [https://img.shields.io/pypi/v/petals.svg?color=green]
 Generate text using distributed 176B-parameter [BLOOM](https://huggingface.co/
 bigscience/bloom) or [BLOOMZ](https://huggingface.co/bigscience/bloomz) and
 fine-tune them for your own tasks: ```python from petals import
 DistributedBloomForCausalLM model = DistributedBloomForCausalLM.from_pretrained
 ("bigscience/bloom-petals", tuning_mode="ptune", pre_seq_len=16) # Embeddings &
@@ -34,33 +34,33 @@
 ```
                             ð  Try_now_in_Colab
 ð Your data will be processed by other people in the public swarm. Learn
 more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/
 Security,-privacy,-and-AI-safety). For sensitive data, you can set up a
 [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
 own-swarm) among people you trust. ### Connect your GPU and increase Petals
-capacity Run this in an [Anaconda](https://www.anaconda.com) env (requires
-Linux and Python 3.7+): ```bash conda install pytorch pytorch-cuda=11.7 -
-c pytorch -c nvidia pip install -U petals python -m petals.cli.run_server
-bigscience/bloom-petals ``` Or use our [Docker](https://www.docker.com) image
-(works on Linux, macOS, and Windows with [WSL2](https://learn.microsoft.com/en-
-us/windows/ai/directml/gpu-cuda-in-wsl)): ```bash sudo docker run -p 31330:
-31330 --ipc host --gpus all --volume petals-cache:/cache --rm \ learningathome/
-petals:main python -m petals.cli.run_server bigscience/bloom-petals --port
-31330 ``` ð See [FAQ](https://github.com/bigscience-workshop/petals/wiki/
-FAQ:-Frequently-asked-questions#running-a-server) to learn how to configure the
-server to use multiple GPUs, address common issues, etc. You can also host
-[BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of BLOOM fine-
-tuned to follow human instructions in the zero-shot regime â just replace
-`bloom-petals` with `bloomz-petals`. ð Hosting a server does not allow
-others to run custom code on your computer. Learn more about security [here]
-(https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-
-safety). ð¬ If you have any issues or feedback, let us know on [our Discord
-server](https://discord.gg/D9MwApKgWa)! ### Check out tutorials, examples, and
-more Basic tutorials: - Getting started: [tutorial](https://
+capacity Run our [Docker](https://www.docker.com) image (works on Linux, macOS,
+and Windows with [WSL2](https://learn.microsoft.com/en-us/windows/ai/directml/
+gpu-cuda-in-wsl)): ```bash sudo docker run -p 31330:31330 --ipc host --gpus all
+--volume petals-cache:/cache --rm \ learningathome/petals:main python -
+m petals.cli.run_server bigscience/bloom-petals --port 31330 ``` Or run these
+commands in an [Anaconda](https://www.anaconda.com) env (requires Linux and
+Python 3.7+): ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
+c nvidia pip install -U petals python -m petals.cli.run_server bigscience/
+bloom-petals ``` ð See [FAQ](https://github.com/bigscience-workshop/petals/
+wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to
+configure the server to use multiple GPUs, address common issues, etc. You can
+also host [BLOOMZ](https://huggingface.co/bigscience/bloomz), a version of
+BLOOM fine-tuned to follow human instructions in the zero-shot regime â just
+replace `bloom-petals` with `bloomz-petals`. ð Hosting a server does not
+allow others to run custom code on your computer. Learn more about security
+[here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-
+and-AI-safety). ð¬ If you have any issues or feedback, let us know on [our
+Discord server](https://discord.gg/D9MwApKgWa)! ### Check out tutorials,
+examples, and more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1Ervk6HPNS6AYVr3xVdQnY5a-TjjmLCdQ?usp=sharing)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-personachat.ipynb) - Prompt-tune BLOOM for text semantic
 classification: [tutorial](https://colab.research.google.com/github/bigscience-
 workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb) Useful tools and
 advanced guides: - [Chatbot web app](http://chat.petals.ml) (connects to Petals
@@ -73,67 +73,69 @@
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ð If you build an app running
 BLOOM with Petals, make sure it follows the BLOOM's [terms of use](https://
 huggingface.co/bigscience/bloom). ## How does it work? - Petals runs large
 language models like [BLOOM-176B](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
-people serving the other parts to run inference or fine-tuning. - Inference
-runs at â 1 sec per step (token) â 10x faster than possible with
-offloading, enough for chatbots and other interactive apps. Parallel inference
-reaches hundreds of tokens/sec. - Beyond classic language model APIs â you
-can employ any fine-tuning and sampling methods by executing custom paths
-through the model or accessing its hidden states. You get the comforts of an
-API with the flexibility of PyTorch.
+people serving the other parts to run inference or fine-tuning. - Single-batch
+inference runs at â 1 sec per step (token) â [up to 10x faster](https://
+github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for
+[chatbots](http://chat.petals.ml) and other interactive apps. Parallel
+inference reaches hundreds of tokens/sec. - Beyond classic language model APIs
+â you can employ any fine-tuning and sampling methods, execute custom paths
+through the model, or see its hidden states. You get the comforts of an API
+with the flexibility of PyTorch.
                        [https://i.imgur.com/RTYF3yW.png]
                    ð  See_FAQ            ð  Read_paper
-## Installation Here's how to install Petals with conda: ```bash conda install
-pytorch pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` This
-script uses Anaconda to install CUDA-enabled PyTorch. If you don't have
-anaconda, you can get it from [here](https://www.anaconda.com/products/
-distribution). If you don't want anaconda, you can install PyTorch [any other
-way](https://pytorch.org/get-started/locally/). If you want to run models with
-8-bit weights, please install **PyTorch with CUDA 11** or newer for compatility
-with [bitsandbytes](https://github.com/timDettmers/bitsandbytes). __System
-requirements:__ Petals only supports Linux for now. If you don't have a Linux
-machine, consider running Petals in Docker (see our [image](https://
-hub.docker.com/r/learningathome/petals)) or, in case of Windows, in WSL2 ([read
-more](https://learn.microsoft.com/en-us/windows/ai/directml/gpu-cuda-in-wsl)).
-CPU is enough to run a client, but you probably need a GPU to run a server
-efficiently. ## ð ï¸ Development Petals uses pytest with a few plugins. To
-install them, run: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
-c nvidia git clone https://github.com/bigscience-workshop/petals.git && cd
-petals pip install -e .[dev] ``` To run minimalistic tests, you need to make a
-local swarm with a small model and some servers. You may find more information
-about how local swarms work and how to run them in [this tutorial](https://
-github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm). ```bash
-export MODEL_NAME=bloom-testing/test-bloomd-560m-main python -
-m petals.cli.run_server $MODEL_NAME --block_indices 0:12 \ --identity tests/
-test.id --host_maddrs /ip4/127.0.0.1/tcp/31337 --new_swarm &> server1.log &
-sleep 5 # wait for the first server to initialize DHT python -
-m petals.cli.run_server $MODEL_NAME --block_indices 12:24 \ --initial_peers
-SEE_THE_OUTPUT_OF_THE_1ST_PEER &> server2.log & tail -f server1.log server2.log
-# view logs for both servers ``` Then launch pytest: ```bash export
-MODEL_NAME=bloom-testing/test-bloomd-560m-main REF_NAME=bigscience/bloom-560m
-export INITIAL_PEERS=/ip4/127.0.0.1/tcp/31337/p2p/
-QmS9KwZptnVdB9FFV7uGgaTq4sEKBwcYeKZDfSpyKDUd1g PYTHONPATH=. pytest tests --
-durations=0 --durations-min=1.0 -v ``` After you're done, you can terminate the
-servers and ensure that no zombie processes are left with `pkill -
-f petals.cli.run_server && pkill -f p2p`. The automated tests use a more
-complex server configuration that can be found [here](https://github.com/
-bigscience-workshop/petals/blob/main/.github/workflows/run-tests.yaml). ###
-Code style We use [black](https://black.readthedocs.io/en/stable/
-the_black_code_style/current_style.html) and [isort](https://pycqa.github.io/
-isort/) for all pull requests. Before committing your code, simply run `black .
-&& isort .` and you will be fine. ## ð Citation Alexander Borzunov, Dmitry
-Baranchuk, Tim Dettmers, Max Ryabinin, Younes Belkada, Artem Chumachenko, Pavel
-Samygin, and Colin Raffel. [Petals: Collaborative Inference and Fine-tuning of
-Large Models.](https://arxiv.org/abs/2209.01188) _arXiv preprint arXiv:
-2209.01188,_ 2022. ```bibtex @article{borzunov2022petals, title = {Petals:
-Collaborative Inference and Fine-tuning of Large Models}, author = {Borzunov,
-Alexander and Baranchuk, Dmitry and Dettmers, Tim and Ryabinin, Max and
-Belkada, Younes and Chumachenko, Artem and Samygin, Pavel and Raffel, Colin},
-journal = {arXiv preprint arXiv:2209.01188}, year = {2022}, url = {https://
-arxiv.org/abs/2209.01188} } ``` -----------------------------------------------
----------------------------------
+## Installation Here's how to install Petals with [Anaconda](https://
+www.anaconda.com/products/distribution) on Linux: ```bash conda install pytorch
+pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` If you don't
+use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/
+get-started/locally/). If you want to run models with 8-bit weights, please
+install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes]
+(https://github.com/timDettmers/bitsandbytes). See the instructions for macOS
+and Windows, the full requirements, and troubleshooting advice in our [FAQ]
+(https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-
+questions#running-a-client). ## Benchmarks
+     Network               Single-batch inference Parallel forward
+                           (steps/s)              (tokens/s)
+     Bandwidth  Round-trip Sequence length        Batch size
+                latency    128           2048       1              64
+     Offloading, max. possible speed on 1x A100 1
+     256 Gbit/s            0.18          0.18     2.7           170.3
+     128 Gbit/s            0.09          0.09     2.4           152.8
+     Petals on 14 heterogeneous servers across Europe and North America 2
+             Real world    0.83          0.79     32.6          179.4
+     Petals on 3 servers, with one A100 each 3
+      1 Gbit/s     < 5 ms  1.71          1.54     70.0          253.6
+     100 Mbit/s    < 5 ms  1.66          1.49     56.4          182.0
+     100 Mbit/s    100 ms  1.23          1.11     19.7          112.2
+1 **An upper bound for offloading performance.** We base our offloading numbers
+on the best possible hardware setup for offloading: CPU RAM offloading via PCIe
+4.0 with 16 PCIe lanes per GPU and PCIe switches for pairs of GPUs. We assume
+zero latency for the upper bound estimation. In 8-bit, the model uses 1 GB of
+memory per billion parameters. PCIe 4.0 with 16 lanes has a throughput of 256
+Gbit/s, so offloading 176B parameters takes 5.5 seconds. The throughput is
+twice as slow (128 Gbit/s) if we have two GPUs behind the same PCIe switch. 2
+**A real-world distributed setting** with 14 servers holding 2Ã RTX 3060, 4Ã
+2080Ti, 2Ã 3090, 2Ã A4000, and 4Ã A5000 GPUs. These are personal servers and
+servers from university labs, spread across Europe and North America and
+connected to the Internet at speeds of 100â1000 Mbit/s. 4 servers operate
+from under firewalls. 3 **An optimistic setup** that requires least
+communication. The client nodes have 8 CPU cores and no GPU. We provide more
+evaluations and discuss these results in more detail in **Section 3.3** of our
+[paper](https://arxiv.org/pdf/2209.01188.pdf). ## ð ï¸ Contributing Please
+see our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-
+Frequently-asked-questions#contributing) on contributing. ## ð Citation
+Alexander Borzunov, Dmitry Baranchuk, Tim Dettmers, Max Ryabinin, Younes
+Belkada, Artem Chumachenko, Pavel Samygin, and Colin Raffel. [Petals:
+Collaborative Inference and Fine-tuning of Large Models.](https://arxiv.org/
+abs/2209.01188) _arXiv preprint arXiv:2209.01188,_ 2022. ```bibtex @article
+{borzunov2022petals, title = {Petals: Collaborative Inference and Fine-tuning
+of Large Models}, author = {Borzunov, Alexander and Baranchuk, Dmitry and
+Dettmers, Tim and Ryabinin, Max and Belkada, Younes and Chumachenko, Artem and
+Samygin, Pavel and Raffel, Colin}, journal = {arXiv preprint arXiv:2209.01188},
+year = {2022}, url = {https://arxiv.org/abs/2209.01188} } ``` -----------------
+---------------------------------------------------------------
           This project is a part of the BigScience research workshop.
                       [https://petals.ml/bigscience.png]
```

### Comparing `petals-1.1.3/src/petals.egg-info/SOURCES.txt` & `petals-1.1.4/src/petals.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,20 @@
 src/petals/server/throughput.py
 src/petals/utils/__init__.py
 src/petals/utils/asyncio.py
 src/petals/utils/convert_block.py
 src/petals/utils/disk_cache.py
 src/petals/utils/generation_algorithms.py
 src/petals/utils/generation_constraints.py
-src/petals/utils/linear8bitlt_patch.py
 src/petals/utils/logging.py
 src/petals/utils/misc.py
 src/petals/utils/version.py
 tests/test_aux_functions.py
 tests/test_block_exact_match.py
 tests/test_chained_calls.py
 tests/test_full_model.py
-tests/test_linear8bitlt.py
 tests/test_priority_pool.py
 tests/test_remote_sequential.py
 tests/test_sequence_manager.py
 tests/test_server_stats.py
 tests/test_tensor_parallel.py
 tests/test_utils.py
```

### Comparing `petals-1.1.3/tests/test_aux_functions.py` & `petals-1.1.4/tests/test_aux_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import torch
-from test_utils import MODEL_NAME
 
 from petals.client import DistributedBloomConfig
-from petals.server.throughput import measure_compute_rps, measure_network_rps
+from petals.server.throughput import measure_compute_rps
+from test_utils import MODEL_NAME
 
 
 @pytest.mark.forked
 @pytest.mark.parametrize("tensor_parallel", [False, True])
 def test_compute_throughput(tensor_parallel: bool):
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
     tensor_parallel_devices = ("cpu", "cpu") if tensor_parallel else ()
```

### Comparing `petals-1.1.3/tests/test_block_exact_match.py` & `petals-1.1.4/tests/test_chained_calls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,79 @@
-import random
+######
+# Warning:torch this test is a work in progress. It will be modified soon.
+# - if you want more stable tests, see test_block_exact_match
+# - if you want to figure out chained inference, ask yozh
+
 
 import hivemind
 import pytest
 import torch
-from test_utils import *
 
 from petals.bloom.from_pretrained import load_pretrained_block
 from petals.client import DistributedBloomConfig
-from petals.client.remote_sequential import RemoteTransformerBlock
-from petals.data_structures import UID_DELIMITER
-from petals.dht_utils import get_remote_module
+from petals.client.remote_sequential import RemoteSequential
+from petals.dht_utils import get_remote_sequence
+from test_utils import *
 
 
 @pytest.mark.forked
-def test_remote_block_exact_match(atol_forward=1e-4, atol_inference=1e-3):
+def test_forward_backward_exact_match(atol_forward=1e-4, atol_backward=1e-4, seq_length=1):
     dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
+    remote_blocks = get_remote_sequence(dht, 3, 6, config)
+    assert isinstance(remote_blocks, RemoteSequential)
+
+    ref_blocks = [
+        load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch.float32),
+        load_pretrained_block(MODEL_NAME, 4, torch_dtype=torch.float32),
+        load_pretrained_block(MODEL_NAME, 5, torch_dtype=torch.float32),
+    ]
+    inputs = torch.randn(1, seq_length, config.hidden_size, requires_grad=True)
+    outputs_rpc = remote_blocks.forward(inputs)
+    outputs_rpc.sum().backward()
+    grads_rpc = inputs.grad
+
+    inputs.grad = None
+    hidden_states = inputs
+    for ref_block in ref_blocks:
+        hidden_states = ref_block.forward(hidden_states)[0]
+    outputs_ref = hidden_states
+    outputs_ref.sum().backward()
+    grads_ref = inputs.grad
 
-    for block_index in random.sample(range(config.n_layer), 3):
-        remote_block = get_remote_module(dht, f"{MODEL_NAME}{UID_DELIMITER}{block_index}", config)
-        assert isinstance(remote_block, RemoteTransformerBlock)
-
-        inputs = torch.randn(1, 8, config.hidden_size)
-        outputs_forward = remote_block(inputs)
-
-        outputs_inference = []
-        with remote_block.inference_session(max_length=inputs.shape[1]) as sess:
-            for i in range(inputs.shape[1]):
-                outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
-
-            # test that max length is respected
-            with pytest.raises(ValueError, match=r"Maximum length exceeded") as exc_info:
-                sess.step(inputs[:, -1:, :])
-            assert "Maximum length exceeded" in repr(exc_info.value)
+    assert torch.allclose(outputs_ref, outputs_rpc, rtol=0, atol=atol_forward)
+    assert torch.allclose(grads_ref, grads_rpc, rtol=0, atol=atol_backward)
 
-        outputs_inference = torch.cat(outputs_inference, dim=1)
 
-        ref_block = load_pretrained_block(MODEL_NAME, block_index, torch_dtype=torch.float32)
-        (outputs_local,) = ref_block(inputs)
+@pytest.mark.forked
+def test_chained_inference_exact_match(atol_inference=1e-4):
+    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
+    config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
+    remote_blocks = get_remote_sequence(dht, 3, 5, config)
+    assert isinstance(remote_blocks, RemoteSequential)
+
+    inputs = torch.randn(1, 8, config.hidden_size)
 
-        assert torch.allclose(outputs_local, outputs_forward, rtol=0, atol=atol_forward)
-        assert torch.allclose(outputs_local, outputs_inference, rtol=0, atol=atol_inference)
+    outputs_inference = []
+    with remote_blocks.inference_session(max_length=inputs.shape[1]) as sess:
+        for i in range(inputs.shape[1]):
+            outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
+    outputs_inference = torch.cat(outputs_inference, dim=1)
+
+    ref_blocks = [
+        load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch.float32),
+        load_pretrained_block(MODEL_NAME, 4, torch_dtype=torch.float32),
+    ]
+    outputs_ref = []
+    caches = [None, None]
+    for i in range(inputs.shape[1]):
+        new_caches = []
+        hidden_states = inputs[:, i : i + 1, :]
+        for ref_block, cache in zip(ref_blocks, caches):
+            with torch.no_grad():
+                hidden_states, new_cache = ref_block.forward(hidden_states, use_cache=True, layer_past=cache)
+                new_caches.append(new_cache)
+
+        outputs_ref.append(hidden_states)
+        caches = new_caches
+    outputs_ref = torch.cat(outputs_ref, dim=1)
+    assert torch.allclose(outputs_ref, outputs_inference, rtol=0, atol=atol_inference)
```

### Comparing `petals-1.1.3/tests/test_chained_calls.py` & `petals-1.1.4/tests/test_block_exact_match.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,90 @@
-######
-# Warning:torch this test is a work in progress. It will be modified soon.
-# - if you want more stable tests, see test_block_exact_match
-# - if you want to figure out chained inference, ask yozh
-
+import random
+from typing import Union
 
 import hivemind
 import pytest
 import torch
-from test_utils import *
+from transformers.models.bloom.configuration_bloom import BloomConfig
 
-from petals.bloom.from_pretrained import load_pretrained_block
+from petals.bloom.block import WrappedBloomBlock
+from petals.bloom.from_pretrained import DTYPE_MAP, _load_state_dict, load_pretrained_block
 from petals.client import DistributedBloomConfig
-from petals.client.remote_sequential import RemoteSequential
-from petals.dht_utils import get_remote_sequence
+from petals.client.remote_sequential import RemoteTransformerBlock
+from petals.data_structures import UID_DELIMITER
+from petals.dht_utils import get_remote_module
+from test_utils import *
 
 
 @pytest.mark.forked
-def test_forward_backward_exact_match(atol_forward=1e-4, atol_backward=1e-4, seq_length=1):
+def test_remote_block_exact_match(atol_forward=1e-4, atol_inference=1e-3):
     dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
-    remote_blocks = get_remote_sequence(dht, 3, 6, config)
-    assert isinstance(remote_blocks, RemoteSequential)
 
-    ref_blocks = [
-        load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch.float32),
-        load_pretrained_block(MODEL_NAME, 4, torch_dtype=torch.float32),
-        load_pretrained_block(MODEL_NAME, 5, torch_dtype=torch.float32),
-    ]
-    inputs = torch.randn(1, seq_length, config.hidden_size, requires_grad=True)
-    outputs_rpc = remote_blocks.forward(inputs)
-    outputs_rpc.sum().backward()
-    grads_rpc = inputs.grad
-
-    inputs.grad = None
-    hidden_states = inputs
-    for ref_block in ref_blocks:
-        hidden_states = ref_block.forward(hidden_states)[0]
-    outputs_ref = hidden_states
-    outputs_ref.sum().backward()
-    grads_ref = inputs.grad
+    for block_index in random.sample(range(config.n_layer), 3):
+        remote_block = get_remote_module(dht, f"{MODEL_NAME}{UID_DELIMITER}{block_index}", config)
+        assert isinstance(remote_block, RemoteTransformerBlock)
+
+        inputs = torch.randn(1, 8, config.hidden_size)
+        outputs_forward = remote_block(inputs)
+
+        outputs_inference = []
+        with remote_block.inference_session(max_length=inputs.shape[1]) as sess:
+            for i in range(inputs.shape[1]):
+                outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
+
+            # test that max length is respected
+            with pytest.raises(ValueError, match=r"Maximum length exceeded") as exc_info:
+                sess.step(inputs[:, -1:, :])
+            assert "Maximum length exceeded" in repr(exc_info.value)
+
+        outputs_inference = torch.cat(outputs_inference, dim=1)
+
+        ref_block = load_pretrained_block(MODEL_NAME, block_index, torch_dtype=torch.float32)
+        (outputs_local,) = ref_block(inputs)
+
+        assert torch.allclose(outputs_local, outputs_forward, rtol=0, atol=atol_forward)
+        assert torch.allclose(outputs_local, outputs_inference, rtol=0, atol=atol_inference)
+
+
+def _old_load_pretrained_block(
+    converted_model_name_or_path: str,
+    block_index: int,
+    torch_dtype: Union[torch.dtype, str] = "auto",
+) -> WrappedBloomBlock:
+    """Load the BLOOM block by directly initializing the weights.
+    This test is used to check consistency with the previous implementation and can be removed in the future."""
+    config = BloomConfig.from_pretrained(converted_model_name_or_path)
+
+    block = WrappedBloomBlock(config)
+    state_dict = _load_state_dict(
+        converted_model_name_or_path,
+        block_index,
+        config,
+        cache_dir=None,
+    )
+
+    if torch_dtype == "auto":
+        with torch.no_grad():
+            for name, param in block.named_parameters():
+                assert name in state_dict, f"{name} not in state dict"
+                param.data = param.data.to(state_dict[name].dtype)
+    else:
+        assert torch_dtype in DTYPE_MAP.values(), f"torch_dtype must be one of {list(DTYPE_MAP.values())}"
+        block = block.to(dtype=torch_dtype)
 
-    assert torch.allclose(outputs_ref, outputs_rpc, rtol=0, atol=atol_forward)
-    assert torch.allclose(grads_ref, grads_rpc, rtol=0, atol=atol_backward)
+    block.load_state_dict(state_dict, strict=True)
+    return block
 
 
 @pytest.mark.forked
-def test_chained_inference_exact_match(atol_inference=1e-4):
-    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
+def test_init_pretrained_block(torch_dtype=torch.float32, atol_forward=1e-8):
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
-    remote_blocks = get_remote_sequence(dht, 3, 5, config)
-    assert isinstance(remote_blocks, RemoteSequential)
+    torch.random.manual_seed(0)
+    inputs = torch.randn(1, 16, config.hidden_size, dtype=torch_dtype)
 
-    inputs = torch.randn(1, 8, config.hidden_size)
+    block = load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch_dtype)
+    ref_block = _old_load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch_dtype)
 
-    outputs_inference = []
-    with remote_blocks.inference_session(max_length=inputs.shape[1]) as sess:
-        for i in range(inputs.shape[1]):
-            outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
-    outputs_inference = torch.cat(outputs_inference, dim=1)
-
-    ref_blocks = [
-        load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch.float32),
-        load_pretrained_block(MODEL_NAME, 4, torch_dtype=torch.float32),
-    ]
-    outputs_ref = []
-    caches = [None, None]
-    for i in range(inputs.shape[1]):
-        new_caches = []
-        hidden_states = inputs[:, i : i + 1, :]
-        for ref_block, cache in zip(ref_blocks, caches):
-            with torch.no_grad():
-                hidden_states, new_cache = ref_block.forward(hidden_states, use_cache=True, layer_past=cache)
-                new_caches.append(new_cache)
-
-        outputs_ref.append(hidden_states)
-        caches = new_caches
-    outputs_ref = torch.cat(outputs_ref, dim=1)
-    assert torch.allclose(outputs_ref, outputs_inference, rtol=0, atol=atol_inference)
+    outputs = block.forward(inputs)[0]
+    outputs_ref = ref_block.forward(inputs)[0]
+    assert torch.allclose(outputs, outputs_ref, rtol=0, atol=atol_forward)
```

### Comparing `petals-1.1.3/tests/test_full_model.py` & `petals-1.1.4/tests/test_full_model.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 import torch
 import transformers
 from hivemind import get_logger
-from test_utils import *
 from transformers.generation import BeamSearchScorer
 from transformers.models.bloom import BloomForCausalLM
 
 from petals.client.remote_model import DistributedBloomForCausalLM
+from test_utils import *
 
 logger = get_logger(__name__)
 
 
 @pytest.mark.forked
 @pytest.mark.parametrize("pass_empty_tensors", (True, False))
 def test_full_model_exact_match(pass_empty_tensors: bool, atol_forward=1e-3, atol_inference=1e-3):
```

### Comparing `petals-1.1.3/tests/test_priority_pool.py` & `petals-1.1.4/tests/test_priority_pool.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.3/tests/test_remote_sequential.py` & `petals-1.1.4/tests/test_remote_sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 import torch
 import torch.nn.functional as F
-from hivemind import DHT, BatchTensorDescriptor, get_logger, use_hivemind_log_handler
+from hivemind import DHT, BatchTensorDescriptor, get_logger
 from hivemind.proto import runtime_pb2
-from test_utils import *
 
 from petals.bloom.from_pretrained import load_pretrained_block
 from petals.client import RemoteSequenceManager, RemoteSequential
 from petals.client.remote_model import DistributedBloomConfig
 from petals.data_structures import UID_DELIMITER
+from test_utils import *
 
 logger = get_logger(__name__)
 
 
 @pytest.mark.forked
 def test_remote_sequential():
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
@@ -44,15 +44,15 @@
 
     (second_half_outputs * grad_proj).sum().backward()
     assert torch.allclose(test_inputs.grad, full_grad, atol=1e-3)
 
     # test RemoteSequential with lossy compression
     block_uids = [f"{config.dht_prefix}{UID_DELIMITER}{i}" for i in range(config.n_layer)]
     lossy_sequential = RemoteSequential(
-        config, dht, sequence_manager=DummyCustomSequenceManager(dht, block_uids, sequential.p2p, start=True)
+        config, dht, sequence_manager=DummyCustomSequenceManager(dht, block_uids, sequential.p2p)
     )
 
     test_inputs.grad = None
     approx_outputs = lossy_sequential(test_inputs)
     (approx_outputs * grad_proj).sum().backward()
 
     assert not torch.allclose(approx_outputs, full_outputs, rtol=0, atol=1e-4), "compression was not used"
```

### Comparing `petals-1.1.3/tests/test_sequence_manager.py` & `petals-1.1.4/tests/test_sequence_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import threading
 import time
 
 import pytest
 import torch
 from hivemind import DHT, get_logger
-from test_utils import *
 
 from petals.client import RemoteSequenceManager, RemoteSequential
 from petals.client.remote_model import DistributedBloomConfig
 from petals.data_structures import UID_DELIMITER
+from test_utils import *
 
 logger = get_logger(__name__)
 
 
 @pytest.mark.forked
 @pytest.mark.parametrize("mode", ["fastest", "random"])
 def test_sequence_manager_basics(mode: str):
@@ -22,15 +22,15 @@
     shutdown_evt = threading.Event()
 
     # test RemoteSequential with lossy compression
     block_uids = [f"{config.dht_prefix}{UID_DELIMITER}{i}" for i in range(config.n_layer)]
     sequential = RemoteSequential(
         config,
         dht,
-        sequence_manager=TestSequenceManager(dht, block_uids, sequential.p2p, _was_shut_down=shutdown_evt, start=True),
+        sequence_manager=TestSequenceManager(dht, block_uids, sequential.p2p, _was_shut_down=shutdown_evt),
     )
 
     sequence = sequential.sequence_manager.make_sequence(mode=mode)
     assert all(sequence[i].peer_id != sequence[i + 1].peer_id for i in range(len(sequence) - 1))
 
     assert sequential.sequence_manager.is_alive()
     assert sequential.sequence_manager._thread.ready.is_set()
```

### Comparing `petals-1.1.3/tests/test_server_stats.py` & `petals-1.1.4/tests/test_server_stats.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import time
 
 import hivemind
 import pytest
 import torch
-from test_utils import *
 
 from petals.client import DistributedBloomConfig
 from petals.data_structures import UID_DELIMITER
 from petals.dht_utils import get_remote_sequence
 from petals.server.handler import CACHE_TOKENS_AVAILABLE
+from test_utils import *
 
 
 @pytest.mark.forked
 def test_server_info(block_from: int = 22, block_to: int = 24, max_length: int = 100, max_length2: int = 50):
     dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
```

### Comparing `petals-1.1.3/tests/test_tensor_parallel.py` & `petals-1.1.4/tests/test_tensor_parallel.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import random
 
 import pytest
 import torch
 import transformers
 from tensor_parallel import TensorParallel
 from tensor_parallel.slicing_configs import get_bloom_config
-from test_utils import MODEL_NAME
 
 from petals.bloom.from_pretrained import load_pretrained_block
+from test_utils import MODEL_NAME
 
 
 @pytest.mark.forked
 @pytest.mark.parametrize("custom_config", [True, False])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3, ("cpu",) * 4])
 def test_tp_block(devices, custom_config):
     block_index = random.randint(0, 10)
```

