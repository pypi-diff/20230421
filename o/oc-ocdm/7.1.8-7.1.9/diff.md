# Comparing `tmp/oc_ocdm-7.1.8.tar.gz` & `tmp/oc_ocdm-7.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ocdm-7.1.8.tar", max compression
+gzip compressed data, was "oc_ocdm-7.1.9.tar", max compression
```

## Comparing `oc_ocdm-7.1.8.tar` & `oc_ocdm-7.1.9.tar`

### file list

```diff
@@ -1,88 +1,94 @@
--rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.1.8/LICENSE.md
--rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.1.8/oc_ocdm/__init__.py
--rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.1.8/oc_ocdm/abstract_entity.py
--rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/abstract_set.py
--rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.1.8/oc_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/decorators.py
--rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/__init__.py
--rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/__init__.py
--rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/agent_role.py
--rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
--rw-r--r--   0        0        0    48177 2023-01-30 10:39:34.563112 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
--rw-r--r--   0        0        0    16277 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/citation.py
--rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/discourse_element.py
--rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/pointer_list.py
--rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
--rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
--rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
--rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
--rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic_entity.py
--rw-r--r--   0        0        0    18025 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/graph/entities/identifier.py
--rw-r--r--   0        0        0    15453 2023-01-30 10:39:34.563112 oc_ocdm-7.1.8/oc_ocdm/graph/graph_entity.py
--rw-r--r--   0        0        0    19992 2023-01-31 16:12:50.015484 oc_ocdm-7.1.8/oc_ocdm/graph/graph_set.py
--rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/__init__.py
--rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/entities/__init__.py
--rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/entities/dataset.py
--rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/entities/distribution.py
--rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/metadata_entity.py
--rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/metadata/metadata_set.py
--rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/prov/__init__.py
--rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.1.8/oc_ocdm/prov/entities/__init__.py
--rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.1.8/oc_ocdm/prov/entities/snapshot_entity.py
--rw-r--r--   0        0        0     3759 2023-01-31 16:12:50.016485 oc_ocdm-7.1.8/oc_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0    14189 2023-02-12 15:32:09.388098 oc_ocdm-7.1.8/oc_ocdm/prov/prov_set.py
--rw-r--r--   0        0        0    14478 2023-01-31 16:12:50.021422 oc_ocdm-7.1.8/oc_ocdm/reader.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/resources/__init__.py
--rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/resources/querymap.txt
--rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/resources/shexc.txt
--rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/resources/shexc_closed.txt
--rw-r--r--   0        0        0    16225 2023-01-31 16:12:50.022417 oc_ocdm-7.1.8/oc_ocdm/storer.py
--rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/support/__init__.py
--rw-r--r--   0        0        0     3543 2023-01-31 16:12:50.024415 oc_ocdm-7.1.8/oc_ocdm/support/query_utils.py
--rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/support/reporter.py
--rw-r--r--   0        0        0    15017 2023-01-31 16:12:50.025415 oc_ocdm-7.1.8/oc_ocdm/support/support.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/__init__.py
--rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
--rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
--rw-r--r--   0        0        0    69632 2023-01-31 16:12:50.027416 oc_ocdm-7.1.8/oc_ocdm/test/coverage/.coverage
--rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/coverage/.coveragerc
--rw-r--r--   0        0        0      925 2023-01-31 16:12:50.028416 oc_ocdm-7.1.8/oc_ocdm/test/coverage/coverage.svg
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
--rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
--rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
--rw-r--r--   0        0        0     6506 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
--rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
--rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
--rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
--rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
--rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
--rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
--rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
--rw-r--r--   0        0        0     7501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/test_identifier.py
--rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/graph/test_graph_entity.py
--rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.1.8/oc_ocdm/test/graph/test_graph_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/metadata/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/__init__.py
--rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/test_dataset.py
--rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/test_distribution.py
--rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/metadata/test_metadata_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/prov/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/prov/entities/__init__.py
--rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/prov/entities/test_snapshot_entity.py
--rw-r--r--   0        0        0    11157 2023-01-31 16:12:47.428933 oc_ocdm-7.1.8/oc_ocdm/test/prov/test_prov_set.py
--rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/storer/__init__.py
--rw-r--r--   0        0        0    11462 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/storer/test_storer.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.8/oc_ocdm/test/support/__init__.py
--rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.1.8/oc_ocdm/test/support/test_support.py
--rw-r--r--   0        0        0     1574 2023-02-12 15:32:44.812394 oc_ocdm-7.1.8/pyproject.toml
--rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.1.8/README.md
--rw-r--r--   0        0        0     5874 1970-01-01 00:00:00.000000 oc_ocdm-7.1.8/setup.py
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 oc_ocdm-7.1.8/PKG-INFO
+-rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.1.9/LICENSE.md
+-rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.1.9/oc_ocdm/__init__.py
+-rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.1.9/oc_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/abstract_set.py
+-rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.1.9/oc_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/decorators.py
+-rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/__init__.py
+-rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/agent_role.py
+-rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
+-rw-r--r--   0        0        0    48177 2023-01-30 10:39:34.563112 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
+-rw-r--r--   0        0        0    16277 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/citation.py
+-rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/discourse_element.py
+-rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/pointer_list.py
+-rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
+-rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
+-rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
+-rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
+-rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic_entity.py
+-rw-r--r--   0        0        0    18025 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/identifier.py
+-rw-r--r--   0        0        0    15453 2023-01-30 10:39:34.563112 oc_ocdm-7.1.9/oc_ocdm/graph/graph_entity.py
+-rw-r--r--   0        0        0    19992 2023-01-31 16:12:50.015484 oc_ocdm-7.1.9/oc_ocdm/graph/graph_set.py
+-rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/__init__.py
+-rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/__init__.py
+-rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/dataset.py
+-rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/distribution.py
+-rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_entity.py
+-rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_set.py
+-rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/prov/entities/__init__.py
+-rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.1.9/oc_ocdm/prov/entities/snapshot_entity.py
+-rw-r--r--   0        0        0     3759 2023-01-31 16:12:50.016485 oc_ocdm-7.1.9/oc_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0    14189 2023-02-12 15:32:09.388098 oc_ocdm-7.1.9/oc_ocdm/prov/prov_set.py
+-rw-r--r--   0        0        0    11957 2023-03-03 13:42:56.995864 oc_ocdm-7.1.9/oc_ocdm/reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/__init__.py
+-rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/querymap.txt
+-rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-7.1.9/oc_ocdm/resources/shacle.ttl
+-rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/shexc.txt
+-rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/shexc_closed.txt
+-rw-r--r--   0        0        0    16225 2023-01-31 16:12:50.022417 oc_ocdm-7.1.9/oc_ocdm/storer.py
+-rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/support/__init__.py
+-rw-r--r--   0        0        0     3543 2023-01-31 16:12:50.024415 oc_ocdm-7.1.9/oc_ocdm/support/query_utils.py
+-rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/support/reporter.py
+-rw-r--r--   0        0        0    15017 2023-01-31 16:12:50.025415 oc_ocdm-7.1.9/oc_ocdm/support/support.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/__init__.py
+-rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
+-rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
+-rw-r--r--   0        0        0    69632 2023-03-03 14:12:10.094268 oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coverage
+-rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coveragerc
+-rw-r--r--   0        0        0      925 2023-03-03 14:12:10.096270 oc_ocdm-7.1.9/oc_ocdm/test/coverage/coverage.svg
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
+-rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
+-rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
+-rw-r--r--   0        0        0     6506 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
+-rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
+-rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
+-rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
+-rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
+-rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
+-rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
+-rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
+-rw-r--r--   0        0        0     7501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_identifier.py
+-rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_entity.py
+-rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/__init__.py
+-rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_dataset.py
+-rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_distribution.py
+-rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/metadata/test_metadata_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/__init__.py
+-rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/test_snapshot_entity.py
+-rw-r--r--   0        0        0    11157 2023-01-31 16:12:47.428933 oc_ocdm-7.1.9/oc_ocdm/test/prov/test_prov_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/resources/__init__.py
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.1.9/oc_ocdm/test/resources/data.json
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader.json
+-rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader_invalid.json
+-rw-r--r--   0        0        0     2531 2023-03-03 13:43:32.199458 oc_ocdm-7.1.9/oc_ocdm/test/resources/test_shacle.py
+-rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/storer/__init__.py
+-rw-r--r--   0        0        0    11462 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/storer/test_storer.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/support/__init__.py
+-rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.1.9/oc_ocdm/test/support/test_support.py
+-rw-r--r--   0        0        0     1576 2023-03-03 14:12:50.570092 oc_ocdm-7.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.1.9/README.md
+-rw-r--r--   0        0        0     5904 1970-01-01 00:00:00.000000 oc_ocdm-7.1.9/setup.py
+-rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 oc_ocdm-7.1.9/PKG-INFO
```

### Comparing `oc_ocdm-7.1.8/LICENSE.md` & `oc_ocdm-7.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/abstract_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/abstract_set.py` & `oc_ocdm-7.1.9/oc_ocdm/abstract_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/counter_handler/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/counter_handler/counter_handler.py` & `oc_ocdm-7.1.9/oc_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/counter_handler/filesystem_counter_handler.py` & `oc_ocdm-7.1.9/oc_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/counter_handler/in_memory_counter_handler.py` & `oc_ocdm-7.1.9/oc_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/decorators.py` & `oc_ocdm-7.1.9/oc_ocdm/decorators.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/agent_role.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/citation.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/discourse_element.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/pointer_list.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/reference_annotation.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/reference_pointer.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic/responsible_agent.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/bibliographic_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/entities/identifier.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/entities/identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/graph_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/graph/graph_set.py` & `oc_ocdm-7.1.9/oc_ocdm/graph/graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/entities/dataset.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/entities/distribution.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/metadata_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/metadata/metadata_set.py` & `oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/prov/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/prov/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/prov/entities/snapshot_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/prov/entities/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/prov/prov_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/prov/prov_set.py` & `oc_ocdm-7.1.9/oc_ocdm/prov/prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/reader.py` & `oc_ocdm-7.1.9/oc_ocdm/reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 from __future__ import annotations
 
 import json
 import os
