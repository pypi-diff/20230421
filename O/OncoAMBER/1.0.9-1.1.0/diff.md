# Comparing `tmp/OncoAMBER-1.0.9.tar.gz` & `tmp/OncoAMBER-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.0.9.tar", last modified: Fri Apr 21 17:45:04 2023, max compression
+gzip compressed data, was "OncoAMBER-1.1.0.tar", last modified: Fri Apr 21 20:53:01 2023, max compression
```

## Comparing `OncoAMBER-1.0.9.tar` & `OncoAMBER-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.413552 OncoAMBER-1.0.9/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.404703 OncoAMBER-1.0.9/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      545 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 17:45:04.413235 OncoAMBER-1.0.9/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2870 2023-04-21 16:41:55.000000 OncoAMBER-1.0.9/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.411516 OncoAMBER-1.0.9/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1784 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Cell.py
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.412843 OncoAMBER-1.0.9/amber/Micro-Oxygenation/
--rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Micro-Oxygenation/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Micro-Oxygenation/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    20622 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1607 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      760 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/RunTopas.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14142 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6181 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    20872 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      176 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/config_instance.py
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 17:45:04.413630 OncoAMBER-1.0.9/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     2967 2023-04-21 17:45:02.000000 OncoAMBER-1.0.9/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.675457 OncoAMBER-1.1.0/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.657758 OncoAMBER-1.1.0/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2381 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      579 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2381 2023-04-21 20:53:01.675158 OncoAMBER-1.1.0/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1626 2023-04-21 20:48:33.000000 OncoAMBER-1.1.0/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.674000 OncoAMBER-1.1.0/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-21 20:10:54.000000 OncoAMBER-1.1.0/amber/CONFIG_default.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1784 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    20986 2023-04-21 20:25:50.000000 OncoAMBER-1.1.0/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.0/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      760 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/RunTopas.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14142 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6181 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    21181 2023-04-21 20:26:24.000000 OncoAMBER-1.1.0/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      597 2023-04-21 19:40:53.000000 OncoAMBER-1.1.0/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      104 2023-04-21 19:20:43.000000 OncoAMBER-1.1.0/amber/config_instance.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 20:53:01.675580 OncoAMBER-1.1.0/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-04-21 20:48:56.000000 OncoAMBER-1.1.0/setup.py
```

### Comparing `OncoAMBER-1.0.9/amber/BasicGeometries.py` & `OncoAMBER-1.1.0/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Cell.py` & `OncoAMBER-1.1.0/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Micro-Oxygenation/BetaDistributionCalibration.py` & `OncoAMBER-1.1.0/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Process.py` & `OncoAMBER-1.1.0/amber/Process.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
         plt.xlabel('Time')
         plt.ylabel('Tumor volume [mm^3]')
         plt.grid(True)
         plt.savefig('Plots/Tumor_size_evolution.png')
         plt.show()
     def show(self, world: World, t = 0): #this function is used to show the world at a certain time
 
+        if not os.path.exists('Plots/CurrentPlotting/'):
+            os.makedirs('Plots/CurrentPlotting/')
+
         DPI = 100
         size = world.half_length
 
         #plot vasculature
         if config.show_tumor_and_vessels_3D:
             fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(25, 25), dpi=150, subplot_kw={'projection': '3d'})
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
@@ -143,25 +146,29 @@
 
             number_tumor_cells.append(sum([voxel.number_of_tumor_cells() for voxel in world.voxel_list]))
             number_necrotic_cells.append(sum([voxel.number_of_necrotic_cells() for voxel in world.voxel_list]))
             tumor_size_ = world.measure_tumor_volume()
             tumor_size.append(tumor_size_ * 1000)
             times.append(self.time)
 
+            if not os.path.exists('DataOutput/'):
+                os.makedirs('DataOutput/')
+
             np.save('DataOutput/number_tumor_cells.npy', number_tumor_cells)
             np.save('DataOutput/number_necrotic_cells.npy', number_necrotic_cells)
             np.save('DataOutput/tumor_size.npy', tumor_size)
             np.save('DataOutput/times.npy', times)
 
             if config.show_cell_and_tumor_volume:
                 self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, tumor_size, times)
 
             self.time += self.dt
 
         print('Simulation finished')
+
         if config.show_final:
             self.show(world, self.time)
 
         return
 
 class Process: #abstract class, represents all the processes that can happen in the simulation
     def __init__(self, name, dt):
@@ -270,16 +277,21 @@
 
 class UpdateCellOxygen(Process):
     def __init__(self, name, dt, voxel_half_length, effective_vessel_radius):
         super().__init__('UpdateState', dt)
         self.voxel_side = int(voxel_half_length*200) #um/100
         self.effective_vessel_radius = effective_vessel_radius
 
-        alpha_file_name = 'Micro-Oxygenation/save_alpha_dataframe' + str(self.voxel_side) + '.csv'
-        beta_file_name = 'Micro-Oxygenation/save_beta_dataframe' + str(self.voxel_side) + '.csv'
+        amber_dir = os.path.abspath(os.path.dirname(__file__))
+
+        alpha_file_name = 'save_alpha_dataframe' + str(self.voxel_side) + '.csv'
+        beta_file_name = 'save_beta_dataframe' + str(self.voxel_side) + '.csv'
+        alpha_file_name = os.path.join(amber_dir, alpha_file_name)
+        beta_file_name = os.path.join(amber_dir, beta_file_name)
+
         if not os.path.isfile(alpha_file_name) or not os.path.isfile(beta_file_name):
             print('voxel side', self.voxel_side)
             raise ValueError('alpha/beta file not found! It might be in the wrong directory or information for chosen voxel size is not stored. Check "BetaDistributionCalibration.py" to generate the file for the chosen voxel size.')
 
         alpha_dataframe = pd.read_csv(alpha_file_name, index_col=0)
         beta_dataframe = pd.read_csv(beta_file_name, index_col=0)
         # Read the saved dataframes from the CSV files
