# Comparing `tmp/kevin-toolbox-dev-1.0.4.tar.gz` & `tmp/kevin-toolbox-dev-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kevin-toolbox-dev-1.0.4.tar", last modified: Thu Apr 13 08:01:59 2023, max compression
+gzip compressed data, was "dist/kevin-toolbox-dev-1.0.5.tar", last modified: Fri Apr 21 06:51:15 2023, max compression
```

## Comparing `kevin-toolbox-dev-1.0.4.tar` & `kevin-toolbox-dev-1.0.5.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2493 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1926 2023-04-13 08:01:06.000000 kevin-toolbox-dev-1.0.4/README.md
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      410 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1920 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2084 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/pareto_front/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/search/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/search/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/search/binary_search.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       67 2022-09-19 12:30:55.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6422 2023-03-24 06:33:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-04-10 09:48:35.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_dict/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-04-10 09:22:49.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_dict/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      767 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_dict/deep_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_seq/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_seq/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1015 2023-04-09 15:42:24.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_seq/flatten_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-04-09 15:16:33.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_seq/get_subsets.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1231 2023-04-13 07:58:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/get_hash.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/data_structure/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/data_structure/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-03-24 07:07:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/data_structure/executor.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/dangerous/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/dangerous/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2507 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/unified_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/converter/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      100 2022-07-25 12:20:46.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/converter/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      376 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/converter/integrate.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      237 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/read_json.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      297 2022-11-23 12:08:24.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/write_json.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/converter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13150 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/read.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6414 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      514 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/write.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/decorator/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/decorator/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/decorator/restore_original_work_path.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/singleton/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/singleton/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3631 2022-07-14 11:42:11.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/general_matrix_multiplication.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/numerical_characteristics/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/numerical_characteristics/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/numerical_characteristics/iou.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/my_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/my_iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/sequence_map_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/test.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/visualization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-03-08 12:20:02.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/visualization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1880 2022-03-10 05:11:03.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/visualization/multiple_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/check_validity_and_uninstall.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/check_version_and_update.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      131 2022-03-02 05:20:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/of_torch.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/test/test_version.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/compare_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/parse_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/sort_version_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__old_version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-03-24 10:06:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8297 2022-07-06 12:22:29.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_overlap.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/analysis/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/dummy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/convert/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/merge_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/split_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/dct_calculator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/scaling_and_shift/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-08-08 08:50:23.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/convert_dtype.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/get_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/set_crop_by_box.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/arrow3d.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_os/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       27 2023-04-10 12:15:40.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_os/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      618 2023-04-10 12:15:20.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_os/remove.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2518 2023-03-30 13:35:22.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_test/check_consistency.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/concat.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-03-08 08:37:14.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/tile.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/where.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/my_around.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2493 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12135 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/top_level.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-dev-1.0.4/pyproject.toml
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2023-04-13 08:01:59.000000 kevin-toolbox-dev-1.0.4/setup.cfg
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-dev-1.0.4/setup.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2821 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2259 2023-04-21 06:49:32.000000 kevin-toolbox-dev-1.0.5/README.md
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      410 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1920 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2084 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/pareto_front/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/search/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/search/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/search/binary_search.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       67 2022-09-19 12:30:55.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6422 2023-03-24 06:33:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-04-10 09:48:35.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_dict/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-04-10 09:22:49.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_dict/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      767 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_dict/deep_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_seq/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-04-10 09:27:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_seq/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-04-13 09:16:26.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_seq/flatten_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-04-09 15:16:33.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_seq/get_subsets.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-04-13 13:05:12.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/get_hash.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/data_structure/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/data_structure/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-03-24 07:07:59.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/data_structure/executor.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/dangerous/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/dangerous/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2507 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/unified_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/converter/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      100 2022-07-25 12:20:46.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/converter/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      376 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/converter/integrate.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      237 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/read_json.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      297 2022-11-23 12:08:24.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/write_json.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/converter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13150 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/read.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6414 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      514 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/write.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/decorator/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/decorator/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/decorator/restore_original_work_path.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/singleton/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/singleton/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3631 2022-07-14 11:42:11.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/general_matrix_multiplication.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/numerical_characteristics/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/numerical_characteristics/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/numerical_characteristics/iou.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/my_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/my_iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/sequence_map_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/test.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/visualization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-03-08 12:20:02.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/visualization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1880 2022-03-10 05:11:03.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/visualization/multiple_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/check_validity_and_uninstall.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/check_version_and_update.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      131 2022-03-02 05:20:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/of_torch.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/test/test_version.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/compare_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/parse_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/sort_version_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__old_version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-03-24 10:06:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8297 2022-07-06 12:22:29.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_overlap.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/analysis/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/dummy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/convert/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/merge_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/split_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/dct_calculator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/scaling_and_shift/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-08-08 08:50:23.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/convert_dtype.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/get_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/set_crop_by_box.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/arrow3d.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_os/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       27 2023-04-10 12:15:40.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_os/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_os/remove.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2518 2023-03-30 13:35:22.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_test/check_consistency.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/concat.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-03-08 08:37:14.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/tile.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/where.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/my_around.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2821 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12135 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/top_level.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-dev-1.0.5/pyproject.toml
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2023-04-21 06:51:15.000000 kevin-toolbox-dev-1.0.5/setup.cfg
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-dev-1.0.5/setup.py
```

### Comparing `kevin-toolbox-dev-1.0.4/PKG-INFO` & `kevin-toolbox-dev-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox-dev
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -75,7 +75,12 @@
     - This bug will result in the inability to correctly switch compatibility implementations based on the current version
     - There is an error in the implementation of low version in compatible.where
 
 - v 1.0.4（2023-04-13）
   - 更改了 env_info.version.parse_to_array 对于不合规版本字符串的解释方式，可能对 version.compare 的结果早晨用影响
   - modify get_hash() in computer_science.algorithm.utils
 
