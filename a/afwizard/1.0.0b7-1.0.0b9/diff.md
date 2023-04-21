# Comparing `tmp/afwizard-1.0.0b7.tar.gz` & `tmp/afwizard-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afwizard-1.0.0b7.tar", last modified: Wed Jun 15 14:17:45 2022, max compression
+gzip compressed data, was "afwizard-1.0.0b9.tar", last modified: Mon Sep  5 08:46:42 2022, max compression
```

## Comparing `afwizard-1.0.0b7.tar` & `afwizard-1.0.0b9.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.022799 afwizard-1.0.0b7/
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6328 2022-06-15 14:17:45.022799 afwizard-1.0.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.018799 afwizard-1.0.0b7/afwizard/
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46363 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/asprs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17980 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)    20176 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.018799 afwizard-1.0.0b7/afwizard/jupyter/
--rw-r--r--   0 runner    (1001) docker     (121)    10588 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    10452 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/filtering.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9864 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/libraries.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/python.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/segmentation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/jupyter/selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/lastools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/library.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    12042 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/opals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7786 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/pdal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.022799 afwizard-1.0.0b7/afwizard/schema/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/filter.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/lastools.json
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/library.json
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/opals.json
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/opals_nightly.json
--rw-r--r--   0 runner    (1001) docker     (121)     7969 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/pdal.json
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/pipeline.json
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/rasterize.json
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/segment_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/variability.json
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/schema/visualization.json
--rw-r--r--   0 runner    (1001) docker     (121)    25060 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/versioning.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)    12345 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/afwizard/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.018799 afwizard-1.0.0b7/afwizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6328 2022-06-15 14:17:44.000000 afwizard-1.0.0b7/afwizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-06-15 14:17:45.000000 afwizard-1.0.0b7/afwizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:17:44.000000 afwizard-1.0.0b7/afwizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-06-15 14:17:44.000000 afwizard-1.0.0b7/afwizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-06-15 14:17:44.000000 afwizard-1.0.0b7/afwizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-15 14:17:44.000000 afwizard-1.0.0b7/afwizard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-15 14:17:45.022799 afwizard-1.0.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:45.022799 afwizard-1.0.0b7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5393 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_asprs.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_lastools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_library.py
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_opals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_pdal.py
--rw-r--r--   0 runner    (1001) docker     (121)     8549 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-06-15 14:17:43.000000 afwizard-1.0.0b7/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.364983 afwizard-1.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-09-05 08:46:42.364983 afwizard-1.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5854 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.360983 afwizard-1.0.0b9/afwizard/
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46363 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/asprs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.360983 afwizard-1.0.0b9/afwizard/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/data/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17980 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/execute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20176 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.360983 afwizard-1.0.0b9/afwizard/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (121)    10588 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    10452 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/filtering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     9864 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/libraries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/segmentation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/jupyter/selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/lastools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/library.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11949 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/opals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7679 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/pdal.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.364983 afwizard-1.0.0b9/afwizard/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/filter.json
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/lastools.json
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/library.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7415 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/opals.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7969 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/pdal.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/rasterize.json
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/segment_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/variability.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/schema/visualization.json
+-rw-r--r--   0 runner    (1001) docker     (121)    25060 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2671 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12345 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/afwizard/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.360983 afwizard-1.0.0b9/afwizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-05 08:46:42.000000 afwizard-1.0.0b9/afwizard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-09-05 08:46:42.364983 afwizard-1.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:42.364983 afwizard-1.0.0b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5393 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_asprs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_lastools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_opals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_pdal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8549 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-05 08:46:40.000000 afwizard-1.0.0b9/tests/test_widgets.py
```

### Comparing `afwizard-1.0.0b7/LICENSE.md` & `afwizard-1.0.0b9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/PKG-INFO` & `afwizard-1.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: afwizard
-Version: 1.0.0b7
+Version: 1.0.0b9
 Summary: Adaptive Filtering Wizard
-Home-page: UNKNOWN
 Author: Dominic Kempf
 Author-email: ssc@iwr.uni-heidelberg.de
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Welcome to the Adaptive Filtering Wizard
@@ -52,15 +50,15 @@
 
 In order to work with AFwizard, you need the following required pieces of Software.
 
 * A [Conda installation](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)
 
 If you want to use the respective backends, you also need to install the following pieces of software:
 
-* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in the latest (nightly) version that contains the `TerrainFilter` module.
+* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in version 2.5
 * [LASTools](https://rapidlasso.com/)
 
 ## Installing and using
 
 ### Using Conda
 
 Having a [local installation of Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html), the following sequence of commands sets up a new Conda environment and installs `afwizard` into it:
@@ -129,9 +127,7 @@
 * Search through the [GitHub issue tracker](https://github.com/ssciwr/afwizard/issues)
 * Open a new issue on the [GitHub issue tracker](https://github.com/ssciwr/afwizard/issues) providing
   * The version of `afwizard` used
   * Information about your OS
   * The output of `conda list` on your machine
   * As much information as possible about how to reproduce the bug
   * If you can share the data that produced the error, it is much appreciated.
-
-
```

### Comparing `afwizard-1.0.0b7/README.md` & `afwizard-1.0.0b9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 In order to work with AFwizard, you need the following required pieces of Software.
 
 * A [Conda installation](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)
 
 If you want to use the respective backends, you also need to install the following pieces of software:
 
-* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in the latest (nightly) version that contains the `TerrainFilter` module.
+* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in version 2.5
 * [LASTools](https://rapidlasso.com/)
 
 ## Installing and using
 
 ### Using Conda
 
 Having a [local installation of Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html), the following sequence of commands sets up a new Conda environment and installs `afwizard` into it:
```

### Comparing `afwizard-1.0.0b7/afwizard/__init__.py` & `afwizard-1.0.0b9/afwizard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is the single source of truth
-__version__ = "1.0.0b7"
+__version__ = "1.0.0b9"
 
 # Ensure inclusion of the logging configuration
 import afwizard.logger
 
 # Make sure to import modules that register filter backends
 import afwizard.lastools
 import afwizard.opals
```

### Comparing `afwizard-1.0.0b7/afwizard/__main__.py` & `afwizard-1.0.0b9/afwizard/__main__.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/apps.py` & `afwizard-1.0.0b9/afwizard/apps.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/asprs.py` & `afwizard-1.0.0b9/afwizard/asprs.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/dataset.py` & `afwizard-1.0.0b9/afwizard/dataset.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/execute.py` & `afwizard-1.0.0b9/afwizard/execute.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/filter.py` & `afwizard-1.0.0b9/afwizard/filter.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/datasets.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/datasets.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/filtering.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/filtering.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/libraries.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/libraries.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/python.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/python.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/segmentation.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/segmentation.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/jupyter/selection.ipynb` & `afwizard-1.0.0b9/afwizard/jupyter/selection.ipynb`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/lastools.py` & `afwizard-1.0.0b9/afwizard/lastools.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/library.py` & `afwizard-1.0.0b9/afwizard/library.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/logger.py` & `afwizard-1.0.0b9/afwizard/logger.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/opals.py` & `afwizard-1.0.0b9/afwizard/opals.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,26 @@
 import xmltodict
 
 logger = logging.getLogger("afwizard")
 
 _opals_directory = None
 
 
+def parse_opals_version(dir):
+    try:
+        with open(os.path.join(dir, "version.txt")) as f:
+            for line in f:
+                match = re.match('OPALS_VERSION="?(.*)"?', line)
+                if match:
+                    parts = match.groups()[0].split(".")
+                    return int(parts[0]), int(parts[1])
+    except FileNotFoundError:
+        return None
+
+
 def set_opals_directory(dir):
     """Set custom OPALS installation directory
 
     Use this function at the beginning of your code to point AFwizard
     to a custom OPALS installation directory. Alternatively, you can use the
     environment variable :code:`OPALS_DIR` to do so.
 
@@ -37,19 +49,22 @@
     """
     # Globally store the given path
     global _opals_directory
     _opals_directory = dir
 
     # Validate the given directory if it is not None
     if dir is not None:
-        try:
-            get_opals_module_executable("RobFilter", base=dir)
-        except AFwizardError:
-            _opals_directory = None
-            raise AFwizardError(f"Path {dir} does not contain an OPALS installation!")
+        # Parse the version string and check it being 2.5
+        version = parse_opals_version(dir)
+        if version is not None:
+            if version[0] == 2 and version[1] == 5:
+                return
+
+        _opals_directory = None
+        raise AFwizardError(f"Path {dir} does not contain an OPALS v2.5 installation!")
 
 
 def get_opals_directory():
     """Find the OPALS directory specified by the user"""
     global _opals_directory
 
     # Maybe set the directory from an environment variable
@@ -291,31 +306,14 @@
         return schema
 
     @classmethod
     def enabled(cls):
         return opals_is_present()
 
 
-class OPALSNightlyFilter(OPALSFilter, identifier="opals_nightly", backend=True):
-    @classmethod
-    def schema(cls):
-        return load_schema("opals_nightly.json")
-
-    @classmethod
-    def enabled(cls):
-        # We identify the OPALS nightly installation by the existence
-        # of the TerrainFilter module. My OPALS tarball contains an outdated
-        # version file, so that cannot be used as a version source
-        try:
-            get_opals_module_executable("TerrainFilter")
-            return True
-        except AFwizardError:
-            return False
-
-
 class OPALSDataManagerObject(DataSet):
     @classmethod
     def convert(cls, dataset):
         # Idempotency of the conversion
         if isinstance(dataset, OPALSDataManagerObject):
             return dataset
```

### Comparing `afwizard-1.0.0b7/afwizard/paths.py` & `afwizard-1.0.0b9/afwizard/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import click
 import contextlib
 import functools
 import glob
-import hashlib
 import json
 import os
 import platform
-import requests
+import pooch
 import shutil
-import tarfile
 import tempfile
 import uuid
 import xdg
 
 from afwizard.utils import AFwizardError
 
 # Storage for the temporary workspace directory
 _tmp_dir = None
 
 # Storage for the data directory that will be used to resolve relative paths
 _data_dir = None
 
-# The current data archive URL
-TEST_DATA_ARCHIVE = "https://github.com/ssciwr/afwizard-test-data/releases/download/2022-06-09/data.tar.gz"
-TEST_DATA_CHECKSUM = "fae90a3cf758e2346b81fa0e3b005f2914d059ca182202a1de8f627b1ec0c160"
+# Create a pooch for our sample data from HeiData
+nakadake_data = pooch.create(
+    path=pooch.os_cache("afwizard"),
+    base_url="https://heidata.uni-heidelberg.de/api/access/datafile/:persistentId?persistentId=doi:10.11588/data/TJNQZG/",
+    env="AFWIZARD_CACHE_DIR",
+)
+nakadake_data.load_registry(
+    os.path.join(os.path.split(__file__)[0], "data", "registry.txt")
+)
 
 
 def set_data_directory(directory, create_dir=False):
     """Set a custom root directory to locate data files
 
     :param directory:
         The name of the custom data directory.
@@ -88,34 +92,25 @@
     """
     return os.path.join(get_temporary_workspace(), f"{uuid.uuid4()}.{extension}")
 
 
 def download_test_file(filename):
     """Ensure the existence of a dataset file by downloading it"""
 
-    # We download test data to the temporary workspce
-    testdata_dir = os.path.join(get_temporary_workspace(), "data")
-
-    # If we have not done that already, we do so now
-    if not os.path.exists(testdata_dir):
-        archive = requests.get(TEST_DATA_ARCHIVE).content
-        checksum = hashlib.sha256(archive).hexdigest()
-        if checksum != TEST_DATA_CHECKSUM:
-            raise ValueError("Checksum for test data archive failed.")
-
-        archive_file = os.path.join(get_temporary_workspace(), "data.tar.gz")
-        with open(archive_file, "wb") as tar:
-            tar.write(archive)
-
-        with tarfile.open(archive_file, "r:gz") as tar:
-            tar.extractall(path=testdata_dir)
-
-    # Return the filename - it is only a candidate. If the given filename
-    # is not in the test data, the file will not exist.
-    return os.path.join(testdata_dir, filename)
+    # Maybe fetch and unpack the test data archive
+    filelist = pooch.retrieve(
+        url="https://github.com/ssciwr/afwizard-test-data/releases/download/2022-06-09/data.tar.gz",
+        known_hash="sha256:fae90a3cf758e2346b81fa0e3b005f2914d059ca182202a1de8f627b1ec0c160",
+        processor=pooch.Untar(),
+    )
+
+    # Find the file that matches the requested one
+    for fname in filelist:
+        if os.path.split(fname)[-1] == filename:
+            return fname
 
 
 def check_file_extension(filename, possible_values, default_value):
     name, ext = os.path.splitext(filename)
 
     if ext == "" or ext == ".":
         ext = default_value
@@ -166,16 +161,22 @@
     candidates.append(os.path.join(os.getcwd(), filename))
 
     # Use the XDG data directories
     if platform.system() in ["Linux", "Darwin"]:
         for xdg_dir in xdg.xdg_data_dirs():
             candidates.append(os.path.join(xdg_dir, filename))
 
+    # Maybe use the sample data
+    if filename in nakadake_data.registry:
+        candidates.append(nakadake_data.fetch(filename))
+
     # Use the test data directory
-    candidates.append(download_test_file(filename))
+    test_file = download_test_file(filename)
+    if test_file is not None:
+        candidates.append(test_file)
 
     # Iterate through the list to check for file existence
     for candidate in candidates:
         if os.path.exists(candidate):
             return candidate
 
     raise FileNotFoundError(
```

### Comparing `afwizard-1.0.0b7/afwizard/pdal.py` & `afwizard-1.0.0b9/afwizard/pdal.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/schema/lastools.json` & `afwizard-1.0.0b9/afwizard/schema/lastools.json`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/schema/opals.json` & `afwizard-1.0.0b9/afwizard/schema/visualization.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6166666666666667%*

 * *Differences: {"'anyOf'": "{2: {'properties': {replace: OrderedDict([('alg', OrderedDict([('default', 'Horn'), "*

 * *            "('description', 'The literature suggests Zevenbergen & Thorne to be more suited to "*

 * *            "smooth landscapes, whereas Horn’s formula to perform better on rougher terrain.'), "*

 * *            "('enum', ['Horn', 'ZevenbergenThorne']), ('title', 'Algorithm'), ('type', "*

 * *            "'string')])), ('altitude', OrderedDict([('default', 30), ('description', 'Altitude of "*

 * *            'the light, in  […]*

```diff
@@ -1,84 +1,119 @@
 {
     "anyOf": [
         {
             "additionalProperties": false,
             "properties": {
-                "_backend": {
-                    "const": "opals",
+                "alg": {
+                    "default": "Horn",
+                    "description": "The literature suggests Zevenbergen & Thorne to be more suited to smooth landscapes, whereas Horn\u2019s formula to perform better on rougher terrain.",
+                    "enum": [
+                        "Horn",
+                        "ZevenbergenThorne"
+                    ],
+                    "title": "Algorithm",
                     "type": "string"
                 },
-                "debugOutFile": {
-                    "description": "Outputs a xyz file containing all points classified as ground",
-                    "title": "debug ground points file",
-                    "type": "string"
+                "altitude": {
+                    "default": 30,
+                    "description": "Altitude of the light, in degrees. 90 if the light comes from above the DEM, 0 if it is raking light.",
+                    "maximum": 90,
+                    "minimum": 0,
+                    "title": "Angle Altitude (0 to 90 degrees)",
+                    "type": "number"
                 },
-                "filter": {
-                    "description": "If a filter string is specified, point classification is only carried out for the set points selected by the filter condition",
-                    "title": "(tree of )filter(s) to select search points",
-                    "type": "string"
+                "azimuth": {
+                    "default": 315,
+                    "description": "Azimuth of the light, in degrees. 0 if it comes from the top of the raster, 90 from the east, \u2026 The default value, 315, should rarely be changed as it is the value generally used to generate shaded maps.",
+                    "maximum": 360,
+                    "minimum": 0,
+                    "title": "Azimuth angle (0 to 360 degrees)",
+                    "type": "number"
                 },
-                "inFile": {
-                    "description": "The path to the opals datamanager whose point data are being classified",
-                    "title": "input ODM file",
+                "visualization_type": {
+                    "const": "hillshade",
                     "type": "string"
                 },
-                "interpolation": {
-                    "default": "plane",
-                    "description": "The interpolation methods are ordered by their polynomial degree. In case adapting is chosen, a suitable interpolator is determined by the module, Higher degree interpolation is only used, if lower degree surfaces are too rigid.",
+                "zFactor": {
+                    "default": 1.0,
+                    "description": "Vertical exaggeration used to pre-multiply the elevations",
+                    "minimum": 0.0,
+                    "title": "Vertical exaggeration:",
+                    "type": "number"
+                }
+            },
+            "required": [
+                "visualization_type"
+            ],
+            "title": "Hillshade Model",
+            "type": "object"
+        },
+        {
+            "additionalProperties": false,
+            "properties": {
+                "visualization_type": {
+                    "const": "slope",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "visualization_type"
+            ],
+            "title": "Slope Map",
+            "type": "object"
+        },
+        {
+            "additionalProperties": false,
+            "properties": {
+                "alg": {
+                    "default": "Horn",
+                    "description": "The literature suggests Zevenbergen & Thorne to be more suited to smooth landscapes, whereas Horn\u2019s formula to perform better on rougher terrain.",
                     "enum": [
-                        "plane",
-                        "paraboloid",
-                        "adapting"
+                        "Horn",
+                        "ZevenbergenThorne"
                     ],
-                    "title": "robust interpolation method",
+                    "title": "Algorithm",
                     "type": "string"
                 },
-                "maxIter": {
-                    "default": 100,
-                    "description": "Robust interpolation is performed iteratively. In each iteration the individual point weights are adapted based on the residuals (i.e. vertical distance between point and intermediate surface. The process of surface interpolation and re-weighting is repeated until the surface changes are below a threshold or the maximum number of iterations is reached.",
-                    "title": "maximum number of iterations",
-                    "type": "integer"
-                },
-                "maxSigma": {
-                    "default": 0.5,
-                    "description": "If the standard deviation of a unit observation of the robust interpolation (i.e. sigma_0 ) exceeds the specified value, the classification of the affected points remains unchanged.",
-                    "title": "maximum allowed sigma of interpolation",
+                "altitude": {
+                    "default": 30,
+                    "description": "Altitude of the light, in degrees. 90 if the light comes from above the DEM, 0 if it is raking light.",
+                    "maximum": 90,
+                    "minimum": 0,
+                    "title": "Angle Altitude (0 to 90 degrees)",
                     "type": "number"
                 },
-                "penetration": {
-                    "default": 20,
-                    "description": "The laser signal is partly or totally reflected at semi-transparent objects like vegetation. Therefore, not all laser pulses reach the ground. The penetration rate is used in the course of the robust interpolation for apriori estimating a reasonable initial course of the local surfaces",
-                    "title": "estimated penetration rate [%]",
-                    "type": "integer"
-                },
-                "robustWFAdpation": {
-                    "default": "adapting",
-                    "description": "The module supports different adaption functions",
-                    "title": "adaption of the robust weight function",
-                    "type": "string"
+                "azimuth": {
+                    "default": 315,
+                    "description": "Azimuth of the light, in degrees. 0 if it comes from the top of the raster, 90 from the east, \u2026 The default value, 315, should rarely be changed as it is the value generally used to generate shaded maps.",
+                    "maximum": 360,
+                    "minimum": 0,
+                    "title": "Azimuth angle (0 to 360 degrees)",
+                    "type": "number"
                 },
-                "searchRadius": {
-                    "default": 3,
-                    "description": "Only points within the given search radius are considered for the local robust interpolation.If the search area contains too few points for successful interpolation, the classification of the respective points remains unchanged.",
-                    "title": "search radius for point selection",
+                "blending_factor": {
+                    "default": 0.5,
+                    "maximum": 1.0,
+                    "minimum": 0.0,
+                    "title": "Blending factor",
                     "type": "number"
                 },
-                "sigmaApriori": {
-                    "default": "0.15",
-                    "description": "Either a constant accuracy representing all data points or a user-defined formula (using the generic filter syntax) may be applied. It is important thatthe a specified formula provide realistic accuracy values, otherwise therobust interpolation concept will not work properly.",
-                    "title": "a-priori sigma of points",
+                "visualization_type": {
+                    "const": "blended_hillshade_slope",
                     "type": "string"
                 },
-                "type": {
-                    "const": "RobFilter",
-                    "type": "string"
+                "zFactor": {
+                    "default": 1.0,
+                    "description": "Vertical exaggeration used to pre-multiply the elevations",
+                    "minimum": 0.0,
+                    "title": "Vertical exaggeration:",
+                    "type": "number"
                 }
             },
             "required": [
-                "type"
+                "visualization_type"
             ],
-            "title": "RobFilter Module (OPALS)",
+            "title": "Hillshade Model + Slope Map",
             "type": "object"
         }
     ]
 }
```

### Comparing `afwizard-1.0.0b7/afwizard/schema/pdal.json` & `afwizard-1.0.0b9/afwizard/schema/pdal.json`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/schema/pipeline.json` & `afwizard-1.0.0b9/afwizard/schema/pipeline.json`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/schema/rasterize.json` & `afwizard-1.0.0b9/afwizard/schema/rasterize.json`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/schema/variability.json` & `afwizard-1.0.0b9/afwizard/schema/variability.json`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/segmentation.py` & `afwizard-1.0.0b9/afwizard/segmentation.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/utils.py` & `afwizard-1.0.0b9/afwizard/utils.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/versioning.py` & `afwizard-1.0.0b9/afwizard/versioning.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 AFWIZARD_DATAMODEL_MAJOR_VERSION = 0
 
 # Define the current minor version of the filter data model defined by
 # adaptivefiltering. This number should be increased whenever there is a
 # change to the model e.g. the addition or renaming of metadata. When
 # increasing this number you should also add an upgrade function that allows
 # adaptivefiltering to port existing filters to the new minor version.
-AFWIZARD_DATAMODEL_MINOR_VERSION = 0
+AFWIZARD_DATAMODEL_MINOR_VERSION = 1
 
 # A global registry of update functions
 _upgrade_functions = {}
 
 
 def upgrade_function(major, minor):
     """A decorator to use to mark an upgrade function.
@@ -56,14 +56,22 @@
 
     return data
 
 
 #
 # In the following all upgrade functions to the afwizard data model are implemented.
 #
-# A potential first upgrade function could look like this:
-#
-# @upgrade_function(0, 0)
-# def add_keywords_field(config):
-#     config["keywords"] = []
-#     return config
-#
+
+
+@upgrade_function(0, 0)
+def remove_opals_nightly(config):
+    """Update function (0, 0) -> (0, 1)
+
+    The OPALS Nightly backend was a temporary solution to allow usage
+    of the TerrainFilter module. Starting with OPALS v2.5 it is part of
+    main OPALS. We do require that version.
+    """
+    for f in config["filters"]:
+        if f["_backend"] == "opals_nightly":
+            f["_backend"] = "opals"
+
+    return config
```

### Comparing `afwizard-1.0.0b7/afwizard/visualization.py` & `afwizard-1.0.0b9/afwizard/visualization.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard/widgets.py` & `afwizard-1.0.0b9/afwizard/widgets.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/afwizard.egg-info/PKG-INFO` & `afwizard-1.0.0b9/afwizard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: afwizard
-Version: 1.0.0b7
+Version: 1.0.0b9
 Summary: Adaptive Filtering Wizard
-Home-page: UNKNOWN
 Author: Dominic Kempf
 Author-email: ssc@iwr.uni-heidelberg.de
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Welcome to the Adaptive Filtering Wizard
@@ -52,15 +50,15 @@
 
 In order to work with AFwizard, you need the following required pieces of Software.
 
 * A [Conda installation](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)
 
 If you want to use the respective backends, you also need to install the following pieces of software:
 
-* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in the latest (nightly) version that contains the `TerrainFilter` module.
+* [OPALS](https://opals.geo.tuwien.ac.at/html/stable/index.html) in version 2.5
 * [LASTools](https://rapidlasso.com/)
 
 ## Installing and using
 
 ### Using Conda
 
 Having a [local installation of Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html), the following sequence of commands sets up a new Conda environment and installs `afwizard` into it:
@@ -129,9 +127,7 @@
 * Search through the [GitHub issue tracker](https://github.com/ssciwr/afwizard/issues)
 * Open a new issue on the [GitHub issue tracker](https://github.com/ssciwr/afwizard/issues) providing
   * The version of `afwizard` used
   * Information about your OS
   * The output of `conda list` on your machine
   * As much information as possible about how to reproduce the bug
   * If you can share the data that produced the error, it is much appreciated.
-
-
```

### Comparing `afwizard-1.0.0b7/afwizard.egg-info/SOURCES.txt` & `afwizard-1.0.0b9/afwizard.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 afwizard/widgets.py
 afwizard.egg-info/PKG-INFO
 afwizard.egg-info/SOURCES.txt
 afwizard.egg-info/dependency_links.txt
 afwizard.egg-info/entry_points.txt
 afwizard.egg-info/requires.txt
 afwizard.egg-info/top_level.txt
+afwizard/data/registry.txt
 afwizard/jupyter/datasets.ipynb
 afwizard/jupyter/filtering.ipynb
 afwizard/jupyter/libraries.ipynb
 afwizard/jupyter/python.ipynb
 afwizard/jupyter/segmentation.ipynb
 afwizard/jupyter/selection.ipynb
 afwizard/schema/filter.json
 afwizard/schema/lastools.json
 afwizard/schema/library.json
 afwizard/schema/opals.json
-afwizard/schema/opals_nightly.json
 afwizard/schema/pdal.json
 afwizard/schema/pipeline.json
 afwizard/schema/rasterize.json
 afwizard/schema/segment_metadata.json
 afwizard/schema/variability.json
 afwizard/schema/visualization.json
 tests/__init__.py
```

### Comparing `afwizard-1.0.0b7/setup.cfg` & `afwizard-1.0.0b9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 	Click
 	IPython
 	afwizard-library
 	gdal==3.4.0
 	geojson
 	ipyfilechooser
 	ipyleaflet
-	ipywidgets==8.0.0rc0
+	ipywidgets>=8
 	ipywidgets-jsonschema
 	jsonmerge
 	jsonschema<4
 	numpy
 	pdal
 	pillow
+	pooch
 	pyproj
 	pyrsistent
 	pytools
 	wrapt
 	xdg
 	xmltodict
 include_package_data = True
@@ -43,14 +44,15 @@
 	afwizard = afwizard.__main__:main
 	extract_opals_schema = afwizard.opals:_automated_opals_schema
 	upgrade_filter_library = afwizard.library:upgrade_filter_library
 	copy_afwizard_notebooks = afwizard.paths:copy_notebooks
 
 [options.package_data]
 * = 
+	data/*
 	schema/*
 	jupyter/*.ipynb
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `afwizard-1.0.0b7/tests/conftest.py` & `afwizard-1.0.0b9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_apps.py` & `afwizard-1.0.0b9/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_asprs.py` & `afwizard-1.0.0b9/tests/test_asprs.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_dataset.py` & `afwizard-1.0.0b9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_execute.py` & `afwizard-1.0.0b9/tests/test_execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from afwizard.dataset import DataSet
 from afwizard.execute import *
 from afwizard.filter import load_filter
 from afwizard.library import add_filter_library, metadata_hash
-from afwizard.paths import get_temporary_workspace
+from afwizard.paths import download_test_file, get_temporary_workspace
 from afwizard.pdal import PDALInMemoryDataSet
 from afwizard.utils import AFwizardError
 
 import os
 import pytest
 
 
@@ -14,15 +14,16 @@
     monkeypatch.chdir(tmp_path)
 
     # Apply without pipeline information in segmentation
     with pytest.raises(AFwizardError):
         apply_adaptive_pipeline(dataset=dataset, segmentation=dataset_seg)
 
     # Register the test data filter library
-    add_filter_library(os.path.join(get_temporary_workspace(), "data"))
+    pipeline_dir = os.path.split(download_test_file("testfilter1.json"))[0]
+    add_filter_library(pipeline_dir)
 
     # Patch pipeline information into the segementation
     for s in dataset_seg["features"]:
         mapping = {
             "A": "testfilter1.json",
             "B": "testfilter2.json",
             "C": "testfilter2.json",
```

### Comparing `afwizard-1.0.0b7/tests/test_filter.py` & `afwizard-1.0.0b9/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_lastools.py` & `afwizard-1.0.0b9/tests/test_lastools.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_library.py` & `afwizard-1.0.0b9/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_opals.py` & `afwizard-1.0.0b9/tests/test_opals.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_paths.py` & `afwizard-1.0.0b9/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_pdal.py` & `afwizard-1.0.0b9/tests/test_pdal.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_segmentation.py` & `afwizard-1.0.0b9/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `afwizard-1.0.0b7/tests/test_widgets.py` & `afwizard-1.0.0b9/tests/test_widgets.py`

 * *Files identical despite different names*

