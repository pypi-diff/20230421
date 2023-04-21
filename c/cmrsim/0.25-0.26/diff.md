# Comparing `tmp/cmrsim-0.25-py3-none-any.whl.zip` & `tmp/cmrsim-0.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,52 +1,54 @@
-Zip file size: 115604 bytes, number of entries: 50
--rw-r--r--  2.0 unx      317 b- defN 23-Jan-18 09:03 cmrsim/__init__.py
--rw-r--r--  2.0 unx      354 b- defN 22-Dec-07 08:35 cmrsim/analytic/__init__.py
--rw-r--r--  2.0 unx     5002 b- defN 22-Dec-07 08:35 cmrsim/analytic/_composite_signal.py
--rw-r--r--  2.0 unx    14188 b- defN 23-Jan-13 14:32 cmrsim/analytic/simulation.py
--rw-r--r--  2.0 unx      722 b- defN 22-Dec-07 08:35 cmrsim/analytic/contrast/__init__.py
--rw-r--r--  2.0 unx    15609 b- defN 22-Dec-22 10:30 cmrsim/analytic/contrast/base.py
--rw-r--r--  2.0 unx    12878 b- defN 22-Dec-22 10:30 cmrsim/analytic/contrast/coil_sensitivities.py
--rw-r--r--  2.0 unx     4067 b- defN 22-Dec-07 08:35 cmrsim/analytic/contrast/diffusion_weighting.py
--rw-r--r--  2.0 unx     4409 b- defN 22-Dec-22 10:30 cmrsim/analytic/contrast/phase_tracking.py
--rw-r--r--  2.0 unx    13174 b- defN 22-Dec-22 10:30 cmrsim/analytic/contrast/sequences.py
--rw-r--r--  2.0 unx     4764 b- defN 22-Dec-22 10:30 cmrsim/analytic/contrast/t2_star.py
--rw-r--r--  2.0 unx      707 b- defN 22-Dec-07 08:35 cmrsim/analytic/encoding/__init__.py
--rw-r--r--  2.0 unx     2010 b- defN 22-Dec-07 08:35 cmrsim/analytic/encoding/_from_sequence.py
--rw-r--r--  2.0 unx    15979 b- defN 23-Jan-13 14:32 cmrsim/analytic/encoding/base.py
--rw-r--r--  2.0 unx     9365 b- defN 22-Dec-07 08:35 cmrsim/analytic/encoding/cartesian.py
--rw-r--r--  2.0 unx      493 b- defN 22-Dec-22 10:30 cmrsim/bloch/__init__.py
--rw-r--r--  2.0 unx     5423 b- defN 22-Dec-07 08:35 cmrsim/bloch/_base.py
--rw-r--r--  2.0 unx    27333 b- defN 23-Jan-13 14:32 cmrsim/bloch/_generic.py
--rw-r--r--  2.0 unx     3456 b- defN 22-Dec-07 08:35 cmrsim/bloch/_ideal.py
--rw-r--r--  2.0 unx     6674 b- defN 23-Jan-13 14:32 cmrsim/bloch/_multi_coil.py
--rw-r--r--  2.0 unx     7960 b- defN 23-Jan-13 14:32 cmrsim/bloch/submodules.py
--rw-r--r--  2.0 unx      702 b- defN 23-Jan-13 14:32 cmrsim/datasets/__init__.py
--rw-r--r--  2.0 unx     3804 b- defN 23-Jan-13 14:32 cmrsim/datasets/_analytic.py
--rw-r--r--  2.0 unx     2842 b- defN 23-Jan-13 14:32 cmrsim/datasets/_base.py
--rw-r--r--  2.0 unx     1655 b- defN 22-Dec-07 08:35 cmrsim/datasets/_bloch.py
--rw-r--r--  2.0 unx    41432 b- defN 22-Dec-07 08:35 cmrsim/datasets/_cardiac_mesh.py
--rw-r--r--  2.0 unx    23212 b- defN 22-Dec-22 10:30 cmrsim/datasets/_flow.py
--rw-r--r--  2.0 unx    14057 b- defN 23-Jan-13 14:32 cmrsim/datasets/_regular_grid.py
--rw-r--r--  2.0 unx      140 b- defN 22-Dec-07 08:35 cmrsim/reconstruction/__init__.py
--rw-r--r--  2.0 unx     1820 b- defN 22-Dec-07 08:35 cmrsim/reconstruction/base.py
--rw-r--r--  2.0 unx     6823 b- defN 22-Dec-07 08:35 cmrsim/reconstruction/cartesian.py
--rw-r--r--  2.0 unx      189 b- defN 22-Dec-07 08:35 cmrsim/simulation_templates/__init__.py
--rw-r--r--  2.0 unx     9173 b- defN 22-Dec-07 08:35 cmrsim/simulation_templates/experimental_optimization.py
--rw-r--r--  2.0 unx    20327 b- defN 22-Dec-07 08:35 cmrsim/simulation_templates/flow.py
--rw-r--r--  2.0 unx     1394 b- defN 22-Dec-07 08:35 cmrsim/trajectory/__init__.py
--rw-r--r--  2.0 unx     3296 b- defN 23-Jan-13 14:32 cmrsim/trajectory/_base.py
--rw-r--r--  2.0 unx     8492 b- defN 22-Dec-07 08:35 cmrsim/trajectory/_diffusion.py
--rw-r--r--  2.0 unx    26052 b- defN 22-Dec-22 10:30 cmrsim/trajectory/_flow.py
--rw-r--r--  2.0 unx     8349 b- defN 23-Jan-13 14:32 cmrsim/trajectory/_proper_ortho_decomp.py
--rw-r--r--  2.0 unx     7160 b- defN 23-Jan-13 14:32 cmrsim/trajectory/_taylor.py
--rw-r--r--  2.0 unx      376 b- defN 22-Dec-22 10:30 cmrsim/utils/__init__.py
--rw-r--r--  2.0 unx     4170 b- defN 23-Jan-13 14:32 cmrsim/utils/coordinates.py
--rw-r--r--  2.0 unx     6671 b- defN 22-Dec-07 08:35 cmrsim/utils/display.py
--rw-r--r--  2.0 unx     1246 b- defN 22-Dec-07 08:35 cmrsim/utils/particle_properties.py
--rw-r--r--  2.0 unx     7023 b- defN 22-Dec-07 08:35 cmrsim/utils/snr.py
--rw-rw-rw-  2.0 unx    35060 b- defN 23-Jan-18 09:03 cmrsim-0.25.dist-info/LICENSE
--rw-r--r--  2.0 unx     3473 b- defN 23-Jan-18 09:03 cmrsim-0.25.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 09:03 cmrsim-0.25.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 09:03 cmrsim-0.25.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4346 b- defN 23-Jan-18 09:03 cmrsim-0.25.dist-info/RECORD
-50 files, 398267 bytes uncompressed, 108678 bytes compressed:  72.7%
+Zip file size: 119241 bytes, number of entries: 52
+-rw-r--r--  2.0 unx      317 b- defN 23-Apr-21 09:27 cmrsim/__init__.py
+-rw-r--r--  2.0 unx      354 b- defN 23-Apr-13 14:50 cmrsim/analytic/__init__.py
+-rw-r--r--  2.0 unx     5002 b- defN 23-Apr-13 14:50 cmrsim/analytic/_composite_signal.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Apr-13 14:50 cmrsim/analytic/simulation.py
+-rw-r--r--  2.0 unx      790 b- defN 23-Apr-18 15:24 cmrsim/analytic/contrast/__init__.py
+-rw-r--r--  2.0 unx    15609 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/base.py
+-rw-r--r--  2.0 unx    12878 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/coil_sensitivities.py
+-rw-r--r--  2.0 unx     4067 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/diffusion_weighting.py
+-rw-r--r--  2.0 unx     4797 b- defN 23-Apr-18 15:24 cmrsim/analytic/contrast/offresonance.py
+-rw-r--r--  2.0 unx     4409 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/phase_tracking.py
+-rw-r--r--  2.0 unx    13174 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/sequences.py
+-rw-r--r--  2.0 unx     4764 b- defN 23-Apr-13 14:50 cmrsim/analytic/contrast/t2_star.py
+-rw-r--r--  2.0 unx      707 b- defN 23-Apr-13 14:50 cmrsim/analytic/encoding/__init__.py
+-rw-r--r--  2.0 unx     2010 b- defN 23-Apr-13 14:50 cmrsim/analytic/encoding/_from_sequence.py
+-rw-r--r--  2.0 unx    15979 b- defN 23-Apr-13 14:50 cmrsim/analytic/encoding/base.py
+-rw-r--r--  2.0 unx     9365 b- defN 23-Apr-13 14:50 cmrsim/analytic/encoding/cartesian.py
+-rw-r--r--  2.0 unx      493 b- defN 23-Apr-13 14:50 cmrsim/bloch/__init__.py
+-rw-r--r--  2.0 unx     5423 b- defN 23-Apr-13 14:50 cmrsim/bloch/_base.py
+-rw-r--r--  2.0 unx    27333 b- defN 23-Apr-18 15:24 cmrsim/bloch/_generic.py
+-rw-r--r--  2.0 unx     3456 b- defN 23-Apr-13 14:50 cmrsim/bloch/_ideal.py
+-rw-r--r--  2.0 unx     6674 b- defN 23-Apr-13 14:50 cmrsim/bloch/_multi_coil.py
+-rw-r--r--  2.0 unx     7960 b- defN 23-Apr-21 09:01 cmrsim/bloch/submodules.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-13 14:50 cmrsim/datasets/__init__.py
+-rw-r--r--  2.0 unx     3804 b- defN 23-Apr-13 14:50 cmrsim/datasets/_analytic.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Apr-13 14:50 cmrsim/datasets/_base.py
+-rw-r--r--  2.0 unx     1655 b- defN 23-Apr-13 14:50 cmrsim/datasets/_bloch.py
+-rw-r--r--  2.0 unx    41423 b- defN 23-Apr-19 12:18 cmrsim/datasets/_cardiac_mesh.py
+-rw-r--r--  2.0 unx    23224 b- defN 23-Apr-19 12:18 cmrsim/datasets/_flow.py
+-rw-r--r--  2.0 unx    14057 b- defN 23-Apr-13 14:50 cmrsim/datasets/_regular_grid.py
+-rw-r--r--  2.0 unx      140 b- defN 23-Apr-13 14:50 cmrsim/reconstruction/__init__.py
+-rw-r--r--  2.0 unx     1820 b- defN 23-Apr-13 14:50 cmrsim/reconstruction/base.py
+-rw-r--r--  2.0 unx     6823 b- defN 23-Apr-13 14:50 cmrsim/reconstruction/cartesian.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Apr-13 14:50 cmrsim/simulation_templates/__init__.py
+-rw-r--r--  2.0 unx     9173 b- defN 23-Apr-13 14:50 cmrsim/simulation_templates/experimental_optimization.py
+-rw-r--r--  2.0 unx    20333 b- defN 23-Apr-21 09:01 cmrsim/simulation_templates/flow.py
+-rw-r--r--  2.0 unx     1437 b- defN 23-Apr-18 15:24 cmrsim/trajectory/__init__.py
+-rw-r--r--  2.0 unx     3296 b- defN 23-Apr-13 14:50 cmrsim/trajectory/_base.py
+-rw-r--r--  2.0 unx     5577 b- defN 23-Apr-19 13:20 cmrsim/trajectory/_breathing.py
+-rw-r--r--  2.0 unx     8492 b- defN 23-Apr-13 14:50 cmrsim/trajectory/_diffusion.py
+-rw-r--r--  2.0 unx    26071 b- defN 23-Apr-21 09:01 cmrsim/trajectory/_flow.py
+-rw-r--r--  2.0 unx     8394 b- defN 23-Apr-18 15:24 cmrsim/trajectory/_proper_ortho_decomp.py
+-rw-r--r--  2.0 unx     7443 b- defN 23-Apr-19 12:18 cmrsim/trajectory/_taylor.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Apr-13 14:50 cmrsim/utils/__init__.py
+-rw-r--r--  2.0 unx     4170 b- defN 23-Apr-13 14:50 cmrsim/utils/coordinates.py
+-rw-r--r--  2.0 unx     6671 b- defN 23-Apr-13 14:50 cmrsim/utils/display.py
+-rw-r--r--  2.0 unx     1246 b- defN 23-Apr-13 14:50 cmrsim/utils/particle_properties.py
+-rw-r--r--  2.0 unx     7023 b- defN 23-Apr-13 14:50 cmrsim/utils/snr.py
+-rw-rw-rw-  2.0 unx    35060 b- defN 23-Apr-21 09:27 cmrsim-0.26.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3473 b- defN 23-Apr-21 09:27 cmrsim-0.26.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 09:27 cmrsim-0.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-21 09:27 cmrsim-0.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4531 b- defN 23-Apr-21 09:27 cmrsim-0.26.dist-info/RECORD
+52 files, 409293 bytes uncompressed, 112021 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -18,14 +18,17 @@
 
 Filename: cmrsim/analytic/contrast/coil_sensitivities.py
 Comment: 
 
 Filename: cmrsim/analytic/contrast/diffusion_weighting.py
 Comment: 
 