+- v 1.0.5（2023-04-21）【bug fix】
+  - 修复了 computer_science.algorithm.utils.for_seq 中的 flatten_list() 在 depth=None 时候报错的bug
+  - 修复了 computer_science.algorithm.utils 中的 get_hash()
+  - 修复了 patches 中的 for_os.remove() 无法移除非空文件夹的问题，并添加了测试用例。
+
```

### Comparing `kevin-toolbox-dev-1.0.4/README.md` & `kevin-toolbox-dev-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -57,7 +57,12 @@
     - This bug will result in the inability to correctly switch compatibility implementations based on the current version
     - There is an error in the implementation of low version in compatible.where
 
 - v 1.0.4（2023-04-13）
   - 更改了 env_info.version.parse_to_array 对于不合规版本字符串的解释方式，可能对 version.compare 的结果早晨用影响
   - modify get_hash() in computer_science.algorithm.utils
 
+- v 1.0.5（2023-04-21）【bug fix】
+  - 修复了 computer_science.algorithm.utils.for_seq 中的 flatten_list() 在 depth=None 时候报错的bug
+  - 修复了 computer_science.algorithm.utils 中的 get_hash()
+  - 修复了 patches 中的 for_os.remove() 无法移除非空文件夹的问题，并添加了测试用例。
+
```

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/search/binary_search.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/search/binary_search.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_dict/deep_update.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_dict/deep_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/algorithm/utils/for_seq/flatten_list.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/algorithm/utils/for_seq/flatten_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 def _recursion(ls, depth):
     if depth is not None and depth <= 0:
         res = ls
     else:
         res = []
         for i in ls:
             if isinstance(i, (list, tuple,)):
-                res.extend(_recursion(i, depth=depth - 1))
+                res.extend(_recursion(i, depth=depth if depth is None else depth - 1))
             else:
                 res.append(i)
     return res
 
 
 if __name__ == '__main__':
     a = [[1, 2, (3, 4)], [(5,)], 6]
-    print(flatten_list(ls=a, depth=5))
+    print(flatten_list(ls=a, depth=None))
```

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/computer_science/data_structure/executor.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/computer_science/data_structure/executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/unified_reader.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/unified_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/core/reader/unified_reader_base.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/core/reader/unified_reader_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/converter.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/converter.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/data_flow/file/kevin_notation/write.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/data_flow/file/kevin_notation/write.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/producer_consumer/node.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/producer_consumer/node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/general_matrix_multiplication.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/general_matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/numerical_characteristics/iou.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/numerical_characteristics/iou.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/__init__.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/my_iterator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/my_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/temperate/my_iterator_base.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/temperate/my_iterator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/developing/visualization/multiple_axis.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/developing/visualization/multiple_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/check_validity_and_uninstall.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/check_validity_and_uninstall.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/check_version_and_update.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/check_version_and_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/test/test_version.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/test/test_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/compare_version.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/compare_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/parse_version.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/parse_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/env_info/version/sort_version_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/env_info/version/sort_version_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__init__.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/geometry/for_boxes/detect_overlap.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/geometry/for_boxes/detect_overlap.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/factory.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/factory.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/merge_blocks.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/split_blocks.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/split_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/get_primes.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_get_primes.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/number_theory/test/test_prime_factorization.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/number_theory/test/test_prime_factorization.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/dct_calculator.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/dct_calculator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/transform/scaling_and_shift/scaling.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/transform/scaling_and_shift/scaling.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/convert_dtype.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/convert_dtype.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/get_crop_by_box.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/get_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/math/utils/set_crop_by_box.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/math/utils/set_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_matplotlib/arrow3d.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_matplotlib/arrow3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_test/check_consistency.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_test/check_consistency.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/tile.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/tile.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/compatible/where.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/compatible/where.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/get_y_at_x.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/get_y_at_x.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox/patches/for_torch/math/my_around.py` & `kevin-toolbox-dev-1.0.5/kevin_toolbox/patches/for_torch/math/my_around.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/PKG-INFO` & `kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox-dev
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -75,7 +75,12 @@
     - This bug will result in the inability to correctly switch compatibility implementations based on the current version
     - There is an error in the implementation of low version in compatible.where
 
 - v 1.0.4（2023-04-13）
   - 更改了 env_info.version.parse_to_array 对于不合规版本字符串的解释方式，可能对 version.compare 的结果早晨用影响
   - modify get_hash() in computer_science.algorithm.utils
 
+- v 1.0.5（2023-04-21）【bug fix】
+  - 修复了 computer_science.algorithm.utils.for_seq 中的 flatten_list() 在 depth=None 时候报错的bug
+  - 修复了 computer_science.algorithm.utils 中的 get_hash()
+  - 修复了 patches 中的 for_os.remove() 无法移除非空文件夹的问题，并添加了测试用例。
+
```

### Comparing `kevin-toolbox-dev-1.0.4/kevin_toolbox_dev.egg-info/SOURCES.txt` & `kevin-toolbox-dev-1.0.5/kevin_toolbox_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/setup.cfg` & `kevin-toolbox-dev-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.0.4/setup.py` & `kevin-toolbox-dev-1.0.5/setup.py`

 * *Files identical despite different names*

