# Comparing `tmp/kosh-2.2.tar.gz` & `tmp/kosh-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kosh-2.2.tar", last modified: Wed Aug 10 17:01:11 2022, max compression
+gzip compressed data, was "kosh-3.0.tar", last modified: Fri Apr 21 00:13:06 2023, max compression
```

## Comparing `kosh-2.2.tar` & `kosh-3.0.tar`

### file list

```diff
@@ -1,51 +1,93 @@
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.118066 kosh-2.2/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1099 2021-03-30 14:42:19.000000 kosh-2.2/LICENSE
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1164 2021-03-30 14:42:19.000000 kosh-2.2/NOTICE
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     3652 2022-08-10 17:01:11.117064 kosh-2.2/PKG-INFO
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1874 2022-03-15 14:33:31.000000 kosh-2.2/README.md
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.027067 kosh-2.2/kosh/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1159 2022-08-03 20:33:50.000000 kosh-2.2/kosh/__init__.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    16315 2022-08-03 20:33:50.000000 kosh-2.2/kosh/core_sina.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)       24 2022-08-10 16:18:32.000000 kosh-2.2/kosh/current_version.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    46584 2022-08-03 20:33:50.000000 kosh-2.2/kosh/dataset.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    11351 2022-03-15 14:33:31.000000 kosh-2.2/kosh/ensemble.py
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.052060 kosh-2.2/kosh/exec_graphs/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)       74 2021-03-24 14:27:11.000000 kosh-2.2/kosh/exec_graphs/__init__.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    19790 2022-03-15 14:33:31.000000 kosh-2.2/kosh/exec_graphs/core.py
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.082062 kosh-2.2/kosh/loaders/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     3090 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/UltraLoader.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)      377 2022-03-15 14:33:31.000000 kosh-2.2/kosh/loaders/__init__.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    15173 2022-08-03 20:33:50.000000 kosh-2.2/kosh/loaders/core.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     5706 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/hdf5.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1176 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/jsons.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     5099 2022-03-15 14:33:31.000000 kosh-2.2/kosh/loaders/npy.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     3108 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/pgm.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1991 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/pil.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     2520 2022-03-15 13:18:23.000000 kosh-2.2/kosh/loaders/sidre.py
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.088076 kosh-2.2/kosh/operators/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)      124 2022-03-15 14:33:31.000000 kosh-2.2/kosh/operators/__init__.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     5394 2022-03-15 14:33:31.000000 kosh-2.2/kosh/operators/core.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     4743 2022-03-15 13:18:23.000000 kosh-2.2/kosh/schema.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    72977 2022-08-03 20:33:50.000000 kosh-2.2/kosh/store.py
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.107080 kosh-2.2/kosh/transformers/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)      331 2022-03-15 14:33:31.000000 kosh-2.2/kosh/transformers/__init__.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     4725 2022-03-15 14:33:31.000000 kosh-2.2/kosh/transformers/core.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     8789 2022-03-15 13:18:23.000000 kosh-2.2/kosh/transformers/npy.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     4060 2022-03-15 13:18:23.000000 kosh-2.2/kosh/transformers/sidre.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    11617 2022-03-15 13:18:23.000000 kosh-2.2/kosh/transformers/skl.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1959 2022-03-15 13:18:23.000000 kosh-2.2/kosh/transformers/utils.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    20040 2022-08-03 20:33:50.000000 kosh-2.2/kosh/utils.py
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     6253 2022-08-03 20:33:50.000000 kosh-2.2/kosh/wrapper.py
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.044076 kosh-2.2/kosh.egg-info/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     3652 2022-08-10 17:01:10.000000 kosh-2.2/kosh.egg-info/PKG-INFO
--rw-------   0 cdoutrix (45773) cdoutrix (45773)      855 2022-08-10 17:01:10.000000 kosh-2.2/kosh.egg-info/SOURCES.txt
--rw-------   0 cdoutrix (45773) cdoutrix (45773)        1 2022-08-10 17:01:10.000000 kosh-2.2/kosh.egg-info/dependency_links.txt
--rw-------   0 cdoutrix (45773) cdoutrix (45773)        1 2022-08-10 16:13:22.000000 kosh-2.2/kosh.egg-info/not-zip-safe
--rw-------   0 cdoutrix (45773) cdoutrix (45773)       33 2022-08-10 17:01:10.000000 kosh-2.2/kosh.egg-info/requires.txt
--rw-------   0 cdoutrix (45773) cdoutrix (45773)        5 2022-08-10 17:01:10.000000 kosh-2.2/kosh.egg-info/top_level.txt
--rw-------   0 cdoutrix (45773) cdoutrix (45773)      545 2022-08-10 16:35:18.000000 kosh-2.2/pyproject.toml
-drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2022-08-10 17:01:11.114059 kosh-2.2/scripts/
--rw-------   0 cdoutrix (45773) cdoutrix (45773)    49114 2022-08-10 17:01:10.000000 kosh-2.2/scripts/kosh
--rwx------   0 cdoutrix (45773) cdoutrix (45773)     2953 2022-03-15 13:18:23.000000 kosh-2.2/scripts/sbang
--rw-------   0 cdoutrix (45773) cdoutrix (45773)       38 2022-08-10 17:01:11.119058 kosh-2.2/setup.cfg
--rw-------   0 cdoutrix (45773) cdoutrix (45773)     1796 2022-08-10 16:20:18.000000 kosh-2.2/setup.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.248299 kosh-3.0/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1099 2021-03-30 14:42:19.000000 kosh-3.0/LICENSE
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1164 2021-03-30 14:42:19.000000 kosh-3.0/NOTICE
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2323 2023-04-21 00:13:06.247309 kosh-3.0/PKG-INFO
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1873 2023-04-20 19:47:29.000000 kosh-3.0/README.md
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.129308 kosh-3.0/kosh/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1194 2023-04-20 19:47:29.000000 kosh-3.0/kosh/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    16480 2023-04-20 19:47:29.000000 kosh-3.0/kosh/core_sina.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)       24 2023-04-20 19:30:53.000000 kosh-3.0/kosh/current_version.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    53994 2023-04-20 19:47:29.000000 kosh-3.0/kosh/dataset.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    11351 2022-12-02 19:13:40.000000 kosh-3.0/kosh/ensemble.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.142308 kosh-3.0/kosh/exec_graphs/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)       74 2021-03-24 14:27:11.000000 kosh-3.0/kosh/exec_graphs/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    21546 2023-04-20 19:47:29.000000 kosh-3.0/kosh/exec_graphs/core.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.157309 kosh-3.0/kosh/loaders/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     3090 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/UltraLoader.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)      377 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    16420 2023-04-20 19:47:29.000000 kosh-3.0/kosh/loaders/core.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     5706 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/hdf5.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1176 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/jsons.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     5099 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/npy.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     3108 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/pgm.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1991 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/pil.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2520 2022-12-02 19:13:40.000000 kosh-3.0/kosh/loaders/sidre.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.162310 kosh-3.0/kosh/operators/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)      206 2023-04-20 19:47:29.000000 kosh-3.0/kosh/operators/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     5394 2022-12-02 19:13:40.000000 kosh-3.0/kosh/operators/core.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    19932 2023-04-20 19:47:29.000000 kosh-3.0/kosh/operators/koshClustering.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.164308 kosh-3.0/kosh/sampling_methods/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)        8 2023-04-20 19:47:29.000000 kosh-3.0/kosh/sampling_methods/__init__.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.168305 kosh-3.0/kosh/sampling_methods/cluster_sampling/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    47456 2023-04-20 19:47:29.000000 kosh-3.0/kosh/sampling_methods/cluster_sampling/Clustering.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)       65 2023-04-20 19:47:29.000000 kosh-3.0/kosh/sampling_methods/cluster_sampling/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     4743 2022-12-02 19:13:40.000000 kosh-3.0/kosh/schema.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    76087 2023-04-20 19:47:29.000000 kosh-3.0/kosh/store.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.178311 kosh-3.0/kosh/transformers/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)      331 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/__init__.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     4725 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/core.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8789 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/npy.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     4060 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/sidre.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    11617 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/skl.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1959 2022-12-02 19:13:40.000000 kosh-3.0/kosh/transformers/utils.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    21230 2023-04-20 19:47:29.000000 kosh-3.0/kosh/utils.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     6253 2022-12-02 19:13:40.000000 kosh-3.0/kosh/wrapper.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.138314 kosh-3.0/kosh.egg-info/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2323 2023-04-21 00:13:06.000000 kosh-3.0/kosh.egg-info/PKG-INFO
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2204 2023-04-21 00:13:06.000000 kosh-3.0/kosh.egg-info/SOURCES.txt
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)        1 2023-04-21 00:13:06.000000 kosh-3.0/kosh.egg-info/dependency_links.txt
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)        1 2023-04-20 20:01:56.000000 kosh-3.0/kosh.egg-info/not-zip-safe
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)      109 2023-04-21 00:13:06.000000 kosh-3.0/kosh.egg-info/requires.txt
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)        5 2023-04-21 00:13:06.000000 kosh-3.0/kosh.egg-info/top_level.txt
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.183310 kosh-3.0/scripts/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    50400 2023-04-21 00:13:05.000000 kosh-3.0/scripts/kosh
+-rwx------   0 cdoutrix (45773) cdoutrix (45773)    50400 2023-04-20 19:47:29.000000 kosh-3.0/scripts/kosh_command.py
+-rwx------   0 cdoutrix (45773) cdoutrix (45773)     2953 2022-12-02 19:13:40.000000 kosh-3.0/scripts/sbang
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)       38 2023-04-21 00:13:06.248309 kosh-3.0/setup.cfg
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1866 2023-04-21 00:10:55.000000 kosh-3.0/setup.py
+drwx------   0 cdoutrix (45773) cdoutrix (45773)        0 2023-04-21 00:13:06.245309 kosh-3.0/tests/
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1742 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_broken_loader.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    11507 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_clustering.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8587 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_clustering_raw.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    11220 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_command_line.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1601 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_context_manager.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8195 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_curves.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    21743 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_datasets.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     3963 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_describe_feature.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    10759 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_ensembles.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1238 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_fix_fastsha.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1254 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_flake8.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     9309 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_getitem_back_propagate.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    11654 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_import_export_datasets.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)      982 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_load_sina.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    22566 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_loaders.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1674 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_loaders_multiple_features_name.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    13615 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_mv.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     5177 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_operators.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     3012 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_operators_decorators.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8493 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_reassociate.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     4256 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_rm.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     4412 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_schema.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    13006 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_script_wrapper.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2261 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_search.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1471 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_search_speed.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     3349 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_sina_curves_as_associated.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8180 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_sina_files_section_as_associated.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)    13725 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_store.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2062 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_store_custom_loaders.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     8497 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_sync.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     7484 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_transformers.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2789 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_transformers_decorators.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1603 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_transformers_parent.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     1428 2022-12-02 19:13:40.000000 kosh-3.0/tests/test_kosh_users_and_groups.py
+-rw-------   0 cdoutrix (45773) cdoutrix (45773)     2954 2023-04-20 19:47:29.000000 kosh-3.0/tests/test_kosh_verbose_list_features.py
```

### Comparing `kosh-2.2/LICENSE` & `kosh-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kosh-2.2/NOTICE` & `kosh-3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `kosh-2.2/README.md` & `kosh-3.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 Contributions must be made under the same license as Kosh (see the bottom of this file).
 
 # Release and License
 Kosh is distributed under the terms of the MIT license; new contributions must be made under this license.
 
 SPDX-License-Identifier: MIT
 
-``LLNL-CODE-814755``
+``LLNL-CODE-814755``
```