+Filename: cmrsim/analytic/contrast/offresonance.py
+Comment: 
+
 Filename: cmrsim/analytic/contrast/phase_tracking.py
 Comment: 
 
 Filename: cmrsim/analytic/contrast/sequences.py
 Comment: 
 
 Filename: cmrsim/analytic/contrast/t2_star.py
@@ -102,14 +105,17 @@
 
 Filename: cmrsim/trajectory/__init__.py
 Comment: 
 
 Filename: cmrsim/trajectory/_base.py
 Comment: 
 
+Filename: cmrsim/trajectory/_breathing.py
+Comment: 
+
 Filename: cmrsim/trajectory/_diffusion.py
 Comment: 
 
 Filename: cmrsim/trajectory/_flow.py
 Comment: 
 
 Filename: cmrsim/trajectory/_proper_ortho_decomp.py
@@ -129,23 +135,23 @@
 
 Filename: cmrsim/utils/particle_properties.py
 Comment: 
 
 Filename: cmrsim/utils/snr.py
 Comment: 
 
-Filename: cmrsim-0.25.dist-info/LICENSE
+Filename: cmrsim-0.26.dist-info/LICENSE
 Comment: 
 
-Filename: cmrsim-0.25.dist-info/METADATA
+Filename: cmrsim-0.26.dist-info/METADATA
 Comment: 
 
