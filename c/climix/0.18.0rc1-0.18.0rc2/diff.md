# Comparing `tmp/climix-0.18.0rc1.tar.gz` & `tmp/climix-0.18.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climix-0.18.0rc1.tar", last modified: Fri Apr 21 15:44:54 2023, max compression
+gzip compressed data, was "climix-0.18.0rc2.tar", last modified: Fri Apr 21 17:20:58 2023, max compression
```

## Comparing `climix-0.18.0rc1.tar` & `climix-0.18.0rc2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.033679 climix-0.18.0rc1/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12135 2023-04-21 15:40:53.000000 climix-0.18.0rc1/CHANGELOG.md
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11357 2023-04-20 14:40:21.000000 climix-0.18.0rc1/LICENSE
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      136 2023-04-21 15:40:53.000000 climix-0.18.0rc1/MANIFEST.in
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 15:44:54.032679 climix-0.18.0rc1/PKG-INFO
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      487 2020-01-31 10:13:09.000000 climix-0.18.0rc1/README.md
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.010679 climix-0.18.0rc1/climix/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3759 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/aggregators.py
--rw-r--r--   0 a002160  (66459) smhiprimgrp  (2000)     5029 2023-04-04 13:04:32.000000 climix-0.18.0rc1/climix/dask_setup.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2552 2022-05-10 13:36:30.000000 climix-0.18.0rc1/climix/dask_take_along_axis.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    14730 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/datahandling.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.017679 climix-0.18.0rc1/climix/etc/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2300 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/etc/SMHI_extra.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5591 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/etc/climix_config.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)   107695 2023-04-21 14:07:50.000000 climix-0.18.0rc1/climix/etc/index_definitions.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     6964 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/etc/metadata.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2350 2023-04-21 14:07:50.000000 climix-0.18.0rc1/climix/etc/variables.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2449 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/index.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.019679 climix-0.18.0rc1/climix/index_functions/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      716 2023-04-19 14:56:21.000000 climix-0.18.0rc1/climix/index_functions/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    21861 2023-04-19 14:56:21.000000 climix-0.18.0rc1/climix/index_functions/index_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    18224 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/index_functions/percentile_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5197 2023-04-19 14:56:21.000000 climix-0.18.0rc1/climix/index_functions/spell_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11954 2023-04-19 14:56:21.000000 climix-0.18.0rc1/climix/index_functions/spell_kernels.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     9543 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/index_functions/support.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5426 2022-05-10 13:36:30.000000 climix-0.18.0rc1/climix/iris.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12580 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/main.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    17790 2023-04-20 14:40:21.000000 climix-0.18.0rc1/climix/metadata.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4911 2023-03-14 14:27:51.000000 climix-0.18.0rc1/climix/period.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.021679 climix-0.18.0rc1/climix/util/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      435 2023-02-08 09:48:44.000000 climix-0.18.0rc1/climix/util/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3949 2022-05-10 13:36:30.000000 climix-0.18.0rc1/climix/util/change_pr_units.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    13809 2023-03-14 14:27:51.000000 climix-0.18.0rc1/climix/util/cube_diffs.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.013679 climix-0.18.0rc1/climix.egg-info/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/PKG-INFO
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1495 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/SOURCES.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        1 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/dependency_links.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1531 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/entry_points.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/requires.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       13 2023-04-21 15:44:53.000000 climix-0.18.0rc1/climix.egg-info/top_level.txt
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.022679 climix-0.18.0rc1/docs/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      585 2023-03-30 14:33:33.000000 climix-0.18.0rc1/docs/Makefile
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      791 2019-07-03 09:39:58.000000 climix-0.18.0rc1/docs/make.bat
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       24 2023-04-21 14:45:55.000000 climix-0.18.0rc1/docs/requirements-docs.txt
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.023679 climix-0.18.0rc1/docs/source/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2704 2023-04-21 14:45:55.000000 climix-0.18.0rc1/docs/source/conf.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      446 2023-04-21 14:45:55.000000 climix-0.18.0rc1/docs/source/index.rst
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      546 2023-04-20 14:40:21.000000 climix-0.18.0rc1/environment.yml
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.024679 climix-0.18.0rc1/jobscripts/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      485 2022-12-08 14:42:09.000000 climix-0.18.0rc1/jobscripts/climix-mpi.sh
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3790 2022-12-08 14:42:09.000000 climix-0.18.0rc1/jobscripts/climix.sh
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3281 2023-04-20 14:40:21.000000 climix-0.18.0rc1/pyproject.toml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       38 2023-04-21 15:44:54.033679 climix-0.18.0rc1/setup.cfg
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.025679 climix-0.18.0rc1/tests/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc1/tests/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1130 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/conftest.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.027679 climix-0.18.0rc1/tests/integration/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/integration/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    10413 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/integration/configuration.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      779 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/integration/conftest.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4158 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/integration/test_indices.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.028679 climix-0.18.0rc1/tests/unit/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc1/tests/unit/__init__.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 15:44:54.031679 climix-0.18.0rc1/tests/unit/index_functions/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc1/tests/unit/index_functions/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2370 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/unit/index_functions/conftest.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    70106 2023-04-21 14:07:50.000000 climix-0.18.0rc1/tests/unit/index_functions/test_index_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3567 2023-03-14 14:27:51.000000 climix-0.18.0rc1/tests/unit/index_functions/test_percentile_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2353 2023-04-19 14:56:21.000000 climix-0.18.0rc1/tests/unit/index_functions/test_support.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2043 2023-03-14 14:27:51.000000 climix-0.18.0rc1/tests/unit/test_main.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.142170 climix-0.18.0rc2/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12135 2023-04-21 17:20:00.000000 climix-0.18.0rc2/CHANGELOG.md
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11357 2023-04-20 14:40:21.000000 climix-0.18.0rc2/LICENSE
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      136 2023-04-21 15:55:28.000000 climix-0.18.0rc2/MANIFEST.in
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 17:20:58.142170 climix-0.18.0rc2/PKG-INFO
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      487 2020-01-31 10:13:09.000000 climix-0.18.0rc2/README.md
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.111170 climix-0.18.0rc2/climix/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3759 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/aggregators.py
+-rw-r--r--   0 a002160  (66459) smhiprimgrp  (2000)     5029 2023-04-04 13:04:32.000000 climix-0.18.0rc2/climix/dask_setup.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2552 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/dask_take_along_axis.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    14730 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/datahandling.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.122170 climix-0.18.0rc2/climix/etc/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2300 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/SMHI_extra.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5591 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/climix_config.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)   107695 2023-04-21 14:07:50.000000 climix-0.18.0rc2/climix/etc/index_definitions.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     6964 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/metadata.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2350 2023-04-21 14:07:50.000000 climix-0.18.0rc2/climix/etc/variables.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2449 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.125170 climix-0.18.0rc2/climix/index_functions/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      716 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    21861 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/index_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    18224 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index_functions/percentile_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5197 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/spell_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11954 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/spell_kernels.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     9543 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index_functions/support.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5426 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/iris.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12580 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/main.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    17790 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/metadata.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4911 2023-03-14 14:27:51.000000 climix-0.18.0rc2/climix/period.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.128170 climix-0.18.0rc2/climix/util/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      435 2023-02-08 09:48:44.000000 climix-0.18.0rc2/climix/util/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3949 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/util/change_pr_units.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    13809 2023-03-14 14:27:51.000000 climix-0.18.0rc2/climix/util/cube_diffs.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.117170 climix-0.18.0rc2/climix.egg-info/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/PKG-INFO
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1495 2023-04-21 17:20:58.000000 climix-0.18.0rc2/climix.egg-info/SOURCES.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        1 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/dependency_links.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1488 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/entry_points.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/requires.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       13 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/top_level.txt
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.131170 climix-0.18.0rc2/docs/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      585 2023-03-30 14:33:33.000000 climix-0.18.0rc2/docs/Makefile
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      791 2019-07-03 09:39:58.000000 climix-0.18.0rc2/docs/make.bat
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       24 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/requirements-docs.txt
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.132170 climix-0.18.0rc2/docs/source/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2704 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/source/conf.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      446 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/source/index.rst
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      546 2023-04-20 14:40:21.000000 climix-0.18.0rc2/environment.yml
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.134170 climix-0.18.0rc2/jobscripts/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      485 2022-12-08 14:42:09.000000 climix-0.18.0rc2/jobscripts/climix-mpi.sh
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3790 2022-12-08 14:42:09.000000 climix-0.18.0rc2/jobscripts/climix.sh
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3236 2023-04-21 17:20:00.000000 climix-0.18.0rc2/pyproject.toml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       38 2023-04-21 17:20:58.142170 climix-0.18.0rc2/setup.cfg
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.135170 climix-0.18.0rc2/tests/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1130 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/conftest.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.137170 climix-0.18.0rc2/tests/integration/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    10413 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/configuration.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      779 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/conftest.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4158 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/test_indices.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.138170 climix-0.18.0rc2/tests/unit/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/unit/__init__.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.141170 climix-0.18.0rc2/tests/unit/index_functions/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/unit/index_functions/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2370 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/unit/index_functions/conftest.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    70106 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/unit/index_functions/test_index_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3567 2023-03-14 14:27:51.000000 climix-0.18.0rc2/tests/unit/index_functions/test_percentile_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2353 2023-04-19 14:56:21.000000 climix-0.18.0rc2/tests/unit/index_functions/test_support.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2043 2023-03-14 14:27:51.000000 climix-0.18.0rc2/tests/unit/test_main.py
```

### Comparing `climix-0.18.0rc1/CHANGELOG.md` & `climix-0.18.0rc2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ### Removed
 
 ### Fixed
 
 ### Security
 
 
