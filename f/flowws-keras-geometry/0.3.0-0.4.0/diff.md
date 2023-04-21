# Comparing `tmp/flowws-keras-geometry-0.3.0.tar.gz` & `tmp/flowws-keras-geometry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowws-keras-geometry-0.3.0.tar", last modified: Tue Feb 15 20:13:39 2022, max compression
+gzip compressed data, was "flowws-keras-geometry-0.4.0.tar", last modified: Fri Apr 21 18:48:20 2023, max compression
```

## Comparing `flowws-keras-geometry-0.3.0.tar` & `flowws-keras-geometry-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1060 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/LICENSE
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1235 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1001)      729 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/README.md
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.041346 flowws-keras-geometry-0.3.0/doc/
--rw-r--r--   0 matthew   (1000) matthew   (1001)      638 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/doc/Makefile
--rw-r--r--   0 matthew   (1000) matthew   (1001)      799 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/doc/make.bat
--rw-r--r--   0 matthew   (1000) matthew   (1001)       29 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/doc/requirements.txt
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.041346 flowws-keras-geometry-0.3.0/doc/source/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1870 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/doc/source/conf.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1359 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/doc/source/index.rst
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.041346 flowws-keras-geometry-0.3.0/flowws_keras_geometry/
--rw-r--r--   0 matthew   (1000) matthew   (1001)      101 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)      200 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/algebra.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     6757 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/MD17.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     7223 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/ModelNet.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     4890 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PDBCache.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     9868 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PDBCoarseGrained.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     4583 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PyriodicDataset.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     2080 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/RMD17.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)      338 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)      921 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/internal.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)      175 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/layers.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     5108 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/CrystalStructureClassification.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     7762 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/MoleculeForceRegression.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     8820 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/PDBInverseCoarseGrain.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     3272 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/PDBInverseCoarseGrainTransformer.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)      193 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)    25098 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/internal.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)       22 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/version.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     5878 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/BackmapCoarseGrainViewer.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     7204 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/MoleculeAttentionViewer.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)     6467 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/ParticleAttentionViewer.py
--rw-r--r--   0 matthew   (1000) matthew   (1001)        1 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/__init__.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1001)        0 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1235 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1001)     1355 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 matthew   (1000) matthew   (1001)        1 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 matthew   (1000) matthew   (1001)     2608 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/entry_points.txt
--rw-r--r--   0 matthew   (1000) matthew   (1001)       33 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/requires.txt
--rw-r--r--   0 matthew   (1000) matthew   (1001)       22 2022-02-15 20:13:38.000000 flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/top_level.txt
--rw-r--r--   0 matthew   (1000) matthew   (1001)       38 2022-02-15 20:13:39.044679 flowws-keras-geometry-0.3.0/setup.cfg
--rw-r--r--   0 matthew   (1000) matthew   (1001)     2573 2022-02-15 20:13:30.000000 flowws-keras-geometry-0.3.0/setup.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.072617 flowws-keras-geometry-0.4.0/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1440 2023-04-21 18:48:20.072617 flowws-keras-geometry-0.4.0/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      729 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/README.md
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.070617 flowws-keras-geometry-0.4.0/flowws_keras_geometry/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      101 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      200 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/algebra.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.071617 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4045 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/ImportMatProjChargeDensity.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8634 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/MD17.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8751 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/MatProjChargeDensity.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     7311 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/ModelNet.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4890 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PDBCache.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     9868 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PDBCoarseGrained.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4583 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PyriodicDataset.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2172 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/RMD17.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      558 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2327 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/internal.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      175 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/layers.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.072617 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5108 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/CrystalStructureClassification.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    13914 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/GalaMoleculeForceRegression.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    12851 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/GalaPDBInverseCoarseGrain.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8004 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/MoleculeForceRegression.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     8820 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/PDBInverseCoarseGrain.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3272 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/PDBInverseCoarseGrainTransformer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      544 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    25098 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/internal.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       22 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/version.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.072617 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     5878 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/BackmapCoarseGrainViewer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3345 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/MatProjChargeDensityViewer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     7204 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/MoleculeAttentionViewer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     6467 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/ParticleAttentionViewer.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/__init__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 18:48:20.070617 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1440 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1542 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3816 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/entry_points.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       33 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/requires.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       22 2023-04-21 18:48:20.000000 flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/top_level.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2023-04-21 18:48:20.072617 flowws-keras-geometry-0.4.0/setup.cfg
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2737 2023-04-21 18:48:04.000000 flowws-keras-geometry-0.4.0/setup.py
```

### Comparing `flowws-keras-geometry-0.3.0/README.md` & `flowws-keras-geometry-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/MD17.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/MD17.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os
 import subprocess
 
 import flowws
 from flowws import Argument as Arg
 import numpy as np