-Filename: cmrsim-0.25.dist-info/WHEEL
+Filename: cmrsim-0.26.dist-info/WHEEL
 Comment: 
 
-Filename: cmrsim-0.25.dist-info/top_level.txt
+Filename: cmrsim-0.26.dist-info/top_level.txt
 Comment: 
 
-Filename: cmrsim-0.25.dist-info/RECORD
+Filename: cmrsim-0.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmrsim/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.25'
+__version__ = '0.26'
 __all__ = ["trajectory", "analytic", "bloch",
            "datasets", "reconstruction", "simulation_templates", "utils"]
 
 import cmrsim.analytic
 import cmrsim.utils
 import cmrsim.bloch
 import cmrsim.datasets
```

## cmrsim/analytic/contrast/__init__.py

```diff
@@ -3,12 +3,13 @@
 
 from cmrsim.analytic.contrast.base import *
 from cmrsim.analytic.contrast.coil_sensitivities import *
 from cmrsim.analytic.contrast.diffusion_weighting import *
 from cmrsim.analytic.contrast.phase_tracking import *
 from cmrsim.analytic.contrast.sequences import *
 from cmrsim.analytic.contrast.t2_star import *
+from cmrsim.analytic.contrast.offresonance import *
 
 _submodules = ["base", "coil_sensitivities", "diffusion_weighting", "phase_tracking", "sequences",
-               "t2_star"]
+               "t2_star", "offresonance"]
 mod_handles = [importlib.import_module(f"cmrsim.analytic.contrast.{m}") for m in _submodules]
 __all__ = [item for m in mod_handles for item in getattr(m, '__all__')]
