# Comparing `tmp/mbGDML-0.0.4.tar.gz` & `tmp/mbGDML-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbGDML-0.0.4.tar", last modified: Mon Dec 12 18:01:00 2022, max compression
+gzip compressed data, was "mbGDML-0.1.0.tar", last modified: Fri Apr 21 03:33:57 2023, max compression
```

## Comparing `mbGDML-0.0.4.tar` & `mbGDML-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-12 18:00:50.000000 mbGDML-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-12 18:00:50.000000 mbGDML-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2022-12-12 18:00:50.000000 mbGDML-0.0.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2022-12-12 18:01:00.536899 mbGDML-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2022-12-12 18:00:50.000000 mbGDML-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.532899 mbGDML-0.0.4/mbGDML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-12 18:01:00.000000 mbGDML-0.0.4/mbGDML.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/_gdml/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/desc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/perm.py
--rw-r--r--   0 runner    (1001) docker     (123)    43138 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    37175 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/torchtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    61736 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/_gdml/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/alchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/analysis/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/analysis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/analysis/problematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/analysis/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/data/basedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/data/predictset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/interfaces/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    38176 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/mbe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/models/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/models/gap_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/models/gdml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/models/schnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:01:00.536899 mbGDML-0.0.4/mbgdml/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/predictors/gap_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/predictors/gdml_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/predictors/schnet_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    42793 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2022-12-12 18:00:50.000000 mbGDML-0.0.4/mbgdml/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2022-12-12 18:01:00.536899 mbGDML-0.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2022-12-12 18:00:50.000000 mbGDML-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2022-12-12 18:00:50.000000 mbGDML-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 03:33:41.000000 mbGDML-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 03:33:41.000000 mbGDML-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 03:33:41.000000 mbGDML-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-21 03:33:57.311221 mbGDML-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.303221 mbGDML-0.1.0/mbGDML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.315221 mbGDML-0.1.0/mbgdml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/_gdml/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20028 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43148 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/_gdml/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37575 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/torchtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56038 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 03:33:57.315221 mbGDML-0.1.0/mbgdml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/drive_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/sample_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/problematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/basedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/predictset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/interfaces/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47240 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/mbe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/gap_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/gdml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/schnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/gap_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/gdml_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/schnet_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/stress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/structure_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/packmol_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/switching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42748 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-21 03:33:57.311221 mbGDML-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-21 03:33:41.000000 mbGDML-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_mbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_packmol_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_predictsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_structure_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-21 03:33:41.000000 mbGDML-0.1.0/versioneer.py
```

### Comparing `mbGDML-0.0.4/LICENSE` & `mbGDML-0.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022, Alex M. Maldonado
+Copyright (c) 2020-2023, Alex M. Maldonado
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mbGDML-0.0.4/NOTICE` & `mbGDML-0.1.0/NOTICE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright for portions of mbGDML are held by Stefan Chmiela, 2018-2020, as part
 of sGDML (https://github.com/stefanch/sGDML). All other copyright for mbGDML are
-held by Alex M. Maldonado, 2020-2022.
+held by Alex M. Maldonado, 2020-2023.
 
 MIT License
 
 Copyright (c) 2018-2020, Stefan Chmiela
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `mbGDML-0.0.4/PKG-INFO` & `mbGDML-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbGDML
-Version: 0.0.4
+Version: 0.1.0
 Summary: Create, use, and analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML
 Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -52,16 +52,14 @@
     <a href="#motivation">Motivation</a> •
     <a href="#approach">Approach</a> •
     <a href="#features">Features</a>  •
     <a href="#installation">Installation</a>  •
     <a href="#license">License</a>
 </p>
 
-**Disclaimer**: This package is still under active development and not suitable for production.
-
 ## Motivation
 
 Machine learning potentials (i.e., force fields) often rely on local descriptors for size transferability.
 These descriptors partition total properties into atomic contributions; however, they inherently neglect complicated long-range interactions by enforcing atomic radial cutoffs.
 Global descriptors encode the entire structure with no cutoffs and can capture interactions at all scales.
 However, they are restricted to systems with the same number of atoms.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mbGDML Version: 0.0.4 Summary: Create, use, and
+Metadata-Version: 2.1 Name: mbGDML Version: 0.1.0 Summary: Create, use, and
 analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com License: MIT license Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
@@ -11,20 +11,19 @@
                              ****** mbGDML ******
  *** Create, use, and analyze machine learning potentials within the many-body
                            expansion framework. ***
                              *** Documentation ***
   [Build_Status_] [Codecov] [DOI] [License] [Repo_size] [Black_style] [Black
                                     style]
        Motivation â¢ Approach â¢ Features â¢ Installation â¢ License
-**Disclaimer**: This package is still under active development and not suitable
-for production. ## Motivation Machine learning potentials (i.e., force fields)
-often rely on local descriptors for size transferability. These descriptors
-partition total properties into atomic contributions; however, they inherently
-neglect complicated long-range interactions by enforcing atomic radial cutoffs.
-Global descriptors encode the entire structure with no cutoffs and can capture
+## Motivation Machine learning potentials (i.e., force fields) often rely on
+local descriptors for size transferability. These descriptors partition total
+properties into atomic contributions; however, they inherently neglect
+complicated long-range interactions by enforcing atomic radial cutoffs. Global
+descriptors encode the entire structure with no cutoffs and can capture
 interactions at all scales. However, they are restricted to systems with the
 same number of atoms. [https://github.com/keithgroup/mbGDML/blob/main/docs/
 source/images/descriptors/global-vs-local-descriptor.png?raw=true] [Gradient-
 domain machine learning](http://www.sgdml.org/) (GDML) is one example of a ML
 potential with a global descriptor. GDML is unique because it trains directly
 on forces and recovers total energy through analytical integration. This
 provides substantially more information about the potential energy surface
```

### Comparing `mbGDML-0.0.4/README.md` & `mbGDML-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     <a href="#motivation">Motivation</a> •
     <a href="#approach">Approach</a> •
     <a href="#features">Features</a>  •
     <a href="#installation">Installation</a>  •
     <a href="#license">License</a>
 </p>
 
-**Disclaimer**: This package is still under active development and not suitable for production.
-
 ## Motivation
 
 Machine learning potentials (i.e., force fields) often rely on local descriptors for size transferability.
 These descriptors partition total properties into atomic contributions; however, they inherently neglect complicated long-range interactions by enforcing atomic radial cutoffs.
 Global descriptors encode the entire structure with no cutoffs and can capture interactions at all scales.
 However, they are restricted to systems with the same number of atoms.
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
                              ****** mbGDML ******
  *** Create, use, and analyze machine learning potentials within the many-body
                            expansion framework. ***
                              *** Documentation ***
   [Build_Status_] [Codecov] [DOI] [License] [Repo_size] [Black_style] [Black
                                     style]
        Motivation â¢ Approach â¢ Features â¢ Installation â¢ License
-**Disclaimer**: This package is still under active development and not suitable
-for production. ## Motivation Machine learning potentials (i.e., force fields)
-often rely on local descriptors for size transferability. These descriptors
-partition total properties into atomic contributions; however, they inherently
-neglect complicated long-range interactions by enforcing atomic radial cutoffs.
-Global descriptors encode the entire structure with no cutoffs and can capture
+## Motivation Machine learning potentials (i.e., force fields) often rely on
+local descriptors for size transferability. These descriptors partition total
+properties into atomic contributions; however, they inherently neglect
+complicated long-range interactions by enforcing atomic radial cutoffs. Global
+descriptors encode the entire structure with no cutoffs and can capture
 interactions at all scales. However, they are restricted to systems with the
 same number of atoms. [https://github.com/keithgroup/mbGDML/blob/main/docs/
 source/images/descriptors/global-vs-local-descriptor.png?raw=true] [Gradient-
 domain machine learning](http://www.sgdml.org/) (GDML) is one example of a ML
 potential with a global descriptor. GDML is unique because it trains directly
 on forces and recovers total energy through analytical integration. This
 provides substantially more information about the potential energy surface
```

### Comparing `mbGDML-0.0.4/mbGDML.egg-info/PKG-INFO` & `mbGDML-0.1.0/mbGDML.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbGDML
-Version: 0.0.4
+Version: 0.1.0
 Summary: Create, use, and analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML
 Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -52,16 +52,14 @@
     <a href="#motivation">Motivation</a> •
     <a href="#approach">Approach</a> •
     <a href="#features">Features</a>  •
     <a href="#installation">Installation</a>  •
     <a href="#license">License</a>
 </p>
 
-**Disclaimer**: This package is still under active development and not suitable for production.
-
 ## Motivation
 
 Machine learning potentials (i.e., force fields) often rely on local descriptors for size transferability.
 These descriptors partition total properties into atomic contributions; however, they inherently neglect complicated long-range interactions by enforcing atomic radial cutoffs.
 Global descriptors encode the entire structure with no cutoffs and can capture interactions at all scales.
 However, they are restricted to systems with the same number of atoms.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mbGDML Version: 0.0.4 Summary: Create, use, and
+Metadata-Version: 2.1 Name: mbGDML Version: 0.1.0 Summary: Create, use, and
 analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com License: MIT license Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
@@ -11,20 +11,19 @@
                              ****** mbGDML ******
  *** Create, use, and analyze machine learning potentials within the many-body
                            expansion framework. ***
                              *** Documentation ***
   [Build_Status_] [Codecov] [DOI] [License] [Repo_size] [Black_style] [Black
                                     style]
        Motivation â¢ Approach â¢ Features â¢ Installation â¢ License
-**Disclaimer**: This package is still under active development and not suitable
-for production. ## Motivation Machine learning potentials (i.e., force fields)
-often rely on local descriptors for size transferability. These descriptors
-partition total properties into atomic contributions; however, they inherently
-neglect complicated long-range interactions by enforcing atomic radial cutoffs.
-Global descriptors encode the entire structure with no cutoffs and can capture
+## Motivation Machine learning potentials (i.e., force fields) often rely on
+local descriptors for size transferability. These descriptors partition total
+properties into atomic contributions; however, they inherently neglect
+complicated long-range interactions by enforcing atomic radial cutoffs. Global
+descriptors encode the entire structure with no cutoffs and can capture
 interactions at all scales. However, they are restricted to systems with the
 same number of atoms. [https://github.com/keithgroup/mbGDML/blob/main/docs/
 source/images/descriptors/global-vs-local-descriptor.png?raw=true] [Gradient-
 domain machine learning](http://www.sgdml.org/) (GDML) is one example of a ML
 potential with a global descriptor. GDML is unique because it trains directly
 on forces and recovers total energy through analytical integration. This
 provides substantially more information about the potential energy surface
```

### Comparing `mbGDML-0.0.4/mbGDML.egg-info/SOURCES.txt` & `mbGDML-0.1.0/mbGDML.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,23 +15,31 @@
 mbgdml/_version.py
 mbgdml/alchemy.py
 mbgdml/descriptors.py
 mbgdml/logger.py
 mbgdml/losses.py
 mbgdml/mbe.py
 mbgdml/periodic.py
+mbgdml/stress.py
+mbgdml/switching.py
 mbgdml/train.py
 mbgdml/utils.py
 mbgdml/_gdml/__init__.py
 mbgdml/_gdml/desc.py
 mbgdml/_gdml/perm.py
 mbgdml/_gdml/predict.py
 mbgdml/_gdml/sample.py
 mbgdml/_gdml/torchtools.py
 mbgdml/_gdml/train.py
+mbgdml/_gdml/solvers/__init__.py
+mbgdml/_gdml/solvers/analytic.py
+mbgdml/_gdml/solvers/iterative.py
+mbgdml/active_learning/__init__.py
+mbgdml/active_learning/drive_md.py
+mbgdml/active_learning/sample_md.py
 mbgdml/analysis/__init__.py
 mbgdml/analysis/clustering.py
 mbgdml/analysis/models.py
 mbgdml/analysis/problematic.py
 mbgdml/analysis/rdf.py
 mbgdml/data/__init__.py
 mbgdml/data/basedata.py
@@ -43,8 +51,21 @@
 mbgdml/models/base.py
 mbgdml/models/gap_model.py
 mbgdml/models/gdml_model.py
 mbgdml/models/schnet_model.py
 mbgdml/predictors/__init__.py
 mbgdml/predictors/gap_predict.py
 mbgdml/predictors/gdml_predict.py
-mbgdml/predictors/schnet_predict.py
+mbgdml/predictors/schnet_predict.py
+mbgdml/structure_gen/__init__.py
+mbgdml/structure_gen/packmol_gen.py
+mbgdml/structure_gen/utils.py
+tests/test_datasets.py
+tests/test_descriptors.py
+tests/test_mbe.py
+tests/test_packmol_gen.py
+tests/test_predict.py
+tests/test_predictsets.py
+tests/test_rdf.py
+tests/test_structure_gen_utils.py
+tests/test_train.py
+tests/test_utils.py
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/desc.py` & `mbGDML-0.1.0/mbgdml/_gdml/desc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2022 Stefan Chmiela, Luis Galvez
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,28 +19,28 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from functools import partial
 import multiprocessing as mp
-import logging
 import numpy as np
 import scipy as sp
+from ..logger import GDMLLogger
 
 try:
     import torch
 except ImportError:
     _HAS_TORCH = False
 else:
     _HAS_TORCH = True
 
 Pool = mp.get_context("fork").Pool
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def _pbc_diff(diffs, lat_and_inv, use_torch=False):
     r"""Clamp differences of vectors to super cell.
 
     Parameters
     ----------
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/perm.py` & `mbGDML-0.1.0/mbgdml/_gdml/perm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2021, Stefan Chmiela
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,27 +21,27 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import print_function
 
 import multiprocessing as mp
 from functools import partial
-import logging
 import numpy as np
 import scipy.optimize
 import scipy.spatial.distance
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import minimum_spanning_tree, connected_components
 from ase import Atoms
 from ase.geometry.analysis import Analysis
 from .desc import Desc, _pdist, _squareform
+from ..logger import GDMLLogger
 
 Pool = mp.get_context("fork").Pool
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 glob = {}
 
 
 def share_array(arr_np, typecode):
     arr = mp.RawArray(typecode, arr_np.ravel())
     return arr, arr_np.shape
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/predict.py` & `mbGDML-0.1.0/mbgdml/_gdml/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2022, Stefan Chmiela, Gregory Fonseca
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,23 +18,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import sys
-import logging
 import os
 import multiprocessing as mp
 import timeit
 from functools import partial
 import numpy as np
 import psutil
 
 from .. import __version__
+from ..logger import GDMLLogger
 from .desc import Desc
 
 try:
     import torch
 except ImportError:
     _HAS_TORCH = False
 else:
@@ -49,15 +49,15 @@
 try:
     _TORCH_CUDA_IS_AVAILABLE = torch.cuda.is_available()
 except (NameError, AttributeError):
     _TORCH_CUDA_IS_AVAILABLE = False
 
 Pool = mp.get_context("fork").Pool
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def share_array(arr_np):
     """
     Return a ctypes array allocated from shared memory with data from a
     NumPy array of type `float`.
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/sample.py` & `mbGDML-0.1.0/mbgdml/_gdml/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2020, Stefan Chmiela
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,14 +18,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 # pylint: disable-next=invalid-name
 def draw_strat_sample(T, n, excl_idxs=None):
     """
     Draw sample from dataset that preserves its original distribution.
 
     The distribution is estimated from a histogram were the bin size is
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/torchtools.py` & `mbGDML-0.1.0/mbgdml/_gdml/torchtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2019-2022, Stefan Chmiela, Jan Hermann
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -47,33 +47,32 @@
 _TORCH_MPS_IS_AVAILABLE = False
 
 try:
     _TORCH_CUDA_IS_AVAILABLE = torch.cuda.is_available()
 except (NameError, AttributeError):
     _TORCH_CUDA_IS_AVAILABLE = False
 
+import logging
+
+log = logging.getLogger(__name__)
+
 # pylint: disable=no-member
 
 _dtype = torch.float64
 
 
 def _next_batch_size(n_total, batch_size):
 
     batch_size += 1
     while n_total % batch_size != 0:
         batch_size += 1
 
     return batch_size
 
 
-import logging
-
-log = logging.getLogger(__name__)
-
-
 class GDMLTorchAssemble(nn.Module):
     """
     PyTorch version of the kernel assembly routines in :class:`~predict.GDMLTrain`.
     Derives from :class:`torch.nn.Module`. Contains no trainable parameters.
     """
 
     def __init__(
@@ -428,24 +427,22 @@
             (unit GB) Maximum allocated memory for prediction.
         """
 
         global _batch_size, _n_perm_batches
 
         super(GDMLTorchPredict, self).__init__()
 
-        log = logging.getLogger(__name__)
-
         model = dict(model)
 
         self._lat_and_inv = (
             None
             if lat_and_inv is None
             else (
-                torch.tensor(lat_and_inv[0]),
-                torch.tensor(lat_and_inv[1]),
+                torch.tensor(lat_and_inv[0], dtype=_dtype),
+                torch.tensor(lat_and_inv[1], dtype=_dtype),
             )
         )
 
         self.dim_d, self.n_train = model["R_desc"].shape[:2]
         self.dim_i = 3 * int((1 + np.sqrt(8 * self.dim_d + 1)) / 2)
         self.n_perms, self.n_atoms = model["perms"].shape
 
@@ -488,14 +485,22 @@
                         for i in range(torch.cuda.device_count())
                     ]
                 )
                 // 2**30
             )  # bytes to GB
         else:  # TODO: what about MPS?
             default_cpu_max_mem = 32
