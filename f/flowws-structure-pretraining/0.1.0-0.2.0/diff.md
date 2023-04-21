# Comparing `tmp/flowws-structure-pretraining-0.1.0.tar.gz` & `tmp/flowws-structure-pretraining-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowws-structure-pretraining-0.1.0.tar", last modified: Tue Sep 13 20:28:29 2022, max compression
+gzip compressed data, was "flowws-structure-pretraining-0.2.0.tar", last modified: Fri Apr 21 19:05:46 2023, max compression
```

## Comparing `flowws-structure-pretraining-0.1.0.tar` & `flowws-structure-pretraining-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.260896 flowws-structure-pretraining-0.1.0/
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1060 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/LICENSE
--rw-r--r--   0 matthew   (1000) matthew   (1000)      781 2022-09-13 20:28:29.260896 flowws-structure-pretraining-0.1.0/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)      212 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/README.md
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.257896 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      174 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/ClearMetrics.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3991 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/DistanceNeighbors.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2906 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/FileLoader.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1595 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/LimitAccuracyCallback.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     5085 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/LoadModel.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      891 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/NearestNeighbors.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1170 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/NormalizeNeighborDistance.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2242 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/PyriodicLoader.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3212 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/SANNeighbors.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1259 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/VoronoiNeighbors.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      488 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/__init__.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.259896 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2099 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/AutoencoderVisualizer.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2560 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/BondDenoisingVisualizer.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     5663 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/ClassifierPlotter.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     7365 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingDistance.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     5025 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingDistanceTrajectory.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     5875 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingPlotter.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2900 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EvaluateEmbedding.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1909 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/NoisyBondVisualizer.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      832 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/PCAEmbedding.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3289 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/RegressorPlotter.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2538 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/ShiftIdentificationVisualizer.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      871 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/UMAPEmbedding.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1177 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3656 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/internal.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      351 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/internal.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.259896 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/
--rw-r--r--   0 matthew   (1000) matthew   (1000)    12388 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaBondClassifier.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)    11795 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaBondRegressor.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)    18138 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaBottleneckAutoencoder.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)    11537 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaScalarRegressor.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)    12732 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaVectorAutoencoder.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      275 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1604 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/internal.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.260896 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2849 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/AutoencoderTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     5196 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/DenoisingTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     8867 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/FrameClassificationTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1187 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/FrameRegressionTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3303 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/NearestBondTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     4586 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/NoisyBondTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     4299 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/ShiftIdentificationTask.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)      347 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     4269 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/internal.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)       22 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/version.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-09-13 20:28:29.258896 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      781 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2674 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/SOURCES.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/dependency_links.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)     7471 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/entry_points.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)      201 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/requires.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       29 2022-09-13 20:28:29.000000 flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/top_level.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       46 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/pyproject.toml
--rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2022-09-13 20:28:29.260896 flowws-structure-pretraining-0.1.0/setup.cfg
--rw-r--r--   0 matthew   (1000) matthew   (1000)     3552 2022-09-13 20:28:23.000000 flowws-structure-pretraining-0.1.0/setup.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.142086 flowws-structure-pretraining-0.2.0/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      810 2023-04-21 19:05:46.142086 flowws-structure-pretraining-0.2.0/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      212 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/README.md
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.139086 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      174 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/ClearMetrics.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3991 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/DistanceNeighbors.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2906 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/FileLoader.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1595 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/LimitAccuracyCallback.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5194 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/LoadModel.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      891 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/NearestNeighbors.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1170 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/NormalizeNeighborDistance.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2242 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/PyriodicLoader.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3212 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/SANNeighbors.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1259 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/VoronoiNeighbors.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      488 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/__init__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.141086 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2099 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/AutoencoderVisualizer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2560 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/BondDenoisingVisualizer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5663 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/ClassifierPlotter.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     7616 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingDistance.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5025 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingDistanceTrajectory.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5875 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingPlotter.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2900 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EvaluateEmbedding.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1909 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/NoisyBondVisualizer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      832 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/PCAEmbedding.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3289 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/RegressorPlotter.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2538 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/ShiftIdentificationVisualizer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      871 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/UMAPEmbedding.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1177 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3656 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/internal.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      351 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/internal.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.141086 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2960 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaBondClassifier.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2458 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaBondRegressor.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8747 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaBottleneckAutoencoder.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    18179 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaCore.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4029 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaPotentialRegressor.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2242 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaScalarRegressor.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1954 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaVectorAutoencoder.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      306 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5924 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/internal.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.142086 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2849 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/AutoencoderTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5305 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/DenoisingTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     9202 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/FrameClassificationTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1187 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/FrameRegressionTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5239 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/NearBondTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3303 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/NearestBondTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4695 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/NoisyBondTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    15357 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/PointGroupTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4408 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/ShiftIdentificationTask.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      429 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4269 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/internal.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    10309 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/point_groups.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       22 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/version.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 19:05:46.140086 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      810 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2931 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8273 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/entry_points.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      201 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/requires.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       29 2023-04-21 19:05:46.000000 flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/top_level.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       46 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/pyproject.toml
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2023-04-21 19:05:46.142086 flowws-structure-pretraining-0.2.0/setup.cfg
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3640 2023-04-21 19:05:29.000000 flowws-structure-pretraining-0.2.0/setup.py
```

### Comparing `flowws-structure-pretraining-0.1.0/PKG-INFO` & `flowws-structure-pretraining-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: flowws-structure-pretraining
-Version: 0.1.0
+Version: 0.2.0
 Summary: Stage-based scientific workflows for pretraining deep learning models on self-assembly data
 Home-page: UNKNOWN
 Author: Matthew Spellings
 Author-email: mspells@vectorinstitute.ai
 License: MIT