```

### Comparing `OncoAMBER-1.0.9/amber/ReadAndWrite.py` & `OncoAMBER-1.1.0/amber/ReadAndWrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 
-
 def DoseOnWorld(file_path : str):
     # Get the current dose on the world
     # file_path is the path to the file containing the dose
     nn = np.array([])
     doses = np.array([])
     arr = np.loadtxt(file_path, skiprows=1, delimiter=",")
     num_voxels = len(np.unique(arr[:, 0]))
```

### Comparing `OncoAMBER-1.0.9/amber/RunTopas.py` & `OncoAMBER-1.1.0/amber/RunTopas.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/ScalarField.py` & `OncoAMBER-1.1.0/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Terminal.py` & `OncoAMBER-1.1.0/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Vessel.py` & `OncoAMBER-1.1.0/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/Voxel.py` & `OncoAMBER-1.1.0/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.9/amber/World.py` & `OncoAMBER-1.1.0/amber/World.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
 from scipy.stats import qmc
 import matplotlib.tri as mtri
 import scipy.sparse as sparse
 from amber.config_instance import config
 
-
-
 class World:
     def __init__(self, half_length, number_of_voxels : int = 20):
         self.half_length = half_length
         self.voxel_list = []
         self.total_number_of_voxels = number_of_voxels ** 3
         voxel_length = 2 * half_length / number_of_voxels
 
@@ -49,15 +47,15 @@
                                         weight_vegf = weight_vegf,
                                         weight_pressure = weight_pressure,
                                         pressure = pressure,
                                         vegf_gradient = vegf_gradient)
         self.vasculature.update_vessels_radius_from_last(config.radius_root_vessels, radius_pressure_sensitive, pressure)
         return
 
-    def generate_healthy_vasculature(self, initial_vessel_number):
+    def generate_healthy_vasculature(self, initial_vessel_number, splitting_rate =0.3, mult_macro_steps=1, micro_steps=8, weight_direction=3.0, weight_vegf=1.0, weight_pressure=0.0, extra_step = True):
         initial_vessel_number = int(initial_vessel_number * 4 * self.half_length ** 2)
         sampler = qmc.Halton(2, seed=config.seed)
         points_z = (sampler.random(initial_vessel_number)[:,0] - 0.5) * self.half_length*2
         points_y = (sampler.random(initial_vessel_number)[:,1] - 0.5) * self.half_length*2
         points_x = np.append(self.half_length * np.ones(initial_vessel_number//2), -self.half_length * np.ones(initial_vessel_number//2))
         points = []
         for i in range(len(points_x)):
@@ -73,43 +71,44 @@
         print('Initial vessels: ', points[0], points2[0])
 
         list_of_vessels = []
         for j in range(len(points)):
             list_of_vessels.append(Vessel([points[j], points2[j]], 0.5))
         self.initiate_vasculature(list_of_vessels)
         def pressure(point):
-            return (self.half_length - abs(point[0]))
+            return (self.half_length - abs(point[0]))*0.3
         def vegf_gradient(point):
             if point[0] > 0:
                 return np.array([-point[0],0,0])*0.1
             else:
                 return np.array([-point[0],0,0])*0.1
 
         self.vasculature.grow_and_split(
             dt=1,
-            splitting_rate=0.3,
+            splitting_rate=splitting_rate,
             vegf_gradient= vegf_gradient,
             pressure= pressure,
-            macro_steps=int(8.5*self.half_length),
-            micro_steps=8,
-            weight_direction=3.0,
-            weight_vegf=1.0,
-            weight_pressure=0.0
-        )
-        self.vasculature.grow_and_split(
-            dt=1,
-            splitting_rate=0.3,
-            vegf_gradient=vegf_gradient,
-            pressure=pressure,
-            macro_steps=1,
-            micro_steps=8,
-            weight_direction=5.0,
-            weight_vegf=0.1,
-            weight_pressure=0.0
+            macro_steps=int(8.5*self.half_length*mult_macro_steps),
+            micro_steps=micro_steps,
+            weight_direction=weight_direction,
+            weight_vegf=weight_vegf,
+            weight_pressure=weight_pressure
         )
+        if extra_step:
+            self.vasculature.grow_and_split(
+                dt=1,
+                splitting_rate=splitting_rate,
+                vegf_gradient=vegf_gradient,
+                pressure=pressure,
+                macro_steps=1,
+                micro_steps=micro_steps,
+                weight_direction=weight_direction,
+                weight_vegf=0.1,
+                weight_pressure=0.0
+            )
 
 
         self.vasculature.update_vessels_radius_from_last(config.radius_root_vessels, False, pressure)
         for vessel in self.vasculature.list_of_vessels:
             vessel.in_growth = False
             vessel.visible = config.visible_original_vessels
         return
```

### Comparing `OncoAMBER-1.0.9/setup.py` & `OncoAMBER-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
 
@@ -84,17 +84,18 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(),
+    package_data={'': ['*.txt', '*.csv'],},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     # include_package_data=True,
     zip_safe=False,
     license='MIT',
-    classifiers=[    'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
+    classifiers=[   'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
     cmdclass={
         'upload' : UploadCommand,
     }
 )
```