-from importlib import resources
 from typing import TYPE_CHECKING
 from zipfile import ZipFile
 
 import rdflib
 from filelock import FileLock
-from pyshex import ShExEvaluator
-from rdflib import RDF, ConjunctiveGraph, Graph, Namespace
+from rdflib import RDF, ConjunctiveGraph, Graph, Namespace, URIRef
 from SPARQLWrapper import RDFXML, SPARQLWrapper
 
 from oc_ocdm.graph.graph_entity import GraphEntity
 from oc_ocdm.support.reporter import Reporter
 
 if TYPE_CHECKING:
     from typing import Any, Dict, List, Optional, Set
 
-    from rdflib import URIRef, term
+    from rdflib import term
 
     from oc_ocdm.graph.graph_set import GraphSet
 
+from pyshacl import validate
+
 
 class Reader(object):
 
     def __init__(self, repok: Reporter = None, reperr: Reporter = None, context_map: Dict[str, Any] = None) -> None:
 
         if context_map is not None:
             self.context_map: Dict[str, Any] = context_map
@@ -130,101 +130,53 @@
         for p, o in graph.predicate_objects(subject):
             if isinstance(o, rdflib.term.Literal):
                 o = rdflib.term.Literal(lexical_or_value=str(o), datatype=None)
             g.add((subject, p, o))
         return g
 
     @staticmethod
