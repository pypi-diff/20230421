# Comparing `tmp/napari-generic-SIMulator-0.0.8.tar.gz` & `tmp/napari-generic-SIMulator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-generic-SIMulator-0.0.8.tar", last modified: Fri Jul  1 13:04:49 2022, max compression
+gzip compressed data, was "napari-generic-SIMulator-0.0.9.tar", last modified: Fri Jul  1 13:54:58 2022, max compression
```

## Comparing `napari-generic-SIMulator-0.0.8.tar` & `napari-generic-SIMulator-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.209210 napari-generic-SIMulator-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-07-01 13:04:49.217210 napari-generic-SIMulator-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.209210 napari-generic-SIMulator-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-07-01 13:04:48.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-01 13:04:49.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 13:04:48.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-01 13:04:48.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-01 13:04:48.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-01 13:04:48.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:49.213210 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-01 13:04:47.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/baseSIMulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/hexSIMulator.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11396 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/raw_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-07-01 13:04:26.000000 napari-generic-SIMulator-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.340675 napari-generic-SIMulator-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/.napari/
+-rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-07-01 13:54:58.340675 napari-generic-SIMulator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-07-01 13:54:58.340675 napari-generic-SIMulator-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-07-01 13:54:57.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-01 13:54:58.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 13:54:57.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-01 13:54:57.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-01 13:54:58.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-01 13:54:58.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.336675 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:58.340675 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-01 13:54:57.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/baseSIMulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/hexSIMulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11396 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/raw_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-07-01 13:54:40.000000 napari-generic-SIMulator-0.0.9/tox.ini
```

### Comparing `napari-generic-SIMulator-0.0.8/.github/workflows/test_and_deploy.yml` & `napari-generic-SIMulator-0.0.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/.gitignore` & `napari-generic-SIMulator-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/.napari/DESCRIPTION.md` & `napari-generic-SIMulator-0.0.9/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/.pre-commit-config.yaml` & `napari-generic-SIMulator-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/LICENSE` & `napari-generic-SIMulator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/PKG-INFO` & `napari-generic-SIMulator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-generic-SIMulator
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple plugin to use with napari to simulate raw image stacks in Structured illumination microscopy (SIM) with napari.
 Home-page: https://github.com/Meizhu-Liang/napari-generic-SIMulator
 Author: Meizhu Liang
 Author-email: ml2618@ic.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Meizhu-Liang/napari-generic-SIMulator/issues
 Project-URL: Documentation, https://github.com/Meizhu-Liang/napari-generic-SIMulator#README.md
```

### Comparing `napari-generic-SIMulator-0.0.8/README.md` & `napari-generic-SIMulator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/setup.cfg` & `napari-generic-SIMulator-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/PKG-INFO` & `napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-generic-SIMulator
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple plugin to use with napari to simulate raw image stacks in Structured illumination microscopy (SIM) with napari.
 Home-page: https://github.com/Meizhu-Liang/napari-generic-SIMulator
 Author: Meizhu Liang
 Author-email: ml2618@ic.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Meizhu-Liang/napari-generic-SIMulator/issues
 Project-URL: Documentation, https://github.com/Meizhu-Liang/napari-generic-SIMulator#README.md