+            if max_memory is None:
+                pytorch_mem_limit = 2**30 * default_cpu_max_mem * 1e-9  # GB
+                log.info(
+                    "PyTorch CPU memory budget is limited to %.2f GB"
+                    " by default, which may impact performance",
+                    pytorch_mem_limit,
+                )
+                log.info("If necessary, adjust memory limit with option '-m'")
             max_memory = (
                 max_memory or default_cpu_max_mem
             )  # 32 GB as default (hardcoded for now...)
         max_memory = int(2**30 * max_memory)  # GB to bytes
 
         min_const_mem, min_per_sample_mem = self.est_mem_requirement(return_min=True)
 
@@ -540,23 +545,23 @@
             self.set_n_perm_batches(n_perm_batches)
         except RuntimeError as e:
             if "out of memory" in str(e):
                 if _TORCH_CUDA_IS_AVAILABLE:
                     torch.cuda.empty_cache()
 
                 if n_perm_batches == 1:
-                    self.set_n_perm_batches(
-                        2
-                    )  # Set to 2 perm batches, because that's the first batch size (and fastest) that is not cached.
+                    # Set to 2 perm batches, because that's the first batch size
+                    # (and fastest) that is not cached.
+                    self.set_n_perm_batches(2)
                     pass
                 else:
                     log.critical(
-                        "Could not allocate enough memory to store model parameters on GPU. There is no hope!"
+                        "Could not allocate enough memory to store model parameters "
+                        "on GPU. There is no hope!"
                     )
-                    print()
                     os._exit(1)
             else:
                 raise e
 
         const_mem, per_sample_mem = self.est_mem_requirement(return_min=False)
         _batch_size = (
             max((max_memory - const_mem) // per_sample_mem, 1)
@@ -849,15 +854,15 @@
 
         q = np.sqrt(5) / self._sig
         i, j = self.tril_indices
 
         is_train_pred = Rs_or_train_idxs.dim() == 1
         if not is_train_pred:  # Rs
 
-            Rs = Rs_or_train_idxs
+            Rs = Rs_or_train_idxs.type(_dtype)
             diffs = Rs[:, :, None, :] - Rs[:, None, :, :]  # N, a, a, 3
             diffs = diffs[:, i, j, :]  # N, d, 3
 
             if self._lat_and_inv is not None:
 
                 diffs_shape = diffs.shape
```

### Comparing `mbGDML-0.0.4/mbgdml/_gdml/train.py` & `mbGDML-0.1.0/mbgdml/_gdml/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2022, Stefan Chmiela
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,30 +19,27 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # pylint: disable=too-many-branches, too-many-statements
 
-import sys
-import logging
-import warnings
 from functools import partial
 import multiprocessing as mp
 import numpy as np
-import scipy as sp
 import psutil
 
+from .solvers.analytic import Analytic
 from .predict import GDMLPredict
 from .desc import Desc
 from .sample import draw_strat_sample
 from .perm import find_perms
 from ..utils import md5_data, chunk_array
 from ..losses import mae, rmse
-
+from ..logger import GDMLLogger
 from .. import _version
 
 mbgdml_version = _version.get_versions()["version"]
 
 Pool = mp.get_context("fork").Pool
 
 try:
@@ -65,15 +62,15 @@
 
 # TODO: remove exception handling once iterative solver ships
 try:
     from .solvers.iterative import Iterative
 except ImportError:
     pass
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def _share_array(arr_np, typecode_or_type):
     r"""Return a ctypes array allocated from shared memory with data from a
     NumPy array.
 
     Parameters
@@ -123,15 +120,15 @@
 
     Returns
     -------
     :obj:`int`
         Number of kernel matrix blocks created, divided by 2
         (symmetric blocks are always created at together).
     """
-    # pylint: disable=invalid-name
+    # pylint: disable=invalid-name, undefined-variable
     global glob  # pylint: disable=global-variable-not-assigned
 
     R_desc = np.frombuffer(glob["R_desc"]).reshape(glob["R_desc_shape"])
     R_d_desc = np.frombuffer(glob["R_d_desc"]).reshape(glob["R_d_desc_shape"])
     K = np.frombuffer(glob["K"]).reshape(glob["K_shape"])
 
     desc_func = glob["desc_func"]
@@ -839,15 +836,15 @@
             n_atoms,
             max_processes=self._max_processes,
         )
 
         n_perms = task["perms"].shape[0]
         tril_perms = np.array([desc.perm(p) for p in task["perms"]])
 
-        # dim_i = 3 * n_atoms
+        # dim_i = 3 * n_atoms  # Unused variable
         dim_d = desc.dim
 
         perm_offsets = np.arange(n_perms)[:, None] * dim_d
         tril_perms_lin = (tril_perms + perm_offsets).flatten("F")
 
         lat_and_inv = None
         if "lattice" in task:
@@ -871,15 +868,15 @@
         y, y_std, E_train_mean = self.train_labels(
             task["F_train"], task["use_E"], task["use_E_cstr"], E=E_train
         )
 
         max_memory_bytes = self._max_memory * 1024**3
 
         # Memory cost of analytic solver
-        est_bytes_analytic = self.analytic_est_memory_requirement(n_train, n_atoms)
+        est_bytes_analytic = Analytic.est_memory_requirement(n_train, n_atoms)
 
         # Memory overhead (solver independent)
         est_bytes_overhead = y.nbytes
         est_bytes_overhead += R.nbytes
         est_bytes_overhead += R_desc.nbytes
         est_bytes_overhead += R_d_desc.nbytes
 
@@ -887,44 +884,36 @@
 
         use_analytic_solver = (
             est_bytes_analytic + est_bytes_overhead
         ) < max_memory_bytes
 
         ###   mbGDML CHANGE START   ###
         if task["solver_name"] is None:
-            # Fall back to analytic solver, if iterative solver file is missing.
-            # Force analytic solver because iterative solver is not released yet.
+            # Fall back to analytic solver
             use_analytic_solver = True
-            # base_path = os.path.dirname(os.path.abspath(__file__))
-            # iter_solver_path = os.path.join(base_path, 'solvers/iterative.py')
-            # if not os.path.exists(iter_solver_path):
-            #     log.debug('Iterative solver not installed.')
-            #     use_analytic_solver = True
         else:
             solver = task["solver_name"]
-            if solver == "analytic":
-                use_analytic_solver = True
-            else:
-                raise ValueError(f"{solver} is not currently supported")
+            assert solver in ("analytic", "iterative")
+            use_analytic_solver = bool(solver == "analytic")
         ###   mbGDML CHANGE END   ###
 
         if use_analytic_solver:
             mem_req_mb = (est_bytes_analytic + est_bytes_overhead) * 1e-6  # MB
             log.info(
                 "Using analytic solver (expected memory requirement: ~%.2f MB)",
                 mem_req_mb,
             )
             ###   mbGDML CHANGE START   ###
-            alphas = self.solve_analytic(
-                task, desc, R_desc, R_d_desc, tril_perms_lin, y
-            )
+            analytic = Analytic(self, desc)
+            alphas = analytic.solve(task, R_desc, R_d_desc, tril_perms_lin, y)
             solver_keys["norm_y_train"] = np.linalg.norm(y)
             ###   mbGDML CHANGE END   ###
 
         else:
+            # Iterative solver
             max_n_inducing_pts = Iterative.max_n_inducing_pts(
                 n_train, n_atoms, max_memory_bytes
             )
             est_bytes_iterative = Iterative.est_memory_requirement(
                 n_train, max_n_inducing_pts, n_atoms
             )
             mem_req_mb = (est_bytes_iterative + est_bytes_overhead) * 1e-6  # MB
@@ -1011,149 +1000,14 @@
                 if E_train_mean is None
                 else E_train_mean
             )
             model["c"] = c
 
         return model
 