-    def _validate(graph: Graph, shex: str, valid_graph: Graph, focus: URIRef, shape: URIRef) -> bool:
-        node_result = ShExEvaluator().evaluate(rdf=graph, shex=shex, focus=focus, start=shape)[0]
-        if node_result.result:
-            for triple in graph.triples((focus, None, None)):
-                valid_graph.add(triple)
-        return node_result.result
-
-    @staticmethod
     def _extract_subjects(graph: Graph) -> Set[URIRef]:
         subjects: Set[URIRef] = set()
         for s in graph.subjects():
             subjects.add(s)
         return subjects
 
-    @staticmethod
-    def graph_validation(graph: Graph, closed: bool = False) -> Graph:
+    def graph_validation(self, graph: Graph, closed: bool = False) -> Graph:
         valid_graph: Graph = Graph(identifier=graph.identifier)
-
+        sg = Graph()
         if closed:
-            shex = resources.read_text('oc_ocdm.resources', 'shexc_closed.txt')
+            sg.parse(os.path.join('oc_ocdm', 'resources', 'shacle_closed.ttl'))
         else:
-            shex = resources.read_text('oc_ocdm.resources', 'shexc.txt')
-
-        BIRO: Namespace = Namespace("http://purl.org/spar/biro/")
-        C4O: Namespace = Namespace("http://purl.org/spar/c4o/")
-        CITO: Namespace = Namespace("http://purl.org/spar/cito/")
-        DATACITE: Namespace = Namespace("http://purl.org/spar/datacite/")
-        DEO: Namespace = Namespace("http://purl.org/spar/deo/")
-        FABIO: Namespace = Namespace("http://purl.org/spar/fabio/")
-        FOAF: Namespace = Namespace("http://xmlns.com/foaf/0.1/")
-        OA: Namespace = Namespace("http://www.w3.org/ns/oa#")
-        PRO: Namespace = Namespace("http://purl.org/spar/pro/")
-
-        OC: Namespace = Namespace("https://opencitations.net/shex/")
-
-        for subject in Reader._extract_subjects(graph):
-            # ReferenceAnnotation
-            if (subject, RDF.type, OA.Annotation) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.ReferenceAnnotationShape)
-
-            # AgentRole
-            elif (subject, RDF.type, PRO.RoleInTime) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.AgentRoleShape)
-
-            # BibliographicReference
-            elif (subject, RDF.type, BIRO.BibliographicReference) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.BibliographicReferenceShape)
-
-            # BibliographicResource
-            elif (subject, RDF.type, FABIO.Expression) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.BibliographicResourceShape)
-
-            # Citation
-            elif (subject, RDF.type, CITO.Citation) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.CitationShape)
-
-            # DiscourseElement
-            elif (subject, RDF.type, DEO.DiscourseElement) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.DiscourseElementShape)
-
-            # Identifier
-            elif (subject, RDF.type, DATACITE.Identifier) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.IdentifierShape)
-
-            # PointerList
-            elif (subject, RDF.type, C4O.SingleLocationPointerList) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.PointerListShape)
-
-            # ResponsibleAgent
-            elif (subject, RDF.type, FOAF.Agent) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.ResponsibleAgentShape)
-
-            # ResourceEmbodiment
-            elif (subject, RDF.type, FABIO.Manifestation) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.ResourceEmbodimentShape)
-
-            # ReferencePointer
-            elif (subject, RDF.type, C4O.InTextReferencePointer) in graph:
-                Reader._validate(graph, shex, valid_graph, subject, OC.ReferencePointerShape)
-
+            sg.parse(os.path.join('oc_ocdm', 'resources', 'shacle.ttl'))
+        _, report_g, _ = validate(graph,
+            shacl_graph=sg,
+            ont_graph=None,
+            inference=None,
+            abort_on_first=False,
+            allow_infos=False,
+            allow_warnings=False,
+            meta_shacl=False,
+            advanced=False,
+            js=False,
+            debug=False)
+        invalid_nodes = set()
+        for triple in report_g.triples((None, URIRef('http://www.w3.org/ns/shacl#focusNode'), None)):
+            invalid_nodes.add(triple[2])
+        for subject in self._extract_subjects(graph):
+            if subject not in invalid_nodes:
+                for valid_subject_triple in graph.triples((subject, None, None)):
+                    valid_graph.add(valid_subject_triple)
         return valid_graph
 
     @staticmethod
     def import_entities_from_graph(g_set: GraphSet, graph: Graph, resp_agent: str,
                                    enable_validation: bool = False, closed: bool = False) -> List[GraphEntity]:
         if enable_validation:
-            graph = Reader.graph_validation(graph, closed)
+            reader = Reader()
+            graph = reader.graph_validation(graph, closed)
         imported_entities: List[GraphEntity] = []
         for subject in Reader._extract_subjects(graph):
             types: List[term] = []
             for o in graph.objects(subject, RDF.type):
                 types.append(o)
             # ReferenceAnnotation
             if GraphEntity.iri_note in types:
```

### Comparing `oc_ocdm-7.1.8/oc_ocdm/resources/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/resources/querymap.txt` & `oc_ocdm-7.1.9/oc_ocdm/resources/querymap.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/resources/shexc.txt` & `oc_ocdm-7.1.9/oc_ocdm/resources/shexc.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/resources/shexc_closed.txt` & `oc_ocdm-7.1.9/oc_ocdm/resources/shexc_closed.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/storer.py` & `oc_ocdm-7.1.9/oc_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/support/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/support/query_utils.py` & `oc_ocdm-7.1.9/oc_ocdm/support/query_utils.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/support/reporter.py` & `oc_ocdm-7.1.9/oc_ocdm/support/reporter.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/support/support.py` & `oc_ocdm-7.1.9/oc_ocdm/support/support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py` & `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py` & `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/coverage/.coverage` & `oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coverage`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -14,15 +14,15 @@
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
 INSERT INTO meta VALUES('sys_argv','[''python -m unittest'', ''discover'', ''-s'', ''oc_ocdm/test'', ''-p'', ''test_*.py'']');
 INSERT INTO meta VALUES('version','6.5.0');
-INSERT INTO meta VALUES('when','2023-01-29 14:35:28');
+INSERT INTO meta VALUES('when','2023-02-12 15:35:45');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
@@ -117,55 +117,55 @@
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'0000cb77affbfdbbffffefdffbfbfbbffd7dfdfdaff704');
 INSERT INTO line_bits VALUES(3,1,X'00000d');
-INSERT INTO line_bits VALUES(4,1,X'00007df717a040f11b036304207eff006ff7aebfedebfe13822f1100c00d2000000000808020');
+INSERT INTO line_bits VALUES(4,1,X'00007df71720c2f11b036304207eff006ff7aebfedebfe13822f2100c0052000000000808040');
 INSERT INTO line_bits VALUES(5,1,X'000006');
-INSERT INTO line_bits VALUES(6,1,X'000055c1fffffefffffffffffffffffffffffffffffb7ff26f8c16007377975300e07033743e');
-INSERT INTO line_bits VALUES(7,1,X'00006d61282e00090a000101408205c002340b00fe029fbbcf06');
+INSERT INTO line_bits VALUES(6,1,X'000055c1fffffefffffffffffffffffffffffffffff37ff86f8c16005355955300e07033743e');
+INSERT INTO line_bits VALUES(7,1,X'00006d212a2e00090a000101408205c002340b00fe029fbbcf06');
 INSERT INTO line_bits VALUES(8,1,X'000062');
-INSERT INTO line_bits VALUES(9,1,X'0000bd400900a8f195feafc11bf7defdffa45ce6cc989780978793879380970020a0200d6afc722f0300000040e7');
+INSERT INTO line_bits VALUES(9,1,X'0000bd400900a8f195feafc11bf7defdffa45ce6cc989780978793879380970040a0202f7afd622f0300000040e7');
 INSERT INTO line_bits VALUES(10,1,X'000015fbfdfc121001');
 INSERT INTO line_bits VALUES(11,1,X'000015cc03e73c9cee6b');
-INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffd4c3ffad53bdfa55af7ad5ab5efdaa57bdfa55ef16a0f4ef2b00e0f9ffff7f017f010101010101017f01');
-INSERT INTO line_bits VALUES(13,1,X'0000ad301405be011880');
-INSERT INTO line_bits VALUES(14,1,X'00007ddf020a0000040040000000008001038301000000000000001800000000000018');
+INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5e4ffd8c3ffad633dfb59cf7ad6b39efdac673dfb59ef16a0f4ef2b00e0f9ffff7f017f010101010101017f01');
+INSERT INTO line_bits VALUES(13,1,X'0000ad101505be000880');
+INSERT INTO line_bits VALUES(14,1,X'00007ddf020a0000040040000000008000018101000000000000002800000000000028');
 INSERT INTO line_bits VALUES(15,1,X'00000e');
-INSERT INTO line_bits VALUES(16,1,X'0000d9010060000006006000c00060');
-INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20f91700000001005300c0b6eddef57f74edfdbbd5fbfb4fa5bb3fd99be705000010800d01d806');
-INSERT INTO line_bits VALUES(18,1,X'0000954cfc0500c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
+INSERT INTO line_bits VALUES(16,1,X'000059010060000006006000c00060');
+INSERT INTO line_bits VALUES(17,1,X'0000bd4c2d20f92700000001005300c0b6eddef57f74edfdbbd5fbeb4fa5bb3f599bef05000010800d01d806');
+INSERT INTO line_bits VALUES(18,1,X'00009554fc0900c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
 INSERT INTO line_bits VALUES(19,1,X'000006');
-INSERT INTO line_bits VALUES(20,1,X'0000556401d020c137003400a40020e1df0d');
+INSERT INTO line_bits VALUES(20,1,X'0000556401d020c117003400a40020e1df0d');
 INSERT INTO line_bits VALUES(21,1,X'0000ad1200d03f0c');
-INSERT INTO line_bits VALUES(22,1,X'00002dce1800809ea060030006000d00d000a001400300b801001a008006000d001a0034006800d000a001400380bec0');
+INSERT INTO line_bits VALUES(22,1,X'00002d4e0a00809ea0600100020005005000a000400100b800000a0080020005000a00140028005000a000400180bec0');
 INSERT INTO line_bits VALUES(23,1,X'0000fe07');
-INSERT INTO line_bits VALUES(24,1,X'000055cc0600000000821b002c487003c082040bc002b0002c08');
-INSERT INTO line_bits VALUES(25,1,X'00005598c1000000000206008005098001d000000430002c08');
-INSERT INTO line_bits VALUES(26,1,X'0000b5c0cc00007433333333332368005890a00160418219002c48700d800600206800f08204d7006800008206002c48d0006041826b00340000c135001a0080e01ba001200936003400800080005000200014000a000580024001a00050002800100008000580024001a0004000280014000a00050002000180004000200010000a000500024001a0005000280010000a000580024001800010');
-INSERT INTO line_bits VALUES(27,1,X'0000d562061800000000400003c0820430002c48c000002f48c000c08204180016240005a00014800250000a400108');
-INSERT INTO line_bits VALUES(28,1,X'00005598610000000000000103c08204c00068000002180016240006400300100003a0010008180016246000106000001000140014001400140014001400140004');
-INSERT INTO line_bits VALUES(29,1,X'000055cc18000000040cc08204c00068');
-INSERT INTO line_bits VALUES(30,1,X'000055cc800100000430005810');
-INSERT INTO line_bits VALUES(31,1,X'00005598610000000010300058900006000b12c000604102600068');
-INSERT INTO line_bits VALUES(32,1,X'00002dce0c00000000020c000b123000c02948c00000a7200106800509000580');
-INSERT INTO line_bits VALUES(33,1,X'000055660c000000000206000b1230002c48c000b02001064003');
+INSERT INTO line_bits VALUES(24,1,X'000055cc0200000000820b002c487001c082040bc002b0002c08');
+INSERT INTO line_bits VALUES(25,1,X'0000559850000000000202008005098000d000000410002c08');
+INSERT INTO line_bits VALUES(26,1,X'0000b5c05400007433333333332328005890a00060418209002c487005800600202800f0820457006800008202002c4850006041822b00340000c115001a0080e00ba001200916003400800080005000200014000a000580024001a00050002800100008000580024001a0004000280014000a00050002000180004000200010000a000500024001a0005000280010000a000580024001800010');
+INSERT INTO line_bits VALUES(27,1,X'0000d562020a00000000400001c0820410002c484000002f484000c08204080016240005a00014800250000a400108');
+INSERT INTO line_bits VALUES(28,1,X'00005598280000000000000101c08204400068000002080016240002400300100001a0010008080016242000106000001000140014001400140014001400140004');
+INSERT INTO line_bits VALUES(29,1,X'0000554c0a0000000404c08204400068');
+INSERT INTO line_bits VALUES(30,1,X'0000554ca00000000410005810');
+INSERT INTO line_bits VALUES(31,1,X'00005598280000000010100058900002000b124000604102200068');
+INSERT INTO line_bits VALUES(32,1,X'00002d4e05000000000204000b121000c02948400000a7200102800509000580');
+INSERT INTO line_bits VALUES(33,1,X'0000552605000000000202000b1210002c484000b02001024003');
 INSERT INTO line_bits VALUES(34,1,X'000006');
-INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bf1bff1d102605e3313400000000010');
-INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935aec2ab5e5b004bc11710');
+INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff33f8bff1d102605a1111400000000010');
+INSERT INTO line_bits VALUES(36,1,X'0000f54b93d935cec2b39e5b004b411710');
 INSERT INTO line_bits VALUES(37,1,X'000006');
-INSERT INTO line_bits VALUES(38,1,X'000075c10c000000000000000206800509180016246000b02001038005091880060020c0003400000103c08204c0003400000106800509800168');
-INSERT INTO line_bits VALUES(39,1,X'0000d5c20c00000000002060005890800160410206000b123000589080016041020680050918001604');
+INSERT INTO line_bits VALUES(38,1,X'0000754105000000000000000202800509080016242000b0200101800509088006002040003400000101c0820440003400000102800509800068');
+INSERT INTO line_bits VALUES(39,1,X'0000d5420500000000002020005890800060410202000b121000589080006041020280050908001604');
 INSERT INTO line_bits VALUES(40,1,X'000006');
-INSERT INTO line_bits VALUES(41,1,X'0000d58241ff4dec633473');
-INSERT INTO line_bits VALUES(42,1,X'0000dd45eb68daafdbefbbbf7f7619b66bdf7ea6cbd67e7b0f00dd011c00ddcfae');
+INSERT INTO line_bits VALUES(41,1,X'0000d58250ff09ee633453');
+INSERT INTO line_bits VALUES(42,1,X'0000dd45eb48dcafdbefbbbf7e7619b66bdffe4c97adfdf61e00bc033800aa9f5d01');
 INSERT INTO line_bits VALUES(43,1,X'000002');
-INSERT INTO line_bits VALUES(44,1,X'0000d50583a0018005091a00b020c102c08204b701d000000418002c48d00060418206002c48b001b020');
+INSERT INTO line_bits VALUES(44,1,X'0000d50591a0008005090a00b020c102c08204b700d000000408002c48500060418202002c48b000b020');
 INSERT INTO line_bits VALUES(45,1,X'0000a5bdbffffdefbff7fbefbfbff7f7bffffdfbfefe7dbfdff7f727');
 INSERT INTO line_bits VALUES(46,1,X'02');
 INSERT INTO line_bits VALUES(47,1,X'02');
 INSERT INTO line_bits VALUES(48,1,X'02');
 INSERT INTO line_bits VALUES(49,1,X'0000cdeebbdd6eb79b');
 INSERT INTO line_bits VALUES(50,1,X'000035bbf776bb09');
 INSERT INTO line_bits VALUES(51,1,X'000035bbbfb7b7dbedf7efdfdddede6eb7dbdbed76bbdd6eb7dbed76bbdd6eb7dbed76bbdd6eb7dbed76bb09');
@@ -188,15 +188,15 @@
 INSERT INTO line_bits VALUES(68,1,X'02');
 INSERT INTO line_bits VALUES(69,1,X'02');
 INSERT INTO line_bits VALUES(70,1,X'000075f6de77dfbddddededede04');
 INSERT INTO line_bits VALUES(71,1,X'0000757677f7f6db8ff6df3ddbffaddfde7e7bfb68ffd66f7febb7fbde3601');
 INSERT INTO line_bits VALUES(72,1,X'02');
 INSERT INTO line_bits VALUES(73,1,X'0000bfcedffeffffffffffffff0fffff3ffc27');
 INSERT INTO line_bits VALUES(74,1,X'02');
-INSERT INTO line_bits VALUES(75,1,X'0000ebb8ab9e76b3f6f576b75afdef7f02');
+INSERT INTO line_bits VALUES(75,1,X'0000ebb8ab9e76b3f2f576b75afdef7f02');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/coverage/coverage.svg` & `oc_ocdm-7.1.9/oc_ocdm/test/coverage/coverage.svg`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 000002e0: 6765 3c2f 7465 7874 3e0d 0a20 2020 2020  ge</text>..     
 000002f0: 2020 203c 7465 7874 2078 3d22 3331 2e35     <text x="31.5
 00000300: 2220 793d 2231 3422 3e63 6f76 6572 6167  " y="14">coverag
 00000310: 653c 2f74 6578 743e 0d0a 2020 2020 2020  e</text>..      
 00000320: 2020 3c74 6578 7420 783d 2238 3022 2079    <text x="80" y
 00000330: 3d22 3135 2220 6669 6c6c 3d22 2330 3130  ="15" fill="#010
 00000340: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
