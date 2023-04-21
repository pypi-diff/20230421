# Comparing `tmp/OncoAMBER-1.0.8.tar.gz` & `tmp/OncoAMBER-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.0.8.tar", last modified: Fri Apr 21 16:42:26 2023, max compression
+gzip compressed data, was "OncoAMBER-1.0.9.tar", last modified: Fri Apr 21 17:45:04 2023, max compression
```

## Comparing `OncoAMBER-1.0.8.tar` & `OncoAMBER-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:42:26.326007 OncoAMBER-1.0.8/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:42:26.314767 OncoAMBER-1.0.8/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 16:42:26.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      515 2023-04-21 16:42:26.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:42:26.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 16:42:26.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        4 2023-04-21 16:42:26.000000 OncoAMBER-1.0.8/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 16:42:26.325621 OncoAMBER-1.0.8/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2870 2023-04-21 16:41:55.000000 OncoAMBER-1.0.8/README.md
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 16:42:26.326094 OncoAMBER-1.0.8/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     2967 2023-04-21 16:42:24.000000 OncoAMBER-1.0.8/setup.py
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:42:26.324093 OncoAMBER-1.0.8/src/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1782 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Cell.py
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:42:26.325285 OncoAMBER-1.0.8/src/Micro-Oxygenation/
--rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Micro-Oxygenation/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Micro-Oxygenation/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    20610 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1607 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      752 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/RunTopas.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14138 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6179 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    20862 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      172 2023-04-21 16:39:43.000000 OncoAMBER-1.0.8/src/config_instance.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.413552 OncoAMBER-1.0.9/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.404703 OncoAMBER-1.0.9/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      545 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-21 17:45:04.000000 OncoAMBER-1.0.9/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3625 2023-04-21 17:45:04.413235 OncoAMBER-1.0.9/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2870 2023-04-21 16:41:55.000000 OncoAMBER-1.0.9/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.411516 OncoAMBER-1.0.9/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1784 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Cell.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 17:45:04.412843 OncoAMBER-1.0.9/amber/Micro-Oxygenation/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Micro-Oxygenation/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Micro-Oxygenation/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    20622 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1607 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      760 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/RunTopas.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14142 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6181 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    20872 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)        0 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.0.9/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      176 2023-04-21 17:44:48.000000 OncoAMBER-1.0.9/amber/config_instance.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 17:45:04.413630 OncoAMBER-1.0.9/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2967 2023-04-21 17:45:02.000000 OncoAMBER-1.0.9/setup.py
```

### Comparing `OncoAMBER-1.0.8/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.0.9/OncoAMBER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.8
+Version: 1.0.9
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.8/PKG-INFO` & `OncoAMBER-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.0.8
+Version: 1.0.9
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.0.8/README.md` & `OncoAMBER-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/setup.py` & `OncoAMBER-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```

### Comparing `OncoAMBER-1.0.8/src/BasicGeometries.py` & `OncoAMBER-1.0.9/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/src/Cell.py` & `OncoAMBER-1.0.9/amber/Cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from src.config_instance import config
+from amber.config_instance import config
 
 class Cell (object):
     def __init__(self, radius, cycle_hours = 10, type = 'NormalCell'):
         self.radius = radius
         self.necrotic = False
         self.usual_cycle_length = cycle_hours
         self.doubling_time = self.random_doubling_time(self.usual_cycle_length, config.doubling_time_sd) #new cells have a random doubling time
```

### Comparing `OncoAMBER-1.0.8/src/Micro-Oxygenation/BetaDistributionCalibration.py` & `OncoAMBER-1.0.9/amber/Micro-Oxygenation/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/src/Process.py` & `OncoAMBER-1.0.9/amber/Process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from src.World import *
-from src.Voxel import *
-from src.ScalarField import *
-import src.Terminal as term
-import src.ReadAndWrite as rw
+from amber.World import *
+from amber.Voxel import *
+from amber.ScalarField import *
+import amber.Terminal as term
+import amber.ReadAndWrite as rw
 import pandas as pd
 from matplotlib.colors import TwoSlopeNorm
-from src.config_instance import config
+from amber.config_instance import config
 import matplotlib.pyplot as plt
 import os
 
 class Simulator: #this class is used to run the whole simulation
 
     def __init__(self, list_of_process : list, finish_time, dt):
         self.list_of_process = list_of_process
```

### Comparing `OncoAMBER-1.0.8/src/ReadAndWrite.py` & `OncoAMBER-1.0.9/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/src/RunTopas.py` & `OncoAMBER-1.0.9/amber/RunTopas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from src.Terminal import *
+from amber.Terminal import *
 import os
-import src.ReadAndWrite as rw
-from src.World import World
+import amber.ReadAndWrite as rw
+from amber.World import World
 import matplotlib.pyplot as plt
-from src.config_instance import config
+from amber.config_instance import config
 
 def RunTopasSimulation():
 
     world = World(config.half_length_world, config.voxel_per_side)
     world.topas_param_file(config.TOPAS_file)
     RunTopasSimulation(config.TOPAS_file)
```

### Comparing `OncoAMBER-1.0.8/src/ScalarField.py` & `OncoAMBER-1.0.9/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/src/Terminal.py` & `OncoAMBER-1.0.9/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.0.8/src/Vessel.py` & `OncoAMBER-1.0.9/amber/Vessel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
-from src.BasicGeometries import *
+from amber.BasicGeometries import *
 import sys
-from src.config_instance import config
+from amber.config_instance import config
 
 sys.setrecursionlimit(1500)
 rng = np.random.default_rng(config.seed)
 
 class Vessel:
     def __init__(self, path, radius, parent_id=None, children_ids=None, in_growth=True):
         if children_ids is None:
```

### Comparing `OncoAMBER-1.0.8/src/Voxel.py` & `OncoAMBER-1.0.9/amber/Voxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from src.config_instance import config
+from amber.config_instance import config
 
 def sigmoid(L, x, x0, k):
     return L/(1 + np.exp(-k*(x-x0)))
 
 class Voxel(object): #extra parameters are max_occupancy, viscosity
         def __init__(self, position = np.array([0,0,0]), half_length = 0.1, list_of_cells_in=None, oxygen = 0, voxel_number = 0):
                 if list_of_cells_in is None:
```

### Comparing `OncoAMBER-1.0.8/src/World.py` & `OncoAMBER-1.0.9/amber/World.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from src.Voxel import *
-from src.Vessel import *
-from src.ScalarField import *
-from src.BasicGeometries import *
+from amber.Voxel import *
+from amber.Vessel import *
+from amber.ScalarField import *
+from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
 from scipy.stats import qmc
 import matplotlib.tri as mtri
 import scipy.sparse as sparse
-from src.config_instance import config
+from amber.config_instance import config
 
 
 
 class World:
     def __init__(self, half_length, number_of_voxels : int = 20):
         self.half_length = half_length
         self.voxel_list = []
```