+Description: 
+        # Flowws Modules for Self-supervised Pretraining
+        
+        `flowws-structure-pretraining` is a set of
+        [flowws](https://flowws.readthedocs.io) modules to train machine
+        learning models on self-supervised pretraining tasks.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: pyriodic
 Provides-Extra: analysis
-License-File: LICENSE
-
-
-# Flowws Modules for Self-supervised Pretraining
-
-`flowws-structure-pretraining` is a set of
-[flowws](https://flowws.readthedocs.io) modules to train machine
-learning models on self-supervised pretraining tasks.
-
+Provides-Extra: pyriodic
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/DistanceNeighbors.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/DistanceNeighbors.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/FileLoader.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/FileLoader.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/LimitAccuracyCallback.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/LimitAccuracyCallback.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/LoadModel.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/LoadModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,17 @@
         )
         with keras_gtar.Trajectory(filename, 'r') as traj:
             if not self.arguments['no_model']:
                 weights = traj.get_weights()
             workflow = json.loads(traj.handle.readStr('workflow.json'))
             stages = []
             for stage in workflow['stages']:
-                if stage['type'] in ('FileLoader', 'PyriodicLoader'):
+                if stage['type'] in self.scope.get('skip_loaded_stages', []):
+                    continue
+                elif stage['type'] in ('FileLoader', 'PyriodicLoader'):
                     continue
                 elif stage['type'] in ('Train', 'Save'):
                     continue
                 elif stage['type'] == 'InitializeTF':
                     if self.arguments['no_model']:
                         continue
                 elif any(
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/NearestNeighbors.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/NearestNeighbors.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/NormalizeNeighborDistance.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/NormalizeNeighborDistance.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/PyriodicLoader.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/PyriodicLoader.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/SANNeighbors.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/SANNeighbors.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/VoronoiNeighbors.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/VoronoiNeighbors.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/AutoencoderVisualizer.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/AutoencoderVisualizer.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/BondDenoisingVisualizer.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/BondDenoisingVisualizer.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/ClassifierPlotter.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/ClassifierPlotter.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingDistance.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingDistance.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,22 +83,30 @@
 
     def run(self, scope, storage):
         mode = self.arguments['mode']
         if self.arguments['use_annoy']:
             metric = 'angular' if mode.endswith('cosine') else 'euclidean'
         else:
             metric = 'cosine' if mode.endswith('cosine') else 'euclidean'
-        reference_embedding = scope.get('reference_embedding', scope['embedding'])
+        reference_embedding = scope.get(
+            'reference_embedding', scope.get('embedding', None)
+        )
         scope['reference_embedding'] = reference_embedding
 
-        child_arg_names = {arg.name for arg in EvaluateEmbedding.ARGS}
-        child_args = {k: v for (k, v) in self.arguments.items() if k in child_arg_names}
-        EvaluateEmbedding(**child_args).run(scope, storage)
-        contexts = scope['embedding_contexts']
-        query_embedding = scope['embedding']
+        if 'query_embedding' not in scope:
+            child_arg_names = {arg.name for arg in EvaluateEmbedding.ARGS}
+            child_args = {
+                k: v for (k, v) in self.arguments.items() if k in child_arg_names
+            }
+            EvaluateEmbedding(**child_args).run(scope, storage)
+            contexts = scope['embedding_contexts']
+            query_embedding = scope['embedding']
+        else:
+            contexts = scope['query_embedding_contexts']
+            query_embedding = scope['query_embedding']
 
         if self.arguments['summarize']:
             print('Reference embedding shape:', reference_embedding.shape)
             print('Query embedding shape:', query_embedding.shape)
             dim = reference_embedding.shape[-1]
             ref_covering = len(reference_embedding) ** (1.0 / dim)
             query_covering = len(query_embedding) ** (1.0 / dim)
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingDistanceTrajectory.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingDistanceTrajectory.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EmbeddingPlotter.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EmbeddingPlotter.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/EvaluateEmbedding.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/EvaluateEmbedding.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/NoisyBondVisualizer.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/NoisyBondVisualizer.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/PCAEmbedding.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/PCAEmbedding.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/RegressorPlotter.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/RegressorPlotter.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/ShiftIdentificationVisualizer.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/ShiftIdentificationVisualizer.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/UMAPEmbedding.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/UMAPEmbedding.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/__init__.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/analysis/internal.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/analysis/internal.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/models/GalaBondRegressor.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/models/GalaBottleneckAutoencoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,342 +1,263 @@
-from .internal import NeighborDistanceNormalization
+from .GalaCore import GalaCore
 
 import flowws
 from flowws import Argument as Arg
 from geometric_algebra_attention import keras as gala
-import numpy as np
 from tensorflow import keras
+import tensorflow as tf
 
-NORMALIZATION_LAYERS = {
-    None: lambda _: [],
-    'none': lambda _: [],
-    'batch': lambda _: [keras.layers.BatchNormalization()],
-    'layer': lambda _: [keras.layers.LayerNormalization()],
-    'momentum': lambda _: [gala.MomentumNormalization()],
-    'momentum_layer': lambda _: [gala.MomentumLayerNormalization()],
-}
-
-NORMALIZATION_LAYER_DOC = ' (any of {})'.format(
-    ','.join(map(str, NORMALIZATION_LAYERS))
-)
+
+class VAESampler(keras.layers.Layer):
+    def __init__(self, dim, loss_sum_axes=(-1,), loss_scale=1.0, *args, **kwargs):
+        self.dim = dim
+        self.loss_sum_axes = loss_sum_axes
+        self.loss_scale = loss_scale
+
+        self.z_mean_projection = keras.layers.Dense(self.dim)
+        self.z_log_var_projection = keras.layers.Dense(self.dim)
+
+        super().__init__(*args, **kwargs)
+
+    def call(self, inputs):
+        z_mean = self.z_mean_projection(inputs)
+        z_log_var = self.z_log_var_projection(inputs)
+        shape = tf.shape(z_mean)
+        loss = -0.5 * (1 + z_log_var - tf.square(z_mean) - tf.exp(z_log_var))
+        loss = tf.reduce_mean(tf.reduce_sum(loss, self.loss_sum_axes))
+        loss = loss * self.loss_scale
+        self.add_metric(loss, name='kl_loss')
+        self.add_loss(loss)
+        return tf.random.normal(shape, z_mean, tf.exp(0.5 * z_log_var))
+
+    def get_config(self):
+        result = super().get_config()
+        result['dim'] = self.dim
+        result['loss_sum_axes'] = tuple(self.loss_sum_axes)
+        result['loss_scale'] = self.loss_scale
+        return result
+
+
+def expand_neighborhood_dim(x):
+    return x[..., None, :]
+
+
+def stack_vector_layers(
+    AttentionVector,
+    r,
+    v,
+    n_vectors,
+    scorefun,
+    valuefun,
+    scalefun,
+    join_fun,
+    merge_fun,
+    n_dim=32,
+    rank=2,
+    invar_mode='full',
+    covar_mode='full',
+    include_normalized_products=False,
+    convex_covariants=False,
+):
+    pieces = []
+    for _ in range(n_vectors):
+        layer = AttentionVector(
+            scorefun(),
+            valuefun(n_dim),
+            scalefun(1),
+            reduce=True,
+            invariant_mode=invar_mode,
+            covariant_mode=covar_mode,
+            include_normalized_products=include_normalized_products,
+            merge_fun=merge_fun,
+            join_fun=join_fun,
+            rank=rank,
+            convex_covariants=convex_covariants,
+        )
+        piece = layer([r, v])
+        piece = keras.layers.Lambda(expand_neighborhood_dim)(piece)
+        pieces.append(piece)
+
+    return keras.layers.Concatenate(axis=-2)(pieces)
+
+
+class SVDLayer(keras.layers.Layer):
+    def build(self, input_shape):
+        self.num_vectors, self.n_dim = input_shape[-2:]
+        return super().build(input_shape)
+
+    def call(self, inputs):
+        s, u, v = tf.linalg.svd(inputs)
+        result = tf.matmul(u, v, adjoint_b=True)
+        if self.num_vectors < self.n_dim:
+            cross = tf.linalg.cross(result[..., 0, :], result[..., 1, :])[..., None, :]
+            result = tf.concat([result, cross], axis=-2)
+        return result
+
+
+class NormalizeLayer(keras.layers.Layer):
+    def call(self, inputs):
+        return tf.linalg.normalize(inputs, axis=-1)[0]
+
+
+class StaticEmbedding(keras.layers.Embedding):
+    def call(self, inputs):
+        return super().call(tf.range(0, self.input_dim)[None, :])
 
 
 @flowws.add_stage_arguments
-class GalaBondRegressor(flowws.Stage):
-    """Regress one bond for a given environment using geometric algebra attention"""
+class GalaBottleneckAutoencoder(GalaCore):
+    """Reproduce point clouds after a bottleneck layer"""
 
-    ARGS = [
-        Arg('n_dim', '-n', int, 32, help='Working dimension of model'),
-        Arg('dilation_factor', None, float, 2.0, help='Width factor for MLPs'),
-        Arg(
-            'block_nonlinearity',
-            '-b',
-            bool,
-            True,
-            help='Add a nonlinearity to each block',
-        ),
-        Arg(
-            'residual',
-            '-r',
-            bool,
-            True,
-            help='Use residual connections over each block',
-        ),
-        Arg(
-            'join_fun',
-            '-j',
-            str,
-            'concat',
-            help='Function to use for joining invariant and node-level signals',
-        ),
+    ARGS = GalaCore.ARGS + [
         Arg(
-            'merge_fun',
-            '-m',
-            str,
-            'concat',
-            help='Function to use for merging node-level signals',
-        ),
-        Arg('dropout', '-d', float, 0, help='Dropout probability within network'),
-        Arg('num_blocks', None, int, 1, help='Number of blocks to use'),
-        Arg('rank', None, int, 2, help='Attention calculation rank'),
-        Arg(
-            'activation',
-            '-a',
-            str,
-            'relu',
-            help='Activation function to use within network',
-        ),
-        Arg(
-            'normalize_distances',
-            None,
-            str,
-            help='Create scale-invariant networks by normalizing neighbor distances (mean/min)',
-        ),
-        Arg('invar_mode', '-i', str, 'full', help='Rotation-invariant mode switch'),
-        Arg('covar_mode', '-c', str, 'full', help='Rotation-covariant mode switch'),
-        Arg(
-            'score_normalization',
-            None,
-            str,
-            'layer',
-            help=(
-                'Normalizations to apply to score (attention) function'
-                + NORMALIZATION_LAYER_DOC
-            ),
-        ),
-        Arg(
-            'value_normalization',
-            None,
-            str,
-            'layer',
-            help=(
-                'Normalizations to apply to value function' + NORMALIZATION_LAYER_DOC
-            ),
-        ),
-        Arg(
-            'block_normalization',
+            'num_vector_blocks',
             None,
-            str,
-            'layer',
-            help=(
-                'Normalizations to apply to the output of each attention block'
-                + NORMALIZATION_LAYER_DOC
-            ),
+            int,
+            1,
+            help='Number of vector-valued blocks to use',
         ),
+        Arg('variational', '-v', bool, True, help='If True, make a VAE'),
+        Arg('vae_dim', None, int, 8, help='Dimensionality of latent space for VAE'),
         Arg(
-            'invariant_value_normalization',
+            'vae_scale',
             None,
-            str,
-            'momentum',
-            help=(
-                'Normalizations to apply to value function, before MLP layers'
-                + NORMALIZATION_LAYER_DOC
-            ),
+            float,
+            1e-5,
+            help='Loss term scale for variational component',
         ),
         Arg(
-            'equivariant_value_normalization',
+            'num_reference_vectors',
             None,
-            str,
-            'layer',
-            help=(
-                'Normalizations to apply to equivariant results'
-                + NORMALIZATION_LAYER_DOC
-            ),
+            int,
+            2,
+            help='Number of reference vectors to produce',
         ),
         Arg(
-            'use_multivectors',
+            'cross_attention',
             None,
             bool,
-            False,
-            help='If True, use multivector intermediates for calculations',
-        ),
-        Arg(
-            'drop_geometric_embeddings',
-            None,
-            bool,
-            False,
-            help='If True, use vector inputs rather than geometric accumulations around the embedding layer',
-        ),
-        Arg(
-            'include_normalized_products',
-            None,
-            bool,
-            False,
-            help='Also include normalized geometric product terms',
-        ),
-        Arg(
-            'normalize_equivariant_values',
-            None,
-            bool,
-            False,
-            help='If True, multiply vector values by normalized vectors at each attention step',
+            True,
+            help='If True, generate embeddings using cross-attention between the '
+            'generated basis set and vector intermediates',
         ),
         Arg(
             'transfer_freeze',
             None,
             bool,
             False,
             help='If True, freeze pretrained weights for transfer learning',
         ),
     ]
 
     def run(self, scope, storage):
-        use_weights = scope.get('use_bond_weights', False)
-        n_dim = self.arguments['n_dim']
-        dilation = self.arguments['dilation_factor']
-        block_nonlin = self.arguments['block_nonlinearity']
-        residual = self.arguments['residual']
-        join_fun = self.arguments['join_fun']
-        merge_fun = self.arguments['merge_fun']
-        dropout = self.arguments['dropout']
-        num_blocks = self.arguments['num_blocks']
-        rank = self.arguments['rank']
-        activation = self.arguments['activation']
-        distance_norm = self.arguments.get('normalize_distances', None)
-        invar_mode = self.arguments['invar_mode']
-        covar_mode = self.arguments['covar_mode']
-        DropoutLayer = scope.get('dropout_class', keras.layers.Dropout)
-
-        normalization_getter = lambda key: (
-            NORMALIZATION_LAYERS[self.arguments.get(key + '_normalization', None)](rank)
-        )
+        n_ref = self.arguments['num_reference_vectors']
 
-        if self.arguments['use_multivectors']:
-            Attention = gala.MultivectorAttention
-            AttentionVector = gala.Multivector2MultivectorAttention
-            maybe_upcast_vector = gala.Vector2Multivector()
-            maybe_downcast_vector = gala.Multivector2Vector()
-        else:
-            Attention = gala.VectorAttention
-            AttentionVector = gala.Vector2VectorAttention
-            maybe_upcast_vector = lambda x: x
-            maybe_downcast_vector = lambda x: x
-
-        type_dim = 2 * scope.get('max_types', 1)
-        dilation_dim = int(np.round(n_dim * dilation))
-
-        def make_layer_inputs(x, v):
-            nonnorm = (x, v, w_in) if use_weights else (x, v)
-            if self.arguments['normalize_equivariant_values']:
-                xnorm = keras.layers.LayerNormalization()(x)
-                norm = (xnorm, v, w_in) if use_weights else (xnorm, v)
-                return [nonnorm] + (rank - 1) * [norm]
-            else:
-                return rank * [nonnorm]
-
-        def make_scorefun():
-            layers = [keras.layers.Dense(dilation_dim)]
-
-            layers.extend(normalization_getter('score'))
-
-            layers.append(keras.layers.Activation(activation))
-            if dropout:
-                layers.append(DropoutLayer(dropout))
-
-            layers.append(keras.layers.Dense(1))
-            return keras.models.Sequential(layers)
-
-        def make_valuefun(dim, in_network=True):
-            layers = []
-
-            if in_network:
-                layers.extend(normalization_getter('invariant_value'))
-
-            layers.append(keras.layers.Dense(dilation_dim))
-            layers.extend(normalization_getter('value'))
-
-            layers.append(keras.layers.Activation(activation))
-            if dropout:
-                layers.append(DropoutLayer(dropout))
-
-            layers.append(keras.layers.Dense(dim))
-            return keras.models.Sequential(layers)
-
-        def make_block(last_x, last):
-            residual_in_x = last_x
-            residual_in = last
-            if self.arguments['use_multivectors']:
-                arg = make_layer_inputs(last_x, last)
-                last_x = gala.Multivector2MultivectorAttention(
-                    make_scorefun(),
-                    make_valuefun(n_dim),
-                    make_valuefun(1),
-                    False,
-                    rank=rank,
-                    join_fun=join_fun,
-                    merge_fun=merge_fun,
-                    invariant_mode=invar_mode,
-                    covariant_mode=covar_mode,
-                    include_normalized_products=self.arguments[
-                        'include_normalized_products'
-                    ],
-                )(arg)
-
-            arg = make_layer_inputs(last_x, last)
-            last = Attention(
-                make_scorefun(),
-                make_valuefun(n_dim),
-                False,
-                rank=rank,
-                join_fun=join_fun,
-                merge_fun=merge_fun,
-                invariant_mode=invar_mode,
-                covariant_mode=covar_mode,
+        def make_labeled_block(last):
+            last_x = self.AttentionLabeled(
+                self.make_scorefun(),
+                self.make_valuefun(self.n_dim),
+                self.make_valuefun(1),
+                True,
+                rank=self.rank,
+                join_fun=self.join_fun,
+                merge_fun=self.merge_fun,
+                invariant_mode=self.invar_mode,
+                covariant_mode=self.covar_mode,
                 include_normalized_products=self.arguments[
                     'include_normalized_products'
                 ],
-            )(arg)
-
-            if block_nonlin:
-                last = make_valuefun(n_dim, in_network=False)(last)
-
-            if residual:
-                last = last + residual_in
+                convex_covariants=self.arguments['convex_covariants'],
+            )([last, (reference_last_x, reference_embedding)])
 
-            for layer in normalization_getter('block'):
-                last = layer(last)
-
-            if self.arguments['use_multivectors']:
-                last_x = residual_in_x + last_x
-                for layer in normalization_getter('equivariant_value'):
-                    last_x = layer(last_x)
-
-            return last_x, last
+            return last_x
 
+        self._init(scope, storage)
         if 'encoded_base' in scope:
             (last_x, last) = scope['encoded_base']
             inputs = scope['input_symbol']
-            saved_x_in = maybe_upcast_vector(inputs[0])
 
             if self.arguments['transfer_freeze']:
                 frozen_model = keras.models.Model(inputs, scope['encoded_base'])
                 frozen_model.trainable = False
                 (last_x, last) = frozen_model(inputs)
         else:
-            x_in = keras.layers.Input((None, 3), name='rij')
-            v_in = keras.layers.Input((None, type_dim), name='tij')
-            w_in = None
-            inputs = [x_in, v_in]
-            if use_weights:
-                w_in = keras.layers.Input((None,), name='wij')
-                inputs = [x_in, v_in, w_in]
-
-            last_x = x_in
-            if distance_norm in ('mean', 'min'):
-                last_x = NeighborDistanceNormalization(distance_norm)(last_x)
-            elif distance_norm == 'none':
-                pass
-            elif distance_norm:
-                raise NotImplementedError(distance_norm)
-
-            last_x = saved_x_in = maybe_upcast_vector(last_x)
-            last = keras.layers.Dense(n_dim)(v_in)
-            for _ in range(num_blocks):
-                last_x, last = make_block(last_x, last)
+            super().run(scope, storage)
+
+            (last_x, last) = scope['encoded_base']
+            inputs = scope['input_symbol']
+
+            if self.arguments['transfer_freeze']:
+                frozen_model = keras.models.Model(inputs, scope['encoded_base'])
+                frozen_model.trainable = False
+                (last_x, last) = frozen_model(inputs)
+
+            reference_last_x = stack_vector_layers(
+                self.AttentionVector,
+                last_x,
+                last,
+                n_ref,
+                self.make_scorefun,
+                self.make_valuefun,
+                self.make_valuefun,
+                self.join_fun,
+                self.merge_fun,
+                self.n_dim,
+                self.rank,
+                self.invar_mode,
+                self.covar_mode,
+                include_normalized_products=self.arguments[
+                    'include_normalized_products'
+                ],
+                convex_covariants=self.arguments['convex_covariants'],
+            )
+
+            reference_last_x = SVDLayer()(self.maybe_downcast_vector(reference_last_x))
+            reference_last_x = self.maybe_upcast_vector(reference_last_x)
+            n_ref = max(n_ref, 3)
+
+            reference_embedding = StaticEmbedding(n_ref, self.n_dim)(inputs[0])
 
             embedding = last
+            if self.arguments['cross_attention']:
+                arg = [last_x, last, w_in] if self.use_weights else [last_x, last]
+                arg = [arg, [reference_last_x, reference_embedding]]
+                embedding = last = self.Attention(
+                    self.make_scorefun(),
+                    self.make_valuefun(self.n_dim),
+                    False,
+                    rank=self.rank,
+                    join_fun=self.join_fun,
+                    merge_fun=self.merge_fun,
+                    invariant_mode=self.invar_mode,
+                    covariant_mode=self.covar_mode,
+                    include_normalized_products=self.arguments[
+                        'include_normalized_products'
+                    ],
+                )(arg)
+
+            if self.arguments['variational']:
+                samp = VAESampler(
+                    self.arguments['vae_dim'], (-1,), self.arguments['vae_scale']
+                )
+                embedding = samp.z_mean_projection(last)
+                last = samp(last)
+                if self.n_dim != self.arguments['vae_dim']:
+                    last = keras.layers.Dense(self.n_dim)(last)
+
+            last_x = make_labeled_block(last)
+
             scope['encoded_base'] = (last_x, last)
             embedding_model = keras.models.Model(inputs, embedding)
             scope['embedding_model'] = embedding_model
 
-        if self.arguments['drop_geometric_embeddings']:
-            arg = [saved_x_in, last, w_in] if use_weights else [saved_x_in, last]
-        else:
-            arg = make_layer_inputs(last_x, last)
-        (last_x, ivs, att) = AttentionVector(
-            make_scorefun(),
-            make_valuefun(n_dim),
-            make_valuefun(1),
-            True,
-            name='final_attention',
-            rank=rank,
-            join_fun=join_fun,
-            merge_fun=merge_fun,
-            invariant_mode=invar_mode,
-            covariant_mode=covar_mode,
-            include_normalized_products=self.arguments['include_normalized_products'],
-        )(arg, return_invariants=True, return_attention=True)
-        last_x = maybe_downcast_vector(last_x)
+        for _ in range(self.arguments['num_vector_blocks']):
+            last_x = self.make_vector_block(last_x, last)
+
+        last_x = self.maybe_downcast_vector(last_x)
+
+        if 'equivariant_rescale_factor' in scope:
+            last_x = last_x / scope['equivariant_rescale_factor']
 
         scope['input_symbol'] = inputs
         scope['output'] = last_x
         scope['model'] = keras.models.Model(inputs, scope['output'])
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/AutoencoderTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/AutoencoderTask.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/DenoisingTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/DenoisingTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,25 @@
         subsample=None,
         register=False,
     ):
         env_gen = env_gen.sample(seed, not evaluate, subsample)
         rng = np.random.default_rng(seed + 1)
         x_scale = self.arguments['x_scale']
         batch_size = self.arguments['batch_size']
+        done = False
 
-        while True:
+        while not done:
             rs, vs, ys, ws, ctxs = [], [], [], [], []
             max_size = 0
             while len(rs) < batch_size:
                 try:
                     ((r, v, w), context) = next(env_gen)
                 except StopIteration:
-                    return
+                    done = True
+                    break
                 ctxs.append(context)
 
                 y = r
                 if evaluate:
                     x = r.copy()
                 else:
                     noise = rng.normal(scale=self.arguments['noise'], size=r.shape)
@@ -152,11 +154,13 @@
                 pad(rs, max_size, 3),
                 pad(vs, max_size, self.type_dim),
                 pad(ws, max_size, None),
             )
             if not self.use_weights:
                 x = x[:-1]
 
+            if not len(x[0]):
+                return
             if evaluate:
                 yield x, pad(ys, max_size, 3), ctxs
             else:
                 yield x, pad(ys, max_size, 3)
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/FrameClassificationTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/FrameClassificationTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,21 @@
         ),
         Arg(
             'cluster_term',
             None,
             float,
             help='If given, use the value to add a loss penalty for non-close probabilities',
         ),