-    def analytic_est_memory_requirement(self, n_train, n_atoms):
-        est_bytes = 3 * (n_train * 3 * n_atoms) ** 2 * 8  # K + factor(s) of K
-        est_bytes += (n_train * 3 * n_atoms) * 8  # alpha
-        return est_bytes
-
-    def solve_analytic(self, task, desc, R_desc, R_d_desc, tril_perms_lin, y):
-        r"""Condensed :class:`sgdml.solvers.analytic.Analytic` class.
-
-        Parameters
-        ----------
-        task : :obj:`dict`
-
-        R_desc : :obj:`numpy.ndarray`
-            Array containing the descriptor for each training point.
-            Computed from :func:`~mbgdml._gdml.desc._r_to_desc`.
-        R_d_desc : :obj:`numpy.ndarray`
-            Array containing the gradient of the descriptor for
-            each training point. Computed from
-            :func:`~mbgdml._gdml.desc._r_to_d_desc`.
-        tril_perms_lin : :obj:`numpy.ndarray`, ndim: ``1``
-            An array containing all recovered permutations expanded as one large
-            permutation to be applied to a tiled copy of the object to be
-            permuted.
-        y : :obj:`numpy.ndarray`, ndim: ``1``
-            The train labels computed in
-            :meth:`~mbgdml._gdml.train.GDMLTrain.train_labels`.
-        """
-        # pylint: disable=invalid-name
-        log.info(
-            "\n-------------------------\n"
-            "|   Analytical solver   |\n"
-            "-------------------------\n"
-        )
-
-        sig = task["sig"]
-        lam = task["lam"]
-        use_E_cstr = task["use_E_cstr"]
-        log.log_model(task)
-
-        n_train, dim_d = R_d_desc.shape[:2]
-        n_atoms = int((1 + np.sqrt(8 * dim_d + 1)) / 2)
-        dim_i = 3 * n_atoms
-
-        # Compress kernel based on symmetries
-        col_idxs = np.s_[:]
-        if "cprsn_keep_atoms_idxs" in task:
-
-            cprsn_keep_idxs = task["cprsn_keep_atoms_idxs"]
-            cprsn_keep_idxs_lin = (
-                np.arange(dim_i).reshape(n_atoms, -1)[cprsn_keep_idxs, :].ravel()
-            )
-
-            col_idxs = (
-                cprsn_keep_idxs_lin[:, None] + np.arange(n_train) * dim_i
-            ).T.ravel()
-
-        log.info("\nAssembling kernel matrix")
-        t_assemble = log.t_start()
-        K = self._assemble_kernel_mat(
-            R_desc,
-            R_d_desc,
-            tril_perms_lin,
-            sig,
-            desc,
-            use_E_cstr=use_E_cstr,
-            col_idxs=col_idxs,
-        )
-        log.t_stop(t_assemble)
-
-        # with warnings.catch_warnings():
-        #     warnings.simplefilter("ignore")
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", r"Ill-conditioned matrix")
-
-            if K.shape[0] == K.shape[1]:
-
-                K[np.diag_indices_from(K)] -= lam  # regularize
-
-                try:
-                    t_cholesky = log.t_start()
-                    log.info("Solving linear system (Cholesky factorization)")
-                    # Cholesky
-                    L, lower = sp.linalg.cho_factor(
-                        -K, overwrite_a=True, check_finite=False
-                    )
-                    alphas = -sp.linalg.cho_solve(
-                        (L, lower), y, overwrite_b=True, check_finite=False
-                    )
-
-                    log.t_stop(t_cholesky, message="Done in {time} s")
-                except np.linalg.LinAlgError:
-                    # try a solver that makes less assumptions
-                    log.t_stop(
-                        t_cholesky, message="Cholesky factorization failed in {time} s"
-                    )
-                    log.info("Solving linear system (LU factorization)")
-
-                    try:
-                        # LU
-                        t_lu = log.t_start()
-                        alphas = sp.linalg.solve(
-                            K, y, overwrite_a=True, overwrite_b=True, check_finite=False
-                        )
-                        log.t_stop(t_lu, message="Done in {time} s")
-                    except MemoryError:
-                        log.t_stop(
-                            t_lu,
-                            message="LU factorization failed in {time} s",
-                            level=50,
-                        )
-                        log.critical(
-                            "Not enough memory to train this system using a closed "
-                            "form solver.\nPlease reduce the size of the training set "
-                            "or consider one of the approximate solver options."
-                        )
-                        sys.exit()
-
-                except MemoryError:
-                    log.critical(
-                        "Not enough memory to train this system using a closed "
-                        "form solver.\nPlease reduce the size of the training set "
-                        "or consider one of the approximate solver options."
-                    )
-                    sys.exit()
-            else:
-                log.info(
-                    "Solving overdetermined linear system (least squares approximation)"
-                )
-                t_least_squares = log.t_start()
-                # least squares for non-square K
-                alphas = np.linalg.lstsq(K, y, rcond=-1)[0]
-                log.t_stop(t_least_squares)
-
-        return alphas
-
     def _recov_int_const(
         self, model, task, R_desc=None, R_d_desc=None, require_E_eval=False
     ):
         r"""Estimate the integration constant for a force field model.
 
         The offset between the energies predicted for the original training
         data and the true energy labels is computed in the least square sense.
```

### Comparing `mbGDML-0.0.4/mbgdml/alchemy.py` & `mbGDML-0.1.0/mbgdml/switching.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,40 +16,33 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""Alchemical utilities."""
+"""Switching functions."""
 
-import logging
+from .logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
-class mbeAlchemyScale:
-    r"""Scale many-body interactions according to an alchemical parameter."""
-
-    def __init__(self, entity_id, order, factor):
-        r"""
-        Parameters
-        ----------
-        entity_id : :obj:`int`
-            Entity ID to scale interactions of.
-        order : :obj:`int`
-            Many-body order interactions to scale.
-        factor : :obj:`float`
-            Scaling factor that should be between ``0.`` and ``1.``.
-        """
-        self.entity_id = entity_id
-        self.order = order
-        self.factor = factor
-
-    def scale(self, data):
-        r"""Scale energies and forces.
-
-        Parameters
-        ----------
-        data : :obj:`float` or :obj:`numpy.ndarray`
-        """
-        return self.factor * data
+def linear_switching(data, factor):
+    r"""Linear switching function:
+
+    .. math::
+
+        y = Ax
+
+    where :math:`x` is ``data``, :math:`A` is the scaling ``factor``, and :math:`y` is
+    the scaled data.
+
+    Parameters
+    ----------
+    data : :obj:`float` or :obj:`numpy.ndarray`
+        Data to apply switching function to.
+    factor : :obj:`float`
+        Scaling factor :math:`a` between 0 and 1.
+    """
+    assert 0 <= factor <= 1
+    return factor * data
```

### Comparing `mbGDML-0.0.4/mbgdml/analysis/clustering.py` & `mbGDML-0.1.0/mbgdml/analysis/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,26 +16,26 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
+from ..logger import GDMLLogger
 
 try:
     from sklearn.cluster import AgglomerativeClustering
     from sklearn.cluster import KMeans
 
     _HAS_SKLEARN = True
 except ImportError:
     _HAS_SKLEARN = False
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def get_clustered_data(cl_idxs, data):
     r"""Cluster data according to cluster indices.
 
     Parameters
     ----------
```

### Comparing `mbGDML-0.0.4/mbgdml/analysis/models.py` & `mbGDML-0.1.0/mbgdml/analysis/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,14 +19,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Analyses for models."""
 
 import numpy as np
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 
 def gdml_mat52_wrk(r_desc, sig, n_perms, R_desc_perms):
     r"""Compute the Matérn 5/2 covariance function for a single structure with
     respect to a GDML train set.
 
     Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/analysis/problematic.py` & `mbGDML-0.1.0/mbgdml/analysis/problematic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2020 monopsony
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,61 +22,73 @@
 # SOFTWARE.
 
 """Identifies problematic (high error) structures for model to train on next.
 Some code within this module is modified from https://github.com/fonsecag/MLFF.
 """
 
 import os
-import logging
 import numpy as np
 from scipy.spatial.distance import pdist
 
 from . import clustering
 from ..mbe import mbePredict
 from ..utils import save_json
 from ..losses import loss_f_mse
+from ..logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 class ProblematicStructures:
     r"""Find problematic structures for models in datasets.
 
     Clusters all structures in a dataset using agglomerative and k-means
     algorithms using a structural descriptor and energies.
     """
 
     def __init__(
-        self, models, predict_model, use_ray=False, n_workers=None, wkr_chunk_size=100
+        self,
+        models,
+        predict_model,
+        use_ray=False,
+        n_workers=1,
+        ray_address="auto",
+        wkr_chunk_size=100,
     ):
         """
         Parameters
         ----------
         models : :obj:`list` of :obj:`mbgdml.models.Model`
             Machine learning model objects that contain all information to make
             predictions using ``predict_model``.
         predict_model : ``callable``
-            A function that takes ``z, R, entity_ids, nbody_gen, model`` and
-            computes energies and forces. This will be turned into a ray remote
+            A function that takes ``Z``, ``R``, ``entity_ids``, ``nbody_gen``, ``model``
+            and computes energies and forces. This will be turned into a ray remote
             function if ``use_ray = True``. This can return total properties
             or all individual :math:`n`-body energies and forces.
         use_ray : :obj:`bool`, default: ``False``
-            Parallelize predictions using ray. Note that initializing ray tasks
-            comes with some overhead and can make smaller computations much
-            slower. Thus, this is only recommended with more than 10 or so
-            entities.
-        n_workers : :obj:`int`, default: :obj:`None`
-            Total number of workers available for predictions when using ray.
+            Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
+            computations.
+        n_workers : :obj:`int`, default: ``1``
+            Total number of workers available for ray. This is ignored if ``use_ray``
+            is ``False``.
+        ray_address : :obj:`str`, default: ``"auto"``
+            Ray cluster address to connect to.
         wkr_chunk_size : :obj:`int`, default: ``100``
             Number of :math:`n`-body structures to assign to each spawned
             worker with ray.
         """
         self.models = models
         self.mbe_pred = mbePredict(
-            models, predict_model, use_ray, n_workers, wkr_chunk_size
+            models,
+            predict_model,
+            use_ray=use_ray,
+            n_workers=n_workers,
+            ray_address=ray_address,
+            wkr_chunk_size=wkr_chunk_size,
         )
 
         self.course_n_cl_r = 10
         r"""Number of clusters used in the course stage for geometries.
 
         There will be a total of ``course_n_cl_r`` clusters.
 
@@ -389,14 +401,15 @@
             cl_idxs_write = [np.array(R_idxs[idxs]) for idxs in cl_idxs]
             self.json_dict["clustering"] = {}
             self.json_dict["clustering"]["indices"] = cl_idxs_write
             self.json_dict["clustering"]["population"] = cl_pop
 
         log.info("\nPredicting structures")
         t_prediction = log.t_start()
+        # pylint: disable-next=unbalanced-tuple-unpacking
         E_pred, F_pred = self.mbe_pred.predict(Z, R, entity_ids, comp_ids)
         log.t_stop(t_prediction, message="Took {time} s")
         log.info("Computing prediction errors")
         E_errors = E_pred - E
         F_errors = F_pred - F
         log.debug("Energy errors")
         log.log_array(E_errors, level=10)
```

### Comparing `mbGDML-0.0.4/mbgdml/analysis/rdf.py` & `mbGDML-0.1.0/mbgdml/analysis/rdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,14 +22,18 @@
 
 """Compute RDF curves under periodic boundary conditions."""
 
 import ray
 import numpy as np
 from ..periodic import Cell
 from ..utils import gen_combs, chunk_iterable
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
+
 
 # Possible ray task.
 def _bin_distances(R, R_idxs, atom_pairs, rdf_settings, cell_vectors):
     r"""Compute relevant RDF data for one or more structures.
 
     Parameters
     ----------
@@ -85,15 +89,17 @@
         Z,
         entity_ids,
         comp_ids,
         cell_vectors,
         bin_width=0.05,
         rdf_range=(0.0, 15.0),
         inter_only=True,
-        n_workers=None,
+        use_ray=False,
+        ray_address="auto",
+        n_workers=1,
     ):
         r"""
         Parameters
         ----------
         Z : :obj:`numpy.ndarray`, ndim: ``1``
             Atomic numbers of all atoms in the system.
         entity_ids : :obj:`numpy.ndarray`, ndim: ``1``
@@ -103,33 +109,49 @@
             Labels for each ``entity_id`` used to determine the desired entity
             for RDF computations.
         cell_vectors : :obj:`numpy.ndarray`
             The three cell vectors.
         inter_only : :obj:`bool`, default: ``True``
             Only intermolecular distances are allowed. If ``True``, atoms that
             have the same ``entity_id`` are ignored.
-        n_workers : :obj:`int`, default: :obj:`None`
-            Number workers we can use for ray tasks. If :obj:`None` results in
-            serial operation.
+        use_ray : :obj:`bool`, default: ``False``
+            Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
+            computations.
+        n_workers : :obj:`int`, default: ``1``
+            Total number of workers available for ray. This is ignored if ``use_ray``
+            is ``False``.
+        ray_address : :obj:`str`, default: ``"auto"``
+            Ray cluster address to connect to.
         """
         # Store data
         self.Z = Z
         self.entity_ids = entity_ids
         self.comp_ids = comp_ids
         self.cell_vectors = cell_vectors
         self.bin_width = bin_width
         self.rdf_range = rdf_range
         self.inter_only = inter_only
+        self.use_ray = use_ray
         self.n_workers = n_workers
 
         # Setup ray
-        if n_workers is not None:
+        if use_ray:
             if not ray.is_initialized():
-                ray.init(address="auto")
-            assert ray.is_initialized()
+                log.debug("ray is not initialized")
+                # Try to connect to already running ray service (from ray cli).
+                try:
+                    log.debug("Trying to connect to ray at address %r", ray_address)
+                    ray.init(address=ray_address)
+                except ConnectionError:
+                    log.debug("Failed to connect to ray at %r", ray_address)
+                    log.debug("Trying to initialize ray with %d cores", n_workers)
+                    ray.init(num_cpus=n_workers)
+                log.debug("Successfully initialized ray")
+            else:
+                log.debug("Ray was already initialized")
             self._max_chunk_size = 300
 
     def _setup(self, comp_id_pair, entity_idxs):
         r"""Prepare to do RDF computation.
 
         Parameters
         ----------