```

## cmrsim/bloch/submodules.py

```diff
@@ -134,15 +134,15 @@
 
             max_shape = tf.reduce_max(tf.stack([tf.shape(gradient_wave_form),
                                                 tf.shape(trajectories)]), axis=0)[0:3]
 
             n_reps, n_batch, n_steps = tf.unstack(max_shape, axis=0)
             x, y, z = trajectories[...,0],trajectories[...,1],trajectories[...,2]
             gx, gy, gz = gradient_wave_form[...,0],gradient_wave_form[...,1],gradient_wave_form[...,2]
-            omega = ((gx * z + gz * x / 2) ** 2 + (
+            omega = ((gx * z - gz * x / 2) ** 2 + (
                         gy * z - gz * y / 2) ** 2) / self._b0 / 2. * self._gamma
             phi = omega * dt
             return tf.reshape(phi, [n_reps, n_batch, n_steps])
 
 
 # pylint: disable=abstract-method
 class OffResonance(BaseSubmodule):
```

## cmrsim/datasets/_cardiac_mesh.py

```diff
@@ -3,15 +3,15 @@
 __all__ = ["MeshDataset", "CardiacMeshDataset"]
 
 import os
 from typing import List, Union, Tuple, Iterable
 
 import pyvista
 import numpy as np
-from tqdm.notebook import tqdm
+from tqdm import tqdm
 from pint import Quantity
 import vtk
 from scipy import interpolate
 
 
 class MeshDataset:
     """This class bundles basic functionality to handles dynamic meshes and implements convenience
```

## cmrsim/datasets/_flow.py

```diff
@@ -110,15 +110,15 @@
         :return: None
         """
         image_box = np.max(mesh.points, axis=0) - np.min(mesh.points, axis=0)
         dims = (image_box / lookup_map_spacing).astype(int)
         resolution = image_box / dims
         origin = np.min(mesh.points, axis=0)
 
-        uniform_grid = pyvista.UniformGrid(dims=dims,
+        uniform_grid = pyvista.UniformGrid(dimensions=dims,
                                            spacing=resolution,
                                            origin=origin)
         self.lookup_map_spacing = lookup_map_spacing
 
         uniform_grid = uniform_grid.sample(mesh)
         uniform_grid["in_mesh"] = np.array(uniform_grid["vtkValidPointMask"], dtype=np.float64)
         self.gridded_mesh = uniform_grid
@@ -167,15 +167,15 @@
                                                         self.slice_bounding_box)
 
         # Create uniform grid with specified seeding slice boundaries
         image_box = np.max(r_slice, axis=0) - np.min(r_slice, axis=0)
         dims = (image_box / self.seeding_vol_spacing).astype(int)
         resolution = image_box / dims
         origin = np.min(r_slice, axis=0)
-        gridded_seeding_volume = pyvista.UniformGrid(dims=dims + 1,
+        gridded_seeding_volume = pyvista.UniformGrid(dimensions=dims + 1,
                                                      spacing=resolution,
                                                      origin=origin)
         self.gridded_seeding_volume = self.gridded_mesh.probe(gridded_seeding_volume)
 
         active_indx = np.where(self.gridded_seeding_volume.ptc().cell_data["in_mesh"] > 0.7)
         active_cell_centers = self.gridded_seeding_volume.cell_centers().ptc().points[active_indx]
```

## cmrsim/simulation_templates/flow.py

```diff
@@ -56,15 +56,15 @@
         :raises: ValueError if repetition numbers of specified simulation modules are inconsistent
 
         :return: List[Iterable[int], ...] for each simulation module specify which repetition index
                  corresponds to which k-space-line
         """
         # Check if all required properties are provided by the dataset:
         required_properties = ["magnetization, M0, T1, T2"]
-        for cm in self.contrast_modules + self.prep_modules + [self.readout_module, ]:
+        for cm in list(self.contrast_modules) + self.prep_modules + [self.readout_module, ]:
             for sm in cm.submodules:
                 required_properties.extend(sm.required_quantities)
         required_properties = set(required_properties)
 
         provided_properties = [v[0] for v in self._refilling_dataset.field_list[1:]]
         provided_properties += self._refilling_dataset.particle_properties
```

## cmrsim/trajectory/__init__.py

```diff
@@ -16,13 +16,14 @@
 import importlib
 
 from cmrsim.trajectory._base import *
 from cmrsim.trajectory._flow import *
 from cmrsim.trajectory._taylor import *
 from cmrsim.trajectory._diffusion import *
 from cmrsim.trajectory._proper_ortho_decomp import *
+from cmrsim.trajectory._breathing import *
 
 # Compose __all__ on import
 module_names = glob.glob(os.path.join(os.path.dirname(__file__), "_*.py"))
 alls = [importlib.import_module("cmrsim.trajectory." + os.path.basename(f)[:-3]).__all__
         for f in module_names if os.path.isfile(f) and not f.endswith('__init__.py')]
 __all__ = [a for alls_sub in alls for a in alls_sub]
```

## cmrsim/trajectory/_flow.py

```diff
@@ -105,15 +105,15 @@
         :param verbose: bool
         :param return_velocities: if True, the velocities for each time-step is saved and returned
                                     as entry of the additional fields dictionary
         :return: (#particles, n_steps, 3) - tf.Tensors, Trajectory,
                   dict(field-name: tf.Tensor with shape (#particles, n_steps, n_components))
                   field values at trajectory locations
         """
-        time_grid = np.arange(0., timing[-1], dt_max)
+        time_grid = np.arange(0., timing[-1], dt_max).astype(np.float32)
         insertion_index = np.searchsorted(time_grid, timing)
         time_grid = np.unique(np.insert(time_grid, insertion_index, timing))
         saving_indices = iter(enumerate(np.concatenate([np.searchsorted(time_grid, timing), [-1]])))
 
         positions = np.empty([timing.shape[0], *initial_positions.shape], dtype=np.float32)
 
         additional_fields = []
```

## cmrsim/trajectory/_proper_ortho_decomp.py

```diff
@@ -133,15 +133,16 @@
         idx_before = self.current_batch_idx.read_value()
         self.current_batch_idx.assign(batch_index)
         pos = self._evaluate_trajectory(timing)
         self.current_batch_idx.assign(idx_before)
         return pos, {}
 
     @tf.function
-    def increment_particles(self, r: tf.Tensor, dt: tf.Tensor, **kwargs) -> (tf.Tensor, dict):
+    def increment_particles(self, particle_positions: tf.Tensor,
+                            dt: tf.Tensor, **kwargs) -> (tf.Tensor, dict):
         """Evaluates the particle position for the time self.current_time_ms + dt and adds the
         delta t to the current_time_ms variable
 
         :param r: unused parameter (to adhere to calling signature of trajectory modules)
         :param dt: temporal step lengths
         :param kwargs: unused parameter (to adhere to calling signature of trajectory modules)
         :return: (#batch, self._channels), {}
```

## cmrsim/trajectory/_taylor.py

```diff
@@ -41,18 +41,20 @@
     #: Together with self.current_batch_size determines the subset of particle trajectories that
     #: is evaluated on call and increment_particles
     batch_size: tf.Variable
     #: Stores the order of the TaylorPolynomial, defined on instantiation
     order: tf.Variable
     #: Stores the result of fitting the TaylorPolynomial for all particle trajectories
     optimal_parameters: tf.Variable
+    #: Is periodic
+    is_periodic: tf.constant
 
     # pylint: disable=too-many-arguments
     def __init__(self, order: int, time_grid: np.ndarray, particle_trajectories: np.ndarray,
-                 batch_size: int = None, fit_on_init: bool = True):
+                 batch_size: int = None, fit_on_init: bool = True, is_periodic: bool = False):
         """
         :param order: Order of the fitted TaylorPolynomial
         :param time_grid: (#timesteps, )
         :param particle_trajectories: (#particles, #timesteps, 3)
         :param batch_size: used for evaluating the particle trajectories in batches
         :param fit_on_init: If True, the Polynomial is fitted on instantiation of the module.
         """
@@ -76,40 +78,44 @@
             dtype=tf.float32, shape=(None, None, None), trainable=False)
 
         super().__init__(name=f"taylor_trajectory_order{order}")
         if fit_on_init:
             t_zero_ref = time_grid - self.ref_time
             self.fit(t_zero_ref, particle_trajectories)
 
+        self.is_periodic = tf.constant(is_periodic, dtype=tf.bool)
+
     def fit(self, t_grid: np.ndarray, particle_trajectories: np.ndarray):
         """ Fits a Taylor polynomial of order self.order to each particle trajectory.
 
         :param t_grid: (T, ) times corresponding to the particle positions
         :param particle_trajectories: (N, T, dim)
         :return: optimal motion parameters (N, order, dim) containing all parameters
                 (r0, v, a, j, ...) for N particles
         """
         n_particles, n_steps, n_dims = particle_trajectories.shape
         flattened_trajectories = np.swapaxes(particle_trajectories, 0, 1).reshape(n_steps, -1)
         flat_coefficients = np.polynomial.polynomial.polyfit(t_grid, flattened_trajectories,
                                                              deg=self._int_order)
         coefficients = np.swapaxes(
-            flat_coefficients.reshape(self._int_order + 1, n_particles, n_dims)
-            , 0, 1)
+            flat_coefficients.reshape(self._int_order + 1, n_particles, n_dims),
+            0, 1)
         self.optimal_parameters.assign(coefficients.astype(np.float32))
 
     @tf.function
     def _evaluate_trajectory(self, t: tf.Tensor) -> tf.Tensor:
         """ Evaluates the taylor expansion for a the current batch of particles at the specified
         times t.
 
         :param t: (#timesteps)
         :return: (#particles, #timesteps, 3)
         """
         t = t - self.ref_time
+        if self.is_periodic:
+            t = tf.math.floormod(t, self.end_time - self.ref_time)
         batch_start = self.current_batch_idx * self.batch_size
         batch_end = batch_start + self.batch_size
         factors = self.optimal_parameters[batch_start:batch_end]
         exponents = tf.range(0, tf.cast(self.order + 1, dtype=tf.float32))[:, tf.newaxis]
         t_pow_n = t[np.newaxis] ** exponents  # (order, time)
         out = tf.reduce_sum(factors[:, :, tf.newaxis] * t_pow_n[tf.newaxis, :, :, tf.newaxis],
                             axis=1)
@@ -126,15 +132,16 @@
         idx_before = self.current_batch_idx.read_value()
         self.current_batch_idx.assign(batch_index)
         pos = self._evaluate_trajectory(timing)
         self.current_batch_idx.assign(idx_before)
         return pos, {}
 
     @tf.function
-    def increment_particles(self, r: tf.Tensor, dt: tf.Tensor, **kwargs) -> (tf.Tensor, dict):
+    def increment_particles(self, particle_positions: tf.Tensor,
+                            dt: tf.Tensor, **kwargs) -> (tf.Tensor, dict):
         """ Evaluates the particle position for the time self.current_time_ms + dt and adds the
         delta t to the current_time_ms variable
 
         :param r: unused parameter (to adhere to calling signature of trajectory modules)
         :param dt: temporal step lengths
         :param kwargs: unused parameter (to adhere to calling signature of trajectory modules)
         :return: (#batch, 3)
```

## Comparing `cmrsim-0.25.dist-info/LICENSE` & `cmrsim-0.26.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cmrsim-0.25.dist-info/METADATA` & `cmrsim-0.26.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrsim
-Version: 0.25
+Version: 0.26
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrsim
 Author: Jonathan Weine, Charles McGrath
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrsim/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrsim
 Project-URL: Institute, https://cmr.ethz.ch/
```

## Comparing `cmrsim-0.25.dist-info/RECORD` & `cmrsim-0.26.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-cmrsim/__init__.py,sha256=xd4oCiOu-sTEmXy-m1Rjpqf4APOY52J2uCEqfB32r4A,317
+cmrsim/__init__.py,sha256=sMa1VXpkgXzPdV3-Wqlcr7ij55H9A5exgxwNyAGzHiM,317
 cmrsim/analytic/__init__.py,sha256=NuSQvtJg-2uNXpk2zNl8_jZnVFUcQUTmgGTtRNidY7U,354
 cmrsim/analytic/_composite_signal.py,sha256=QO9oGB4pE3p1wmYa6DWN9XpZZPkxgQ4q4FCf2nPGZdI,5002
 cmrsim/analytic/simulation.py,sha256=ZUh1QV3wQiHOSZVleBji1IZI2pOlLZqc1IuitPQ2qNc,14188
-cmrsim/analytic/contrast/__init__.py,sha256=ZLMlqVQacx5BRNy8a8nf5lBGPdXOt7gpggRJqbCU38g,722
+cmrsim/analytic/contrast/__init__.py,sha256=SCgESekO5Hz6aGI9UPGHuLz1yAhE4GCMAeMze1Zqbko,790
 cmrsim/analytic/contrast/base.py,sha256=GIZqoOWCzrYekmXFbMBroJokF4Z4urwG0vfUk3S4EQo,15609
 cmrsim/analytic/contrast/coil_sensitivities.py,sha256=8wvS8V8iZ_k4jprj3mveC5tLelTn7U76h5FvQzKtF6E,12878
 cmrsim/analytic/contrast/diffusion_weighting.py,sha256=RGcQmAU-8WTTxPrUpLJK6jJmmAgs6wUYiuGEdMw3vOI,4067
+cmrsim/analytic/contrast/offresonance.py,sha256=Di4m75df20czXL0ib8u6M-RZ1q2YPjDh_dRTsMwlzwI,4797
 cmrsim/analytic/contrast/phase_tracking.py,sha256=aPZrxDQHSsCHiXM9X5W2fULi4rsV1X18QMiVbp7aYg8,4409
 cmrsim/analytic/contrast/sequences.py,sha256=vqhmXlUjdJKkxjtkKGFmcLO2djZNS5mpRQXkahgIxTo,13174
 cmrsim/analytic/contrast/t2_star.py,sha256=1TIJVK7VCJliF_dY-iZZX_QbHTYrkCmVCOPA_XseIrI,4764
 cmrsim/analytic/encoding/__init__.py,sha256=JOmanhQ_Q8ld_dv_4WtJPXvz0HI_-F9O-dX6AXOZu4k,707
 cmrsim/analytic/encoding/_from_sequence.py,sha256=dFLFk1qSEs85hypj93MgbNco-4ekr-icH3liXIBg6n0,2010
 cmrsim/analytic/encoding/base.py,sha256=7F9i36t-ussBmRLj0CfcxwBqwTdV5PnHYHPqgToKanw,15979
 cmrsim/analytic/encoding/cartesian.py,sha256=lP1gHOpxuhepa4NZT5pj0NAlJ6QONkHRoFPqWTX_6uw,9365
 cmrsim/bloch/__init__.py,sha256=yOOiwFJzQ_VyAXvwPtOo-Lt1ClItQ-MpcMW2BnMtWxU,493
 cmrsim/bloch/_base.py,sha256=mL556LQBeT04t_k7rbIyzn3mowTOvZewRB507bPSLg0,5423
 cmrsim/bloch/_generic.py,sha256=MAoUzcz4kP-WMGJvkP82zPZImjo4mkfgYOygkW649HE,27333
 cmrsim/bloch/_ideal.py,sha256=bdvxy7XDJ-FHfSEtJQElUyItoIi_1_xeSqeLS3TpT2I,3456
 cmrsim/bloch/_multi_coil.py,sha256=L4OtA0WN-49Sxfu9muJcf-QU8BE5QSpOYwgAw6CoGl8,6674
-cmrsim/bloch/submodules.py,sha256=nz4N7TJzwKFXQZT-TnDy1RrcD8YPprmx5Vn4VQM5Sgw,7960
+cmrsim/bloch/submodules.py,sha256=Nz5cgrvwvL79ED5O2MvLzG5jbBbPQEZ5CZOFCZQ3aAc,7960
 cmrsim/datasets/__init__.py,sha256=6M0sq3lC51UXkZHqzz4bYr0nyqSsmpdkIq4LLioOWoY,702
 cmrsim/datasets/_analytic.py,sha256=rk7-H0N2DukfL0JmOQxQW5F_k2wJ1xAYvk1hVIVEYMQ,3804
 cmrsim/datasets/_base.py,sha256=u81LvuJZXaARTsBblVYzRfNUYWmCiibqCoMxIyNzZJI,2842
 cmrsim/datasets/_bloch.py,sha256=BKTFf17i_gtetC9t44Nu76TYizferzwX0Q9gLmHh7U8,1655
-cmrsim/datasets/_cardiac_mesh.py,sha256=5PpN1dginLvksJanJNjc58zHE9DrMqC9zq9dSNvDBDo,41432
-cmrsim/datasets/_flow.py,sha256=9Hp5fH1ON93F9EzBeqg7Lwph0oJk-_WSFEeHZa0j2mk,23212
+cmrsim/datasets/_cardiac_mesh.py,sha256=BvnmCPS97RoznZrMwR1wurwa_VYLKMnNIxWHKoIvkEI,41423
+cmrsim/datasets/_flow.py,sha256=xRkMtOIDDHcEwRal-NBnpoca-SjCAOKjLVBbixOCR-E,23224
 cmrsim/datasets/_regular_grid.py,sha256=snowk30oL5Md6P4bA-OYRa2wbRvdZivyvGvLlFOmCk4,14057
 cmrsim/reconstruction/__init__.py,sha256=BtyMpXTuc44kylT7yDqcws9w1OWg5X-lvCyyDAFfY-E,140
 cmrsim/reconstruction/base.py,sha256=oLiZZpXVWlStNu81tF3kzkl9MyB09ctSSUvxRQhCOLo,1820
 cmrsim/reconstruction/cartesian.py,sha256=E-hBfhX5iKkK0RwWqu-wyuEYM5u3bCx0ka8rkle6sRA,6823
 cmrsim/simulation_templates/__init__.py,sha256=gVY--lD9ruZAiq0mEUR5Z-iarQQj4MLGO_NJM9AuPiQ,189
 cmrsim/simulation_templates/experimental_optimization.py,sha256=O93dDCQb6p5s0XNHkc3L2KE8QaB2ISlS7n3umIo8lVM,9173
-cmrsim/simulation_templates/flow.py,sha256=Ca-5A5wkncw84KUx9P3l1c2Jq6goHONX1WwveR9xuq8,20327
-cmrsim/trajectory/__init__.py,sha256=yaJCc_eEEm0BuqqC43RBLoPqX4oVhbmZH13SKkoEbIA,1394
+cmrsim/simulation_templates/flow.py,sha256=6-IbQoL6U2cU8i-KGHqAwHnmzton_spk8wMtpGoECiI,20333
+cmrsim/trajectory/__init__.py,sha256=zt2a2jGJz5QUNQtyO7524oJtBOdOxZ6Le2XQLuN38aU,1437
 cmrsim/trajectory/_base.py,sha256=JViZ-Iwo1epG1hLI84c_QiMtr0jJKI5pyRAKKBpRHx4,3296
+cmrsim/trajectory/_breathing.py,sha256=FDigWs7Jx2jZjQFvOJAofIvt0NIWbMAK19qMojQJuGI,5577
 cmrsim/trajectory/_diffusion.py,sha256=7FFpkl8Q2i5kmGM4B71tvCQQQdO3IPnnw0Xs7-k8gmk,8492
-cmrsim/trajectory/_flow.py,sha256=aSGAaa5h16YNEkXxTpkg1kAn_vsbgyTyuYpeJYR0fS0,26052
-cmrsim/trajectory/_proper_ortho_decomp.py,sha256=jV9t0hK3WXbxPrMoUOxPtSjDZD74ny9utI9PKi0algU,8349
-cmrsim/trajectory/_taylor.py,sha256=OZV9BDERKf2fKxzqzucB9P-mKxYvBrrdDa6tal-MXuQ,7160
+cmrsim/trajectory/_flow.py,sha256=JG5KLzOGJ5RGVFhxzOkSrPo765Pj-VBqh5tCDo_8WQs,26071
+cmrsim/trajectory/_proper_ortho_decomp.py,sha256=Ld1S8N7945RcVWDHlguzUziSc0QiyCL3MggxmgRglRA,8394
+cmrsim/trajectory/_taylor.py,sha256=yhZp8aoZ7dL3dj1toAdo4jejSW4TOno4pVNThkR6GMU,7443
 cmrsim/utils/__init__.py,sha256=2RGU3ArstSrIT9aCTRhk_Bg0lfgKtx9fax4YosLcmLY,376
 cmrsim/utils/coordinates.py,sha256=v5K3HxuifZnhVa0gysJeP4hFdu49Z9Rhm5gbP6Q81G4,4170
 cmrsim/utils/display.py,sha256=RcxxU1etz0RdEcIO3YwRO-Ke4XzLGPjNMsSsesXm5As,6671
 cmrsim/utils/particle_properties.py,sha256=uQ39Bn-m8Pmqqh9ClmOI2OFt4Lc0K7GfKyCjzWSjvZg,1246
 cmrsim/utils/snr.py,sha256=0FzHqQF9ozoKxx1N9Gyzt93qL8cFGqjbkUTwXBlEapE,7023
-cmrsim-0.25.dist-info/LICENSE,sha256=YMlRaEyusWa3XSqFtOXCB46lJDU9CmwCp6s45xyijwY,35060
-cmrsim-0.25.dist-info/METADATA,sha256=g4MAv8LNqf8eFb2AxggRXHTh2_9S9y362Mq0K2O7NOA,3473
-cmrsim-0.25.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cmrsim-0.25.dist-info/top_level.txt,sha256=nBnY6lAjSHggBmbuEyNTRh9ZWw0lnCrHZNgNxKGoRJQ,7
-cmrsim-0.25.dist-info/RECORD,,
+cmrsim-0.26.dist-info/LICENSE,sha256=YMlRaEyusWa3XSqFtOXCB46lJDU9CmwCp6s45xyijwY,35060
+cmrsim-0.26.dist-info/METADATA,sha256=2f64HKodaxzjgXfJab9OPHDSURLewVQDcOGbv2KlZJ0,3473
+cmrsim-0.26.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmrsim-0.26.dist-info/top_level.txt,sha256=nBnY6lAjSHggBmbuEyNTRh9ZWw0lnCrHZNgNxKGoRJQ,7
+cmrsim-0.26.dist-info/RECORD,,
```