### Comparing `kosh-2.2/kosh/__init__.py` & `kosh-3.0/kosh/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .current_version import current_version
 import os
+# import .sampling_methods  # noqa
 kosh_cache_dir = os.path.join(os.path.expanduser("~"), ".cache", "kosh")  # noqa
 from .loaders import KoshLoader, KoshSinaLoader  # noqa
 from .utils import create_new_db, walk_dictionary_keys, version  # noqa
 from .schema import KoshSchema  # noqa
 from .operators import KoshOperator  # noqa
 import pkg_resources  # noqa
 from .store import KoshStore, connect  # noqa
```

### Comparing `kosh-2.2/kosh/core_sina.py` & `kosh-3.0/kosh/core_sina.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,26 @@
                     else:
                         self.__store__.__sync__dict__[Id] = record
                         record["user_defined"]["last_update_from_db"] = time.time()
             else:
                 deleted_items = False
                 for att in self.__dict__["__protected__"]:
                     if att in record["data"]:
-                        del(record["data"][att])
+                        del record["data"][att]
                         deleted_items = True
                 if deleted_items:
                     if store.__sync__:
                         self._update_record(record)
                     else:
                         self.__store__.__sync__dict__[Id] = record
 
         metadata_copy = metadata.copy()
         for key in metadata:
             if att in self.__dict__["__protected__"]:
-                del(metadata_copy[key])
+                del metadata_copy[key]
         self.update(metadata_copy)
 
     def __getattr__(self, name):
         """__getattr__ get an attribute
 
         :param name: attribute to retrieve
         :type name: str
@@ -168,15 +168,15 @@
 
     def update(self, attributes):
         """update many attributes at once to limit db writes
         :param: attributes: dictionary with attributes to update
         :type attributes: dict
         """
         if 'id' in attributes:
-            del(attributes['id'])
+            del attributes['id']
         rec = None
         N = len(attributes)
         n = 0
         for name, value in attributes.items():
             n += 1
             if n == N:
                 update_db = True
@@ -207,15 +207,15 @@
         :rtype: sina.model.Record
         """
         if name in self.__protected__:  # Cannot set protected attributes
             return record
         if record is None:
             record = self.get_record()
         if name == "schema":
-            assert(isinstance(value, KoshSchema))
+            assert isinstance(value, KoshSchema)
             value.validate(self)
         elif self.schema is not None:
             self.schema.validate_attribute(name, value)
 
         # For datasets we need to check if the att comes from ensemble
         from kosh.dataset import KoshDataset
         if isinstance(self, KoshDataset) and not force:
@@ -327,15 +327,19 @@
         """
         if name in self.__protected__:
             return
         record = self.get_record()
         last_modif_att = "{name}_last_modified".format(name=name)
         now = time.time()
         record["user_defined"][last_modif_att] = now
-        del(record["data"][name])
+        # We need to remember we touched it otherwise
+        # if we create it again the db will look
+        # out of sync.
+        self.__dict__[last_modif_att] = now
+        del record["data"][name]
         if self.__store__.__sync__:
             self._update_record(record)
 
     def sync(self):
         """sync this object with database"""
         self.__store__.sync([self.id, ])
```

### Comparing `kosh-2.2/kosh/dataset.py` & `kosh-3.0/kosh/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -219,24 +219,26 @@
         elif Id not in self._associated_data_:
             raise RuntimeError(
                 "object {Id} is not associated with this dataset".format(
                     Id=Id))
         return self.__store__.open(Id, loader, *args, **kargs)
 
     def list_features(self, Id=None, loader=None,
-                      use_cache=True, *args, **kargs):
+                      use_cache=True, verbose=False, *args, **kargs):
         """list_features list features available if multiple associated data lead to duplicate feature name
         then the associated_data uri gets appended to feature name
 
         :param Id: id of associated object to get list of features from, defaults to None which means all
         :type Id: str, optional
         :param loader: loader to use to search for feature, will return ONLY features that the loader knows about
         :type loader: kosh.loaders.KoshLoader
         :param use_cache: If features is found on cache use it (default: True)
         :type use_cache: bool
+        :param verbose: Verbose mode will show which file is being opened and errors on it
+        :type verbose: bool
         :raises RuntimeError: object id not associated with dataset
         :return: list of features available
         :rtype: list
         """
         if use_cache and self.__dict__["__features__"].get(
                 Id, {}).get(loader, None) is not None:
             return self.__dict__["__features__"][Id][loader]
@@ -249,27 +251,31 @@
             self.__store__.__sync__dict__ = {}
             self.__store__.synchronous()
         features = []
         loaders = []
         associated_data = self._associated_data_
         if Id is None:
             for associated in associated_data:
+                if verbose:
+                    asso = self.__store__._load(associated)
+                    print("Finding features for {}".format(asso.uri))
                 if loader is None:
-                    ld, _ = self.__store__._find_loader(associated)
+                    ld, _ = self.__store__._find_loader(associated, requestorId=self.id, verbose=verbose)
                 else:
-                    if associated not in self.__store__._cached_loaders:
-                        self.__store__._cached_loaders[associated] = loader(
-                            self.__store__._load(associated)), None
-                    ld, _ = self.__store__._cached_loaders[associated]
+                    if (associated, self.id) not in self.__store__._cached_loaders:
+                        self.__store__._cached_loaders[associated, self.id] = loader(
+                            self.__store__._load(associated), requestorId=self.id), None
+                    ld, _ = self.__store__._cached_loaders[associated, self.id]
                 loaders.append(ld)
                 try:
                     features += ld._list_features(*
                                                   args, use_cache=use_cache, **kargs)
-                except Exception:  # Ok the loader couldn't get the feature list
-                    pass
+                except Exception as err:  # Ok the loader couldn't get the feature list
+                    if verbose:
+                        print("\tCould not obtain features from loader {}\n\t\tError:{}".format(loader, err))
             if len(features) != len(set(features)):
                 # duplicate features we need to redo
                 # Adding uri to feature name
                 ided_features = []
                 for index, associated in enumerate(associated_data):
                     ld = loaders[index]
                     if ld is None:
@@ -289,15 +295,18 @@
                             ided_features.append(feature)
                 features = ided_features
         elif Id not in self._associated_data_:
             raise RuntimeError(
                 "object {Id} is not associated with this dataset".format(
                     Id=Id))
         else:
-            ld, _ = self.__store__._find_loader(Id)
+            if loader is not None:
+                ld = loader
+            else:
+                ld, _ = self.__store__._find_loader(Id, requestorId=self.id, verbose=verbose)
             features = ld._list_features(*args, use_cache=use_cache, **kargs)
         features_id = self.__dict__["__features__"].get(Id, {})
         features_id[loader] = features
         self.__dict__["__features__"][Id] = features_id
         if saved_sync:
             # we need to restore sync mode
             self.__store__.__sync__dict__ = backup
@@ -336,54 +345,69 @@
         if not isinstance(feature, list):
             features = [feature, ]
         else:
             features = feature
         possibles = {}
         inter = None
         union = set()
-        for feature_ in features:
+        for index, feature_ in enumerate(features):
             possible_ids = []
             if Id is None:
                 for a in self._associated_data_:
                     a_original = a
                     if "__uri__" in a:
                         # Ok this is a pure sina file with mime_type
                         a, _ = a.split("__uri__")
                     a_obj = self.__store__._load(a)
                     if loader is None:
-                        ld, _ = self.__store__._find_loader(a_original)
+                        ld, _ = self.__store__._find_loader(a_original, requestorId=self.id)
                         if ld is None:  # unknown mimetype probably
                             continue
                     else:
                         if a_obj.mime_type in loader.types:
-                            ld = loader(a_obj)
+                            ld = loader(a_obj, requestorId=self.id)
                         else:
                             continue
                     # Dataset with curve have themselves as uri
                     obj_uri = getattr(ld.obj, "uri", "self")
-                    if ("_@_" not in feature_ and feature_ in ld._list_features()) or\
+                    ld_features = ld._list_features()
+                    if isinstance(ld, kosh.loaders.core.KoshSinaLoader):
+                        # ok we have to be careful list_features can be returned two ways
+                        if isinstance(ld_features[0], tuple) and isinstance(feature_, six.string_types):
+                            # we need to convert the feature to str
+                            possibilities = kosh.utils.find_curveset_and_curve_name(feature_, self.get_record())
+                            if len(possibilities) > 1:
+                                raise ValueError("cannot uniquely pinpoint {}, could be one of {}".format(
+                                    feature_, possibilities))
+                            feature_ = possibilities[0]
+                            features[index] = feature_
+                        elif isinstance(ld_features[0], six.string_types) and isinstance(feature_, tuple):
+                            feature_ = "/".join(feature_)
+                            features[index] = feature_
+
+                    if ("_@_" not in feature_ and feature_ in ld_features) or\
                             feature_ is None or\
-                            (feature_[:-len(obj_uri) - 3] in ld._list_features() and
+                            (feature_[:-len(obj_uri) - 3] in ld_features and
                              feature_[-len(obj_uri):] == obj_uri):
                         possible_ids.append(a_original)
                 if possible_ids == []:  # All failed but could be something about the feature
                     raise ValueError(
                         "Cannot find feature {} in dataset".format(feature_))
             elif Id == self.id:
                 # Ok asking for data not associated externally
                 # Likely curve
-                ld, _ = self.__store__._find_loader(Id)
+                ld, _ = self.__store__._find_loader(Id, requestorId=self.id)
                 if feature_ in ld._list_features():
                     possible_ids = [Id, ]
                 else:  # ok not a curve maybe a file?
                     rec = self.get_record()
                     for uri in rec["files"]:
                         if "mimetype" in rec["files"][uri]:
                             full_id = "{}__uri__{}".format(Id, uri)
-                            ld, _ = self.__store__._find_loader(full_id)
+                            ld, _ = self.__store__._find_loader(full_id, requestorId=self.id)
                             if ld is not None and feature_ in ld.list_features():
                                 possible_ids = [full_id, ]
             elif Id not in self._associated_data_:
                 raise RuntimeError(
                     "object {Id} is not associated with this dataset".format(
                         Id=Id))
             else:
@@ -402,41 +426,41 @@
         # Now let's go through each possible uri
         # and group features in them
         for id_ in union:
             matching_features = []
             for feature_ in features:
                 if feature_ in possibles and id_ in possibles[feature_]:
                     matching_features.append(feature_)
-                    del(possibles[feature_])
+                    del possibles[feature_]
             if len(matching_features) > 0:
                 ids[id_] = matching_features
 
         out = []
         for id_ in ids:
             features = ids[id_]
             for Id in possible_ids:
                 tmp = None
                 try:
                     if loader is None:
-                        ld, _ = self.__store__._find_loader(Id)
+                        ld, _ = self.__store__._find_loader(Id, requestorId=self.id)
                         mime_type = ld._mime_type
                     else:
-                        if Id not in self.__store__._cached_loaders:
+                        if (Id, self.id) not in self.__store__._cached_loaders:
                             a_obj = self.__store__._load(Id)
-                            self.__store__._cached_loaders[Id] = loader(a_obj)
+                            self.__store__._cached_loaders[Id, self.id] = loader(a_obj, requestorId=self.id)
                             mime_type = a_obj.mime_type
-                        ld = self.__store__._cached_loaders[Id]
+                        ld = self.__store__._cached_loaders[Id, self.id]
                     # Essentially make a copy
                     # Because we want to attach the feature to it
                     # But let's not lose the cached list_features
                     saved_listed_features = ld.__dict__[
                         "_KoshLoader__listed_features"]
                     ld_uri = getattr(ld, "uri", None)
                     ld = ld.__class__(
-                        ld.obj, mime_type=ld._mime_type, uri=ld_uri)
+                        ld.obj, mime_type=ld._mime_type, uri=ld_uri, requestorId=self.id)
                     ld.__dict__[
                         "_KoshLoader__listed_features"] = saved_listed_features
                     # Ensures there is a possible path to format
                     get_graph(mime_type, ld, transformers)
                     final_features = []
                     obj_uri = getattr(ld.obj, "uri", "")
                     for feature_ in features:
@@ -584,26 +608,26 @@
         :raises RuntimeError: object id not associated with dataset
         :return: dictionary describing the feature
         :rtype: dict
         """
         loader = None
         if Id is None:
             for a in self._associated_data_:
-                ld, _ = self.__store__._find_loader(a)
+                ld, _ = self.__store__._find_loader(a, requestorId=self.id)
                 if feature in ld._list_features(**kargs) or \
                         (feature[:-len(ld.obj.uri) - 3] in ld._list_features()
                          and feature[-len(ld.obj.uri):] == ld.obj.uri):
                     loader = ld
                     break
         elif Id not in self._associated_data_:
             raise RuntimeError(
                 "object {Id} is not associated with this dataset".format(
                     Id=Id))
         else:
-            loader, _ = self.__store__._find_loader(Id)
+            loader, _ = self.__store__._find_loader(Id, requestorId=self.id)
         return loader.describe_feature(feature)
 
     def dissociate(self, uri, absolute_path=True):
         """dissociates a uri/mime_type with this dataset
 
         :param uri: uri to access file
         :type uri: str
@@ -616,15 +640,15 @@
         if absolute_path and os.path.exists(uri):
             uri = os.path.abspath(uri)
         rec = self.get_record()
         if uri not in rec["files"]:
             # Not associated with this uri anyway
             return
         kosh_id = str(rec["files"][uri]["kosh_id"])
-        del(rec["files"][uri])
+        del rec["files"][uri]
         now = time.time()
         rec["user_defined"]["{uri}___associated_last_modified".format(
             uri=uri)] = now
         if self.__store__.__sync__:
             self._update_record(rec)
         # Get all object that have been associated with this uri
         rec = self.__store__.get_record(kosh_id)
@@ -633,16 +657,18 @@
         rec.data["associated"]["value"] = associated_ids
         if self.__store__.__sync__:
             self._update_record(rec)
         else:
             self._update_record(rec, self.__store__._added_unsync_mem_store)
         if len(associated_ids) == 0:  # ok no other object is associated
             self.__store__.delete(kosh_id)
-            if kosh_id in self.__store__._cached_loaders:
-                del(self.__store__._cached_loaders[kosh_id])
+            if (kosh_id, self.id) in self.__store__._cached_loaders:
+                del self.__store__._cached_loaders[kosh_id, self.id]
+            if (kosh_id, None) in self.__store__._cached_loaders:
+                del self.__store__._cached_loaders[kosh_id, None]
 
         # Since we changed the associated, we need to cleanup
         # the features cache
         self.__dict__["__features__"][None] = {}
         self.__dict__["__features__"][kosh_id] = {}
 
     def associate(self, uri, mime_type, metadata={},
@@ -735,15 +761,15 @@
                         rec_obj["data"][key]["value"] = meta[key]
                     last_modif_att = "{name}_last_modified".format(name=key)
                     rec_obj["user_defined"][last_modif_att] = time.time()
                 if not self.__store__.__sync__:
                     rec_obj["user_defined"]["last_update_from_db"] = time.time()
                     self.__store__.__sync__dict__[Id] = rec_obj
             except TypeError as err:
-                raise(err)
+                raise err
             except Exception:
                 # file already in there
                 # Let's get the matching id
                 if rec_obj["data"]["mime_type"]["value"] != mime_types[i]:
                     raise TypeError("file {} is already associated with this dataset with mimetype"
                                     " '{}' you specified mime_type '{}'".format(uri, existing_mime, mime_type))
                 else:
@@ -945,15 +971,15 @@
         :type ids_only: bool
         """
         for rel in self.get_sina_store().relationships.find(
                 self.id, self.__store__._ensemble_predicate, None):
             if ids_only:
                 yield rel.object_id
             else:
-                yield self.__store__.open(rel.object_id)
+                yield self.__store__.open(rel.object_id, requestorId=self.id)
 
     def leave_ensemble(self, ensemble):
         """Removes this dataset from an ensemble
         :param ensemble: The ensemble to leave
         :type ensemble: str or KoshEnsemble
         """
         from kosh.ensemble import KoshEnsemble
@@ -972,15 +998,15 @@
     def join_ensemble(self, ensemble):
         """Adds this dataset to an ensemble
         :param ensemble: The ensemble to join
         :type ensemble: str or KoshEnsemble
         """
         from kosh.ensemble import KoshEnsemble
         if isinstance(ensemble, six.string_types):
-            ensemble = self.__store__.open(ensemble)
+            ensemble = self.__store__.open(ensemble, requestorId=self.id)
         if not isinstance(ensemble, KoshEnsemble):
             raise ValueError(
                 "cannot join `ensemble` since object `{}` does not map to an ensemble".format(ensemble))
         ensemble.add(self)
 
     def clone(self, preserve_ensembles_memberships=False, id_only=False):
         """Clones the dataset, e.g makes an identical copy.
@@ -1035,15 +1061,15 @@
         :type ensemble_id: bool
         :returns: True or ensemble of origin id if the attribute belongs to an ensemble False/"" otherwise
         """
         if ensembles is None:
             ensembles = self.get_ensembles()
         elif isinstance(ensembles, str):
             try:
-                ensembles = self.__store__.open(ensembles)
+                ensembles = self.__store__.open(ensembles, requestorId=self.id)
             except Exception:
                 raise ValueError(
                     "could not find object with id {} in the store".format(ensembles))
             ensembles = [ensembles, ]
         elif not isinstance(ensembles, Iterable):
             ensembles = [ensembles, ]
         for ensemble in ensembles:
@@ -1057,7 +1083,131 @@
                     return ensemble.id
                 else:
                     return True
         if ensemble_id:
             return ""
         else:
             return False