+        Arg(
+            'delete_context_keys',
+            None,
+            [str],
+            [],
+            help='Delete the given context keys when mapping labels',
+        ),
     ]
 
     def run(self, scope, storage):
         max_types = scope['max_types']
         x_scale = self.arguments['x_scale']
         remap = Remap()
         if self.arguments['zero_class']:
@@ -95,28 +102,31 @@
         else:
             pad_size = max(np.max(frame.nlist.neighbor_counts) for frame in frames)
 
         rng = np.random.default_rng(self.arguments['seed'])
 
         rs, ts, ws, ys, ctxs = [], [], [], [], []
         for frame in frames:
+            context = dict(frame.context)
+            for key in self.arguments.get('delete_context_keys', []):
+                context.pop(key, None)
+            encoded_type = remap(frozenset(sorted(context.items())))
             samp = np.arange(len(frame.positions))
             if 'subsample' in self.arguments:
                 filt = rng.uniform(size=len(samp))
                 filt = filt < self.arguments['subsample']
                 samp = samp[filt]
                 if not len(samp):
                     continue
 
             (rijs, tijs, wijs) = index_frame(frame, samp, pad_size, 2 * max_types)
 
             rs.append(rijs)
             ts.append(tijs)
             ws.append(wijs)
-            encoded_type = remap(frozenset(frame.context.items()))
             ys.append(np.full_like(rijs[..., :1], encoded_type, dtype=np.int32))
             ctxs.extend(len(rijs) * [frame.context])
 
         rs = np.concatenate(rs, axis=0)
         ts = np.concatenate(ts, axis=0)
         ws = np.concatenate(ws, axis=0)
         ys = np.concatenate(ys, axis=0)
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/FrameRegressionTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/FrameRegressionTask.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/NearestBondTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/NearestBondTask.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/NoisyBondTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/NoisyBondTask.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,23 +86,25 @@
         self, env_gen, seed=13, round_neighbors=4, evaluate=False, subsample=None
     ):
         env_gen = env_gen.sample(seed, not evaluate, subsample)
         rng = np.random.default_rng(seed + 1)
         x_scale = self.arguments['x_scale']
         noise_magnitude = self.arguments['noise_magnitude']
         batch_size = self.arguments['batch_size']