@@ -278,24 +300,24 @@
 
         TODO: Support different cell sizes for each structure.
         """
         self._setup(comp_id_pair, entity_idxs)
 
         # Computing histogram.
         # Serial operation.
-        if self.n_workers is None:
+        if not self.use_ray:
             for i in range(0, len(R), step):
                 count, volume_contrib, n_R = _bin_distances(
                     R, i, self._atom_pairs, self._hist_settings, self.cell_vectors
                 )
                 self._count += count
                 self._cuml_volume += volume_contrib
                 self._n_analyzed += n_R
         # Parallel operation with ray.
-        elif self.n_workers >= 1:
+        else:
             _bin_distances_remote = ray.remote(_bin_distances)
             chunk_size = min(
                 self._max_chunk_size,
                 int(len(tuple(range(0, len(R), step))) / self.n_workers),
             )
             chunker = chunk_iterable(range(0, len(R), step), chunk_size)
```

### Comparing `mbGDML-0.0.4/mbgdml/data/basedata.py` & `mbGDML-0.1.0/mbgdml/data/basedata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,14 +17,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 
 # pylint: disable-next=invalid-name
 class mbGDMLData:
     r"""Parent class for mbGDML structure, data, and predict sets."""
 
     def __init__(self):
```

### Comparing `mbGDML-0.0.4/mbgdml/data/dataset.py` & `mbGDML-0.1.0/mbgdml/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,17 +22,20 @@
 
 import os
 import numpy as np
 from cclib.parser.utils import convertor
 from .basedata import mbGDMLData
 from .. import utils
 from .. import _version
+from ..logger import GDMLLogger
 
 mbgdml_version = _version.get_versions()["version"]
 
+log = GDMLLogger(__name__)
+
 
 class DataSet(mbGDMLData):
     r"""For creating, loading, manipulating, and using data sets."""
 
     def __init__(self, dset_path=None, Z_key="Z", R_key="R", E_key="E", F_key="F"):
         """
         Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/data/predictset.py` & `mbGDML-0.1.0/mbgdml/data/predictset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,51 +21,49 @@
 # SOFTWARE.
 
 import ray
 import numpy as np
 from .. import __version__ as mbgdml_version
 from .basedata import mbGDMLData
 from ..mbe import mbePredict, decomp_to_total
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 
 class PredictSet(mbGDMLData):
     r"""A predict set is a data set with mbGDML predicted energy and forces
     instead of training data.
 
-    When analyzing many structures using mbGDML it is easier to
-    predict all many-body contributions once and then analyze the stored data.
-
-    Attributes
-    ----------
-    name : :obj:`str`
-        File name of the predict set.
-    theory : :obj:`str`
-        Specifies the level of theory used for GDML training.
-    entity_ids : :obj:`numpy.ndarray`
-        A uniquely identifying integer specifying what atoms belong to
-        which entities. Entities can be a related set of atoms, molecules,
-        or functional group. For example, a water and methanol molecule
-        could be ``[0, 0, 0, 1, 1, 1, 1, 1, 1]``.
-    comp_ids : :obj:`numpy.ndarray`
-        Relates ``entity_id`` to a fragment label for chemical components
-        or species. Labels could be ``WAT`` or ``h2o`` for water, ``MeOH``
-        for methanol, ``bz`` for benzene, etc. There are no standardized
-        labels for species. The index of the label is the respective
-        ``entity_id``. For example, a water and methanol molecule could
-        be ``['h2o', 'meoh']``.
+    When analyzing many structures using mbGDML it is easier to predict all many-body
+    contributions once and then analyze the stored data.
     """
 
     def __init__(self, pset=None, Z_key="Z", R_key="R", E_key="E", F_key="F"):
         r"""
         Parameters
         ----------
-        pset : :obj:`str` or :obj:`dict`, optional
+        pset : :obj:`str` or :obj:`dict`, default: ``None``
             Predict set path or dictionary to initialize with.
+        Z_key : :obj:`str`, default: ``Z``
+            :obj:`dict` key in ``pset`` for atomic numbers.
+        R_key : :obj:`str`, default: ``R``
+            :obj:`dict` key in ``pset`` for Cartesian coordinates.
+        E_key : :obj:`str`, default: ``E``
+            :obj:`dict` key in ``pset`` for energies.
+        F_key : :obj:`str`, default: ``F``
+            :obj:`dict` key in ``pset`` for atomic forces.
         """
         self.name = "predictset"
+        r"""File name of the predict set.
+
+        Default: ``"predictset"``
+
+        :type: :obj:`str`
+        """
         self.type = "p"
         self.mbgdml_version = mbgdml_version
         self._loaded = False
         self._predicted = False
 
         # Set keys for atomic properties.
         self.Z_key = Z_key
@@ -78,15 +76,15 @@
 
     def prepare(self):
         r"""Prepares a predict set by calculated the decomposed energy and
         force contributions.
 
         Note
         -----
-        You must load a dataset first to specify ``z``, ``R``, ``entity_ids``,
+        You must load a dataset first to specify ``Z``, ``R``, ``entity_ids``,
         and ``comp_ids``.
         """
         E_nbody, F_nbody, entity_combs, nbody_orders = self.mbePredict.predict_decomp(
             self.Z, self.R, self.entity_ids, self.comp_ids
         )
         self.nbody_orders = nbody_orders
         for i, order in enumerate(nbody_orders):
@@ -165,14 +163,82 @@
         """
         return self._F_true
 
     @F_true.setter
     def F_true(self, var):
         self._F_true = var  # pylint: disable=invalid-name
 
+    @property
+    def entity_ids(self):
+        r"""1D array specifying which atoms belong to which entities.
+
+        An entity represents a related set of atoms such as a single molecule,
+        several molecules, or a functional group. For mbGDML, an entity usually
+        corresponds to a model trained to predict energies and forces of those
+        atoms. Each ``entity_id`` is an :obj:`int` starting from ``0``.
+
+        It is conceptually similar to PDBx/mmCIF ``_atom_site.label_entity_ids``
+        data item.
+
+        Examples
+        --------
+        A single water molecule would be ``[0, 0, 0]``. A water (three atoms)
+        and methanol (six atoms) molecule in the same structure would be
+        ``[0, 0, 0, 1, 1, 1, 1, 1, 1]``.
+
+        :type: :obj:`numpy.ndarray`
+        """
+        if hasattr(self, "_entity_ids"):
+            return self._entity_ids
+
+        return np.array([])
+
+    @entity_ids.setter
+    def entity_ids(self, var):
+        self._entity_ids = np.array(var)
+
+    @property
+    def comp_ids(self):
+        r"""A 1D array relating ``entity_id`` to a fragment label for chemical
+        components or species. Labels could be ``WAT`` or ``h2o`` for water,
+        ``MeOH`` for methanol, ``bz`` for benzene, etc. There are no
+        standardized labels for species. The index of the label is the
+        respective ``entity_id``. For example, a water and methanol molecule
+        could be ``['h2o', 'meoh']``.
+
+        Examples
+        --------
+        Suppose we have a structure containing a water and methanol molecule.
+        We can use the labels of ``h2o`` and ``meoh`` (which could be
+        anything): ``['h2o', 'meoh']``. Note that the
+        ``entity_id`` is a :obj:`str`.
+
+        :type: :obj:`numpy.ndarray`
+        """
+        if hasattr(self, "_comp_ids"):
+            return self._comp_ids
+
+        return np.array([])
+
+    @property
+    def theory(self):
+        r"""The level of theory used to compute energy and gradients of the data
+        set.
+
+        :type: :obj:`str`
+        """
+        if hasattr(self, "_theory"):
+            return self._theory
+
+        return "n/a"
+
+    @theory.setter
+    def theory(self, var):
+        self._theory = var
+
     def load(self, pset):
         r"""Reads predict data set and loads data.
 
         Parameters
         ----------
         pset : :obj:`str` or :obj:`dict`
             Path to predict set ``npz`` file or a dictionary.
@@ -200,37 +266,63 @@
         for i in pset["nbody_orders"]:
             setattr(self, f"{self.E_key}_{i}", pset[f"{self.E_key}_{i}"])
             setattr(self, f"{self.F_key}_{i}", pset[f"{self.F_key}_{i}"])
             setattr(self, f"entity_combs_{i}", pset[f"entity_combs_{i}"])
 
         self._loaded = True
 
-    def nbody_predictions(self, nbody_orders, n_workers=1):
+    @comp_ids.setter
+    def comp_ids(self, var):
+        self._comp_ids = np.array(var)
+
+    def nbody_predictions(
+        self, nbody_orders, use_ray=False, n_workers=1, ray_address="auto"
+    ):
         r"""Energies and forces of all structures including ``nbody_order``
         contributions.
 
         Predict sets have data that is broken down into many-body contributions.
         This function sums the many-body contributions up to the specified
         level; for example, ``3`` returns the energy and force predictions when
         including one, two, and three body contributions/corrections.
 
         Parameters
         ----------
         nbody_orders : :obj:`list` of :obj:`int`
             :math:`n`-body orders to include.
+        use_ray : :obj:`bool`, default: ``False``
+            Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
+            computations.
+        n_workers : :obj:`int`, default: ``1``
+            Total number of workers available for ray. This is ignored if ``use_ray``
+            is ``False``.
+        ray_address : :obj:`str`, default: ``"auto"``
+            Ray cluster address to connect to.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             Energy of structures up to and including n-order corrections.
         :obj:`numpy.ndarray`
             Forces of structures up to an including n-order corrections.
         """
-        if n_workers != 1:
-            ray.is_initialized()
+        if use_ray:
+            if not ray.is_initialized():
+                log.debug("ray is not initialized")
+                # Try to connect to already running ray service (from ray cli).
+                try:
+                    log.debug("Trying to connect to ray at address %r", ray_address)
+                    ray.init(address=ray_address)
+                except ConnectionError:
+                    log.debug("Failed to connect to ray at %r", ray_address)
+                    log.debug("Trying to initialize ray with %d cores", n_workers)
+                    ray.init(num_cpus=n_workers)
+                log.debug("Successfully initialized ray")
+            else:
+                log.debug("Ray was already initialized")
 
         E = np.zeros(self.E_true.shape)
         F = np.zeros(self.F_true.shape)
         for nbody_order in nbody_orders:
             E_decomp = getattr(self, f"{self.E_key}_{nbody_order}")
             F_decomp = getattr(self, f"{self.F_key}_{nbody_order}")
             entity_combs = getattr(self, f"entity_combs_{nbody_order}")
@@ -286,43 +378,50 @@
             self.r_unit = dset["r_unit"]
         if isinstance(dset["e_unit"], np.ndarray):
             self.e_unit = str(dset["e_unit"].item())
         else:
             self.e_unit = dset["e_unit"]
 
     def load_models(
-        self, models, predict_model, use_ray=False, n_workers=None, wkr_chunk_size=100
+        self,
+        models,
+        predict_model,
+        use_ray=False,
+        n_workers=1,
+        ray_address="auto",
+        wkr_chunk_size=100,
     ):
         r"""Loads model(s) in preparation to create a predict set.
 
         Parameters
         ----------
-        models : :obj:`list` of :obj:`mbgdml.predictors.mlWorker`
+        models : :obj:`list` of :obj:`mbgdml.models.Model`
             Machine learning model objects that contain all information to make
             predictions using ``predict_model``.
         predict_model : ``callable``
             A function that takes ``Z, R, entity_ids, nbody_gen, model`` and
             computes energies and forces. This will be turned into a ray remote
             function if ``use_ray = True``. This can return total properties
             or all individual :math:`n`-body energies and forces.
         use_ray : :obj:`bool`, default: ``False``
-            Parallelize predictions using ray. Note that initializing ray tasks
-            comes with some overhead and can make smaller computations much
-            slower. Thus, this is only recommended with more than 10 or so
-            entities.
-        n_workers : :obj:`int`, default: :obj:`None`
-            Total number of workers available for predictions when using ray.
+            Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
+            computations.
+        n_workers : :obj:`int`, default: ``1``
+            Total number of workers available for ray. This is ignored if ``use_ray``
+            is ``False``.
+        ray_address : :obj:`str`, default: ``"auto"``
+            Ray cluster address to connect to.
         wkr_chunk_size : :obj:`int`, default: ``100``
             Number of :math:`n`-body structures to assign to each spawned
             worker with ray.
         """
         if use_ray:
             assert ray.is_initialized()
         self.mbePredict = mbePredict(
-            models, predict_model, use_ray, n_workers, wkr_chunk_size
+            models, predict_model, use_ray, n_workers, ray_address, wkr_chunk_size
         )
 
         models_md5, nbody_orders = [], []
         for model in self.mbePredict.models:
             if use_ray:
                 model = ray.get(model)
             nbody_orders.append(model.nbody_order)
```

### Comparing `mbGDML-0.0.4/mbgdml/descriptors.py` & `mbGDML-0.1.0/mbgdml/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,19 +17,19 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import itertools
-import logging
 import numpy as np
 from qcelemental import periodictable as ptable
+from .logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 class Criteria:
     r"""Descriptor criteria for accepting a structure based on a descriptor
     and cutoff.
     """
```

### Comparing `mbGDML-0.0.4/mbgdml/interfaces/ase.py` & `mbGDML-0.1.0/mbgdml/interfaces/ase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,20 +18,24 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from ase.calculators.calculator import Calculator
 import numpy as np
+import ray
+from ..logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 # pylint: disable-next=invalid-name
 class mbeCalculator(Calculator):
-    r"""ASE calculator using the many-body expansion predictor in mbGDML."""
+    r"""ASE calculator for a many-body expansion predictor."""
 
-    implemented_properties = ["energy", "forces"]
+    implemented_properties = ["energy", "forces", "stress"]
 
     def __init__(
         self, mbe_pred, parameters=None, e_conv=1.0, f_conv=1.0, atoms=None, **kwargs
     ):
         """
         Parameters
         ----------
@@ -44,44 +48,68 @@
         f_conv : :obj:`float`, default: ``1.0``
             Model forces conversion factor to eV/A (required by ASE).
         """
         self.name = "mbGDML"
         Calculator.__init__(self, restart=None, label=None, atoms=atoms, **kwargs)
 
         self.mbe_pred = mbe_pred
+        self.mbe_pred.use_voigt = True
 
         self.e_conv = e_conv
         self.f_conv = f_conv
 
         if parameters is None:
             parameters = {}
         self.parameters = parameters
 
     # pylint: disable-next=unused-argument, keyword-arg-before-vararg
     def calculate(self, atoms=None, *args, **kwargs):
-        r"""Predicts energy and forces using many-body GDML models."""
+        r"""Predicts all available properties using the MBE predictor."""
+        is_periodic = bool(self.mbe_pred.periodic_cell)
+
         if atoms is not None:
-            if self.mbe_pred.periodic_cell is not None:
+            if is_periodic:
                 atoms.wrap()
             self.atoms = atoms.copy()
 
         parameters = self.parameters
         entity_ids = parameters["entity_ids"]
         comp_ids = parameters["comp_ids"]
 
-        e, f = self.mbe_pred.predict(
-            atoms.get_atomic_numbers(), atoms.get_positions(), entity_ids, comp_ids
+        predict_kwargs = {}
+        if is_periodic:
+            # Update cell vectors and cutoff
+            cell_vectors = atoms.get_cell()[:]
+            periodic_cell = self.mbe_pred.periodic_cell
+            if self.mbe_pred.use_ray:
+                periodic_cell = ray.get(periodic_cell)
+            periodic_cell.cell_v = cell_vectors
+            self.mbe_pred.periodic_cell = periodic_cell
+
+            if not self.mbe_pred.compute_stress:
+                self.mbe_pred.compute_stress = True
+
+        E, F, *stress = self.mbe_pred.predict(
+            atoms.get_atomic_numbers(),
+            atoms.get_positions(),
+            entity_ids,
+            comp_ids,
+            **predict_kwargs
         )
-        e = e[0]
-
+        E = E[0]
+        F = F.reshape(-1, 3)
         # Unit conversions
-        e *= self.e_conv
-        f *= self.f_conv
+        E *= self.e_conv
+        F *= self.f_conv
+
+        self.results = {"energy": E, "forces": F}
 
-        self.results = {"energy": e, "forces": f.reshape(-1, 3)}
+        if is_periodic:
+            stress = stress[0][0]
+            self.results["stress"] = stress * self.e_conv
 
     def todict(self, skip_default=True):
         defaults = self.get_default_parameters()
         dct = {}
         for key, value in self.parameters.items():
             if hasattr(value, "todict"):
                 value = value.todict()
```

### Comparing `mbGDML-0.0.4/mbgdml/logger.py` & `mbGDML-0.1.0/mbgdml/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,88 +20,99 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 import random
 import time
 import numpy as np
-from .utils import atoms_by_element
+from qcelemental import periodictable as ptable
 from . import _version
 
 __version__ = _version.get_versions()["version"]
 
 
-class TimeTracker:
-    r"""Simple way to keep track of multiple timings."""
+def set_log_level(level):
+    """Dynamically control the log level of mbGDML.
 
-    def __init__(self):
-        self.t_hashes = {}
-
-    def t_start(self):
-        r"""Record the time and return a random hash."""
-        t_hash = random.getrandbits(128)
-        self.t_hashes[t_hash] = time.time()
-        return t_hash
-
-    def t_stop(self, t_hash, message="Took {time} s", precision=5, level=20):
-        r"""Determine timing from a hash.
-
-        Parameters
-        ----------
-        t_hash : :obj:`str`
-            Timing hash generated from ``TimeTracker.start()``.
-        log : ``GDMLLogger``
-            Log object to write to.
-        message : :obj:`str`, default: ``'Took {time} s'``
-            Timing message to be written to log. ``'{time}'`` will be replaced
-            with for the elapsed time.
-        precision : :obj:`int`, default: ``5``
-            Number of decimal points to print time.
-        """
-        t_stop = time.time()
-        t_elapsed = t_stop - self.t_hashes[t_hash]
-        del self.t_hashes[t_hash]
-        # pylint: disable-next=no-member
-        self.log(level, message.replace("{time}", f"%.{precision}f" % t_elapsed))
-        return t_elapsed
+    Parameters
+    ----------
+    level : :obj:`int`
+        The desired logging level.
+    """
+    for logger_name in logging.root.manager.loggerDict:  # pylint: disable=no-member
+        if "mbgdml" in logger_name:
+            logger = logging.getLogger(logger_name)
+            logger.setLevel(level)
+            for handler in logger.handlers:
+                handler.setLevel(level)
+
+
+def atoms_by_element(atom_list):
+    r"""Converts a list of atoms identified by their atomic number to their
+    elemental symbol in the same order.
+
+    Parameters
+    ----------
+    atom_list : :obj:`list` [:obj:`int`]
+        Atomic numbers of atoms within a structure.
+
+    Returns
+    -------
+    :obj:`list` [:obj:`str`]
+        Element symbols of atoms within a structure.
+    """
+    return [ptable.to_symbol(z) for z in atom_list]
+
+
+class GDMLLogger:
+    def __init__(self, name, level=logging.INFO):
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(level)
+
+        # '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+        self.formatter = logging.Formatter("%(message)s")
+        self.handler = logging.StreamHandler()
+        self.handler.setLevel(level)
+        self.handler.setFormatter(self.formatter)
+        self.logger.addHandler(self.handler)
 
+        self.t_hashes = {}
 
-class GDMLLogger(logging.Logger, TimeTracker):
-
-    level = logging.INFO
+    def log(self, level, msg, *args, **kwargs):
+        self.logger.log(level, msg, *args, **kwargs)
 
-    def __init__(self, name):
+    def debug(self, msg, *args, **kwargs):
+        self.logger.log(logging.DEBUG, msg, *args, **kwargs)
 
-        logging.Logger.__init__(self, name, self.level)
-        TimeTracker.__init__(self)
+    def info(self, msg, *args, **kwargs):
+        self.logger.log(logging.INFO, msg, *args, **kwargs)
 
-        # only display levelname and message
-        formatter = logging.Formatter("%(message)s")
+    def warning(self, msg, *args, **kwargs):
+        self.logger.log(logging.WARNING, msg, *args, **kwargs)
 
-        # this handler will write to sys.stderr by default
-        hd = logging.StreamHandler()  # pylint: disable=invalid-name
-        hd.setFormatter(formatter)
-        hd.setLevel(self.level)
+    def error(self, msg, *args, **kwargs):
+        self.logger.log(logging.ERROR, msg, *args, **kwargs)
 
-        self.addHandler(hd)
+    def critical(self, msg, *args, **kwargs):
+        self.logger.log(logging.CRITICAL, msg, *args, **kwargs)
 
-    def log_array(self, array, level=20):
+    def log_array(self, array, level=logging.INFO):
         if isinstance(array, (list, tuple)):
             array = np.array(array)
         arr_str = np.array2string(array, separator=", ")
-        self.log(level, arr_str)
+        self.logger.log(level, arr_str)
 
     def log_package(self):
         title = r"""           _      ____ ____  __  __ _
  _ __ ___ | |__  / ___|  _ \|  \/  | |    
 | '_ ` _ \| '_ \| |  _| | | | |\/| | |    
 | | | | | | |_) | |_| | |_| | |  | | |___ 
 |_| |_| |_|_.__/ \____|____/|_|  |_|_____|"""
         self.info(title)
-        self.info("%s\n", __version__)
+        self.info(f"{__version__}\n")
 
     # pylint: disable-next=too-many-branches
     def log_model(self, model):
         r"""Log the relevant model properties
 
         Parameters
         ----------
@@ -145,9 +156,37 @@
         if d_type == "t":
             self.info("use_E_cstr : %r", model["use_E_cstr"])
         elif d_type == "m":
             if "alphas_E" in model.keys():  # pylint: disable=simplifiable-if-statement
                 use_E_cstr = True
             else:
                 use_E_cstr = False
-            self.info("use_E_cstr : %r", use_E_cstr)
-        self.info("use_cprsn : %r", model["use_cprsn"])
+            self.info(f"use_E_cstr : {use_E_cstr}")
+        self.info(f"use_cprsn : {model['use_cprsn']}")
+
+    def t_start(self):
+        r"""Record the time and return a random hash."""
+        t_hash = random.getrandbits(128)
+        self.t_hashes[t_hash] = time.time()
+        return t_hash
+
+    def t_stop(self, t_hash, message="Took {time} s", precision=5, level=20):
+        r"""Determine timing from a hash.
+
+        Parameters
+        ----------
+        t_hash : :obj:`str`
+            Timing hash generated from ``TimeTracker.start()``.
+        message : :obj:`str`, default: ``'Took {time} s'``
+            Timing message to be written to log. ``'{time}'`` will be replaced
+            with for the elapsed time.
+        precision : :obj:`int`, default: ``5``
+            Number of decimal points to print.
+        level : :obj:`int`, default: ``20``
+            Log level.
+        """
+        t_stop = time.time()
+        t_elapsed = t_stop - self.t_hashes[t_hash]
+        del self.t_hashes[t_hash]
+        # pylint: disable-next=no-member
+        self.log(level, message.replace("{time}", f"%.{precision}f" % t_elapsed))
+        return t_elapsed
```

### Comparing `mbGDML-0.0.4/mbgdml/losses.py` & `mbGDML-0.1.0/mbgdml/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,18 +16,18 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
+from .logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def mae(errors):
     r"""Mean absolute error (MAE).
 
     .. math::
```

### Comparing `mbGDML-0.0.4/mbgdml/mbe.py` & `mbGDML-0.1.0/mbgdml/mbe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,22 +19,22 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Many-body utilities."""
 
 import itertools
-import logging
 import math
 import numpy as np
 import ray
 from .utils import chunk_array, chunk_iterable, gen_combs
+from .stress import to_voigt, virial_finite_diff
+from .logger import GDMLLogger
 
-
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 def gen_r_entity_combs(r_prov_spec, entity_ids_lower):
     r"""Generate ``entity_id`` combinations of a specific size for a single
     structure.
 
     ``r_prov_spec[2:]`` provides ``entity_ids`` of a reference structure.
@@ -124,44 +124,52 @@
         worker.
     :obj:`numpy.ndarray`
         Many-body energy contributions for the worker structure indices.
     :obj:`numpy.ndarray`
         Many-body derivative (i.e., gradients or forces depending on the sign)
         contributions for the worker structure indices.
     """
+    log.debug("MBE contributions")
+    log.debug("Parent size %i", np.unique(entity_ids).shape[0])
     E = np.zeros(len(r_idxs))
     Deriv = np.zeros((len(r_idxs), *r_shape))
 
     # Loop through every structure in the reference data set.
     for i, i_r in enumerate(r_idxs):
         # We have to match the molecule information for each reference
         # structure to the molecules in this lower-order structure to remove
         # the right contribution.
         r_prov_spec = r_prov_specs[i_r]  # r_prov_specs of this structure.
+        log.debug("Supersystem structure r_prov_spec: %r", r_prov_spec.tolist())
 
         # Loop through every molecular combination.
         for entity_comb in gen_r_entity_combs(r_prov_spec, entity_ids_lower):
             # r_prov_spec of the lower-order structure.
             # Combines [r_prov_id, r_idx] with the entity combination.
             r_prov_spec_lower_comb = np.block([r_prov_spec[:2], np.array(entity_comb)])
+            log.debug("Fragment r_prov_spec: %r", r_prov_spec_lower_comb.tolist())
 
             # Index of the structure in the lower data set.
             try:
+                log.debug("Searching for fragment's r_prov_spec")
                 i_r_lower = np.where(
                     np.all(r_prov_specs_lower == r_prov_spec_lower_comb, axis=1)
                 )[0][0]
+                log.debug("Found fragment index: %d", i_r_lower)
             except IndexError as e:
+                log.debug("Could not find fragment. This can be expected sometimes.")
                 if "for axis 0 with size 0" in str(e):
                     continue
                 raise
 
             deriv_lower = Deriv_lower[i_r_lower]
 
             # Adding or removing energy contributions.
             E[i] += E_lower[i_r_lower]
+            log.debug("Fragment energy: %r", E_lower[i_r_lower])
 
             # Adding or removing derivative contributions.
             # We have to determine the corresponding atom indices of both the
             # reference and lower-order structure.
             # This is done by matching the entity_id_prov between the two r_prov_specs.
             # The position of entity_id_prov in r_prov_specs (with r_prov_id and
             # r_idx removed) specifies the entity_id of the
@@ -171,22 +179,25 @@
             # entity_id_lower: the entity_id in the lower-order structure.
             # i_z: atom indices of the reference structure to add or remove
             # lower-order structure.
             # i_z_lower: atom indices of lower-order contribution.
             for entity_id_prov in r_prov_spec_lower_comb[2:]:
                 entity_id = np.where(r_prov_spec[2:] == entity_id_prov)[0][0]
                 i_z = np.where(entity_ids == entity_id)[0]
+                log.debug("atom slice : %r", i_z.tolist())
 
                 entity_id_lower = np.where(
                     r_prov_spec_lower_comb[2:] == entity_id_prov
                 )[0][0]
                 i_z_lower = np.where(entity_ids_lower == entity_id_lower)[0]
 
                 Deriv[i][i_z] += deriv_lower[i_z_lower]
 
+            log.debug("Fragment successfully accounted for")
+
     return r_idxs, E, Deriv
 
 
 def gen_r_idxs_worker(r_prov_specs, r_prov_ids_lower, n_workers):
     r"""Generates the assigned structures for each worker.
 
     Parameters
@@ -233,24 +244,24 @@
     Deriv_lower,
     entity_ids_lower,
     r_prov_ids_lower,
     r_prov_specs_lower,
     operation="remove",
     use_ray=False,
     ray_address="auto",
-    n_workers=2,
+    n_workers=1,
 ):
     r"""Adds or removes energy and derivative (i.e., gradients or forces)
     contributions from a reference.
 
     We use the term "lower" to refer to the lower-order (i.e., smaller) systems.
     These are the energy and derivative contributions to remove or add to a
     reference.
 
-    Making :math:`n`-body predictions (i.e., ``operation = 'add'``) will often
+    Making :math:`n`-body predictions (i.e., ``operation = "add"``) will often
     not have ``r_prov_ids`` or ``r_prov_specs`` as all lower contributions are
     derived exclusively from these structures. Use :obj:`None` for both of these
     and this function will assume that all ``_lower`` properties apply.
 
     Parameters
     ----------
     E : :obj:`numpy.ndarray`, ndim: ``1``
@@ -293,28 +304,45 @@
         Structure provenance IDs. This specifies the ``r_prov_id``, structure
         index from the ``r_prov_id`` source, and ``entity_ids`` making up
         lower-order structures.
     operation : :obj:`str`, default: ``'remove'``
         ``'add'`` or ``'remove'`` the contributions.
     use_ray : :obj:`bool`, default: ``False``
         Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
-        calculations.
-    n_workers : :obj:`int`, default: ``2``
-        Number of ray workers to use. This is ignored if ``use_ray`` is
-        ``False``.
-    ray_address : :obj:`str`, default: ``'auto'``
+        computations.
+    n_workers : :obj:`int`, default: ``1``
+        Total number of workers available for ray. This is ignored if ``use_ray``
+        is ``False``.
+    ray_address : :obj:`str`, default: ``"auto"``
         Ray cluster address to connect to.
 
     Returns
     -------
     :obj:`numpy.ndarray`
         Energies with lower-order contributions added or removed.
     :obj:`numpy.ndarray`
         Derivatives with lower-order contributions added or removed.
     """