+
+    def add_curve(self, curve, curve_set=None, curve_name=None, independent=None, units=None, tags=None):
+        """Add a curve to a dataset
+        :param curve: The curve data
+        :type curve: array-like
+        :param curve_set: Name of the curve_set.
+                          If not passed will be set to curve_x where x is the highest number available
+                          (if non exist then curve_set_0 will be created)
+        :type curve_set: str
+        :param curve_name: name of the curve.
+                           If not set it will be set to: curve_x where x is the number of curves in this curve_set
+        :type curve_name: str
+        :param independent: Is it an independent variable. If not passed, it will be set to False
+                            unless no independent curve exists, e.g first curve is set as independent
+                            You can avoid this by explicitly passing False
+        :type independent: bool
+        :param units: Units of the curve (if any)
+        :type units: str
+        :param tags: Tags on the curve (if any)
+        :type tags: dict
+
+        :returns: the curve_set/curve_name path
+        :rtype: str
+        """
+        # let's obtain the record
+        rec = self.get_record()
+        # Let's figure out the curve_set name
+        if curve_set is None:
+            i = 0
+            while "curve_set_"+str(i) in rec.raw["curve_sets"]:
+                i += 1
+            if i > 0:
+                i -= 1
+            curve_set = "curve_set_"+str(i)
+
+        # Let's create curveset if not present
+        if curve_set not in rec.raw["curve_sets"]:
+            cs = rec.add_curve_set(curve_set)
+        else:
+            cs = rec.get_curve_set(curve_set)
+        # Ok now let's get a curve_name
+        if curve_name is None:
+            i = 0
+            while "curve_"+str(i) in cs.dependent or "curve_"+str(i) in cs.independent:
+                i += 1
+            curve_name = "curve_"+str(i)
+
+        if curve_name in cs.independent or curve_name in cs.dependent:
+            raise ValueError("curve {} already exist in curve_set {}".format(curve_name, curve_set))
+        # Finally the independent part
+        if independent is None:
+            if len(cs.independent) == 0:
+                independent = True
+            else:
+                independent = False
+        if independent:
+            cs.add_independent(curve_name, curve, units, tags)
+        else:
+            cs.add_dependent(curve_name, curve, units, tags)
+
+        if self.__store__.__sync__:
+            self._update_record(rec)
+        else:
+            self._update_record(rec, self.__store__._added_unsync_mem_store)
+
+        # Since we changed the curves, we need to cleanup
+        # the features cache
+        self.__dict__["__features__"][None] = {}
+
+        return "{}/{}".format(curve_set, curve_name)
+
+    def remove_curve_or_curve_set(self, curve, curve_set=None):
+        """Removes a curve or curve_set from the dataset
+        :param curve: name of the curve or curve_set to remove
+        :type curve: str
+        :param curve_set: curve_set the curve_name belongs to.
+                          If not passed then assumes it is in the curve
+                          name.
+        :type curve_set: str
+        """
+        original_curve_set = curve_set
+        rec = self.get_record()
+        if curve_set is None:
+            # User did not pass the curve_set
+            # The curve_set might be prepended to the curve_name then.
+            try:
+                curve_set, curve = kosh.utils.find_curveset_and_curve_name(curve, rec)[0]
+            except Exception:
+                raise ValueError("You need to pass a curve set for curve {}".format(curve))
+        if curve_set not in rec.raw["curve_sets"]:
+            if original_curve_set is None:
+                if curve in rec.raw["curve_sets"]:
+                    del rec.raw["curve_sets"][curve]
+                    if self.__store__.__sync__:
+                        self._update_record(rec)
+                    else:
+                        self._update_record(rec, self.__store__._added_unsync_mem_store)
+                    self.__dict__["__features__"][None] = {}
+                    return
+            else:
+                raise ValueError("The curve set {} does not exists".format(curve_set))
+        cs = rec.get_curve_set(curve_set)
+        if curve in cs.independent:
+            del rec.raw["curve_sets"][curve_set]["independent"][curve]
+        elif curve in cs.dependent:
+            del rec.raw["curve_sets"][curve_set]["dependent"][curve]
+        elif curve is None:
+            # We want to delete the whole curveset
+            del rec.raw["curve_sets"][curve_set]
+        else:
+            raise ValueError("Could not find {} in curve_set {}".format(curve, curve_set))
+        # In case we removed everything
+        if len(cs.dependent) == 0 and len(cs.independent) == 0:
+            del rec.raw["curve_sets"][curve_set]
+
+        if self.__store__.__sync__:
+            self._update_record(rec)
+        else:
+            self._update_record(rec, self.__store__._added_unsync_mem_store)
+
+        # Since we changed the curves, we need to cleanup
+        # the features cache
+        self.__dict__["__features__"][None] = {}
+        return
```

### Comparing `kosh-2.2/kosh/ensemble.py` & `kosh-3.0/kosh/ensemble.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/exec_graphs/core.py` & `kosh-3.0/kosh/exec_graphs/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import collections
 
 
 def possible_ends(graph, start_nodes, end_nodes):
     """Finds all network ends that can be reached by all start nodes
     :param graph: The full graph
-    :type graph: networkx.OrderedDiGraph
+    :type graph: networkx.DiGraph (OrderedDiGraph on older version of networkx)
     :param start_nodes: Node to start paths from
     :type start_nodes: list of nodes
     :param end_nodes: Node to end paths from
     :type end_nodes: list of nodes
     :returns: list of possible end nodes
     :rtype: list
     """
@@ -63,17 +63,17 @@
             else:
                 for final_fmt in next_nodes[0].types[format]:
                     final_node = (final_fmt, None, G.seed)
                     G.add_edge(this_node, final_node)
 
 
 def find_network_ends(G, start=True, end=True):
-    """Given a networkx.OrderedDiGraph finds start or end nodes or both.
+    """Given an Ordered networkx.DiGraph finds start or end nodes or both.
     :param G: Network of interest
-    :type G: networkx.OrderedDiGraph
+    :type G: networkx.DiGraph (OrderedDiGraph on older version of networkx)
     :param start: Are we searching for start nodes?
     :type start: bool
     :param end: Are we searching for end nodes?
     :type end: bool
     :returns: start and end node lists or just start/end node list
     :rtype: (tuple of) list
     :raises ValueError: if neither start or end is True
@@ -164,15 +164,18 @@
     def __init__(self, *inputs, **kw):
         graphs = []
         # Get a new seed
         self.seed = random.random()
         # Set the variable to receive results per index
         self.index_results = {}
         # Create a new merged graph
-        new_graph = nx.OrderedDiGraph()
+        try:
+            new_graph = nx.OrderedDiGraph()
+        except AttributeError:
+            new_graph = nx.DiGraph()
         new_graph.seed = random.random()
         for i, G in enumerate(inputs):
             if isinstance(G, KoshExecutionGraph):
                 G = G.execution_graph()
             elif not hasattr(G, "seed"):
                 G.seed = random.random()
             # remember all graph we sent in
@@ -247,18 +250,21 @@
         :type seed: int
         :param verbose: verbose generation, also generates a png with the grap representation
                         Mostly used for debug purposes
         :type verbose: bool
         :param png_template: template to use to generate graph png in verbose mode
                              "_IN"/"_OUT" will be appended and seed will be fed
         :type png_template: str
-        :return a new graph with new seed
-        :rtype: networkx.OrderedDiGraph
+        :return a new ordered graph with new seed
+        :rtype: networkx.DiGraph
         """
-        G = nx.OrderedDiGraph()
+        try:
+            G = nx.OrderedDiGraph()
+        except AttributeError:
+            G = nx.DiGraph()
         if seed is None:
             seed = random.random()
         G.seed = seed
         if verbose:
             try:
                 if "DISPLAY" not in os.environ or os.environ["DISPLAY"] == "":
                     import matplotlib
@@ -341,15 +347,18 @@
             for start_node in start_nodes:
                 pths.append(nx.shortest_path(G, start_node, end_node))
             self.paths[format] = pths
         else:
             pths = self.paths[format]
 
         # Ok let's generate the new network with only the paths
-        out = nx.OrderedDiGraph()
+        try:
+            out = nx.OrderedDiGraph()
+        except AttributeError:
+            out = nx.DiGraph()
         out.seed = G.seed
         for pth in pths:
             for i, node in enumerate(pth[:-1]):
                 if pth[i+1][1] is not None:
                     pth[i+1][1].parent = node[1]
                 out.add_edge(node, pth[i + 1])
 
@@ -484,7 +493,45 @@
                     data.append(pickle.load(f))
                 except Exception:
                     cont = False
         if len(data) == 1:
             return data[0]
         else:
             return data
+
+    def get_input_loaders(self):
+        """Return a generator of the originating loaders for the inputs.
+        It will crawl the graph backward when
+        it encounters transformers or operators.
+        :return: generator of Kosh datasets
+        :rtype: KoshLoader generator
+        """
+        for start_node in self.start_nodes:
+            loader = start_node[1]
+            yield loader
+
+    def get_input_datasets(self):
+        """Return a generator of the originating datasets for the inputs.
+        It will crawl the graph backward when
+        it encounters transformers or operators.
+        :return: generator of Kosh datasets
+        :rtype: KoshDataset generator
+        """
+        for start_node in self.start_nodes:
+            loader = start_node[1]
+            yield loader.get_requestor()
+
+    def describe_entries(self):
+        """Return a generator of describe_feature for each entry feature.
+        It will crawl the graph backward when
+        it encounters transformers or operators.
+        If a loader did not implement `describe_feature` an empty dictionary
+        will be used instead.
+        :return: generator of info dictionaries
+        """
+        for start_node in self.start_nodes:
+            loader = start_node[1]
+            try:
+                info = loader.describe_feature(loader.feature)
+            except NotImplementedError:
+                info = {}
+            yield info
```

### Comparing `kosh-2.2/kosh/loaders/UltraLoader.py` & `kosh-3.0/kosh/loaders/UltraLoader.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/core.py` & `kosh-3.0/kosh/loaders/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from kosh.transformers import kosh_cache_dir
 import os
 import hashlib
 import pickle
+import six
 from kosh.exec_graphs import KoshExecutionGraph
 import numpy
 from ..core_sina import KoshSinaObject, KoshSinaFile
-from ..utils import get_graph
+from ..utils import get_graph, find_curveset_and_curve_name
 from ..dataset import KoshDataset
 from ..ensemble import KoshEnsemble
 
 
 class KoshGenericObjectFromFile(KoshSinaObject):
     """Kosh object pointing to a file"""
 
@@ -33,23 +34,26 @@
     """
     :param types: types is a dictionary on known type that can be loaded
     as key and export format as value, defaults to {"dataset": []}
     :type types: dict
     """
     types = {"dataset": []}
 
-    def __init__(self, obj, mime_type=None, uri=None):
+    def __init__(self, obj, mime_type=None, uri=None, requestorId=None):
         """KoshLoader generic Kosh loader
         :param obj: object the loader will try to load from
         :type obj: object
         :param mime_type: If you want to force the mime_type to use
         :type mime_type: str
         :param uri: If you want/need to force the uri to use
         :type uri: str