+        done = False
 
-        while True:
+        while not done:
             rs, vs, ys, ws, ctxs = [], [], [], [], []
             max_size = 0
             while len(rs) < batch_size:
                 try:
                     ((r, v, w), context) = next(env_gen)
                 except StopIteration:
-                    return
+                    done = True
+                    break
                 ctxs.append(context)
 
                 y = np.zeros(len(r), dtype=np.int32)
                 if not evaluate:
                     sel = rng.permutation(len(r))[: len(r) // 2]
                     r[sel] += rng.normal(scale=noise_magnitude, size=(len(sel), 3))
                     y[sel] = 1
@@ -122,11 +124,13 @@
                 pad(rs, max_size, 3),
                 pad(vs, max_size, self.type_dim),
                 pad(ws, max_size, None),
             )
             if not self.use_weights:
                 x = x[:-1]
 
+            if not len(x[0]):
+                return
             if evaluate:
                 yield x, pad(ys, max_size), ctxs
             else:
                 yield x, pad(ys, max_size)
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/ShiftIdentificationTask.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/ShiftIdentificationTask.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,23 +77,25 @@
     def batch_generator(
         self, env_gen, seed=13, round_neighbors=4, evaluate=False, subsample=None
     ):
         env_gen = env_gen.sample(seed, not evaluate, subsample)
         rng = np.random.default_rng(seed + 1)
         x_scale = self.arguments['x_scale']
         batch_size = self.arguments['batch_size']