+    if use_ray:
+        if not ray.is_initialized():
+            log.debug("ray is not initialized")
+            # Try to connect to already running ray service (from ray cli).
+            try:
+                log.debug("Trying to connect to ray at address %r", ray_address)
+                ray.init(address=ray_address)
+            except ConnectionError:
+                log.debug("Failed to connect to ray at %r", ray_address)
+                log.debug("Trying to initialize ray with %d cores", n_workers)
+                ray.init(num_cpus=n_workers)
+            log.debug("Successfully initialized ray")
+        else:
+            log.debug("Ray was already initialized")
+    else:
+        log.debug("Not using ray")
+
     log.debug("Computing many-body expansion contributions")
     if operation not in ("add", "remove"):
         raise ValueError(f'{operation} is not "add" or "remove"')
     log.debug("MBE operation : %s", operation)
 
     # Checks that the r_prov_md5 hashes match the same r_prov_id
     if (r_prov_ids is not None) and (r_prov_ids != {}):
@@ -386,14 +414,15 @@
             )
 
         # Run all workers.
         while len(worker_list) != 0:
             done_id, worker_list = ray.wait(worker_list)
 
             r_idxs_worker, E_worker, Deriv_worker = ray.get(done_id)[0]
+            log.debug("Worker %r has finished", done_id)
             if operation == "remove":
                 E[r_idxs_worker] -= E_worker
                 Deriv[r_idxs_worker] -= Deriv_worker
             elif operation == "add":
                 E[r_idxs_worker] += E_worker
                 Deriv[r_idxs_worker] += Deriv_worker
 
@@ -402,16 +431,16 @@
 
 def decomp_to_total(
     E_nbody,
     F_nbody,
     entity_ids,
     entity_combs,
     use_ray=False,
+    n_workers=1,
     ray_address="auto",
-    n_workers=2,
 ):
     r"""Sum decomposed :math:`n`-body energies and forces for total
     :math:`n`-body contribution.
 
     This is a wrapper around :func:`mbgdml.mbe.mbe_contrib`.
 
     Parameters
@@ -427,19 +456,19 @@
         supersystem (not the :math:`n`-body structure).
     entity_combs : :obj:`numpy.ndarray`, ndim: ``2``
         Structure indices and Entity IDs of all structures in increasing
         order of :math:`n`. Column 0 is the structure index and
         the remaining columns are entity IDs.
     use_ray : :obj:`bool`, default: ``False``
         Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
-        calculations.
-    n_workers : :obj:`int`, default: ``2``
-        Number of ray workers to use. This is ignored if ``use_ray`` is
-        ``False``.
-    ray_address : :obj:`str`, default: ``'auto'``
+        computations.
+    n_workers : :obj:`int`, default: ``1``
+        Total number of workers available for ray. This is ignored if ``use_ray``
+        is ``False``.
+    ray_address : :obj:`str`, default: ``"auto"``
         Ray cluster address to connect to.
 
     Returns
     -------
     :obj:`numpy.ndarray`, ndim: ``1``
         Total :math:`n`-body energies.
     """
@@ -469,16 +498,16 @@
         E_nbody,
         F_nbody,
         entity_ids_lower,
         {0: ""},
         r_prov_specs_lower,
         operation="add",
         use_ray=use_ray,
-        ray_address=ray_address,
         n_workers=n_workers,
+        ray_address=ray_address,
     )
     return E, F
 
 
 class mbePredict:
     r"""Predict energies and forces of structures using machine learning
     many-body models.
@@ -490,93 +519,216 @@
     """
 
     def __init__(
         self,
         models,
         predict_model,
         use_ray=False,
-        n_workers=2,
+        n_workers=1,
         ray_address="auto",
         wkr_chunk_size=None,
         alchemy_scalers=None,
         periodic_cell=None,
+        compute_stress=False,
     ):
-        """
+        r"""
         Parameters
         ----------
         models : :obj:`list` of :obj:`mbgdml.models.Model`
             Machine learning model objects that contain all information to make
             predictions using ``predict_model``.
         predict_model : ``callable``
-            A function that takes ``Z, R, entity_ids, nbody_gen, model`` and
-            computes energies and forces. This will be turned into a ray remote
+            A function that takes ``Z``, ``R``, ``entity_ids``, ``nbody_gen``, ``model``
+            and computes energies and forces. This will be turned into a ray remote
             function if ``use_ray`` is ``True``. This can return total properties
             or all individual :math:`n`-body energies and forces.
         use_ray : :obj:`bool`, default: ``False``
-            Parallelize predictions using ray.
-        n_workers : :obj:`int`, default: ``2``
-            Total number of workers available for predictions when using ray.
-            This is ignored if ``use_ray`` is ``False``.
-        ray_address : :obj:`str`, default: ``'auto'``
+            Use `ray <https://docs.ray.io/en/latest/>`__ to parallelize
+            computations.
+        n_workers : :obj:`int`, default: ``1``
+            Total number of workers available for ray. This is ignored if ``use_ray``
+            is ``False``.
+        ray_address : :obj:`str`, default: ``"auto"``
             Ray cluster address to connect to.
         wkr_chunk_size : :obj:`int`, default: :obj:`None`
             Number of :math:`n`-body structures to assign to each spawned
             worker with ray. If :obj:`None`, it will divide up the number of
             predictions by ``n_workers``.
-        alchemical_scaling : :obj:`list` of ``mbgdml.alchemy.mbeAlchemyScale``,
+        alchemical_scaling : :obj:`list` of :class:`~mbgdml.alchemy.mbeAlchemyScale`, \
         default: :obj:`None`
             Alchemical scaling of :math:`n`-body interactions of entities.
+
+            .. warning::
+
+                This has not been thoroughly tested.
         periodic_cell : :obj:`mbgdml.periodic.Cell`, default: :obj:`None`
             Use periodic boundary conditions defined by this object. If this
-            is not :obj:`None` only ``mbePredict.predict()`` can be used.
+            is not :obj:`None` only :meth:`~mbgdml.mbe.mbePredict.predict` can be used.
+        compute_stress : :obj:`bool`, default: ``False``
+
+            .. danger::
+
+                This implementation is experimental and has not been verified. We do
+                not recommend using this.
+
+            Compute the internal virial contribution,
+            :math:`\mathbf{W} \left( \mathbf{r}^N \right) / V`, of :math:`N`
+            particles at positions :math:`\mathbf{r}` to the pressure stress tensor of
+            a periodic box with volume :math:`V`. The kinetic contribution is not
+            computed here.
         """
         self.models = models
         self.predict_model = predict_model
 
         if models[0].type == "gap":
             assert not use_ray
         elif models[0].type == "schnet":
             assert not use_ray
 
-        self.use_ray = use_ray
+        self.use_ray = use_ray  # Do early because some setters are dependent on this.
         self.n_workers = n_workers
         self.wkr_chunk_size = wkr_chunk_size
         if alchemy_scalers is None:
             alchemy_scalers = []
         self.alchemy_scalers = alchemy_scalers
         self.periodic_cell = periodic_cell
+        self.compute_stress = compute_stress
+
+        self.virial_form = "group"
+        r"""The form to use from
+        `10.1063/1.3245303 <https://doi.org/10.1063/1.3245303>`__ to compute the
+        internal virial contribution to the pressure stress tensor.
+        :math:`\mathbf{W} \left( \mathbf{r}^N \right)` is the internal virial of
+        :math:`N` atoms and :math:`\otimes` is the outer tensor product (i.e.,
+        ``np.multiply.outer``).
+
+        ``group`` (**default**)
+
+            This computes the virial by considering contributions based on groups
+            of atoms. The number of groups, number of atoms in each group, and
+            number of groups is completely arbitrary. Thus, we can straightforwardly
+            use :math:`n`-body combinations as groups and get more insight into
+            the virial contributions origin.
+
+            .. math::
+
+                \mathbf{W} \left( \mathbf{r}^N \right) =
+                \sum_{k \in \mathbf{0}} \sum_{w = 1}^{N_k} \mathbf{r}_w^k
+                \otimes \mathbf{F}_w^k.
+
+            Here, :math:`k` is a group of atoms that must be in the local cell
+            (i.e., :math:`k \in \mathbf{0}`). :math:`w` is the atom index within
+            group :math:`k` (:math:`N_k` is the total number of atoms in the group).
+
+            .. important::
+
+                This has to be specifically implemented in the relevant predictor
+                functions.
+
+        ``finite_diff``
+
+            Uses finite differences by perturbing the cell vectors.
+
+        :type: :obj:`str`
+        """
+        self.finite_diff_dh = 1e-4
+        r"""Forward and backward displacement of the cell vectors for finite
+        differences.
+
+        Default: ``1e-4``
+
+        :type: :obj:`float`
+        """
+        self.use_voigt = False
+        r"""Convert the stress tensor to the 1D Voigt notation (xx, yy, zz, yz, xz, xy).
+
+        Default: ``False``
+
+        :type: :obj:`bool`
+        """
+        self.only_normal_stress = False
+        r"""Only compute normal (xx, yy, and zz) stress. All other elements will be
+        zero. This is recommended for MD simulations to avoid altering box angular
+        momentum due to the antisymmetric contributions (yz, xz, and xy).
+
+        Default: ``False``
+
+        :type: :obj:`bool`
+        """
+        self.box_scaling_type = "anisotropic"
+        r"""Treatment of box scaling when
+        :attr:`mbgdml.mbe.mbePredict.only_normal_stress` is ``True``.
+
+        ``anisotropic`` (**default**)
+
+            No modifications are made to normal stresses which allows box vectors
+            to scale independently.
+
+        ``isotropic``
+
+            Average the normal stresses so box vectors will scale identically.
+
+        :type: :obj:`str`
+        """
+
         if use_ray:
             if not ray.is_initialized():
-                ray.init(address=ray_address)
-            assert ray.is_initialized()
+                log.debug("ray is not initialized")
+                # Try to connect to already running ray service (from ray cli).
+                try:
+                    log.debug("Trying to connect to ray at address %r", ray_address)
+                    ray.init(address=ray_address)
+                except ConnectionError:
+                    log.debug("Failed to connect to ray at %r", ray_address)
+                    log.debug("Trying to initialize ray with %d cores", n_workers)
+                    ray.init(num_cpus=n_workers)
+                log.debug("Successfully initialized ray")
+            else:
+                log.debug("Ray was already initialized")
 
             self.models = [ray.put(model) for model in models]
             # if alchemy_scalers is not None:
             #    self.alchemy_scalers = [
             #        ray.put(scaler) for scaler in alchemy_scalers
             #    ]
             self.predict_model = ray.remote(predict_model)
-            if periodic_cell is not None:
-                self.periodic_cell = ray.put(periodic_cell)
+
+    @property
+    def periodic_cell(self):
+        r"""Periodic cell for MBE predictions.
+
+        :type: :obj:`mbgdml.periodic.Cell`
+        """
+        if hasattr(self, "_periodic_cell"):
+            return self._periodic_cell
+
+        return None
+
+    @periodic_cell.setter
+    def periodic_cell(self, var):
+        if var is not None:
+            if self.use_ray:
+                var = ray.put(var)
+        self._periodic_cell = var
 
     def get_avail_entities(self, comp_ids_r, comp_ids_model):
         r"""Determines available ``entity_ids`` for each ``comp_id`` in a
         structure.
 
         Parameters
         ----------
         comp_ids_r : :obj:`numpy.ndarray`, ndim: ``1``
             Component IDs of the structure to predict.
         comp_ids_model : :obj:`numpy.ndarray`, ndim: ``1``
             Component IDs of the model.
 
         Returns
         -------