+        :param requestorId: The id of the dataset requesting data
+        :type requestorId: str
         """
+        self.requestorId = requestorId
         self.signature = hashlib.sha256(repr(self.__class__).encode())
         self.signature = self.update_signature(obj.id)
         if mime_type is None:
             self._mime_type = obj.mime_type
         else:
             self._mime_type = mime_type
         if uri is None:
@@ -72,14 +76,21 @@
                     open_anything = True
             if not open_anything:
                 raise RuntimeError(
                     "will not be able to load object of type {mime_type}".format(mime_type=self._mime_type))
         self.obj = obj
         self.__listed_features = None
 
+    def get_requestor(self):
+        """Returns the Kosh object requesting the data"""
+        try:
+            return self.obj.__store__.open(self.requestorId)
+        except Exception:  # some kosh object do not have an open function
+            return self.obj.__store__._load(self.requestorId)
+
     def known_types(self):
         """Lists types of Kosh objects this loader can handle
 
         :return: list of Kosh type this loader can handle
         :rtype: list
         """
         return list(self.types.keys())
@@ -260,15 +271,15 @@
         """preprocess sets things up for the extract function
 
         This should be preceeded by a call to 'get' which stored its args
         in self._user_passed_parameters
         """
         return
 
-    def extract(self, feature, format):
+    def extract(self):
         """extract this function does the heavy lifting of the extraction
         it needs to be implemented by each loader.
 
         We recommend returning pointer to the data as much as possible
 
         :raises NotImplementedError:
         """
@@ -285,16 +296,16 @@
         return data
 
 
 class KoshFileLoader(KoshLoader):
     """Kosh loader to load content from files"""
     types = {"file": []}
 
-    def __init__(self, obj, **args):
-        super(KoshFileLoader, self).__init__(obj)
+    def __init__(self, obj, **kwargs):
+        super(KoshFileLoader, self).__init__(obj, **kwargs)
 
     def open(self, mode='r'):
         """open/load the matching Kosh Sina File
 
         :param mode: mode to open the file in, defaults to 'r'
         :type mode: str, optional
         :return: Kosh File object
@@ -360,47 +371,58 @@
             return KoshSinaObject(self.obj.id, self.obj.__store__, record["type"], protected=[
             ], record_handler=self.obj.__store__.__record_handler__, record=record)
 
     def list_features(self):
         record = self.obj.__store__.get_record(self.obj.id)
         # Using set in case a variable is both in independent and dependent
         # Dependent would win when getting the data
-        curves = set()
+        curves = ()
         for curve in record["curve_sets"]:
-            curves.add(curve)
+            curves += ((curve, None), )
             for curve_type in ["independent", "dependent"]:
                 for name in record["curve_sets"][curve][curve_type]:
-                    curves.add("{}/{}".format(curve, name))
-        return sorted(curves)
+                    curves += ((curve, name), )
+        joined = sorted([x if y is None else x+"/"+y for x, y in curves])
+        if joined == sorted(set(joined)):
+            return joined
+        else:
+            return sorted(curves, key=lambda x: (x[0], "" if x[1] is None else x[1]))
 
     def extract(self, *args, **kargs):
         features = self.feature
         if not isinstance(features, list):
             features = [self.feature, ]
         record = self.obj.__store__.get_record(self.obj.id)
         out = []
         for feature in features:
-            sp = feature.split("/")
+            if isinstance(feature, six.string_types):
+                possibilities = find_curveset_and_curve_name(feature, record)
+                if len(possibilities) > 1:
+                    raise ValueError("Could not uniquely resolve {} if to could belong to any of: {}".format(
+                        feature, possibilities))
+                curve_set, curve_name = possibilities[0]
+            else:
+                curve_set, curve_name = feature
             # Here we are assuming the curve root name cannot have "/" in it
-            curve_root = record["curve_sets"][sp[0]]
-            if len(sp) > 1:
-                curve_name = "/".join(sp[1:])
-                if curve_name in curve_root["dependent"]:
-                    curve = curve_root["dependent"][curve_name]["value"]
+            curve_set = record["curve_sets"][curve_set]
+            if curve_name is not None:
+                if curve_name in curve_set["independent"]:
+                    curve = curve_set["independent"][curve_name]["value"]
+                elif curve_name in curve_set["dependent"]:
+                    curve = curve_set["dependent"][curve_name]["value"]
                 else:
-                    curve = curve_root["independent"][curve_name]["value"]
+                    raise ValueError("Cannot find curve {} in curve_set {}".format(curve_name, curve_set))
                 out.append(numpy.array(curve))
             else:
                 # we want all curves
                 all = []
                 # Matching order (indep/dep) that we used in list_features
                 for curve_type in ["independent", "dependent"]:
                     # Same order as list_features()
-                    for curve_name in sorted(curve_root[curve_type].keys()):
-                        curve = curve_root[curve_type][curve_name]["value"]
+                    for curve_name in sorted(curve_set[curve_type].keys()):
+                        curve = curve_set[curve_type][curve_name]["value"]
                         all.append(numpy.array(curve))
                 out.append(all)
-
         if not isinstance(self.feature, list):
             return out[0]
         else:
             return out
```

### Comparing `kosh-2.2/kosh/loaders/hdf5.py` & `kosh-3.0/kosh/loaders/hdf5.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/jsons.py` & `kosh-3.0/kosh/loaders/jsons.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/npy.py` & `kosh-3.0/kosh/loaders/npy.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/pgm.py` & `kosh-3.0/kosh/loaders/pgm.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/pil.py` & `kosh-3.0/kosh/loaders/pil.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/loaders/sidre.py` & `kosh-3.0/kosh/loaders/sidre.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/operators/core.py` & `kosh-3.0/kosh/operators/core.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/schema.py` & `kosh-3.0/kosh/schema.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/store.py` & `kosh-3.0/kosh/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import gc
 import sys
 import uuid
 import sina.utils
 from sina.model import Relationship
 import collections
 if not sys.platform.startswith("win"):
     import fcntl
@@ -186,15 +187,15 @@
 
         if db is None:
             db = 'sql'
         self._dataset_record_type = dataset_record_type
         self.db_uri = db_uri
         if db == "sql":
             if not os.path.exists(db_uri):
-                if ("://" in db_uri and "@" in db_uri):
+                if "://" in db_uri:
                     self.__sina_store = sina_connect(
                         db_uri, read_only=read_only)
                 else:
                     raise ValueError(
                         "Kosh store could not be found at: {}".format(db_uri))
             else:
                 self.lock()
@@ -218,14 +219,17 @@
         self._users_type = rec["data"]["users_type"]["value"]
         self._groups_type = rec["data"]["groups_type"]["value"]
         self._loaders_type = rec["data"]["loaders_type"]["value"]
         self._ensembles_type = rec["data"]["ensembles_type"]["value"]
         self._ensemble_predicate = rec["data"]["ensemble_predicate"]["value"]
         self._kosh_reserved_record_types = kosh_reserved_record_types + \
             rec["data"]["reserved_types"]["value"]
+        kosh_reserved = list(self._kosh_reserved_record_types)
+        kosh_reserved.remove(self._sources_type)
+        self._kosh_datasets_and_sources = sina.utils.Negation(kosh_reserved)
 
         # Associated stores
         self._associated_stores_ = []
         if "associated_stores" in rec["data"]:
             for store in rec["data"]["associated_stores"]["value"]:
                 try:
                     self._associated_stores_.append(kosh.connect(store, read_only=read_only, sync=sync))
@@ -266,14 +270,17 @@
         # Ok we need to map the KoshFileLoader back to whatever the source_type is
         # in this store
         ks = self.loaders["file"]
         for loader in ks:
             loader.types[self._sources_type] = loader.types["file"]
         self.loaders[self._sources_type] = self.loaders["file"]
 
+    def __enter__(self):
+        return self
+
     def add_loader(self, loader, save=False):
         """Adds a loader to the store
 
         :param loader: The Kosh loader you want to add to the store
         :type loader: KoshLoader
         :param save: Do we also save it in store for later re-use
         :type save: bool
@@ -281,21 +288,59 @@
         :return: None
         :rtype: None
         """
         # We add a loader we need to clear the cache
         self._cached_loaders = collections.OrderedDict()
         for k in loader.types:
             if k in self.loaders:
-                self.loaders[k].append(loader)
+                if loader not in self.loaders[k]:
+                    self.loaders[k].append(loader)
             else:
                 self.loaders[k] = [loader, ]
 
         if save:  # do we save it in store
             self.save_loader(loader)
 
+    def delete_loader(self, loader, permanently=False):
+        """Removes a loader from the store and possible from its db
+
+        :param loader: The Kosh loader you want to add to the store
+        :type loader: KoshLoader
+        :param permanently: Do we also remove it from the db if saved there?
+        :type permanently: bool
+
+        :return: None
+        :rtype: None
+        """
+        # We add a loader we need to clear the cache
+        self._cached_loaders = collections.OrderedDict()
+        for k in loader.types:
+            if k in self.loaders:
+                if loader in self.loaders[k]:
+                    self.loaders[k].remove(loader)
+
+        if permanently:  # Remove it from saved in db as well
+            pickled = pickle.dumps(loader).decode("latin1")
+            rec = next(self.find(types="koshloader", code=pickled, ids_only=True), None)
+            if rec is not None:
+                self.lock()
+                self.__record_handler__.delete(rec)
+                self.unlock()
+
+    def remove_loader(self, loader):
+        """Removes a loader from the store and its db
+
+        :param loader: The Kosh loader you want to add to the store
+        :type loader: KoshLoader
+
+        :return: None
+        :rtype: None
+        """
+        self.delete_loader(loader, permanently=True)
+
     def lock(self):
         """Attempts to lock the store, helps when many concurrent requests are made to the store"""
         if not self.use_lock_file:
             return
         locked = False
         while not locked:
             try:
@@ -335,14 +380,18 @@
     def get_sina_records(self):
         """Returns sina store's records"""
         return self.__record_handler__
 
     def close(self):
         """closes store and sina related things"""
         self.__sina_store.close()
+        gc.collect()
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        self.close()
 
     def delete_all_contents(self, force=""):
         """
         Delete EVERYTHING in a datastore; this cannot be undone.
 
         :param force: This function is meant to raise a confirmation prompt. If you
                       want to use it in an automated script (and you're sure of
@@ -360,14 +409,18 @@
         Executed immediately even in async mode
 
         :param loader: Loader to save
         :type loader: KoshLoader
         """
 
         pickled = pickle.dumps(loader).decode("latin1")
+        rec = next(self.find(types="koshloader", code=pickled, ids_only=True), None)
+        if rec is not None:
+            # already in store
+            return
         rec = Record(id=uuid.uuid4().hex, type="koshloader")
         rec.add_data("code", pickled)
         self.lock()
         self.__record_handler__.insert(rec)
         self.unlock()
 
     def get_record(self, Id):
@@ -383,15 +436,15 @@
         else:
             record = self.__record_handler__.get(Id)
             self.__sync__dict__[Id] = record
             if not self.__sync__:  # we are not autosyncing
                 keys = list(record["user_defined"].keys())
                 for key in keys:
                     if key[-14:] == "_last_modified":
-                        del(record["user_defined"][key])
+                        del record["user_defined"][key]
             record["user_defined"]["last_update_from_db"] = time.time()
         return record
 
     def delete(self, Id):
         """remove a record from store.
         for datasets dissociate all associated data first.
 
@@ -406,15 +459,15 @@
             kosh_obj = self.open(Id)
             for uri in list(rec["files"].keys()):
                 # Let's dissociate to remove unused kosh objects as well
                 kosh_obj.dissociate(uri)
         if not self.__sync__:
             self._added_unsync_mem_store.records.delete(Id)
             if Id in self.__sync__dict__:
-                del(self.__sync__dict__[Id])
+                del self.__sync__dict__[Id]
                 self.__sync__deleted__[Id] = rec
                 rec["user_defined"]["deleted_time"] = time.time()
         else:
             self.__record_handler__.delete(Id)
 
     def create_ensemble(self, name="Unnamed Ensemble", id=None, metadata={}, schema=None, **kargs):
         """Create a Kosh ensemble object
@@ -497,40 +550,48 @@
                 out = KoshDataset(Id, store=self, schema=schema, record=rec)
         except Exception as err:  # probably schema validation error
             if self.__sync__:
                 self.lock()
                 self.__record_handler__.delete(Id)
                 self.unlock()
             else:
-                del(self.__sync__dict__[Id])
+                del self.__sync__dict__[Id]
                 self._added_unsync_mem_store.records.delete(rec)
             raise err
         return out
 
-    def _find_loader(self, Id, format=None, transformers=[]):
+    def _find_loader(self, Id, verbose=False, requestorId=None):
         """_find_loader returns a loader that can open Id
 
         :param Id: Id of the object to load
         :type Id: str
+        :param verbose: verbose mode will show errors
+        :type verbose: bool
+        :param requestorId: The id of the dataset requesting data
+        :type requestorId: str
         :return: Kosh loader object
         """
         Id_original = str(Id)
         if "__uri__" in Id:
             # Ok this is a pure sina file with mime_type
             Id, uri = Id.split("__uri__")
         else:
             uri = None
-        if Id_original in self._cached_loaders:
+        if verbose:
+            print("Finding loader for: {}".format(uri))
+        if (Id_original, requestorId) in self._cached_loaders:
             try:
-                feats = self._cached_loaders[Id_original][0].list_features() != [
-                ]
-            except Exception:
+                feats = self._cached_loaders[Id_original, requestorId][0].list_features()  # != []
+            except Exception as err:
                 feats = []
+                if verbose:
+                    print("Error opening {} with loader {}: {}".format(
+                        uri, self._cached_loaders[Id_original, requestorId], err))
             if feats != []:
-                return self._cached_loaders[Id_original]
+                return self._cached_loaders[Id_original, requestorId]
         record = self.get_record(Id)
         obj = self._load(Id)
         # uri not none means it is pure sina record with file and mime_type
         if (record["type"] not in self._kosh_reserved_record_types and uri is None)\
                 or record["type"] in [self._ensembles_type, "__kosh_storeinfo__"]:
             # Not reserved means dataset
             return KoshSinaLoader(obj), record["type"]
@@ -543,51 +604,56 @@
             mime_type_passed = mime_type
         else:  # Pure sina with file/mime_type
             mime_type = mime_type_passed = record["files"][uri]["mimetype"]
         if mime_type in self.loaders:
             for ld in self.loaders[mime_type]:
                 try:
                     feats = ld(obj, mime_type=mime_type_passed, uri=uri).list_features()
-                except Exception:
+                except Exception as err:
                     # Something happened can't list features
                     feats = []
+                    if verbose:
+                        print("Error opening {} with loader {}: {}".format(obj.uri, ld, err))
                 if feats != []:
                     break
-            self._cached_loaders[Id_original] = ld(
-                obj, mime_type=mime_type_passed, uri=uri), record["type"]
-            return self._cached_loaders[Id_original]
+            self._cached_loaders[Id_original, requestorId] = ld(
+                obj, mime_type=mime_type_passed, uri=uri, requestorId=requestorId), record["type"]
+            return self._cached_loaders[Id_original, requestorId]
         # sometime types have subtypes (e.g 'file') let's look if we
         # understand a subtype since we can't figure it out from mime_type
         if record["type"] in self.loaders:  # ok not a generic loader let's use it
             for ld in self.loaders[record["type"]]:
                 try:
-                    feats = ld(obj, mime_type=mime_type_passed, uri=uri).list_features()
+                    feats = ld(obj, mime_type=mime_type_passed, uri=uri, requestorId=requestorId).list_features()
                 except Exception:
                     # Something happened can't list features
                     feats = []
                 if feats != []:
                     break
-            self._cached_loaders[Id_original] = ld(
-                obj, mime_type=mime_type_passed, uri=uri), record["type"]
-            return self._cached_loaders[Id_original]
+            self._cached_loaders[Id_original, requestorId] = ld(
+                obj, mime_type=mime_type_passed, uri=uri, requestorId=requestorId), record["type"]
+            return self._cached_loaders[Id_original, requestorId]
         return None, None
 
-    def open(self, Id, loader=None, *args, **kargs):
+    def open(self, Id, loader=None, requestorId=None, *args, **kargs):
         """open loads an object in store based on its Id
         and run its open function
 
         :param Id: unique id of object to open
         :type Id: str
         :param loader: loader to use, defaults to None which means pick for me
+        :type loader: KoshLoader
+        :param requestorId: The id of the dataset requesting data
+        :type requestorId: str
         :return:
         """
         if loader is None:
-            loader, _ = self._find_loader(Id)
+            loader, _ = self._find_loader(Id, requestorId=requestorId)
         else:
-            loader = loader(self._load(Id))
+            loader = loader(self._load(Id), requestorId=requestorId)
         return loader.open(*args, **kargs)
 
     def _load(self, Id):
         """_load returns an associated source based on id
 
         :param Id: unique id in store
         :type Id: str
@@ -600,32 +666,34 @@
                                 store=self, record=record)
         else:
             return KoshSinaObject(Id, kosh_type=record["type"],
                                   record_handler=self.__record_handler__,
                                   store=self, record=record)
 
     def get(self, Id, feature, format=None, loader=None,
-            transformers=[], *args, **kargs):
+            transformers=[], requestorId=None, *args, **kargs):
         """get returns an associated source's data
 
         :param Id: Id of object to retrieve
         :type Id: str
         :param feature: feature to retrieve
         :type feature: str
         :param format: preferred format, defaults to None means pick for me
         :type format: str, optional
         :param loader: loader to use, defaults to None means pick for me
         :return: data in requested format
         :param transformers: A list of transformers to use after the data is loaded
         :type transformers: kosh.operator.KoshTransformer