+        done = False
 
-        while True:
+        while not done:
             rs, vs, ys, ws, ctxs = [], [], [], [], []
             max_size = 0
             while len(rs) < batch_size:
                 try:
                     ((r, v, w), context) = next(env_gen)
                 except StopIteration:
-                    return
+                    done = True
+                    break
                 ctxs.append(context)
 
                 y = rng.normal(scale=self.arguments['scale'], size=(3,))
                 if evaluate:
                     y[:] = 0
                 x = r + y[None, :]
 
@@ -115,11 +117,13 @@
                 pad(ws, max_size, None),
             )
             if not self.use_weights:
                 x = x[:-1]
 
             ys = np.array(ys)
 
+            if not len(x[0]):
+                return
             if evaluate:
                 yield x, ys, ctxs
             else:
                 yield x, ys
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining/tasks/internal.py` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining/tasks/internal.py`

 * *Files identical despite different names*

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/PKG-INFO` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: flowws-structure-pretraining
-Version: 0.1.0
+Version: 0.2.0
 Summary: Stage-based scientific workflows for pretraining deep learning models on self-assembly data
 Home-page: UNKNOWN
 Author: Matthew Spellings
 Author-email: mspells@vectorinstitute.ai
 License: MIT
+Description: 
+        # Flowws Modules for Self-supervised Pretraining
+        
+        `flowws-structure-pretraining` is a set of
+        [flowws](https://flowws.readthedocs.io) modules to train machine
+        learning models on self-supervised pretraining tasks.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: pyriodic
 Provides-Extra: analysis
-License-File: LICENSE
-
-
-# Flowws Modules for Self-supervised Pretraining
-
-`flowws-structure-pretraining` is a set of
-[flowws](https://flowws.readthedocs.io) modules to train machine
-learning models on self-supervised pretraining tasks.
-
+Provides-Extra: pyriodic
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/SOURCES.txt` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 pyproject.toml
 setup.py
 flowws_structure_pretraining/ClearMetrics.py
 flowws_structure_pretraining/DistanceNeighbors.py
 flowws_structure_pretraining/FileLoader.py
 flowws_structure_pretraining/LimitAccuracyCallback.py