-from tensorflow import keras
-
-from .internal import ScaledMSE, ScaledMAE
 
 @flowws.add_stage_arguments
 class MD17(flowws.Stage):
     """Load data from the MD17 dataset for molecular force regression.
 
     This module downloads files from the MD17 dataset as required. It
     randomly selects molecule snapshots for the specified molecules to
@@ -36,15 +33,21 @@
             help='Random number seed to use'),
         Arg('units', None, str, 'meV',
             help='Energy units to use (meV or kcal/mol)'),
         Arg('y_scale_reduction', None, float, 16,
             help='Factor by which to scale forces for training purposes'),
         Arg('x_scale_reduction', None, float,
             help='Factor by which to scale input distances for training purposes'
-            ' (negative to auto-scale from training data)')
+            ' (negative to auto-scale from training data)'),
+        Arg('energy_labels', '-e', bool, False,
+            help='If True, include energies as labels'),
+        Arg('no_keras', '-k', bool, False,
+            help='If True, don\'t load/import keras'),
+        Arg('normalize_on_energy', None, bool, False,
+            help='If True, normalize energies to have variance of 1 instead of forces'),
     ]
 
     def run(self, scope, storage):
         np.random.seed(self.arguments['seed'])
 
         energy_conversion = 1.
         if self.arguments['units'] == 'meV':
@@ -77,86 +80,121 @@
             seen_types.update(types)
 
         all_types = [0] + list(sorted(seen_types))
         type_map = {t: i for (i, t) in enumerate(all_types)}
         num_types = len(all_types)
 
         datasets = {}
+        energy_means = {}
         for name in ['train', 'val', 'test']:
-            dset_xs, dset_ts, dset_ys = [], [], []
+            dset_xs, dset_ts, dset_ys, dset_Us = [], [], [], []
             for fname in sorted(loaded_files):
                 indices = locals()['{}_indices'.format(name)]
-                (xs, ts), Us = self.get_encoding(
-                    loaded_files[fname], max_atoms, type_map, indices[fname], energy_conversion)
+                encoding = self.get_encoding(
+                    loaded_files[fname], max_atoms, type_map, indices[fname],
+                    energy_conversion, self.arguments['energy_labels'])
+                (xs, ts), Fs, Us = encoding
                 dset_xs.append(xs)
                 dset_ts.append(ts)
-                dset_ys.append(Us)
+                dset_ys.append(Fs)
+
+                if self.arguments['energy_labels']:
+                    if name == 'train':
+                        energy_means[fname] = np.mean(Us)
+                    Us -= energy_means[fname]
+                dset_Us.append(Us)
 
             dset_xs = np.concatenate(dset_xs, axis=0)
             dset_ts = np.concatenate(dset_ts, axis=0)
             dset_ys = np.concatenate(dset_ys, axis=0)
 
             indices = np.arange(len(dset_xs))
             np.random.shuffle(indices)
             dset_xs = dset_xs[indices]
             dset_ts = dset_ts[indices]
             dset_ys = dset_ys[indices]
+            dset = [dset_xs, dset_ts, dset_ys]
 
-            datasets[name] = (dset_xs, dset_ts, dset_ys)
-
-        yscale = np.std(datasets['train'][-1])*self.arguments['y_scale_reduction']
-
-        for (_, _, y) in datasets.values():
-            y /= yscale
-
-        scaled_mse = ScaledMSE(yscale)
-        scaled_mae = ScaledMAE(yscale)
+            if self.arguments['energy_labels']:
+                dset_Us = np.concatenate(dset_Us, axis=0)
+                dset_Us = dset_Us[indices]
+                dset = [dset_xs, dset_ts, dset_ys, dset_Us]
+
+            datasets[name] = dset
+
+        yscale = np.std(datasets['train'][2])*self.arguments['y_scale_reduction']
+        if self.arguments['energy_labels']:
+            if self.arguments['normalize_on_energy']:
+                yscale = np.std(datasets['train'][3])*self.arguments['y_scale_reduction']
+            for dset in datasets.values():
+                dset[3] /= yscale
+        for dset in datasets.values():
+            dset[2] /= yscale
+
+        if not self.arguments['no_keras']:
+            from .internal import ScaledMSE, ScaledMAE
+            metrics = scope.setdefault('metrics', [])
+            scaled_mse = ScaledMSE(yscale, name='scaled_mse')
+            scaled_mae = ScaledMAE(yscale, name='scaled_mae')
+            metrics.extend([scaled_mse, scaled_mae])
 
         xscale = 1.
         if 'x_scale_reduction' in self.arguments:
             xscale = self.arguments['x_scale_reduction']
 
             if xscale <= 0:
                 delta = datasets['train'][0] - datasets['train'][0][:, :1]
                 delta = delta.reshape((-1, 3))
                 filt = np.logical_and(
                     np.any(datasets['train'][0].reshape((-1, 3)) != 0, axis=-1),
                     np.any(delta != 0, axis=-1))
                 delta = np.linalg.norm(delta[filt], axis=-1)
                 xscale = np.std(delta)
 
-            for (x, _, _) in datasets.values():
-                x /= xscale
+            for dset in datasets.values():
+                dset[0] /= xscale
+
+        for (name, dset) in list(datasets.items()):
+            if self.arguments['energy_labels']:
+                datasets[name] = tuple(dset[:2]), tuple(dset[2:])
+            else:
+                datasets[name] = tuple(dset[:2]), dset[2]
 
         scope['y_scale'] = yscale
         scope['x_scale'] = xscale
         scope['neighborhood_size'] = max_atoms
         scope['num_types'] = num_types
-        scope['x_train'] = datasets['train'][:2]
-        scope['y_train'] = datasets['train'][-1]
-        scope['x_test'] = datasets['test'][:2]
-        scope['y_test'] = datasets['test'][-1]
-        scope['validation_data'] = (datasets['val'][:2], datasets['val'][-1])
+        scope['max_types'] = num_types
+        scope['per_molecule'] = True
+        scope['x_train'] = datasets['train'][0]
+        scope['y_train'] = datasets['train'][1]
+        scope['x_test'] = datasets['test'][0]
+        scope['y_test'] = datasets['test'][1]
+        scope['validation_data'] = (datasets['val'][0], datasets['val'][1])
         scope['type_map'] = type_map
-        scope.setdefault('metrics', []).extend([scaled_mse, scaled_mae])
+        scope['energy_labels'] = self.arguments['energy_labels']
 
     def _download(self, name):
         url = self.get_url(name)
         fname = url.split('/')[-1]
 
         if fname not in os.listdir(self.arguments['cache_dir']):
             command = ['wget', '-c', '-P', self.arguments['cache_dir'], url]
             subprocess.check_call(command)
 
         return os.path.join(self.arguments['cache_dir'], fname)
 
     @staticmethod
-    def get_encoding(data, max_atoms, type_map, indices=None, energy_conversion=1.):
+    def get_encoding(data, max_atoms, type_map, indices=None, energy_conversion=1.,
+                     include_energy=False):
         coords = data['R']
+        # (Nt, Natom, 3)
         forces = data['F']*energy_conversion
+        # (Nt, 1)
+        energies = data['E']*energy_conversion if include_energy else None
         types = np.zeros(max_atoms, dtype=np.uint32)
         types[:coords.shape[1]] = [type_map[t] for t in data['z']]
 
         if indices is not None:
             coords = coords[indices]
             forces = forces[indices]
 
@@ -164,21 +202,22 @@
         rs[:, :coords.shape[1], :] = coords
 
         Fs = np.zeros((len(coords), max_atoms, 3))
         Fs[:, :coords.shape[1], :] = forces
 
         types_onehot = np.eye(len(type_map))[types]
         types_onehot = np.tile(types_onehot[np.newaxis, ...], (len(coords), 1, 1))
-        return (rs, types_onehot), Fs
+        return (rs, types_onehot), Fs, energies
 
     @staticmethod
     def get_trajectory_size_types(data):
         (frames, size, _) = data['R'].shape
         return (frames, size, data['z'])
 
     @staticmethod
     def get_url(name):
-        remap = dict(benzene='benzene2017_dft.npz')
+        remap = dict(benzene='benzene2017')
+        name = remap.get(name, name)
 
         base = 'http://quantum-machine.org/gdml/data/npz/'
 
-        return base + remap.get(name, '{}_dft.npz'.format(name.split('_')[0]))
+        return base + 'md17_{}.npz'.format(name.split('_')[0])
```

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/ModelNet.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/ModelNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
                 vertices = self.handle.getRecord(self.group_records[group], index)
                 vertices = vertices.reshape((-1, 3))
 
                 vertices -= np.mean(vertices, axis=0, keepdims=True)
                 scale = np.mean(np.linalg.norm(vertices, axis=-1))
 
                 vertex_choice = rng.choice(
-                    len(vertices), min(len(vertices), self.neighborhood_size),
-                    replace=False)
+                    len(vertices), self.neighborhood_size,
+                    replace=(self.neighborhood_size > len(vertices)))
                 rs[i, :len(vertex_choice)] = vertices[vertex_choice]/scale
                 vs[i, :len(vertex_choice)] = 1
                 ys[i] = y
 
             yield ((rs, vs), ys)
 
     def train_generator(self, batch_size, seed=13):
@@ -128,14 +128,15 @@
         scope['train_generator'] = dataset.train_generator(
             self.arguments['batch_size'], self.arguments['seed'] + 1)
         scope['test_generator'] = dataset.test_generator(
             self.arguments['batch_size'], self.arguments['seed'] + 2)
         if self.arguments['validation_fraction']:
             scope['validation_generator'] = dataset.val_generator(
                 self.arguments['batch_size'], self.arguments['seed'] + 3)
+        scope['neighborhood_size'] = self.arguments['neighborhood_size']
         scope['num_classes'] = len(dataset.labels)
 
     @classmethod
     def _get_dataset(cls, cache_dir):
         fname = os.path.join(cache_dir, 'modelnet40_gtar.zip')
 
         if os.path.exists(fname):
```

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PDBCache.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PDBCache.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PDBCoarseGrained.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PDBCoarseGrained.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/data/PyriodicDataset.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/data/PyriodicDataset.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/CrystalStructureClassification.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/CrystalStructureClassification.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/MoleculeForceRegression.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/MoleculeForceRegression.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,21 @@
             [delta_x, last], return_invariants=True, return_attention=True)
 
         last = keras.layers.Dense(dilation_dim, name='final_mlp')(last)
         last = final_activation_layer()(last)
         last = NeighborhoodReduction()(last)
         use_bias = self.arguments.get('energy_bias', False)
         last = keras.layers.Dense(1, name='energy_projection', use_bias=use_bias)(last)
+        energy_prediction = last
         if not self.arguments['predict_energy']:
             last = GradientLayer()((last, x_in))
 
+        if scope.get('energy_labels', False):
+            last = (last[0], energy_prediction)
+            kwargs = scope.setdefault('compile_kwargs', {})
+            kwargs['loss_weights'] = (1 - 1e-3, 1e-3)
+
         scope['input_symbol'] = [x_in, v_in]
         scope['output'] = last
         scope['loss'] = 'mse'
         scope['attention_model'] = keras.models.Model([x_in, v_in], att)
         scope['invariant_model'] = keras.models.Model([x_in, v_in], ivs)
```

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/PDBInverseCoarseGrain.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/PDBInverseCoarseGrain.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/PDBInverseCoarseGrainTransformer.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/PDBInverseCoarseGrainTransformer.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/models/internal.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/models/internal.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/BackmapCoarseGrainViewer.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/BackmapCoarseGrainViewer.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/MoleculeAttentionViewer.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/MoleculeAttentionViewer.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry/viz/ParticleAttentionViewer.py` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry/viz/ParticleAttentionViewer.py`

 * *Files identical despite different names*

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/SOURCES.txt` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-LICENSE
 README.md
 setup.py
-doc/Makefile
-doc/make.bat
-doc/requirements.txt
-doc/source/conf.py
-doc/source/index.rst
 flowws_keras_geometry/__init__.py
 flowws_keras_geometry/algebra.py
 flowws_keras_geometry/layers.py
 flowws_keras_geometry/version.py
 flowws_keras_geometry.egg-info/PKG-INFO
 flowws_keras_geometry.egg-info/SOURCES.txt
 flowws_keras_geometry.egg-info/dependency_links.txt
 flowws_keras_geometry.egg-info/entry_points.txt
 flowws_keras_geometry.egg-info/requires.txt
 flowws_keras_geometry.egg-info/top_level.txt
+flowws_keras_geometry/data/ImportMatProjChargeDensity.py
 flowws_keras_geometry/data/MD17.py
+flowws_keras_geometry/data/MatProjChargeDensity.py
 flowws_keras_geometry/data/ModelNet.py
 flowws_keras_geometry/data/PDBCache.py
 flowws_keras_geometry/data/PDBCoarseGrained.py
 flowws_keras_geometry/data/PyriodicDataset.py
 flowws_keras_geometry/data/RMD17.py
 flowws_keras_geometry/data/__init__.py
 flowws_keras_geometry/data/internal.py
 flowws_keras_geometry/models/CrystalStructureClassification.py
+flowws_keras_geometry/models/GalaMoleculeForceRegression.py
+flowws_keras_geometry/models/GalaPDBInverseCoarseGrain.py
 flowws_keras_geometry/models/MoleculeForceRegression.py
 flowws_keras_geometry/models/PDBInverseCoarseGrain.py
 flowws_keras_geometry/models/PDBInverseCoarseGrainTransformer.py
 flowws_keras_geometry/models/__init__.py
 flowws_keras_geometry/models/internal.py
 flowws_keras_geometry/viz/BackmapCoarseGrainViewer.py
+flowws_keras_geometry/viz/MatProjChargeDensityViewer.py
 flowws_keras_geometry/viz/MoleculeAttentionViewer.py
 flowws_keras_geometry/viz/ParticleAttentionViewer.py
 flowws_keras_geometry/viz/__init__.py
```

### Comparing `flowws-keras-geometry-0.3.0/flowws_keras_geometry.egg-info/entry_points.txt` & `flowws-keras-geometry-0.4.0/flowws_keras_geometry.egg-info/entry_points.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 [flowws_modules]
 BackmapCoarseGrainViewer = flowws_keras_geometry.viz.BackmapCoarseGrainViewer:BackmapCoarseGrainViewer
 CrystalStructureClassification = flowws_keras_geometry.models.CrystalStructureClassification:CrystalStructureClassification
+GalaMoleculeForceRegression = flowws_keras_geometry.models.GalaMoleculeForceRegression:GalaMoleculeForceRegression
+GalaPDBInverseCoarseGrain = flowws_keras_geometry.models.GalaPDBInverseCoarseGrain:GalaPDBInverseCoarseGrain
+ImportMatProjChargeDensity = flowws_keras_geometry.data.ImportMatProjChargeDensity:ImportMatProjChargeDensity
 MD17 = flowws_keras_geometry.data.MD17:MD17
+MatProjChargeDensity = flowws_keras_geometry.data.MatProjChargeDensity:MatProjChargeDensity
+MatProjChargeDensityViewer = flowws_keras_geometry.viz.MatProjChargeDensityViewer:MatProjChargeDensityViewer
 ModelNet = flowws_keras_geometry.data.ModelNet:ModelNet
 MoleculeAttentionViewer = flowws_keras_geometry.viz.MoleculeAttentionViewer:MoleculeAttentionViewer
 MoleculeForceRegression = flowws_keras_geometry.models.MoleculeForceRegression:MoleculeForceRegression
 PDBCache = flowws_keras_geometry.data.PDBCache:PDBCache
 PDBCoarseGrained = flowws_keras_geometry.data.PDBCoarseGrained:PDBCoarseGrained
 PDBInverseCoarseGrain = flowws_keras_geometry.models.PDBInverseCoarseGrain:PDBInverseCoarseGrain
 PDBInverseCoarseGrainTransformer = flowws_keras_geometry.models.PDBInverseCoarseGrainTransformer:PDBInverseCoarseGrainTransformer
 ParticleAttentionViewer = flowws_keras_geometry.viz.ParticleAttentionViewer:ParticleAttentionViewer
 PyriodicDataset = flowws_keras_geometry.data.PyriodicDataset:PyriodicDataset
 RMD17 = flowws_keras_geometry.data.RMD17:RMD17
+flowws_keras_geometry.data.ImportMatProjChargeDensity = flowws_keras_geometry.data.ImportMatProjChargeDensity:ImportMatProjChargeDensity
 flowws_keras_geometry.data.MD17 = flowws_keras_geometry.data.MD17:MD17
+flowws_keras_geometry.data.MatProjChargeDensity = flowws_keras_geometry.data.MatProjChargeDensity:MatProjChargeDensity
 flowws_keras_geometry.data.ModelNet = flowws_keras_geometry.data.ModelNet:ModelNet
 flowws_keras_geometry.data.PDBCache = flowws_keras_geometry.data.PDBCache:PDBCache
 flowws_keras_geometry.data.PDBCoarseGrained = flowws_keras_geometry.data.PDBCoarseGrained:PDBCoarseGrained
 flowws_keras_geometry.data.PyriodicDataset = flowws_keras_geometry.data.PyriodicDataset:PyriodicDataset
 flowws_keras_geometry.data.RMD17 = flowws_keras_geometry.data.RMD17:RMD17
 flowws_keras_geometry.models.CrystalStructureClassification = flowws_keras_geometry.models.CrystalStructureClassification:CrystalStructureClassification
+flowws_keras_geometry.models.GalaMoleculeForceRegression = flowws_keras_geometry.models.GalaMoleculeForceRegression:GalaMoleculeForceRegression
+flowws_keras_geometry.models.GalaPDBInverseCoarseGrain = flowws_keras_geometry.models.GalaPDBInverseCoarseGrain:GalaPDBInverseCoarseGrain
 flowws_keras_geometry.models.MoleculeForceRegression = flowws_keras_geometry.models.MoleculeForceRegression:MoleculeForceRegression
 flowws_keras_geometry.models.PDBInverseCoarseGrain = flowws_keras_geometry.models.PDBInverseCoarseGrain:PDBInverseCoarseGrain
 flowws_keras_geometry.models.PDBInverseCoarseGrainTransformer = flowws_keras_geometry.models.PDBInverseCoarseGrainTransformer:PDBInverseCoarseGrainTransformer
 flowws_keras_geometry.viz.BackmapCoarseGrainViewer = flowws_keras_geometry.viz.BackmapCoarseGrainViewer:BackmapCoarseGrainViewer
+flowws_keras_geometry.viz.MatProjChargeDensityViewer = flowws_keras_geometry.viz.MatProjChargeDensityViewer:MatProjChargeDensityViewer
 flowws_keras_geometry.viz.MoleculeAttentionViewer = flowws_keras_geometry.viz.MoleculeAttentionViewer:MoleculeAttentionViewer
 flowws_keras_geometry.viz.ParticleAttentionViewer = flowws_keras_geometry.viz.ParticleAttentionViewer:ParticleAttentionViewer
```

### Comparing `flowws-keras-geometry-0.3.0/setup.py` & `flowws-keras-geometry-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,35 +33,40 @@
         flowws_modules.append('{0} = flowws_keras_geometry.{0}:{0}'.format(name))
         entry_points.add(name)
     flowws_modules.append(
         'flowws_keras_geometry.{0} = flowws_keras_geometry.{0}:{0}'.format(name))
 
 subpkg = 'data'
 module_names = [
+    'ImportMatProjChargeDensity',
+    'MatProjChargeDensity',
     'MD17',
     'ModelNet',
     'PDBCache',
     'PDBCoarseGrained',
     'PyriodicDataset',
     'RMD17',
 ]
 add_subpkg(subpkg, module_names)
 
 subpkg = 'models'
 module_names = [
     'CrystalStructureClassification',
+    'GalaMoleculeForceRegression',
+    'GalaPDBInverseCoarseGrain',
     'MoleculeForceRegression',
     'PDBInverseCoarseGrain',
     'PDBInverseCoarseGrainTransformer',
 ]
 add_subpkg(subpkg, module_names)
 
 subpkg = 'viz'
 module_names = [
     'BackmapCoarseGrainViewer',
+    'MatProjChargeDensityViewer',
     'MoleculeAttentionViewer',
     'ParticleAttentionViewer',
 ]
 add_subpkg(subpkg, module_names)
 
 setup(name='flowws-keras-geometry',
       author='Matthew Spellings',
```