+        :param requestorId: The id of the dataset requesting data
+        :type requestorId: str
         """
         if loader is None:
-            loader, _ = self._find_loader(Id)
+            loader, _ = self._find_loader(Id, requestorId=requestorId)
         else:
-            loader = loader(self._load(Id))
+            loader = loader(self._load(Id), requestorId=requestorId)
 
         return loader.get(feature, format, transformers=[], *args, **kargs)
 
     def search(self, *atts, **keys):
         """
         Deprecated use find
         """
@@ -725,21 +793,21 @@
                 "`kosh_type` has been replaced with `types` you cannot use both at same time")
         if "kosh_type" in keys:
             warnings.warn(
                 "`kosh_type` is being deprecated in favor of `types` and will not work in a future version",
                 DeprecationWarning)
             record_types = keys.pop("kosh_type")
         else:
-            record_types = keys.pop("types", None)
+            record_types = keys.pop("types", (None, None))  # can't use just None
 
         if isinstance(record_types, six.string_types):
             record_types = [record_types, ]
-        if record_types is not None and not isinstance(
-                record_types, (list, tuple)):
-            raise ValueError("`types` must be str or list")
+        if record_types not in [None, (None, None)] and not isinstance(
+                record_types, (list, tuple, sina.utils.Negation)):
+            raise ValueError("`types` must be None, str, list or sina.utils.Negation")
 
         if 'file_uri' in keys and 'file' in keys:
             raise ValueError(
                 "`file` has been deprecated for `file_uri` but you cannot use both at same time")
         if 'file' in keys:
             file_uri = keys.pop("file")
         else:
@@ -747,27 +815,27 @@
 
         # Ok now let's look if the user wants to search for an id
         if "id" in keys:
             if "id_pool" in keys:
                 raise ValueError("you cannot use id and id_pool together")
             warnings.warn("When searching by id use id_pool")
             sina_kargs["id_pool"] = keys["id"]
-            del(keys["id"])
+            del keys["id"]
         else:
             sina_kargs["id_pool"] = keys.pop("id_pool", None)
 
         sina_kargs["file_uri"] = file_uri
         sina_kargs["query_order"] = keys.pop(
             "query_order", ("data", "file_uri", "types"))
 
-        # records type
-        if record_types is None and sina_kargs["id_pool"] is None:
-            # Ok we want anything, but we need to exclude Kosh reserved
-            # but only if user did not specified an id_pool
+        if record_types == (None, None):
             record_types = sina.utils.not_(self._kosh_reserved_record_types)
+            if sina_kargs["id_pool"] is not None:
+                record_types = None
+
         sina_kargs["types"] = record_types
         # The data dict for sina
         sina_data = keys.pop("data", {})
         if not isinstance(sina_data, dict):
             keys["data"] = sina_data
             sina_data = {}
         elif len(sina_data) != 0 and (len(keys) != 0 or len(atts) != 0):
@@ -805,15 +873,21 @@
 
         if mode:
             # we need to restore sync mode
             self.__sync__dict__ = backup
             self.synchronous()
 
         for rec_id in match:
-            yield rec_id if ids_only else self.open(rec_id)
+            if ids_only:
+                yield rec_id
+            else:
+                try:
+                    yield self.open(rec_id)
+                except Exception:
+                    yield self._load(rec_id)
 
     def check_sync_conflicts(self, keys):
         """Checks if their will be sync conflicts
         :param keys: keys of objects to syncs (id/type)
         :type keys: list
         :return: dictionary of objects ids and their failing attributes
         :rtype: dict
@@ -1001,27 +1075,27 @@
                 db = self.__record_handler__.get(key)
                 for att in local["user_defined"]:
                     if att[-14:] == "_last_modified":  # We touched it
                         if att[-27:-14] == "___associated":
                             # ok it's an associated thing
                             uri = att[:-27]
                             if uri not in local["files"]:  # dissociated
-                                del(db["files"][uri])
+                                del db["files"][uri]
                             elif att not in db["user_defined"]:  # newly associated
                                 db["files"][uri] = local["files"][uri]
                                 db["user_defined"][att] = local["user_defined"][att]
                             elif local["user_defined"][att] > db["user_defined"][att]:
                                 # last changed locally
                                 db["files"][uri] = local["files"][uri]
                                 db["user_defined"][att] = local["user_defined"][att]
                         else:
                             name = att[:-14]
                             if name not in local["data"]:  # we deleted it
                                 if name in db["data"]:
-                                    del(db["data"][name])
+                                    del db["data"][name]
                             elif local["user_defined"][att] > db["user_defined"][att]:
                                 db["data"][name] = local["data"][name]
                                 db["user_defined"][att] = local["user_defined"][att]
                 if db is not None:
                     update_records.append(db)
                 else:  # db did not have that key and returned None (no error)
                     update_records.append(local)
@@ -1039,18 +1113,18 @@
         relationships.insert(rels)
         for key in list(keys):
             try:
                 self._added_unsync_mem_store.records.delete(key)
             except Exception:
                 pass
             try:
-                del(self.__sync__dict__[key])
+                del self.__sync__dict__[key]
             except Exception:
                 # probably coming from del then
-                del(self.__sync__deleted__[key])
+                del self.__sync__deleted__[key]
 
     def add_user(self, username, groups=[]):
         """add_user adds a user to the Kosh store
 
         :param username: username to add
         :type username: str
         :param groups: kosh specific groups to add to this user
@@ -1299,24 +1373,22 @@
                     merged_attributes = merge_handler(
                         match, atts, "data", **merge_handler_kargs)
                     # Ok at this point no conflict!
                     match.update(merged_attributes)
                     match_rec = match.get_record()
                     remapped[record["id"]] = match_rec.id
                 else:  # Non existent dataset
-                    cont = True
-                    while cont:
-                        try:
-                            self.__record_handler__.get(record["id"])
-                            # Ok this record already exists
-                            # and we need a new unique one
-                            record["id"] = uuid.uuid4().hex
-                        except ValueError:
-                            # Does not exists, let's keep the id
-                            cont = False
+                    try:
+                        self.__record_handler__.get(record["id"])
+                        # Ok this record already exists
+                        # and we need a new unique one
+                        record["id"] = uuid.uuid4().hex
+                    except (KeyError, ValueError):
+                        # Does not exists, let's keep the id
+                        pass
                     match_rec = record
             else:  # ok it is a source
                 # Let's find the source rec that match this uri
                 current_sources = list(
                     self.find(
                         types=[self._sources_type, ],
                         uri=data["uri"]["value"],
@@ -1325,22 +1397,24 @@
                     match = self._load(current_sources[0])
                     if match.id != record["id"]:
                         # Darn this store already associated this uri
                         if match.mime_type != data["mime_type"]["value"]:
                             raise ValueError("trying to import an associated source {} with mime_type {} but "  # noqa
                                              "this store already associated"  # noqa
                                              " this source with mime_type {}".format(data["uri"]["value"],
-                                                                                     data["mime_type"["value"],
-                                                                                     match.mime_type]))
+                                                                                     data["mime_type"]["value"],
+                                                                                     match.mime_type))
                     match_rec = match.get_record()
                 else:
                     match_rec = record
             # update the record
             # But first make sure it is a record :)
             if isinstance(match_rec, dict):
+                if 'id' not in match_rec:
+                    match_rec['id'] = uuid.uuid4().hex
                 match_rec = sina.model.generate_record_from_json(match_rec)
 
             # User defined and files are preserved?
             for section in ["user_defined", "files", "library_data"]:
                 if section in record:
                     if match_rec.raw[section] != record[section] and record[section] != {
                     }:
@@ -1411,15 +1485,15 @@
                 if altered:
                     try:
                         self.__record_handler__.delete(rec["id"])
                     except ValueError:
                         pass
                     self.__record_handler__.insert(rec)
 
-        return [self._load(x) for x in matches]
+        return [self.open(x) for x in matches]
 
     def reassociate(self, target, source=None, absolute_path=True):
         """This function allows to re-associate data whose uri might have changed
 
         The source can be the original uri or sha and target is the new uri to use.
         :param target: New uri
         :type target: str
```

### Comparing `kosh-2.2/kosh/transformers/core.py` & `kosh-3.0/kosh/transformers/core.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/transformers/npy.py` & `kosh-3.0/kosh/transformers/npy.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/transformers/sidre.py` & `kosh-3.0/kosh/transformers/sidre.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/transformers/skl.py` & `kosh-3.0/kosh/transformers/skl.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/transformers/utils.py` & `kosh-3.0/kosh/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/kosh/utils.py` & `kosh-3.0/kosh/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,40 @@
 
 try:
     default_nx_layout = nx.planar_layout
 except AttributeError:  # planar is available from nx version 2.5
     default_nx_layout = nx.circular_layout
 
 
+def find_curveset_and_curve_name(name, rec):
+    """Given a curveset or curveset+curve name,
+    returns all matching curve_sets and curves combinations
+    Assumes curveset and curve are separated by a /
+    curve_sets that exactly match the name return (name, None)
+    :param name: Name to parse
+    :type name: str
+    :param rec: sina record where to look for curves
+    :type rec: sina record
+    :return: All possible combinations of (curveset,curve) that match name
+    :rtype: tuple of tuples
+    """
+    sp = name.split("/")
+    possibilities = ()
+    for i in range(len(sp)+1):
+        curve_set = "/".join(sp[:i])
+        if curve_set in rec["curve_sets"]:
+            cs = rec["curve_sets"][curve_set]
+            curve_name = "/".join(sp[i:])
+            if curve_name in cs["dependent"] or curve_name in cs["independent"]:
+                possibilities += ((curve_set, curve_name), )
+            if curve_set == name:  # ok we asked for the curve_set
+                possibilities += ((curve_set, None),)
+    return possibilities
+
+
 def merge_datasets_handler(target_dataset, imported_dataset, section="data", **kargs):
     """When importing a dataset, checks if the imported dataset has
     attributes that match the one in the dataset already in this store.
     If attributes values conflict then we use 'handling_method to resolve the conflict
 
     The store_dataset is not updated here, we return a list of attributes/values pairs resolving the conflict
 
@@ -86,15 +112,15 @@
             target_dict[attribute] = value
     return target_dict
 
 
 def gen_labels(G):
     """Generates labels to draw on networkx plots of a graph
     :param G: Network to generate labels from
-    :type G: networkx.OrderedDiGraph
+    :type G: networkx.DiGraph (OrderedDiGraph on older version of networkx)
     :returns: labels for this graph
     :rtype: dict
     """
     labels = {}
     cont = True
     nodes = list(G.nodes())
     N = len(nodes)
@@ -461,15 +487,18 @@
     :type transformers: list of KoshTransformer
     :returns: execution graph
     :rtype: networkx.OrderDiGraph
     """
     if input_type not in loader.types:
         raise RuntimeError(
             "loader cannot load mime_type {}".format(input_type))
-    G = nx.OrderedDiGraph()
+    try:
+        G = nx.OrderedDiGraph()
+    except AttributeError:  # networkx 3.0 removed OrderedDiGraph
+        G = nx.DiGraph()
     G.seed = random.random()
     start_node = (input_type, loader, G.seed)  # so each graph is unique
     G.add_node(start_node)
     if len(transformers) == 0:
         # No transformer
         for out_format in loader.types[input_type]:
             node = (out_format, None, G.seed)