@@ -34,20 +33,25 @@
 flowws_structure_pretraining/analysis/ShiftIdentificationVisualizer.py
 flowws_structure_pretraining/analysis/UMAPEmbedding.py
 flowws_structure_pretraining/analysis/__init__.py
 flowws_structure_pretraining/analysis/internal.py
 flowws_structure_pretraining/models/GalaBondClassifier.py
 flowws_structure_pretraining/models/GalaBondRegressor.py
 flowws_structure_pretraining/models/GalaBottleneckAutoencoder.py
+flowws_structure_pretraining/models/GalaCore.py
+flowws_structure_pretraining/models/GalaPotentialRegressor.py
 flowws_structure_pretraining/models/GalaScalarRegressor.py
 flowws_structure_pretraining/models/GalaVectorAutoencoder.py
 flowws_structure_pretraining/models/__init__.py
 flowws_structure_pretraining/models/internal.py
 flowws_structure_pretraining/tasks/AutoencoderTask.py
 flowws_structure_pretraining/tasks/DenoisingTask.py
 flowws_structure_pretraining/tasks/FrameClassificationTask.py
 flowws_structure_pretraining/tasks/FrameRegressionTask.py
+flowws_structure_pretraining/tasks/NearBondTask.py
 flowws_structure_pretraining/tasks/NearestBondTask.py
 flowws_structure_pretraining/tasks/NoisyBondTask.py