```

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_SIMulator.egg-info/SOURCES.txt` & `napari-generic-SIMulator-0.0.9/src/napari_generic_SIMulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/_widget.py` & `napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 @authors: Meizhu Liang @Imperial College
 """
 
-from magicgui import magicgui, magic_factory
+from magicgui import magicgui
 from magicgui.widgets import Container
 from enum import Enum
 from napari_generic_simulator.baseSIMulator import import_cp
 from napari_generic_simulator.hexSIMulator import HexSim_simulator, RightHexSim_simulator
 from qtpy.QtWidgets import QWidget, QVBoxLayout
 
 class Sim_mode(Enum):
@@ -27,30 +27,30 @@
 class SIMulator(QWidget):
     """
     A Napari plugin for the simulation of raw images produced while scanning an object (3D point cloud) through focus as
     the hexSIM illumination pattern is shifted through 7 positions laterally.The raw data is processed by a standard, a
     frame-by-frame and a batch reconstruction to produce the super-resolved output.https://doi.org/10.1098/rsta.2020.0162
     This currently supports hexagonal SIM (1 angle, 7 phases) with three beams and that at right-angles.
     """
-    def __init__(self, viewer):
-        self.viewer = viewer
+    def __init__(self, viewer: 'napari.viewer.Viewer'):
+        self._viewer = viewer
         super().__init__()
         self.parameters()
         self.setup_ui()
         self.start_simulator()
 
     def setup_ui(self):
         self.wrap_widgets()
         layout = QVBoxLayout()
         self.setLayout(layout)
         self.add_magic_function(self.w, layout)
 
     def add_magic_function(self, function, _layout):
-        self.viewer.layers.events.inserted.connect(function.reset_choices)
-        self.viewer.layers.events.removed.connect(function.reset_choices)
+        self._viewer.layers.events.inserted.connect(function.reset_choices)
+        self._viewer.layers.events.removed.connect(function.reset_choices)
         _layout.addWidget(function.native)
 
     def parameters(self, SIM_mode=Sim_mode.HEXSIM_RIGHT_ANGLES, Polarisation=Pol.IN_PLANE, Acceleration=list(Accel)[-1],
                    N: int = 512, pixel_size: float = 5.5, magnification: int = 60, NA: float = 1.1, n: float = 1.33,
                    wavelength: float = 0.52, npoints: int = 500, zrange: float = 7.0, dz: float = 0.4,
                    fwhmz: float = 3.0):
         self.SIM_mode = SIM_mode.value
@@ -125,59 +125,59 @@
         Calculates the 3D PSF and shows it as a stack
         '''
         img = self.sim.point_cloud
 
         # self.viewer.add_image(img,
         #                       name=self.gen.write_name(basename=f'xy_{text}'),
         #                       colormap='twilight')
-        self.viewer.add_image(img)
+        self._viewer.add_image(img)
 
     def get_results(self):
         self.set_att()
         self.re0, self.re1, self.re2, self.re3, self.re4, self.re5 = self.sim.raw_image_stack()
         self.used_par_list = [self.SIM_mode, self.Polarisation,self.Acceleration, self.N, self.pixel_size,
                               self.magnification, self.NA, self.n, self.wavelength, self.npoints, self.zrange, self.dz,
                               self.fwhmz]
 
     def show_img(self):
         self.get_results()
-        self.viewer.add_image(data=self.re0, name='raw image stack')
+        self._viewer.add_image(data=self.re0, name='raw image stack')
 
     def show_raw_img_sum(self, show_raw_img_sum: bool=False):
         if show_raw_img_sum:
             if hasattr(self, 're1'):
                 if self.used_par_list != self.par_list:
                     print('To ensure calculate the raw images stack first.')
                 else:
                     try:
-                        self.viewer.add_image(self.re1, name='raw image sum along z axis')
-                        self.viewer.add_image(self.re2, name='raw image sum along x (or y) axis')
+                        self._viewer.add_image(self.re1, name='raw image sum along z axis')
+                        self._viewer.add_image(self.re2, name='raw image sum along x (or y) axis')
                     except Exception as e:
                         print(str(e))
 
     def show_psf(self, show_3D_psf: bool=False):
         if show_3D_psf:
             if hasattr(self, 're3'):
                 if self.used_par_list != self.par_list:
                     print('To ensure calculate the raw images stack before the psf')
                 else:
                     try:
-                        self.viewer.add_image(self.re3, name='PSF in x-y plane')
+                        self._viewer.add_image(self.re3, name='PSF in x-y plane')
                     except Exception as e:
                         print(e)
 
     def show_otf(self, show_3D_otf: bool=False):
         if show_3D_otf:
             if hasattr(self, 're4'):
                 if self.used_par_list != self.par_list:
                     print('To ensure calculate the raw images stack before the otf')
                 else:
                     try:
-                        self.viewer.add_image(self.re4, name='OTF in y-z plane')
-                        self.viewer.add_image(self.re5, name='OTF in x-z plane')
+                        self._viewer.add_image(self.re4, name='OTF in y-z plane')
+                        self._viewer.add_image(self.re5, name='OTF in x-z plane')
                     except Exception as e:
                         print(str(e))
 
     def wrap_widgets(self):
         w1 = magicgui(self.parameters, layout="vertical", auto_call=True)
         w2 = magicgui(self.show_img, call_button="Calculate raw image stack", auto_call=False)
         w3 = magicgui(self.show_raw_img_sum, auto_call=True)
```

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/baseSIMulator.py` & `napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/baseSIMulator.py`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/hexSIMulator.py` & `napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/hexSIMulator.py`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/src/napari_generic_simulator/raw_data_generator.py` & `napari-generic-SIMulator-0.0.9/src/napari_generic_simulator/raw_data_generator.py`

 * *Files identical despite different names*

### Comparing `napari-generic-SIMulator-0.0.8/tox.ini` & `napari-generic-SIMulator-0.0.9/tox.ini`

 * *Files identical despite different names*