```

### Comparing `kosh-2.2/kosh/wrapper.py` & `kosh-3.0/kosh/wrapper.py`

 * *Files identical despite different names*

### Comparing `kosh-2.2/scripts/kosh` & `kosh-3.0/scripts/kosh`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     if use_shell:
         if not sys.platform.startswith("win"):
             proc = Popen(shell, stdin=PIPE, stdout=PIPE, stderr=PIPE)
             o, e = proc.communicate(command.encode())
         else:
             proc = Popen(command, stdout=PIPE, stderr=PIPE, shell=True)
             o, e = proc.communicate()
-            print("COMMNAD:" , command)
+            print("COMMAND:" , command)
             print("OUT:", o.decode())
             print("ERR:", e.decode())
     else:
         if not sys.platform.startswith("win"):
             command = shlex.split(command)
         proc = Popen(command, stdout=PIPE, stderr=PIPE)
         o, e = proc.communicate()
@@ -332,34 +332,64 @@
                     print(ds)
                 for uri in missings:
                     associated = list(ds.find(uri=uri))
                     if len(associated) != 0:
                         print("{} (mime_type={}) is missing".format(
                             associated[0].uri, associated[0].mime_type))
 
+    def create_ensemble(self):
+        """create an ensemble into a Kosh store command"""
+        parser = core_parser(
+            prog="kosh create_ensemble",
+            description='Creates an ensemble into a store')
+        parser.add_argument(
+            "--id", "-i", help="Desired Id for dataset", default=None)
+        args, user_params = parser.parse_known_args(sys.argv[2:])
+        params = {}
+        index = 0
+        while index < len(user_params):
+            term = user_params[index]
+            sp = term.split("=")
+            if len(sp) > 1:
+                params[sp[0]] = eval(sp[1])
+                index += 1
+            else:
+                params[sp[0]] = eval(user_params[index+1])
+                index += 2
+
+        print("Adding ensemble to: {}".format(args.store))
+        store = kosh.connect(args.store)
+        store.create_ensemble(id=args.id, metadata=params)
+
     def add(self):
         """add a dataset to a Kosh store command"""
         parser = core_parser(
             prog="kosh add",
-            description='Adds a dataset to store')
+            description='Adds a dataset to a store and possibly an ensemble')
+        parser.add_argument(
+            "--ensemble", "-e", help="Id of the ensemble we want to add this to", default=None)
         parser.add_argument(
             "--id", "-i", help="Desired Id for dataset", default=None)
         args, metadata = parser.parse_known_args(sys.argv[2:])
         metadata = parse_metadata(metadata)
         store = kosh.KoshStore(
             db_uri=args.store, dataset_record_type=args.dataset_record_type)
         ds = store.create(id=args.id, metadata=metadata)
+        if args.ensemble is not None:
+            ensemble = next(store.find_ensembles(id=args.ensemble))
+            ensemble.add(ds)
+            print(ensemble)
         print(ds.id)
 
     def remove(self):
-        """Remove dataset(s) from store command"""
+        """Remove dataset(s) and or ensemble(s) from store command"""
         parser = core_parser(
             prog="kosh remove",
             description='Removes a dataset from store')
-        parser.add_argument("--ids", "-i", help="ids of datasets to print",
+        parser.add_argument("--ids", "-i", help="ids of datasets/ensembles to remove",
                             nargs="*", required=True, action="append")
         parser.add_argument("--force", "-f", action="store_true",
                             help="remove without asking for confirmation")
         args = parser.parse_args(sys.argv[2:])
         datasets = []
         for i in args.ids:
             datasets += i
@@ -455,17 +485,17 @@
             print(
                 "=======================================================================")
 
     def associate(self):
         """Associate uri with dataset command"""
         parser = core_parser(
             prog="kosh associate",
-            description="Associate a (set of) files with a dataset")
+            description="Associate a (set of) files with a dataset or ensemble")
         parser.add_argument(
-            "--id", "-i", help="id of datasets to which file(s) will be associated", required=True)
+            "--id", "-i", help="id of datasets/ensembles to which file(s) will be associated", required=True)
         parser.add_argument("--uri", "-u", help="uri(s) to associate with dataset",
                             nargs="*", required=True, action="append")
         parser.add_argument(
             "--mime_type", "-m", help="mime type of the uri(s) same for all", required=True)
         args = parser.parse_args(sys.argv[2:])
         uris = []
         for u in args.uri:
@@ -473,20 +503,20 @@
         store = kosh.KoshStore(
             db_uri=args.store, dataset_record_type=args.dataset_record_type)
         ds = store.open(args.id)
         for u in uris:
             ds.associate(u, mime_type=args.mime_type)
 
     def dissociate(self):
-        """dissociate uri from dataset command"""
+        """dissociate uri from dataset/ensemble command"""
         parser = core_parser(
             prog="kosh dissociate",
             description="dissociate a (set of) file(s) from a dataset")
         parser.add_argument(
-            "--id", "-i", help="id of datasets from which file(s) will be dissociated", required=True)
+            "--id", "-i", help="id of datasets/ensembles from which file(s) will be dissociated", required=True)
         parser.add_argument("--uri", "-u", help="uri(s) to dissociate from dataset",
                             nargs="*", required=True, action="append")
         args = parser.parse_args(sys.argv[2:])
         uris = []
         for u in args.uri:
             uris += u
         store = kosh.KoshStore(
@@ -912,14 +942,31 @@
         elif command in ["rm"]:
             cmd = "rm " + " ".join(opts)
         if command == "mv":
             # let's yank the source
             cmd += " --remove-source-files "
         rsync_ran = []
         for i, source in enumerate(sources):
+            # Now let's run the command and see if it worked
+            # But only if not ran for directory before
+            if os.path.dirname(source) + "/" not in sources[:i]:
+                skip_it = False
+                for ran in rsync_ran:
+                    if ran in source:
+                        skip_it = True
+                        break
+                if not skip_it:
+                    rsync_ran.append(source)
+                    cmd_run = cmd + " {} {}".format(source, targets[i])
+                    p, o, e = process_cmd(cmd_run)
+                    if p.returncode != 0:  # Failed!
+                        raise RuntimeError(
+                            "Error running command {}, aborting!\n{}".format(
+                                cmd_run, e.decode()))
+
             for o_store in origin_stores:
                 datasets = o_store.find(file=source)
                 for dataset in datasets:
                     if command == "mv":
                         associated_uris = dataset.find(uri=source)
                         for associated in associated_uris:
                             associated.uri = targets[i]
@@ -942,32 +989,14 @@
                             del(exported["records"][indx])
 
                         for d_store in dest_stores:
                             d_store.import_dataset(
                                 exported, args.dataset_matching_attributes,
                                 merge_handler=args.merge_strategy)
 
-            # Now let's run the command and see if it worked
-            # But only if not ran for directory before
-            if os.path.dirname(source) + "/" not in sources[:i]:
-                skip_it = False
-                for ran in rsync_ran:
-                    if ran in source:
-                        skip_it = True
-                        break
-                if skip_it:
-                    continue
-                rsync_ran.append(source)
-                cmd_run = cmd + " {} {}".format(source, targets[i])
-                p, o, e = process_cmd(cmd_run)
-                if p.returncode != 0:  # Failed!
-                    raise RuntimeError(
-                        "Error runnning command {}, aborting!\n{}".format(
-                            cmd_run, e.decode()))
-
             # Ok it's good let's sync the stores
             for store in origin_stores + dest_stores:
                 store.sync()
 
         # closes stores and send them back to remote if necessary
         close_stores(origin_stores, args.stores)
         close_stores(dest_stores, args.destination_stores)
@@ -1005,15 +1034,15 @@
                 params[sp[0]] = eval(sp[1])
                 index += 1
             else:
                 params[sp[0]] = eval(user_params[index+1])
                 index += 2
 
         print("Adding ds to: {}".format(args.store))
-        store = kosh.KoshStore(args.store)
+        store = kosh.connect(args.store)
         store.create(metadata=params)
 
 
 
 def is_remote(path):
     """Determine if a uri is located on a remote server
     First figures out if there is a ':' in the path (e.g user@host:/path)
```

### Comparing `kosh-2.2/scripts/sbang` & `kosh-3.0/scripts/sbang`

 * *Files identical despite different names*

### Comparing `kosh-2.2/setup.py` & `kosh-3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import shutil
 import os
 
 
 exec(open("./kosh/current_version.py").read())
 version = current_version  # noqa
 sha = None
+
 git_describe_process = Popen(
     ("git",
      "describe",
      "--tags"),
     stdout=PIPE,
     stderr=PIPE)
 try:
@@ -33,35 +34,41 @@
 if sha is not None:
     description += " (sha: {})".format(sha)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 if os.path.exists("scripts/kosh"):
     os.remove("scripts/kosh")
-print("WD:", os.getcwd())
-shutil.copyfile("/g/g19/cdoutrix/git/kosh/scripts/kosh_command.py", "scripts/kosh")
+shutil.copyfile("scripts/kosh_command.py", "scripts/kosh")
 setup(name="kosh",
       version=version,
       description=description,
       url="https://github.com/LLNL/Kosh",
-      author="Charles Doutriaux",
+      author="Charles Doutriaux, Renee Olson",
       author_email="doutriaux1@llnl.gov",
       long_description=long_description,
       long_description_content_type="text/markdown",
       license="MIT",
       packages=find_packages(),
       scripts=["scripts/kosh",
                "scripts/sbang",
                ],
       zip_safe=False,
       install_requires=[
           'llnl-sina >=1.11.0', 
-          'networkx',
-          'numpy',
+          'networkx>=2.6',
+          'numpy>=1.20',
+          'scipy',
+          'h5py>=3',
+          'scikit-learn>=1.0.2',
+          'pandas',
+          'hdbscan',
+          'matplotlib',
+          'tqdm'
       ],
       classifiers=[
           "Programming Language :: Python",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
       )
-Popen(("python", "scripts/render_logos.py",)).communicate()
+
```