+flowws_structure_pretraining/tasks/PointGroupTask.py
 flowws_structure_pretraining/tasks/ShiftIdentificationTask.py
 flowws_structure_pretraining/tasks/__init__.py
-flowws_structure_pretraining/tasks/internal.py
+flowws_structure_pretraining/tasks/internal.py
+flowws_structure_pretraining/tasks/point_groups.py
```

### Comparing `flowws-structure-pretraining-0.1.0/flowws_structure_pretraining.egg-info/entry_points.txt` & `flowws-structure-pretraining-0.2.0/flowws_structure_pretraining.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 EvaluateEmbedding = flowws_structure_pretraining.analysis.EvaluateEmbedding:EvaluateEmbedding
 FileLoader = flowws_structure_pretraining.FileLoader:FileLoader
 FrameClassificationTask = flowws_structure_pretraining.tasks.FrameClassificationTask:FrameClassificationTask
 FrameRegressionTask = flowws_structure_pretraining.tasks.FrameRegressionTask:FrameRegressionTask
 GalaBondClassifier = flowws_structure_pretraining.models.GalaBondClassifier:GalaBondClassifier
 GalaBondRegressor = flowws_structure_pretraining.models.GalaBondRegressor:GalaBondRegressor
 GalaBottleneckAutoencoder = flowws_structure_pretraining.models.GalaBottleneckAutoencoder:GalaBottleneckAutoencoder
+GalaCore = flowws_structure_pretraining.models.GalaCore:GalaCore
+GalaPotentialRegressor = flowws_structure_pretraining.models.GalaPotentialRegressor:GalaPotentialRegressor
 GalaScalarRegressor = flowws_structure_pretraining.models.GalaScalarRegressor:GalaScalarRegressor
 GalaVectorAutoencoder = flowws_structure_pretraining.models.GalaVectorAutoencoder:GalaVectorAutoencoder
 LimitAccuracyCallback = flowws_structure_pretraining.LimitAccuracyCallback:LimitAccuracyCallback
 LoadModel = flowws_structure_pretraining.LoadModel:LoadModel