-00000350: 793d 222e 3322 3e38 3025 3c2f 7465 7874  y=".3">80%</text
+00000350: 793d 222e 3322 3e37 3925 3c2f 7465 7874  y=".3">79%</text
 00000360: 3e0d 0a20 2020 2020 2020 203c 7465 7874  >..        <text
-00000370: 2078 3d22 3830 2220 793d 2231 3422 3e38   x="80" y="14">8
-00000380: 3025 3c2f 7465 7874 3e0d 0a20 2020 203c  0%</text>..    <
+00000370: 2078 3d22 3830 2220 793d 2231 3422 3e37   x="80" y="14">7
+00000380: 3925 3c2f 7465 7874 3e0d 0a20 2020 203c  9%</text>..    <
 00000390: 2f67 3e0d 0a3c 2f73 7667 3e0d 0a         /g>..</svg>..
```

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_citation.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/test_bibliographic_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/entities/test_identifier.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/test_graph_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/graph/test_graph_set.py` & `oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/metadata/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/test_dataset.py` & `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/metadata/entities/test_distribution.py` & `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/metadata/test_metadata_set.py` & `oc_ocdm-7.1.9/oc_ocdm/test/metadata/test_metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/prov/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/prov/entities/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/prov/entities/test_snapshot_entity.py` & `oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/test_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/prov/test_prov_set.py` & `oc_ocdm-7.1.9/oc_ocdm/test/prov/test_prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/storer/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/storer/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/storer/test_storer.py` & `oc_ocdm-7.1.9/oc_ocdm/test/storer/test_storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/support/__init__.py` & `oc_ocdm-7.1.9/oc_ocdm/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/oc_ocdm/test/support/test_support.py` & `oc_ocdm-7.1.9/oc_ocdm/test/support/test_support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/pyproject.toml` & `oc_ocdm-7.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc_ocdm"
-version = "7.1.8"
+version = "7.1.9"
 description = "Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel."
 authors = [
     "Silvio Peroni <essepuntato@gmail.com>",
     "Marilena Daquino <marilena.daquino2@unibo.it>",
     "Fabio Mariani <fabio.mariani6@studio.unibo.it>",
     "Simone Persiani <iosonopersia@gmail.com>",
     "Arcangelo Massari <arcangelo.massari@unibo.it>"
@@ -28,17 +28,17 @@
     "Topic :: System :: Archiving",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 rdflib = "^6.0.0"
-PyShEx = "^0.8.0"
 SPARQLWrapper = "^1.8.5"
 filelock = "^3.6.0"
+pyshacl = "^0.20.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.4.0"
 sphinx_rtd_theme = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
```