-## [0.18.0rc1] - 2023-04-21
+## [0.18.0rc2] - 2023-04-21
 
 ### Added
 - Reference period defined in Index_definition.yml and command line arg -r/-reference_period (fixes #273)
 - Adds global metadata configuration (fixes #36)
 - Adds unit tests for index functions(fixes #299)
 - Read Clix meta version and add information in cube output attribute (fixes #284)
 - Adding integration tests using a subset of indices in NGCD dataset (fixes #275)
@@ -426,16 +426,16 @@
 - Improved directory structure.
 
 ### Removed
 
 - Removed obsolete version.
 
 
-[unreleased]: https://git.smhi.se/climix/climix/compare/0.18.0rc1...HEAD
-[0.18.0rc1]: https://git.smhi.se/climix/climix/compare/0.17.0...0.18.0rc1
+[unreleased]: https://git.smhi.se/climix/climix/compare/0.18.0rc2...HEAD
+[0.18.0rc2]: https://git.smhi.se/climix/climix/compare/0.17.0...0.18.0rc2
 [0.17.0]: https://git.smhi.se/climix/climix/compare/0.16.0...0.17.0
 [0.16.0]: https://git.smhi.se/climix/climix/compare/0.15.0...0.16.0
 [0.15.0]: https://git.smhi.se/climix/climix/compare/0.14.0...0.15.0
 [0.14.0]: https://git.smhi.se/climix/climix/compare/0.13.2...0.14.0
 [0.13.2]: https://git.smhi.se/climix/climix/compare/0.13.1...0.13.2
 [0.13.1]: https://git.smhi.se/climix/climix/compare/0.13.0...0.13.1
 [0.13.0]: https://git.smhi.se/climix/climix/compare/0.12.0...0.13.0
```

### Comparing `climix-0.18.0rc1/LICENSE` & `climix-0.18.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/PKG-INFO` & `climix-0.18.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climix
-Version: 0.18.0rc1
+Version: 0.18.0rc2
 Summary: A climate index package
 Author-email: Lars Bärring <lars.barring@smhi.se>, Klaus Zimmermann <klaus.zimmermann@smhi.se>
 License: Apache-2.0
 Project-URL: Homepage, https://git.smhi.se/climix/climix
 Project-URL: Bug Reports, https://git.smhi.se/climix/climix/issues
 Project-URL: Source, https://git.smhi.se/climix/climix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `climix-0.18.0rc1/climix/aggregators.py` & `climix-0.18.0rc2/climix/aggregators.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/dask_setup.py` & `climix-0.18.0rc2/climix/dask_setup.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/dask_take_along_axis.py` & `climix-0.18.0rc2/climix/dask_take_along_axis.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/datahandling.py` & `climix-0.18.0rc2/climix/datahandling.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/etc/SMHI_extra.yml` & `climix-0.18.0rc2/climix/etc/SMHI_extra.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/etc/climix_config.yml` & `climix-0.18.0rc2/climix/etc/climix_config.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/etc/index_definitions.yml` & `climix-0.18.0rc2/climix/etc/index_definitions.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/etc/metadata.yml` & `climix-0.18.0rc2/climix/etc/metadata.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/etc/variables.yml` & `climix-0.18.0rc2/climix/etc/variables.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index.py` & `climix-0.18.0rc2/climix/index.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/__init__.py` & `climix-0.18.0rc2/climix/index_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/index_functions.py` & `climix-0.18.0rc2/climix/index_functions/index_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/percentile_functions.py` & `climix-0.18.0rc2/climix/index_functions/percentile_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/spell_functions.py` & `climix-0.18.0rc2/climix/index_functions/spell_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/spell_kernels.py` & `climix-0.18.0rc2/climix/index_functions/spell_kernels.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/index_functions/support.py` & `climix-0.18.0rc2/climix/index_functions/support.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/iris.py` & `climix-0.18.0rc2/climix/iris.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/main.py` & `climix-0.18.0rc2/climix/main.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/metadata.py` & `climix-0.18.0rc2/climix/metadata.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/period.py` & `climix-0.18.0rc2/climix/period.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/util/change_pr_units.py` & `climix-0.18.0rc2/climix/util/change_pr_units.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix/util/cube_diffs.py` & `climix-0.18.0rc2/climix/util/cube_diffs.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix.egg-info/PKG-INFO` & `climix-0.18.0rc2/climix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climix
-Version: 0.18.0rc1
+Version: 0.18.0rc2
 Summary: A climate index package
 Author-email: Lars Bärring <lars.barring@smhi.se>, Klaus Zimmermann <klaus.zimmermann@smhi.se>
 License: Apache-2.0
 Project-URL: Homepage, https://git.smhi.se/climix/climix
 Project-URL: Bug Reports, https://git.smhi.se/climix/climix/issues
 Project-URL: Source, https://git.smhi.se/climix/climix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `climix-0.18.0rc1/climix.egg-info/SOURCES.txt` & `climix-0.18.0rc2/climix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/climix.egg-info/entry_points.txt` & `climix-0.18.0rc2/climix.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,8 +18,7 @@
 temperature_sum = climix.index_functions:TemperatureSum
 thresholded_percentile = climix.index_functions:ThresholdedPercentile
 thresholded_running_statistics = climix.index_functions:ThresholdedRunningStatistics
 thresholded_statistics = climix.index_functions:ThresholdedStatistics
 
 [console_scripts]
 climix = climix.main:main
-climix-index-docs = climix.index_docs:main
```

### Comparing `climix-0.18.0rc1/docs/Makefile` & `climix-0.18.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/docs/make.bat` & `climix-0.18.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/docs/source/conf.py` & `climix-0.18.0rc2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/environment.yml` & `climix-0.18.0rc2/environment.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/jobscripts/climix.sh` & `climix-0.18.0rc2/jobscripts/climix.sh`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/pyproject.toml` & `climix-0.18.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 [project.urls]
 Homepage = "https://git.smhi.se/climix/climix"
 "Bug Reports" = "https://git.smhi.se/climix/climix/issues"
 Source = "https://git.smhi.se/climix/climix"
 
 [project.scripts]
 climix = "climix.main:main"
-climix-index-docs = "climix.index_docs:main"
 
 [project.entry-points."climix.index_functions"]
 count_level_crossings = "climix.index_functions:CountLevelCrossings"
 count_occurrences = "climix.index_functions:CountOccurrences"
 count_percentile_occurrences = "climix.index_functions:CountPercentileOccurrences"
 count_thresholded_percentile_occurrences = "climix.index_functions:CountThresholdedPercentileOccurrences"
 count_joint_occurrences_precipitation_temperature = "climix.index_functions:CountJointOccurrencesPrecipitationTemperature"
```

### Comparing `climix-0.18.0rc1/tests/conftest.py` & `climix-0.18.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/integration/configuration.yml` & `climix-0.18.0rc2/tests/integration/configuration.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/integration/conftest.py` & `climix-0.18.0rc2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/integration/test_indices.py` & `climix-0.18.0rc2/tests/integration/test_indices.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/unit/index_functions/conftest.py` & `climix-0.18.0rc2/tests/unit/index_functions/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/unit/index_functions/test_index_functions.py` & `climix-0.18.0rc2/tests/unit/index_functions/test_index_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/unit/index_functions/test_percentile_functions.py` & `climix-0.18.0rc2/tests/unit/index_functions/test_percentile_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/unit/index_functions/test_support.py` & `climix-0.18.0rc2/tests/unit/index_functions/test_support.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc1/tests/unit/test_main.py` & `climix-0.18.0rc2/tests/unit/test_main.py`

 * *Files identical despite different names*