+NearBondTask = flowws_structure_pretraining.tasks.NearBondTask:NearBondTask
 NearestBondTask = flowws_structure_pretraining.tasks.NearestBondTask:NearestBondTask
 NearestNeighbors = flowws_structure_pretraining.NearestNeighbors:NearestNeighbors
 NoisyBondTask = flowws_structure_pretraining.tasks.NoisyBondTask:NoisyBondTask
 NoisyBondVisualizer = flowws_structure_pretraining.analysis.NoisyBondVisualizer:NoisyBondVisualizer
 NormalizeNeighborDistance = flowws_structure_pretraining.NormalizeNeighborDistance:NormalizeNeighborDistance
 PCAEmbedding = flowws_structure_pretraining.analysis.PCAEmbedding:PCAEmbedding
+PointGroupTask = flowws_structure_pretraining.tasks.PointGroupTask:PointGroupTask
 PyriodicLoader = flowws_structure_pretraining.PyriodicLoader:PyriodicLoader
 RegressorPlotter = flowws_structure_pretraining.analysis.RegressorPlotter:RegressorPlotter
 SANNeighbors = flowws_structure_pretraining.SANNeighbors:SANNeighbors
 ShiftIdentificationTask = flowws_structure_pretraining.tasks.ShiftIdentificationTask:ShiftIdentificationTask
 ShiftIdentificationVisualizer = flowws_structure_pretraining.analysis.ShiftIdentificationVisualizer:ShiftIdentificationVisualizer
 UMAPEmbedding = flowws_structure_pretraining.analysis.UMAPEmbedding:UMAPEmbedding
 VoronoiNeighbors = flowws_structure_pretraining.VoronoiNeighbors:VoronoiNeighbors
@@ -54,17 +58,21 @@
 flowws_structure_pretraining.analysis.PCAEmbedding = flowws_structure_pretraining.analysis.PCAEmbedding:PCAEmbedding
 flowws_structure_pretraining.analysis.RegressorPlotter = flowws_structure_pretraining.analysis.RegressorPlotter:RegressorPlotter
 flowws_structure_pretraining.analysis.ShiftIdentificationVisualizer = flowws_structure_pretraining.analysis.ShiftIdentificationVisualizer:ShiftIdentificationVisualizer
 flowws_structure_pretraining.analysis.UMAPEmbedding = flowws_structure_pretraining.analysis.UMAPEmbedding:UMAPEmbedding
 flowws_structure_pretraining.models.GalaBondClassifier = flowws_structure_pretraining.models.GalaBondClassifier:GalaBondClassifier
 flowws_structure_pretraining.models.GalaBondRegressor = flowws_structure_pretraining.models.GalaBondRegressor:GalaBondRegressor
 flowws_structure_pretraining.models.GalaBottleneckAutoencoder = flowws_structure_pretraining.models.GalaBottleneckAutoencoder:GalaBottleneckAutoencoder
+flowws_structure_pretraining.models.GalaCore = flowws_structure_pretraining.models.GalaCore:GalaCore
+flowws_structure_pretraining.models.GalaPotentialRegressor = flowws_structure_pretraining.models.GalaPotentialRegressor:GalaPotentialRegressor
 flowws_structure_pretraining.models.GalaScalarRegressor = flowws_structure_pretraining.models.GalaScalarRegressor:GalaScalarRegressor
 flowws_structure_pretraining.models.GalaVectorAutoencoder = flowws_structure_pretraining.models.GalaVectorAutoencoder:GalaVectorAutoencoder
 flowws_structure_pretraining.tasks.AutoencoderTask = flowws_structure_pretraining.tasks.AutoencoderTask:AutoencoderTask
 flowws_structure_pretraining.tasks.DenoisingTask = flowws_structure_pretraining.tasks.DenoisingTask:DenoisingTask
 flowws_structure_pretraining.tasks.FrameClassificationTask = flowws_structure_pretraining.tasks.FrameClassificationTask:FrameClassificationTask
 flowws_structure_pretraining.tasks.FrameRegressionTask = flowws_structure_pretraining.tasks.FrameRegressionTask:FrameRegressionTask
+flowws_structure_pretraining.tasks.NearBondTask = flowws_structure_pretraining.tasks.NearBondTask:NearBondTask
 flowws_structure_pretraining.tasks.NearestBondTask = flowws_structure_pretraining.tasks.NearestBondTask:NearestBondTask
 flowws_structure_pretraining.tasks.NoisyBondTask = flowws_structure_pretraining.tasks.NoisyBondTask:NoisyBondTask
+flowws_structure_pretraining.tasks.PointGroupTask = flowws_structure_pretraining.tasks.PointGroupTask:PointGroupTask
 flowws_structure_pretraining.tasks.ShiftIdentificationTask = flowws_structure_pretraining.tasks.ShiftIdentificationTask:ShiftIdentificationTask
```

### Comparing `flowws-structure-pretraining-0.1.0/setup.py` & `flowws-structure-pretraining-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,27 +63,31 @@
 add_subpkg(subpkg, module_names)
 
 subpkg = 'models'
 module_names = [
     'GalaBondClassifier',
     'GalaBondRegressor',
     'GalaBottleneckAutoencoder',
+    'GalaCore',
+    'GalaPotentialRegressor',
     'GalaScalarRegressor',
     'GalaVectorAutoencoder',
 ]
 add_subpkg(subpkg, module_names)
 
 subpkg = 'tasks'
 module_names = [
     'AutoencoderTask',
     'DenoisingTask',
     'FrameClassificationTask',
     'FrameRegressionTask',
+    'NearBondTask',
     'NearestBondTask',
     'NoisyBondTask',
+    'PointGroupTask',
     'ShiftIdentificationTask',
 ]
 add_subpkg(subpkg, module_names)
 
 setup(name='flowws-structure-pretraining',
       author='Matthew Spellings',
       author_email='mspells@vectorinstitute.ai',
```