-        :obj:`list`, length: ``len(comp_ids_r)``
-
+        :obj:`list`
+            (length: ``len(comp_ids_r)``)
         """
         # Models have a specific entity order that needs to be conserved in the
         # predictions. Here, we create a ``avail_entity_ids`` list where each item
         # is a list of all entities in ``r`` that match the model entity.
         avail_entity_ids = []
         for comp_id in comp_ids_model:
             matching_entity_ids = np.where(comp_id == comp_ids_r)[0]
@@ -605,29 +757,29 @@
         model : :obj:`mbgdml.models.Model`
             Model that contains all information needed by ``model_predict``.
 
         Returns
         -------
         :obj:`float`
             Total :math:`n`-body energy of ``r``.
-        :obj:`numpy.ndarray`, shape: ``(len(Z), 3)``
-            Total :math:`n`-body atomic forces of ``r``.
+        :obj:`numpy.ndarray`
+            (shape: ``(len(Z), 3)``) - Total :math:`n`-body atomic forces of ``r``.
+        :obj:`numpy.ndarray`
+            (optional, shape: ``(len(Z), 3)``) - The internal virial
+            contribution to the pressure stress tensor in units of energy.
         """
         # Unify r shape.
         if R.ndim == 3:
             log.debug("R has three dimensions (instead of two)")
             if R.shape[0] == 1:
                 log.debug("R[0] was selected to proceed")
                 R = R[0]
             else:
                 raise ValueError("R.ndim is not 2 (only one structure is allowed)")
 
-        E = 0.0
-        F = np.zeros(R.shape, dtype=np.double)
-
         # Creates a generator for all possible n-body combinations regardless
         # of cutoffs.
         if self.use_ray:
             model_comp_ids = ray.get(model).comp_ids
         else:
             model_comp_ids = model.comp_ids
         avail_entity_ids = self.get_avail_entities(comp_ids, model_comp_ids)
@@ -639,21 +791,34 @@
             nbody_order = len(model_comp_ids)
             kwargs_pred["alchemy_scalers"] = [
                 alchemy_scaler
                 for alchemy_scaler in self.alchemy_scalers
                 if alchemy_scaler.order == nbody_order
             ]
 
+        periodic_cell = self.periodic_cell
+        compute_stress = (
+            self.compute_stress and bool(periodic_cell) and self.virial_form == "group"
+        )
+        if compute_stress:
+            virial = np.zeros((3, 3), dtype=np.float64)
+            kwargs_pred["compute_virial"] = True
+
         # Runs the predict_model function to calculate all n-body energies
         # with this model.
         if not self.use_ray:
-            E, F = self.predict_model(
-                Z, R, entity_ids, nbody_gen, model, self.periodic_cell, **kwargs_pred
+            E, F, *virial_model = self.predict_model(
+                Z, R, entity_ids, nbody_gen, model, periodic_cell, **kwargs_pred
             )
+            if compute_stress:
+                virial += virial_model[0]
         else:
+            E = 0.0
+            F = np.zeros(R.shape, dtype=np.float64)
+
             # Put all common data into the ray object store.
             Z = ray.put(Z)
             R = ray.put(R)
             entity_ids = ray.put(entity_ids)
 
             nbody_gen = tuple(nbody_gen)
             if self.wkr_chunk_size is None:
@@ -670,41 +835,47 @@
                 workers.append(
                     predict_model.remote(
                         Z,
                         R,
                         entity_ids,
                         chunk,
                         model,
-                        self.periodic_cell,
+                        periodic_cell,
                         **kwargs_pred,
                     )
                 )
 
             for _ in range(self.n_workers):
                 try:
                     chunk = next(nbody_chunker)
                     add_worker(workers, chunk)
                 except StopIteration:
                     break
 
             # Start workers and collect results.
             while len(workers) != 0:
                 done_id, workers = ray.wait(workers)
-                E_worker, F_worker = ray.get(done_id)[0]
+                E_worker, F_worker, *virial_model = ray.get(done_id)[0]
+
                 E += E_worker
                 F += F_worker
+                if compute_stress:
+                    virial += virial_model[0]
+
                 try:
                     chunk = next(nbody_chunker)
                     add_worker(workers, chunk)
                 except StopIteration:
                     pass
 
             # Cleanup object store
-            del Z, R, entity_ids
+            del Z, entity_ids
 
+        if compute_stress:
+            return E, F, virial
         return E, F
 
     # pylint: disable=too-many-branches, too-many-statements
     def compute_nbody_decomp(self, Z, R, entity_ids, comp_ids, model):
         r"""Compute all :math:`n`-body contributions of a single structure
         using a :obj:`mbgdml.models.Model` object.
 
@@ -727,23 +898,25 @@
             Relates each ``entity_id`` to a fragment label. Each item's index
             is the label's ``entity_id``.
         model : :obj:`mbgdml.models.Model`
             Model that contains all information needed by ``model_predict``.
 
         Returns
         -------
-        :obj:`numpy.ndarray`, ndim: ``1``
+        :obj:`numpy.ndarray`
+            (ndim: ``1``) -
             Energies of all possible :math:`n`-body structures. Some elements
             can be :obj:`numpy.nan` if they are beyond the descriptor cutoff.
-        :obj:`numpy.ndarray`, ndim: ``3``
+        :obj:`numpy.ndarray`
+            (ndim: ``3``) -
             Atomic forces of all possible :math:`n`-body structure. Some
             elements can be :obj:`numpy.nan` if they are beyond the descriptor
             cutoff.
-        :obj:`numpy.ndarray`, ndim: ``2``
-            All possible entity IDs.
+        :obj:`numpy.ndarray`
+            (ndim: ``2``) - All possible entity IDs.
         """
         # Unify r shape.
         if R.ndim == 3:
             log.debug("R has three dimensions (instead of two)")
             if R.shape[0] == 1:
                 log.debug("R[0] was selected to proceed")
                 R = R[0]
@@ -846,33 +1019,89 @@
             Integers specifying which atoms belong to which entities.
         comp_ids : :obj:`numpy.ndarray`, shape: ``(N,)``
             Relates each ``entity_id`` to a fragment label. Each item's index
             is the label's ``entity_id``.
 
         Returns
         -------
-        :obj:`numpy.ndarray`, shape: ``(N,)``
-            Predicted many-body energy
-        :obj:`numpy.ndarray`, shape: ``(N, len(Z), 3)``
-            Predicted atomic forces.
+        :obj:`numpy.ndarray`
+            (shape: ``(N,)``) - Predicted many-body energy
+        :obj:`numpy.ndarray`
+            (shape: ``(N, len(Z), 3)``) - Predicted atomic forces.
+        :obj:`numpy.ndarray`
+            (optional, shape: ``(N, len(Z), 3)``) - The pressure stress tensor in units
+            of energy/distance\ :sup:`3`.
         """
         t_predict = log.t_start()
         if R.ndim == 2:
             R = np.array([R])
+        n_R = R.shape[0]
+        compute_stress = self.compute_stress and bool(self.periodic_cell)
 
         # Preallocate memory for energies and forces.
-        E = np.zeros((R.shape[0],), dtype=np.double)
-        F = np.zeros(R.shape, dtype=np.double)
+        E = np.zeros((n_R,), dtype=np.float64)
+        F = np.zeros(R.shape, dtype=np.float64)
+        if compute_stress:
+            assert self.virial_form in ("group", "finite_diff")
+            stress = np.zeros((n_R, 3, 3), dtype=np.float64)
 
         # Compute all energies and forces with every model.
         for i, r in enumerate(R):
             for model in self.models:
-                E_nbody, F_nbody = self.compute_nbody(Z, r, entity_ids, comp_ids, model)
+                # Extra returns are present for stress. The *stress_nbody captures it.
+                # If it is not requested, it will just be an empty list.
+                E_nbody, F_nbody, *virial_nbody = self.compute_nbody(
+                    Z, r, entity_ids, comp_ids, model
+                )
                 E[i] += E_nbody
                 F[i] += F_nbody
+                if compute_stress and self.virial_form == "group":
+                    stress[i] += virial_nbody[0]
+
+            if compute_stress and self.virial_form == "finite_diff":
+                periodic_cell = self.periodic_cell
+                if self.use_ray:
+                    periodic_cell = ray.get(periodic_cell)
+                cell_v = periodic_cell.cell_v
+                stress[i] = virial_finite_diff(
+                    Z,
+                    r,
+                    entity_ids,
+                    comp_ids,
+                    cell_v,
+                    self,
+                    only_normal_stress=self.only_normal_stress,
+                )
+
+        if compute_stress:  # pylint: disable=too-many-nested-blocks
+            periodic_cell = self.periodic_cell
+            if self.use_ray:
+                periodic_cell = ray.get(periodic_cell)
+            stress /= periodic_cell.volume
+
+            if self.only_normal_stress:
+                for n in range(stress.shape[0]):
+                    for i in range(0, 3):
+                        for j in range(0, 3):
+                            if i != j:
+                                stress[n][i][j] = 0.0
+
+                    if self.box_scaling_type == "isotropic":
+                        stress_average = np.trace(stress[n]) / 3
+                        for i in range(0, 3):
+                            stress[n][i][i] = stress_average
+
+            if self.use_voigt:
+                stress = np.array([to_voigt(r_stress) for r_stress in stress])
+
+            log.t_stop(
+                t_predict, message="Predictions took {time} s", precision=3, level=10
+            )
+            return E, F, stress
+
         log.t_stop(
             t_predict, message="Predictions took {time} s", precision=3, level=10
         )
         return E, F
 
     def predict_decomp(self, Z, R, entity_ids, comp_ids):
         r"""Predict the energies and forces of one or multiple structures.
```

### Comparing `mbGDML-0.0.4/mbgdml/models/base.py` & `mbGDML-0.1.0/mbgdml/models/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,17 +16,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
+from ..logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 class Model:
     r"""A parent class for machine learning model objects.
 
     Attributes
     ----------
```

### Comparing `mbGDML-0.0.4/mbgdml/models/gap_model.py` & `mbGDML-0.1.0/mbgdml/models/gap_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,26 +17,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import hashlib
-import logging
 import numpy as np
 from .base import Model
+from ..logger import GDMLLogger
 
 try:
     import quippy
 
     _HAS_QUIPPY = True
 except ImportError:
     _HAS_QUIPPY = False
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 # pylint: disable-next=invalid-name
 class gapModel(Model):
     def __init__(
         self,
         model_path,
         comp_ids,
```

### Comparing `mbGDML-0.0.4/mbgdml/models/gdml_model.py` & `mbGDML-0.1.0/mbgdml/models/gdml_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2022 Stefan Chmiela, Gregory Fonseca
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,22 +17,22 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
 from .base import Model
 from ..utils import md5_data
 from .._gdml.desc import _from_r
 from .. import __version__ as mbgdml_version
+from ..logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 # pylint: disable-next=invalid-name
 class gdmlModel(Model):
     def __init__(self, model, comp_ids=None, criteria=None, for_predict=True):
         """
         Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/models/schnet_model.py` & `mbGDML-0.1.0/mbgdml/models/schnet_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,26 +17,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import hashlib
-import logging
 import numpy as np
 from .base import Model
+from ..logger import GDMLLogger
 
 try:
     import torch
 
     _HAS_TORCH = True
 except ImportError:
     _HAS_TORCH = False
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 # pylint: disable-next=invalid-name
 class schnetModel(Model):
     def __init__(self, model_path, comp_ids, device, criteria=None):
         """
         Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/periodic.py` & `mbGDML-0.1.0/mbgdml/periodic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,41 +21,45 @@
 # SOFTWARE.
 
 """Periodic boundary conditions."""
 
 from ase.geometry import find_mic
 import numpy as np
 from scipy.spatial.distance import pdist
+from .logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 
 class Cell:
     r"""Enables :math:`n`-body predictions under periodic boundary conditions.
 
     The minimum-image convention (mic) is used to reformat :math:`n`-body
     structures in a form resembling non-periodic structures.
     """
 
-    def __init__(self, cell_v, cutoff, pbc=True):
+    def __init__(self, cell_v, cutoff=None, pbc=True):
         r"""
         Parameters
         ----------
         cell_v : :obj:`numpy.ndarray`, shape: ``(3, 3)``
             The three cell vectors. For example, a cube of length 9.0 would be
             ``[[9.0, 0.0, 0.0], [0.0, 9.0, 0.0], [0.0, 0.0, 9.0]]``.
-        cutoff : :obj:`float`
-            A periodic image interaction cutoff. Must not be larger than half
-            the cube length (non-cubic cells might have slightly larger
-            cutoffs).
+        cutoff : :obj:`float`, default: ``None``
+            A periodic image interaction cutoff. Must be smaller than half
+            the smallest cube length (non-cubic cells might have slightly larger
+            cutoffs). Is automatically calculated if this is ``None``.
         pbc : :obj:`list` or :obj:`bool`
             Periodic boundary conditions in x-, y- and z-direction. Default is
             to assume periodic boundaries in all directions
             (i.e., ``pbc=True``).
         """
         self.cell_v = cell_v
-        self.cutoff = cutoff
+        if cutoff is not None:
+            self.cutoff = cutoff
         self.pbc = pbc
 
     def d_mic(self, d, check_cutoff=True):
         r"""Applies the minimum-image convention to distance vectors.
 
         Also checks that all atomic pairwise distances are less than
         ``self.cutoff``. If any are equal to greater than the cutoff then it
@@ -99,14 +103,33 @@
         """
         # Computes the distance from the first atom.
         assert r.ndim == 2
         d = np.subtract(r, r[0, :])
         return self.d_mic(d)
 
     @property
+    def cell_v(self):
+        r"""The three cell vectors. For example, a cube of length 9.0 would be
+        ``[[9.0, 0.0, 0.0], [0.0, 9.0, 0.0], [0.0, 0.0, 9.0]]``.
+
+        :type: :obj:`numpy.ndarray`
+        """
+        if hasattr(self, "_cell_v"):
+            return self._cell_v
+
+        return None
+
+    @cell_v.setter
+    def cell_v(self, var):
+        var = np.array(var)
+        self._cell_v = var
+        # Update the cutoff
+        self.cutoff = np.min(np.linalg.norm(var, axis=1)) / 2.0
+
+    @property
     def volume(self):
         r"""Volume of the periodic cell.
 
         The volume of the parallelepiped described by ``cell_v``
         (:math:`\boldsymbol{v}`) is computed with
 
         .. math::
```

### Comparing `mbGDML-0.0.4/mbgdml/predictors/gap_predict.py` & `mbGDML-0.1.0/mbgdml/predictors/gap_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,19 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
 import ase
+from ..logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 # Possible ray task.
 # pylint: disable-next=unused-argument
 def predict_gap(Z, R, entity_ids, entity_combs, model, periodic_cell, **kwargs):
     r"""Predict total :math:`n`-body energy and forces of a single structure.
 
     Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/predictors/gdml_predict.py` & `mbGDML-0.1.0/mbgdml/predictors/gdml_predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2022 Stefan Chmiela, Gregory Fonseca
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,18 +17,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
+from ..logger import GDMLLogger
+from ..stress import virial_atom_loop
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 # This calculation is too fast to be a ray task.
 # pylint: disable-next=too-many-statements
 def _predict_gdml_wkr(
     r_desc,
     r_d_desc,
     n_atoms,
@@ -169,15 +170,15 @@
 def predict_gdml(Z, R, entity_ids, entity_combs, model, periodic_cell, **kwargs):
     r"""Predict total :math:`n`-body energy and forces of a single structure.
 
     Parameters
     ----------
     Z : :obj:`numpy.ndarray`, ndim: ``1``
         Atomic numbers of all atoms in ``r`` (in the same order).
-    r : :obj:`numpy.ndarray`, ndim: ``2``
+    R : :obj:`numpy.ndarray`, ndim: ``2``
         Cartesian coordinates of a single structure to predict.
     entity_ids : :obj:`numpy.ndarray`, ndim: ``1``
         1D array specifying which atoms belong to which entities.
     entity_combs : ``iterable``
         Entity ID combinations (e.g., ``(53,)``, ``(0, 2)``,
         ``(32, 55, 293)``, etc.) to predict using this model. These are used
         to slice ``r`` with ``entity_ids``.
@@ -194,76 +195,84 @@
         Predicted :math:`n`-body forces.
     """
     assert R.ndim == 2
     E = 0.0
     F = np.zeros(R.shape)
 
     alchemy_scalers = kwargs.get("alchemy_scalers", None)
+    compute_virial = kwargs.get("compute_virial", False)
 
     periodic = bool(periodic_cell)
+    compute_virial = bool(periodic and compute_virial)
+    if compute_virial:
+        virial = np.zeros((3, 3), dtype=np.float64)
 
     # Getting all contributions for each molecule combination (comb).
     for entity_id_comb in entity_combs:
 
         # Gets indices of all atoms in the combination of molecules.
         # r_slice is a list of the atoms for the entity_id combination.
         r_slice = []
         for entity_id in entity_id_comb:
             r_slice.extend(np.where(entity_ids == entity_id)[0])
 
-        z_comp = Z[r_slice]
-        r_comp = R[r_slice]
+        z = Z[r_slice]
+        r = R[r_slice]
+        # Note: We store the original coordinates in case the virial is requested
 
         # If we are using a periodic cell we convert r_comp into coordinates
         # we can use in many-body expansions.
         if periodic:
-            r_comp = periodic_cell.r_mic(r_comp)
-            if r_comp is None:
+            r = periodic_cell.r_mic(r)
+            if r is None:
                 # Any atomic pairwise distance was larger than cutoff.
                 continue
 
-        # TODO: Check if we can avoid prediction if we have an alchemical factor of
-        # zero?
-
         # Checks criteria cutoff if present and desired.
         if model.criteria is not None:
-            accept_r, _ = model.criteria.accept(z_comp, r_comp)
+            accept_r, _ = model.criteria.accept(z, r)
             if not accept_r:
                 # Do not include this contribution.
                 continue
 
         # Predicts energies and forces.
-        r_desc, r_d_desc = model.desc_func(r_comp.flatten(), model.lat_and_inv)
+        r_desc, r_d_desc = model.desc_func(r.flatten(), model.lat_and_inv)
         wkr_args = (
             r_desc,
             r_d_desc,
-            len(z_comp),
+            len(z),
             model.sig,
             model.n_perms,
             model.R_desc_perms,
             model.R_d_desc_alpha_perms,
             model.alphas_E_lin,
         )
         out = _predict_gdml_wkr(*wkr_args)
 
         out *= model.stdev
         e = out[0] + model.integ_c
-        f = out[1:].reshape((len(z_comp), 3))
+        f = out[1:].reshape((len(z), 3))
 
         # Scale contribution if entity is included.
         if alchemy_scalers not in (None, []):
             for alchemy_scaler in alchemy_scalers:
                 if alchemy_scaler.entity_id in entity_id_comb:
-                    E = alchemy_scaler.scale(E)
-                    F = alchemy_scaler.scale(F)
+                    e = alchemy_scaler.scale(e)
+                    f = alchemy_scaler.scale(f)
 
         # Adds contributions to total energy and forces.
         E += e
         F[r_slice] += f
 
+        if compute_virial:
+            virial += virial_atom_loop(r, f)
+
+    if compute_virial:
+        return E, F, virial
+
     return E, F
 
 
 def predict_gdml_decomp(Z, R, entity_ids, entity_combs, model, **kwargs):
     r"""Predict all :math:`n`-body energies and forces of a single structure.
 
     Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/predictors/schnet_predict.py` & `mbGDML-0.1.0/mbgdml/predictors/schnet_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,17 +16,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import numpy as np
 import ase
+from ..logger import GDMLLogger
 
 try:
     import schnetpack
 
     _HAS_SCHNETPACK = True
 except ImportError:
     _HAS_SCHNETPACK = False
@@ -34,15 +34,15 @@
 try:
     import torch
 
     _HAS_TORCH = True
 except ImportError:
     _HAS_TORCH = False
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 # pylint: disable-next=unused-argument
 def predict_schnet(Z, R, entity_ids, entity_combs, model, periodic_cell, **kwargs):
     r"""Predict total :math:`n`-body energy and forces of a single structure.
 
     Parameters
```

### Comparing `mbGDML-0.0.4/mbgdml/train.py` & `mbGDML-0.1.0/mbgdml/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2020, Stefan Chmiela
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,27 +19,27 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import shutil
-import logging
 import numpy as np
 from bayes_opt import BayesianOptimization, SequentialDomainReductionTransformer
 
 from .models import gdmlModel
 from .analysis.problematic import ProblematicStructures
 from .predictors import predict_gdml
 from ._gdml.train import GDMLTrain, model_errors, add_valid_errors
 from ._gdml.train import save_model, get_test_idxs
 from .utils import save_json
 from .losses import loss_f_rmse, mae, rmse
+from .logger import GDMLLogger
 
-log = logging.getLogger(__name__)
+log = GDMLLogger(__name__)
 
 
 class mbGDMLTrain:
     r"""Train many-body GDML models."""
 
     def __init__(
         self,
@@ -76,16 +76,15 @@
             trained to the energies. This is rarely
             useful for higher order *n*-body models.
         use_cprsn : :obj:`bool`, default: ``False``
             Compresses the kernel matrix along symmetric degrees of freedom to
             try to reduce training time. Usually does not provide significant
             benefits.
         solver : :obj:`str`, default: ``'analytic'``
-            The GDML solver to use. Currently the only option is
-            ``'analytic'``.
+            The GDML solver to use, either ``analytic`` or ``iterative``.
         lam : :obj:`float`, default: ``1e-10``
             Hyper-parameter lambda (regularization strength). This generally
             does not need to change.
         solver_tol : :obj:`float`, default: ``1e-4``
            Solver tolerance.
         use_torch : :obj:`bool`, default: ``False``
             Use PyTorch to enable GPU acceleration.
@@ -182,15 +181,15 @@
                 'kappa': 1.5
             }
 
 
         :type: :obj:`dict`
         """
         self.bayes_opt_params_final = None
-        r"""Bayesian optimization parameters for the final iterative model.
+        r"""Bayesian optimization parameters for the final model.
 
         If :obj:`None`, then ``bayes_opt_params`` are used.
 
         Default: :obj:`None`
 
         :type: :obj:`dict`
         """
@@ -1038,30 +1037,30 @@
         # Saving model.
         save_path = os.path.join(save_dir, model_name)
         model_best.save(save_path)
 
         log.t_stop(t_job, message="\nJob duration : {time} s", precision=2)
         return model_best.model_dict
 
-    def iterative_train(
+    def active_train(
         self,
         dataset,
         model_name,
         n_train_init,
         n_train_final,
         n_valid,
         model0=None,
         n_train_step=100,
         n_test=None,
         save_dir=".",
         overwrite=False,
         write_json=True,
         write_idxs=True,
     ):
-        r"""Iteratively trains a GDML model by using Bayesian optimization and
+        r"""Trains a GDML model by using Bayesian optimization and
         adding problematic (high error) structures to the training set.
 
         Trains a GDML model with :meth:`mbgdml.train.mbGDMLTrain.bayes_opt`.
 
         Parameters
         ----------
         dataset : :obj:`mbgdml.data.DataSet`
@@ -1074,16 +1073,16 @@
             is the size of that model.
         n_train_final : :obj:`int`
             Training set size of the final model.
         n_valid : :obj:`int`
             Size of the validation set to be used for each training task.
             Different structures are sampled for each training task.
         model0 : :obj:`dict`, default: :obj:`None`
-            Initial model to start iterative training with. Training indices
-            will be taken from here.
+            Initial model to start training with. Training indices will be taken from
+            here.
         n_train_step : :obj:`int`, default: ``100``
             Number of problematic structures to add to the training set for
             each iteration.
         n_test : :obj:`int`, default: :obj:`None`
             The number of test points to test the validated GDML model.
             Defaults to testing all available structures.
         save_dir : :obj:`str`, default: ``'.'``
@@ -1096,15 +1095,15 @@
             Write npy files for training, validation, and test indices.
         """
         log.log_package()
 
         t_job = log.t_start()
         log.info(
             "###################\n"
-            "#    Iterative    #\n"
+            "#    Active       #\n"
             "#    Training     #\n"
             "###################\n"
         )
         log.info("Initial training set size : %r", n_train_init)
         if model0 is not None:
             log.info("Initial model was provided")
             log.info("Taking training indices from model")
```

### Comparing `mbGDML-0.0.4/mbgdml/utils.py` & `mbGDML-0.1.0/mbgdml/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020-2022, Alex M. Maldonado
+# Copyright (c) 2020-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,14 +24,17 @@
 import hashlib
 import itertools
 import json
 import numpy as np
 import cclib
 from qcelemental import periodictable as ptable
 from .descriptors import get_center_of_mass
+from .logger import GDMLLogger
+
+log = GDMLLogger(__name__)
 
 
 def get_files(path, expression, recursive=True):
     r"""Returns paths to all files in a given directory that matches a provided
     expression in the file name.
 
     Parameters
@@ -159,14 +162,59 @@
                     comment += "\n"
             else:
                 comment = "\n"
             f.write(comment)
             f.write(string_xyz_arrays(Z, r, precision=data_precision))
 
 
+def parse_xyz(xyz_path):
+    r"""Parses data from xyz file.
+
+    An xyz file is data presented as consecutive xyz structures. The data could be
+    three Cartesian coordinates for each atom, three atomic force vector
+    components, or both coordinates and atomic forces in one line (referred to
+    as extended xyz).
+
+    Parameters
+    ----------
+    xyz_path : :obj:`str`
+        Path to xyz file.
+
+    Returns
+    -------
+    :obj:`tuple` [:obj:`list`]
+        Parsed atoms (as element symbols :obj:`str`), comments, and data as
+        :obj:`float` from string file.
+    """
+    Z, comments, data = [], [], []
+    with open(xyz_path, "r", encoding="utf-8") as f:
+        for _, line in enumerate(f):
+            line = line.strip()
+            if not line:
+                # Skips blank lines
+                pass
+            else:
+                line_split = line.split()
+                if (
+                    len(line_split) == 1
+                    and float(line_split[0]) % int(line_split[0]) == 0.0
+                ):
+                    # Skips number of atoms line, adds comment line, and
+                    # prepares next z and data item.
+                    comment_line = next(f)
+                    comments.append(comment_line.strip())
+                    Z.append([])
+                    data.append([])
+                else:
+                    # Grabs z and data information.
+                    Z[-1].append(line_split[0])
+                    data[-1].append([float(i) for i in line_split[1:]])
+    return Z, comments, data
+
+
 def convert_forces(forces, e_units_calc, r_units_calc, e_units, r_units):
     r"""Converts forces (or gradients) to specified units.
 
     Parameters
     ----------
     forces : :obj:`numpy.ndarray`
         An array with units of energy and distance matching `e_units_calc`
@@ -367,16 +415,17 @@
     -------
     :obj:`numpy.ndarray`
         Centered Cartesian atomic coordinates.
     """
     # Masses of each atom in the same shape of R.
     if R.ndim == 2:
         R = np.array([R])
+    n_atoms = R.shape[1]
 
-    R -= np.repeat(get_center_of_mass(Z, R), R.shape[1]).reshape(R.shape)
+    R -= np.repeat(get_center_of_mass(Z, R), n_atoms, axis=0).reshape(R.shape)
 
     if R.shape[0] == 1:
         R = R[0]
 
     return R
```

### Comparing `mbGDML-0.0.4/setup.cfg` & `mbGDML-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mbGDML-0.0.4/setup.py` & `mbGDML-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.0.4/versioneer.py` & `mbGDML-0.1.0/versioneer.py`

 * *Files identical despite different names*