### Comparing `oc_ocdm-7.1.8/README.md` & `oc_ocdm-7.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.8/setup.py` & `oc_ocdm-7.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,33 @@
  'oc_ocdm.test.graph',
  'oc_ocdm.test.graph.entities',
  'oc_ocdm.test.graph.entities.bibliographic',
  'oc_ocdm.test.metadata',
  'oc_ocdm.test.metadata.entities',
  'oc_ocdm.test.prov',
  'oc_ocdm.test.prov.entities',
+ 'oc_ocdm.test.resources',
  'oc_ocdm.test.storer',
  'oc_ocdm.test.support']
 
 package_data = \
 {'': ['*'], 'oc_ocdm.test': ['coverage/*']}
 
 install_requires = \
-['PyShEx>=0.8.0,<0.9.0',
- 'SPARQLWrapper>=1.8.5,<2.0.0',
+['SPARQLWrapper>=1.8.5,<2.0.0',
  'filelock>=3.6.0,<4.0.0',
+ 'pyshacl>=0.20.0,<0.21.0',
  'rdflib>=6.0.0,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['test = scripts:test']}
 
 setup_kwargs = {
     'name': 'oc-ocdm',
-    'version': '7.1.8',
+    'version': '7.1.9',
     'description': 'Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.',
     'long_description': '# oc_ocdm\n[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/oc_ocdm/master/oc_ocdm/test/coverage/coverage.svg)\n[![Documentation Status](https://readthedocs.org/projects/oc-ocdm/badge/?version=latest)](https://oc-ocdm.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/oc-ocdm.svg)](https://badge.fury.io/py/oc-ocdm)\n![PyPI](https://img.shields.io/pypi/pyversions/oc_meta)\n\n[![DOI](https://zenodo.org/badge/322327342.svg)](https://zenodo.org/badge/latestdoi/322327342)\n[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)\n\nDocumentation can be found here: [https://oc-ocdm.readthedocs.io](https://oc-ocdm.readthedocs.io).\n\n**oc_ocdm** is a Python &ge;3.7 library that enables the user to import, produce, modify and export RDF data\nstructures which are compliant with the [OCDM v2.0.1](https://figshare.com/articles/Metadata_for_the_OpenCitations_Corpus/3443876) specification.\n\n## User\'s guide\nThis package can be simply installed with **pip**:\n``` bash\n    pip install oc_ocdm\n```\n**Please, have a look at the notebooks [available here](https://github.com/opencitations/oc_ocdm/blob/master/notebooks/).**\n\n## Developer\'s guide\n\n### First steps\n  1. Install Poetry:\n``` bash\n    pip install poetry\n```\n  2. Clone this repository:\n``` bash\n    git clone https://github.com/iosonopersia/oc_ocdm\n    cd ./oc_ocdm\n```\n  3. Install all the dependencies:\n``` bash\n    poetry install\n```\n  4. Build the package (_output dir:_ `dist`):\n``` bash\n    poetry build\n```\n  5. Globally install the package (_alternatively, you can also install it inside a virtual-env,\n  by providing the full path to the .tar.gz archive_):\n``` bash\n    pip install ./dist/oc_ocdm-<VERSION>.tar.gz\n```\n  6. If everything went the right way, than you should be able to use the `oc_ocdm` library in your Python modules as follows:\n``` python\n    from oc_ocdm.graph import GraphSet\n    from oc_ocdm.graph.entities.bibliographic import AgentRole\n    # ...\n```\n\n### How to run the tests\nJust run the following command inside the root project folder:\n``` bash\n    poetry run test\n```\n\n### How to manage the project using Poetry\nSee [Poetry commands documentation](https://python-poetry.org/docs/cli/).\n\n**AAA: when adding a non-dev dependency via `poetry add`, always remember to add\nthat same dependency to the `autodoc_mock_imports` list in `docs/source/conf.py`**\n(otherwise "Read the Docs" won\'t be able to compile the documentation correctly!).\n\n### How to publish the package onto Pypi\n``` bash\n    poetry publish --build\n```\n### Install dependencies needed for the documentation\n``` bash\n    pip install Sphinx sphinx_rtd_theme\n```\n### How to generate the documentation\n``` bash\n    rm ./docs/source/modules/*\n    sphinx-apidoc  -o ./docs/source/modules oc_ocdm *test*\n```\n\n### How to build the documentation\n___\n**Warning! In order to avoid getting the following `WARNING: html_static_path entry \'_static\' does not exist`, you\'ll\nneed to manually create an empty `_static` folder with the command:**\n``` bash\n    mkdir docs/source/_static\n```\n___\n  1. Always remember to move inside the `docs` folder:\n``` bash\n    cd docs\n```\n  2. Use the Makefile provided to build the docs:\n      + _on Windows_\n        ```\n            make.bat html\n        ```\n      + _on Linux and MacOs_\n        ```\n            make html\n        ```\n  3. Open the `build/html/index.html` file with a web browser of your choice!\n\n## Acknowledgements\nThis work has been funded by the project “Open Biomedical Citations in Context Corpus”\n(Wellcome Trust, Grant n. 214471/Z/18/Z) and the project “Wikipedia Citations in Wikidata”\n(Wikimedia Foundation, https://meta.wikimedia.org/wiki/Wikicite/grant/Wikipedia_Citations_in_Wikidata).\n\nWe would like to thank (in alphabetic order) Fabio Mariani (@FabioMariani), Arcangelo\nMassari (@arcangelo7), and Gabriele Pisciotta (@GabrielePisciotta) for the constructive feedback.\n',
     'author': 'Silvio Peroni',
     'author_email': 'essepuntato@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://opencitations.net',
```

### Comparing `oc_ocdm-7.1.8/PKG-INFO` & `oc_ocdm-7.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc-ocdm
-Version: 7.1.8
+Version: 7.1.9
 Summary: Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.
 Home-page: https://opencitations.net
 License: ISC
 Keywords: opencitations,openscience,datamodel,mapping
 Author: Silvio Peroni
 Author-email: essepuntato@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Typing :: Typed
-Requires-Dist: PyShEx (>=0.8.0,<0.9.0)
 Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
 Requires-Dist: filelock (>=3.6.0,<4.0.0)
+Requires-Dist: pyshacl (>=0.20.0,<0.21.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0.0)
 Project-URL: Documentation, https://oc-ocdm.readthedocs.io
 Project-URL: Repository, https://github.com/opencitations/oc_ocdm
 Description-Content-Type: text/markdown
 
 # oc_ocdm
 [<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
```

