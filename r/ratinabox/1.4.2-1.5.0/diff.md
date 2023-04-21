# Comparing `tmp/ratinabox-1.4.2.tar.gz` & `tmp/ratinabox-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.4.2.tar", last modified: Tue Apr 18 10:51:10 2023, max compression
+gzip compressed data, was "ratinabox-1.5.0.tar", last modified: Fri Apr 21 10:47:30 2023, max compression
```

## Comparing `ratinabox-1.4.2.tar` & `ratinabox-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.488671 ratinabox-1.4.2/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.2/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-18 10:51:10.488791 ratinabox-1.4.2/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.4.2/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.2/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.478964 ratinabox-1.4.2/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41124 2023-04-11 16:33:06.000000 ratinabox-1.4.2/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    80397 2023-04-17 13:49:59.000000 ratinabox-1.4.2/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.2/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.481601 ratinabox-1.4.2/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.2/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.2/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.2/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.2/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.2/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15009 2023-04-11 17:03:00.000000 ratinabox-1.4.2/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.2/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.2/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.483536 ratinabox-1.4.2/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.2/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.2/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.2/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.2/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    30579 2023-04-17 12:58:07.000000 ratinabox-1.4.2/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.479894 ratinabox-1.4.2/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-18 10:51:10.489117 ratinabox-1.4.2/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.2/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.488539 ratinabox-1.4.2/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.4.2/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.2/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.2/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.2/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.766506 ratinabox-1.5.0/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.5.0/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 10:47:30.766679 ratinabox-1.5.0/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.5.0/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.5.0/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.758424 ratinabox-1.5.0/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41178 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    31941 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    80998 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.5.0/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.5.0/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.760956 ratinabox-1.5.0/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8805 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5787 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3935 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.5.0/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.5.0/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15034 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7275 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.5.0/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.762472 ratinabox-1.5.0/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.5.0/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.5.0/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.5.0/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.5.0/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.5.0/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34227 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.759321 ratinabox-1.5.0/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-21 10:47:30.767187 ratinabox-1.5.0/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.5.0/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.766344 ratinabox-1.5.0/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.5.0/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.5.0/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.5.0/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.5.0/tests/test_neurons.py
```

### Comparing `ratinabox-1.4.2/LICENSE` & `ratinabox-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/PKG-INFO` & `ratinabox-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.2
+Version: 1.5.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.4.2/README.md` & `ratinabox-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/Agent.py` & `ratinabox-1.5.0/ratinabox/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ratinabox
 
+import copy
 import numpy as np
 import os
 import matplotlib
 from matplotlib import pyplot as plt
 
 
 from ratinabox import utils
@@ -44,42 +45,46 @@
             "walls_repel": True,
             "save_history":True,
 
 
         }
     """
 
+    default_params = {
+        "dt": 0.01,
+        # Speed params (leave empty if you are importing trajectory data)
+        # These defaults are fit to match data from Sargolini et al. (2016)
+        # also given are the parameter names as refered to in the methods section of the paper
+        "speed_coherence_time": 0.7,  # time over which speed decoheres, τ_v1 & τ_v2
+        "speed_mean": 0.08,  # mean of speed, σ_v2 μ_v1
+        "speed_std": 0.08,  # std of speed (meaningless in 2D where speed ~rayleigh), σ_v1
+        "rotational_velocity_coherence_time": 0.08,  # time over which speed decoheres, τ_w
+        "rotational_velocity_std": (
+            120 * (np.pi / 180)
+        ),  # std of rotational speed, σ_w wall following parameter
+        "thigmotaxis": 0.5,  # tendency for agents to linger near walls [0 = not at all, 1 = max]
+        "wall_repel_distance": 0.1,
+        "walls_repel": True,  # whether or not the walls repel
+        "save_history": True,  # whether to save position and velocity history as you go
+    }
+
     def __init__(self, Environment, params={}):
         """Initialise Agent, takes as input a parameter dictionary.
         Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
-        default_params = {
-            "dt": 0.01,
-            # Speed params (leave empty if you are importing trajectory data)
-            # These defaults are fit to match data from Sargolini et al. (2016)
-            # also given are the parameter names as refered to in the methods section of the paper
-            "speed_coherence_time": 0.7,  # time over which speed decoheres, τ_v1 & τ_v2
-            "speed_mean": 0.08,  # mean of speed, σ_v2 μ_v1
-            "speed_std": 0.08,  # std of speed (meaningless in 2D where speed ~rayleigh), σ_v1
-            "rotational_velocity_coherence_time": 0.08,  # time over which speed decoheres, τ_w
-            "rotational_velocity_std": (
-                120 * (np.pi / 180)
-            ),  # std of rotational speed, σ_w wall following parameter
-            "thigmotaxis": 0.5,  # tendency for agents to linger near walls [0 = not at all, 1 = max]
-            "wall_repel_distance": 0.1,
-            "walls_repel": True,  # whether or not the walls repel
-            "save_history": True,  # whether to save position and velocity history as you go
-        }
         self.Environment = Environment
-        default_params.update(params)
-        self.params = default_params
-        utils.update_class_params(self, self.params)
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
+        utils.update_class_params(self, self.params, get_all_defaults=True)
+        utils.check_params(self, params.keys())
 
         # initialise history dataframes
         self.history = {}
         self.history["t"] = []
         self.history["pos"] = []
         self.history["vel"] = []
         self.history["rot_vel"] = []
@@ -93,26 +98,26 @@
         # motion model stufff
         self.walls_repel = True  # over ride to switch of wall repulsion
 
         # initialise starting positions and velocity
         if self.Environment.dimensionality == "2D":
             self.pos = self.Environment.sample_positions(n=1, method="random")[0]
             direction = np.random.uniform(0, 2 * np.pi)
-            self.velocity = self.speed_std * np.array(
+            self.velocity = self.speed_mean * np.array(
                 [np.cos(direction), np.sin(direction)]
             )
             self.rotational_velocity = 0
 
         if self.Environment.dimensionality == "1D":
             self.pos = self.Environment.sample_positions(n=1, method="random")[0]
             self.velocity = np.array([self.speed_mean])
             if self.Environment.boundary_conditions == "solid":
                 if self.speed_mean != 0:
                     print(
-                        "Warning you have solid 1D boundary conditions and non-zero speed mean. "
+                        "Warning: You have solid 1D boundary conditions and non-zero speed mean."
                     )
 
         if ratinabox.verbose is True:
             print(
                 f"""An Agent has been successfully initialised with the following parameters {self.params}.
                 Use Ag.update() to move the Agent.
                 Positions and velocities are saved into the Agent.history dictionary.
```

### Comparing `ratinabox-1.4.2/ratinabox/Environment.py` & `ratinabox-1.5.0/ratinabox/Environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ratinabox
 
+import copy
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import shapely
 
 import warnings
 
@@ -42,33 +43,36 @@
             "aspect": 1,
             "dx": 0.01,
             "boundary":None #defaults to rectangular
             "holes":[],#defaults to no holes
         }
     """
 
+    default_params = {
+        "dimensionality": "2D",  # 1D or 2D environment
+        "boundary_conditions": "solid",  # solid vs periodic
+        "scale": 1,  # scale of environment (in metres)
+        "aspect": 1,  # x/y aspect ratio for the (rectangular) 2D environment (how wide this is relative to tall)
+        "dx": 0.01,  # discretises the environment (for plotting purposes only)
+        "boundary": None,  # coordinates [[x0,y0],[x1,y1],...] of the corners of a 2D polygon bounding the Env (if None, Env defaults to rectangular). Corners must be ordered clockwise or anticlockwise, and the polygon must be a 'simple polygon' (no holes, doesn't self-intersect).
+        "holes": [],  # coordinates [[[x0,y0],[x1,y1],...],...] of corners of any holes inside the Env. These must be entirely inside the environment and not intersect one another. Corners must be ordered clockwise or anticlockwise. holes has 1-dimension more than boundary since there can be multiple holes
+    }
+
     def __init__(self, params={}):
         """Initialise Environment, takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
-        default_params = {
-            "dimensionality": "2D",  # 1D or 2D environment
-            "boundary_conditions": "solid",  # solid vs periodic
-            "scale": 1,  # scale of environment (in metres)
-            "aspect": 1,  # x/y aspect ratio for the (rectangular) 2D environment (how wide this is relative to tall)
-            "dx": 0.01,  # discretises the environment (for plotting purposes only)
-            "boundary": None,  # coordinates [[x0,y0],[x1,y1],...] of the corners of a 2D polygon bounding the Env (if None, Env defaults to rectangular). Corners must be ordered clockwise or anticlockwise, and the polygon must be a 'simple polygon' (no holes, doesn't self-intersect).
-            "holes": [],  # coordinates [[[x0,y0],[x1,y1],...],...] of corners of any holes inside the Env. These must be entirely inside the environment and not intersect one another. Corners must be ordered clockwise or anticlockwise. holes has 1-dimension more than boundary since there can be multiple holes
-        }
 
-        default_params.update(params)
-        self.params = default_params
-        utils.update_class_params(self, self.params)
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
+        utils.update_class_params(self, self.params, get_all_defaults=True)
+        utils.check_params(self, params.keys())
 
         if self.dimensionality == "1D":
             self.D = 1
             self.extent = np.array([0, self.scale])
             self.centre = np.array([self.scale / 2, self.scale / 2])
 
         elif self.dimensionality == "2D":
```

### Comparing `ratinabox-1.4.2/ratinabox/Neurons.py` & `ratinabox-1.5.0/ratinabox/Neurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ratinabox
 
+import copy
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import scipy
 from scipy import stats as stats
 
 from ratinabox import utils
@@ -30,22 +31,25 @@
     • ValueNeuron()
     • FieldOfViewNeurons()
 
     The unique function in each child classes is get_state(). Whenever Neurons.update() is called Neurons.get_state() is then called to calculate and return the firing rate of the cells at the current moment in time. This is then saved. In order to make your own Neuron subclass you will need to write a class with the following mandatory structure:
 
     ============================================================================================
     MyNeuronClass(Neurons):
+
+        default_params = {'a_default_param":3.14159} # default params dictionary is defined in the preamble, as a class attribute. Note its values are passed upwards and used in all the parents classes of your class.
+    
         def __init__(self,
                      Agent,
                      params={}): #<-- do not change these
 
-            default_params = {'a_default_param":3.14159} #note this params dictionary is passed upwards and used in all the parents classes of your class.
 
-            default_params.update(params)
-            self.params = default_params
+            self.params = copy.deepcopy(self.__class__.default_params) # it is best to retrieve the default param dictionary as self.__class__. Then, make sure to deepcopy it, as only making a shallow copy can have unintended consequences (i.e., any modifications to it would be propagated to ALL instances of this class!).
+            self.params.update(params)
+
             super().__init__(Agent,self.params)
 
         def get_state(self,
                       evaluate_at='agent',
                       **kwargs) #<-- do not change these
 
             firingrate = .....
@@ -76,34 +80,39 @@
     default_params = {
             "n": 10,
             "name": "Neurons",
             "color": None,  # just for plotting
         }
     """
 
+    default_params = {
+        "n": 10,
+        "name": "Neurons",
+        "color": None,  # just for plotting
+        "noise_std": 0,  # 0 means no noise, std of the noise you want to add (Hz)
+        "noise_coherence_time": 0.5,
+        "save_history": True,  # whether to save history (set to False if you don't intend to access Neuron.history for data after, for better memory performance)
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise Neurons(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}.
 
         Typically you will not actually initialise a Neurons() class, instead you will initialised by one of it's subclasses.
         """
-        default_params = {
-            "n": 10,
-            "name": "Neurons",
-            "color": None,  # just for plotting
-            "noise_std": 0,  # 0 means no noise, std of the noise you want to add (Hz)
-            "noise_coherence_time": 0.5,
-            "save_history": True,  # whether to save history (set to Falsem if you don't intend to acess Neuron.history for data after, for better memory performance)
-        }
+
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
-        utils.update_class_params(self, self.params)
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
+        utils.update_class_params(self, self.params, get_all_defaults=True)
+        utils.check_params(self, params.keys())
 
         self.firingrate = np.zeros(self.n)
         self.noise = np.zeros(self.n)
 
         self.history = {}
         self.history["t"] = []
         self.history["firingrate"] = []
@@ -183,17 +192,14 @@
         spike_data = np.array(self.history["spikes"][startid:endid])
         t = t[startid:endid]
 
         # neurons to plot
         chosen_neurons = self.return_list_of_neurons(chosen_neurons)
         n_neurons_to_plot = len(chosen_neurons)
         if ("shift" not in kwargs.keys()) and ("overlap" not in kwargs.keys()):
-            kwargs["shift"] = max(
-                1.5, min(4, 40 / n_neurons_to_plot)
-            )  # scaled to make plots look nice and be ~constant size
             kwargs["shift"] = 2
             kwargs["overlap"] = 2.2
         spike_data = spike_data[startid:endid, chosen_neurons]
         rate_timeseries = rate_timeseries[:, chosen_neurons]
         if color is None:
             color = self.color
         if imshow == False:
@@ -454,20 +460,17 @@
 
             if fig is None and ax is None:
                 fig, ax = self.Agent.Environment.plot_environment(
                     autosave=False,
                 )
 
             if method != "neither":
-                kwargs = {}
-                kwargs["shift"] = max(
-                    1.5, min(4, 40 / len(chosen_neurons))
-                )  # scaled to make plots look nice and be ~constant size
-                kwargs["shift"] = 2
-                kwargs["overlap"] = 2.2
+                if ("shift" not in kwargs.keys()) and ("overlap" not in kwargs.keys()):
+                    kwargs["shift"] = 2
+                    kwargs["overlap"] = 2.2
                 fig, ax = utils.mountain_plot(
                     X=x, NbyX=rate_maps, color=self.color, fig=fig, ax=ax, **kwargs
                 )
 
             if spikes is True:
                 for i in range(len(chosen_neurons)):
                     pos_ = pos[:, 0]
@@ -642,34 +645,38 @@
                "wall_geometry": "geodesic",
                "min_fr": 0,
                "max_fr": 1,
                "name": "PlaceCells",
            }
     """
 
+    default_params = {
+        "n": 10,
+        "name": "PlaceCells",
+        "description": "gaussian",
+        "widths": 0.20,  # the radii
+        "place_cell_centres": None,  # if given this will overwrite 'n',
+        "wall_geometry": "geodesic",
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "PlaceCells",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise PlaceCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
-        default_params = {
-            "n": 10,
-            "name": "PlaceCells",
-            "description": "gaussian",
-            "widths": 0.20,  # the radii
-            "place_cell_centres": None,  # if given this will overwrite 'n',
-            "wall_geometry": "geodesic",
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "PlaceCells",
-        }
+
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+        
         super().__init__(Agent, self.params)
 
         if self.place_cell_centres is None:
             self.place_cell_centres = self.Agent.Environment.sample_positions(
                 n=self.n, method="uniform_jitter"
             )
         elif type(self.place_cell_centres) is str:
@@ -776,17 +783,24 @@
         if fig is None and ax is None:
             fig, ax = self.Agent.Environment.plot_environment(autosave=False)
         else:
             _, _ = self.Agent.Environment.plot_environment(
                 fig=fig, ax=ax, autosave=False
             )
         place_cell_centres = self.place_cell_centres
+
+        x = place_cell_centres[:, 0]
+        if self.Agent.Environment.dimensionality == "1D":
+            y = np.zeros_like(x)
+        elif self.Agent.Environment.dimensionality == "2D":
+            y = place_cell_centres[:, 1]
+
         ax.scatter(
-            place_cell_centres[:, 0],
-            place_cell_centres[:, 1],
+            x,
+            y,
             c="C1",
             marker="x",
             s=15,
             zorder=2,
         )
         ratinabox.utils.save_figure(fig, "place_cell_locations", save=autosave)
 
@@ -811,33 +825,37 @@
             "random_phase_offsets": True,
             "min_fr": 0,
             "max_fr": 1,
             "name": "GridCells",
         }
     """
 
+    default_params = {
+        "n": 10,
+        "gridscale": 0.45,
+        "random_orientations": True,
+        "random_gridscales": True,
+        "random_phase_offsets": True,
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "GridCells",
+    }
+
+
     def __init__(self, Agent, params={}):
         """Initialise GridCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
-        default_params = {
-            "n": 10,
-            "gridscale": 0.45,
-            "random_orientations": True,
-            "random_gridscales": True,
-            "random_phase_offsets": True,
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "GridCells",
-        }
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)      
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
 
         # Initialise grid cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "grid cells only available in 2D"
         if self.random_phase_offsets == True:
@@ -945,35 +963,38 @@
             "dtheta":2, #angular resolution in degrees
             "min_fr": 0,
             "max_fr": 1,
             "name": "BoundaryVectorCells",
         }
     """
 
+    default_params = {
+        "n": 10,
+        "reference_frame": "allocentric",
+        "pref_wall_dist": 0.15,
+        "angle_spread_degrees": 11.25,
+        "xi": 0.08,
+        "beta": 12,
+        "dtheta": 2,
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "BoundaryVectorCells",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise BoundaryVectorCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
-        default_params = {
-            "n": 10,
-            "reference_frame": "allocentric",
-            "pref_wall_dist": 0.15,
-            "angle_spread_degrees": 11.25,
-            "xi": 0.08,
-            "beta": 12,
-            "dtheta": 2,
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "BoundaryVectorCells",
-        }
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
 
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "boundary cells only possible in 2D"
         assert (
             self.Agent.Environment.boundary_conditions == "solid"
@@ -1234,31 +1255,34 @@
         "xi": 0.08, #parameters determining the distance preferrence function std given the preferred distance. See BoundaryVectorCells or de cothi and barry 2020
         "beta": 12,
         "max_fr":1, # likely max firing rate of an OVC
         "min_fr":0, # likely min firing rate
     }
     """
 
+    default_params = {
+        "n": 10,
+        "name": "ObjectVectorCell",
+        "walls_occlude": True,
+        "reference_frame": "allocentric",
+        "angle_spread_degrees": 15,
+        "pref_object_dist": 0.25,
+        "xi": 0.08,
+        "beta": 12,
+        "max_fr": 1,
+        "min_fr": 0,
+    }
+
+
     def __init__(self, Agent, params={}):
-        default_params = {
-            "n": 10,
-            "name": "ObjectVectorCell",
-            "walls_occlude": True,
-            "reference_frame": "allocentric",
-            "angle_spread_degrees": 15,
-            "pref_object_dist": 0.25,
-            "xi": 0.08,
-            "beta": 12,
-            "max_fr": 1,
-            "min_fr": 0,
-        }
 
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
 
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "object vector cells only possible in 2D"
 
         super().__init__(Agent, self.params)
 
@@ -1419,29 +1443,31 @@
             "max_fr": 1,
             "n":1,
             "angle_spread_degrees":30,
             "name": "HeadDirectionCells",
         }
     """
 
+    default_params = {
+        "min_fr": 0,
+        "max_fr": 1,
+        "n": 4,
+        "angular_spread_degrees": 45,  # width of HDC preference function (degrees)
+        "name": "HeadDirectionCells",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise HeadDirectionCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
-        default_params = {
-            "min_fr": 0,
-            "max_fr": 1,
-            "n": 4,
-            "angular_spread_degrees": 45,  # width of HDC preference function (degrees)
-            "name": "HeadDirectionCells",
-        }
+
         self.Agent = Agent
-        for key in params.keys():
-            default_params[key] = params[key]
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
 
         if self.Agent.Environment.dimensionality == "2D":
             self.n = self.params["n"]
             self.preferred_angles = np.linspace(0, 2 * np.pi, self.n + 1)[:-1]
             # self.preferred_directions = np.array([np.cos(angles),np.sin(angles)]).T #n HDCs even spaced on unit circle
             self.angular_tunings = np.array(
                 [self.params["angular_spread_degrees"] * np.pi / 180] * self.n
@@ -1543,26 +1569,29 @@
     default_params = {
             "min_fr": 0,
             "max_fr": 1,
             "name": "VelocityCells",
         }
     """
 
+    default_params = {
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "VelocityCells",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise VelocityCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
-        default_params = {
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "VelocityCells",
-        }
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         self.one_sigma_speed = self.Agent.speed_mean + self.Agent.speed_std
 
         super().__init__(Agent, self.params)
 
         if ratinabox.verbose is True:
             print(
                 f"VelocityCells successfully initialised. Your environment is {self.Agent.Environment.dimensionality} and you have {self.n} velocity cells"
@@ -1591,27 +1620,30 @@
     default_params = {
             "min_fr": 0,
             "max_fr": 1,
             "name": "SpeedCell",
         }
     """
 
+    default_params = {
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "SpeedCell",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise SpeedCell(), takes as input a parameter dictionary, 'params'. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
-        default_params = {
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "SpeedCell",
-        }
+
         self.Agent = Agent
-        for key in params.keys():
-            default_params[key] = params[key]
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
         self.n = 1
         self.one_sigma_speed = self.Agent.speed_mean + self.Agent.speed_std
 
         if ratinabox.verbose is True:
             print(
                 f"SpeedCell successfully initialised. The speed of the agent is encoded linearly by the firing rate of this cell. Speed = 0 --> min firing rate of of {self.min_fr}. Speed = mean + 1std (here {self.one_sigma_speed} --> max firing rate of {self.max_fr}."
@@ -1668,34 +1700,42 @@
             "activation_params": {
                 "activation": "linear",
             },
             "name": "FeedForwardLayer",
         }
     """
 
+    default_params = {
+        "n": 10,
+        "input_layers": [],  # a list of input layers, or add one by one using self.add_inout
+        "activation_params": {"activation": "linear"},
+        "name": "FeedForwardLayer",
+        "biases": None,  # an array of biases, one for each neuron
+    }
+
     def __init__(self, Agent, params={}):
-        default_params = {
-            "n": 10,
-            "input_layers": [],  # a list of input layers, or add one by one using self.add_inout
-            "activation_params": {"activation": "linear"},
-            "name": "FeedForwardLayer",
-            "biases": None,  # an array of biases, one for each neuron
-        }
+
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
 
         self.inputs = {}
         for input_layer in self.input_layers:
             self.add_input(input_layer)
 
         if self.biases is None:
             self.biases = np.zeros(self.n)
 
+        self.firingrate_prime = np.zeros_like(
+            self.firingrate
+        )  # this will hold the firingrate except passed through the derivative of the activation func
+
         if ratinabox.verbose is True:
             print(
                 f"FeedForwardLayer initialised with {len(self.inputs.keys())} layers. To add another layer use FeedForwardLayer.add_input_layer().\nTo set the weights manually edit them by changing self.inputs['layer_name']['w']"
             )
 
     def add_input(self, input_layer, w=None, w_init_scale=1, **kwargs):
         """Adds an input layer to the class. Each input layer is stored in a dictionary of self.inputs. Each has an associated matrix of weights which are initialised randomly.
@@ -1738,15 +1778,14 @@
         Once the firing rate of the inout layers is established these are multiplied by the weight matrices and then activated to obtain the firing rate of this FeedForwardLayer.
 
         Args:
             evaluate_at (str, optional). Defaults to 'last'.
         Returns:
             firingrate: array of firing rates
         """
-
         if evaluate_at == "last":
             V = np.zeros(self.n)
         elif evaluate_at == "all":
             V = np.zeros(
                 (self.n, self.Agent.Environment.flattened_discrete_coords.shape[0])
             )
         else:
@@ -1764,12 +1803,14 @@
         biases = self.biases
         if biases.shape != V.shape:
             biases = biases.reshape((-1, 1))
         V += biases
 
         firingrate = utils.activate(V, other_args=self.activation_params)
         # saves current copy of activation derivative at firing rate (useful for learning rules)
-        if evaluate_at == "last":
+        if (
+            evaluate_at == "last"
+        ):  # save copy of the firing rate through the dervative of the activation function
             self.firingrate_prime = utils.activate(
                 V, other_args=self.activation_params, deriv=True
             )
         return firingrate
```

### Comparing `ratinabox-1.4.2/ratinabox/README.md` & `ratinabox-1.5.0/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/__init__.py` & `ratinabox-1.5.0/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.5.0/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import *
 from ratinabox.utils import *
 
 import matplotlib
 
+import copy
 import numpy as np
 import math
 
 
 class FieldOfViewNeurons(Neurons):
     """FieldOfViewNeurons are collection of boundary vector cells or object vector cells organised so as to represent the local field of view i.e. what walls or objects the agent can "see" in the local vicinity. They work as follow:
 
@@ -25,27 +26,28 @@
         >>> fig, ax = Ag.animate_trajectory(additional_plot_func=my_FoVNeurons.display_manifold)
 
 
     Args:
         Neurons (_type_): _description_
     """
 
+    default_params = {
+        "FoV_distance": [0.0, 0.2],  # min and max distances the agent can "see"
+        "FoV_angles": [
+            0,
+            90,
+        ],  # angluar FoV in degrees (will be symmetric on both sides, so give range in 0 (forwards) to 180 (backwards)
+        "spatial_resolution": 0.04,  # resolution of each BVC tiling FoV
+        "cell_type": "BVC",  # FoV neurons can either respond to local boundaries ("BVC") or objects ("OVC")
+    }
+
     def __init__(self, Agent, params={}):
-        default_params = {
-            "FoV_distance": [0.0, 0.2],  # min and max distances the agent can "see"
-            "FoV_angles": [
-                0,
-                90,
-            ],  # angluar FoV in degrees (will be symmetric on both sides, so give range in 0 (forwards) to 180 (backwards)
-            "spatial_resolution": 0.04,  # resolution of each BVC tiling FoV
-            "cell_type": "BVC",  # FoV neurons can either respond to local boundaries ("BVC") or objects ("OVC")
-        }
 
-        default_params.update(params)
-        self.params = default_params
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
 
         # tile FoV within angular and distance specifications given as params
         self.FoV_angles_radians = [a * np.pi / 180 for a in self.params["FoV_angles"]]
         dx = self.params["spatial_resolution"]
         radii = np.arange(
             max(0.01, self.params["FoV_distance"][0]),
             self.params["FoV_distance"][1],
```

### Comparing `ratinabox-1.4.2/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.5.0/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import *
 from ratinabox.utils import *
 
+import copy
 import numpy as np
 
 
 class PhasePrecessingPlaceCells(PlaceCells):
     """
     Contributer: Tom George tomgeorge1@btinternet.com
     Date: 05/10/2022
@@ -25,33 +26,36 @@
         • precess_fraction (default 0.5)
 
     List of functions:
         • get_state()
         • theta_modulation_factors()
     """
 
+    default_params = {
+        "n": 10,
+        "min_fr": 0,
+        "max_fr": 1,
+        "theta_freq": 10,
+        "kappa": 1,
+        "precess_fraction": 0.5,
+        "description": "gaussian_threshold",
+        "name": "PhasePrecessingPlaceCell",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise PhasePrecessingPlaceCell(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
-        default_params = {
-            "n": 10,
-            "min_fr": 0,
-            "max_fr": 1,
-            "theta_freq": 10,
-            "kappa": 1,
-            "precess_fraction": 0.5,
-            "description": "gaussian_threshold",
-            "name": "PhasePrecessingPlaceCell",
-        }
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
         self.sigma = np.sqrt(1 / self.kappa)
 
         assert self.description in [
             "gaussian",
             "diff_of_gaussians",
             "gaussian_threshold",
```

### Comparing `ratinabox-1.4.2/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.5.0/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import *
 from ratinabox.utils import *
 
+import copy
 import numpy as np
 
 
 class PlaneWaveNeurons(Neurons):
     """
     Contributer: Tom George tomgeorge1@btinternet.com
     Date: 23/07/2022
@@ -17,30 +18,33 @@
 
     PlaneWaveNeurons defines a set of 'n' neurons whos firing rate is a plane cells with random orientations, lengthscales (around some mean) and offsets). If you want non random orientations and phase offsets just set self.w and self.phase_offsets and self.wavescales manually.
 
     List of functions:
         • get_state()
     """
 
+    default_params = {
+        "n": 10,
+        "wavescale": 0.2,  # metres
+        "min_fr": 0,
+        "max_fr": 1,
+        "name": "PlaneWaveNeurons",
+    }
+
     def __init__(self, Agent, params={}):
         """Initialise PlaneWaveNeurons(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
-        default_params = {
-            "n": 10,
-            "wavescale": 0.2,  # metres
-            "min_fr": 0,
-            "max_fr": 1,
-            "name": "PlaneWaveNeurons",
-        }
         self.Agent = Agent
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Agent, self.params)
 
         # Initialise  cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "PlaneWaveNeurons only available in 2D"
```

### Comparing `ratinabox-1.4.2/ratinabox/contribs/README.md` & `ratinabox-1.5.0/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.5.0/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.5.0/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 from ratinabox.Agent import Agent
 from scipy.interpolate import interp1d
+import copy
 import numpy as np
 
 
 class ThetaSequenceAgent(Agent):
     """ThetaSequneceAgent is a type of Agent who's position is NOT the true position but instead a "theta sequence" over the position. This starts from behind the "true" position and rapidly moves to infront of the true position (default sequence speed = 5ms-1) once every "theta cycle" (default 10Hz). Each theta sequence is split into the following phases (marked as fraction of the theta cycle):
 
     |.......A.........|................B..............|.................C.............|........A'.......|
@@ -24,26 +25,28 @@
     default_params = {
         "dt"          : 0.001,  #this MUST be at least 10x smaller than the theta time period
         "theta_freq"  : 10.0, #theta frequency
         "v_sequence"     : 5.0, #sequence speed in reference frame of Agent, ms-1
         "theta_frac"  : 0.5, #fraction of theta cycle over which}
     """
 
-    def __init__(self, Environment, params={}):
+    default_params = {
+        "v_sequence": 5.0,  # sequence speed in reference frame of Agent, ms-1
+        "theta_freq": 10.0,  # theta frequency
+        "theta_frac": 0.5,  # fraction of theta cycle over which
+        "dt": 0.001,
+    }
 
-        default_params = {
-            "v_sequence": 5.0,  # sequence speed in reference frame of Agent, ms-1
-            "theta_freq": 10.0,  # theta frequency
-            "theta_frac": 0.5,  # fraction of theta cycle over which
-            "dt": 0.001,
-        }
+    def __init__(self, Environment, params={}):
 
         self.Environment = Environment
-        default_params.update(params)
-        self.params = default_params
+
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
+
         super().__init__(Environment, self.params)
 
         # ground truth Agent
         self.TrueAgent = Agent(self.Environment, self.params)
         self.TrueAgent.history[
             "distance_travelled"
         ] = []  # history of distance travelled
```

### Comparing `ratinabox-1.4.2/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.5.0/ratinabox/contribs/ValueNeuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import *
 from ratinabox.utils import *
 
+import copy
 import numpy as np
 
 
 class ValueNeuron(FeedForwardLayer):
     """
     Contributer: Tom George tomgeorge1@btinternet.com
 
@@ -27,27 +28,28 @@
     Input features can be any RatInABox Neurons class here (a set of PlaceCells, BoundaryVectorCells, GridCells etc...or more complex things). It linearly sums these inputs to calculate its firing rate (this summation is all handled by the FeedForwardLayer class). Weights are trained using TD learning, self.update_weights() should be called at each update step and passed the current reward density or reward density vector. For more infor see ratinabox/example_scripts/reinforcement_learning_example/
 
     Since this is a Neurons subclass, after (or even during) learning you can plot the value function just by querying the ValueNeurons rate map (ValueNeuron.plot_rate_map()), or check the estimate of value at a postion using ValueNeuron.get_state(evaluate_at=None, pos=np.array([[x,y]]))
 
     To see the weights try ValueNeuron.inputs['name_of_input_layer']['w']
     """
 
+    default_params = {
+        "input_layer": None,  # the features it is using as inputs
+        "tau": 2,  # discount time horizon (equivalent to gamma in discrete RL)
+        "tau_e": None,  # eligibility trace timescale, must be <= tau (defaults to tau/2)
+        "eta": 0.001,  # learning rate
+        "L2": 0.001,  # L2 regularisation
+        "activation_params": {"activation": "relu"},  # non-linearity for
+        "n": 1,  # how many rewards there will be and thus how many Values function (each represented by one ValueNeuron) there are
+    }
+
     def __init__(self, Agent, params={}):
-        default_params = {
-            "input_layer": None,  # the features it is using as inputs
-            "tau": 2,  # discount time horizon (equivalent to gamma in discrete RL)
-            "tau_e": None,  # eligibility trace timescale, must be <= tau (defaults to tau/2)
-            "eta": 0.001,  # learning rate
-            "L2": 0.001,  # L2 regularisation
-            "activation_params": {"activation": "relu"},  # non-linearity for
-            "n": 1,  # how many rewards there will be and thus how many Values function (each represented by one ValueNeuron) there are
-        }
 
-        default_params.update(params)
-        self.params = default_params
+        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params.update(params)
 
         self.params["input_layers"] = [self.params["input_layer"]]
         super().__init__(Agent, self.params)  # initialise parent class
 
         if self.tau_e == None:
             self.tau_e = self.tau / 2
         self.et = np.zeros(self.n)  # initialise eligibility trace
@@ -55,15 +57,16 @@
         self.firingrate_deriv = np.zeros(self.n)  # initialise firing rate derivative
         self.td_error = np.zeros(self.n)  # initialise td error
 
     def update(self):
         """Updates firing rate as weighted linear sum of feature inputs"""
         firingrate_last = self.firingrate
         # update the firing rate
-        super().update()  # FeedForwardLayer builtin function. this sums the inputs from the input features over the weight matrix and saves the firingrate.
+        super().update()  # FeedForwardLayer builtin function. This sums the inputs from the input features over the weight matrix and saves the firingrate.
+
         # calculate temporal derivative of the firing rate
         self.firingrate_deriv = (self.firingrate - firingrate_last) / self.Agent.dt
         # update eligibility trace
         if self.tau_e == 0:
             self.et = self.input_layer.firingrate
         else:
             self.et = (
```

### Comparing `ratinabox-1.4.2/ratinabox/data/README.md` & `ratinabox-1.5.0/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/data/rat.png` & `ratinabox-1.5.0/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/data/sargolini.npz` & `ratinabox-1.5.0/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/data/tanni.npz` & `ratinabox-1.5.0/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/ratinabox/utils.py` & `ratinabox-1.5.0/ratinabox/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import scipy
+import inspect
 import os
+import warnings
 from datetime import datetime
 from scipy import stats as stats
 import ratinabox
 
 """OTHER USEFUL FUNCTIONS"""
 """Geometry functions"""
 
@@ -591,84 +593,180 @@
         )
         print(
             '    Set a default figure directory `ratinabox.figure_directory = "path/to/my/figs/"`'
         )
         print(f"       (the current working directory is {os.getcwd()})")
         return
 
-    if figure_directory[-1] != "/":
-        figure_directory += "/"
-
-    if not os.path.isdir(figure_directory):
-        os.mkdir(figure_directory)
-
     # make today-specific directory inside figure directory
     today = datetime.strftime(datetime.now(), "%d_%m_%y")
-    if not os.path.isdir(figure_directory + f"{today}/"):
-        os.mkdir(figure_directory + f"{today}/")
+    figdir = os.path.join(figure_directory, f"{today}")
+    os.makedirs(figdir, exist_ok=True)
 
-    figdir = figure_directory + f"{today}/"
     now = datetime.strftime(datetime.now(), "%H%M")
-    path_ = f"{figdir}{save_title}_{now}"
+    path_ = os.path.join(figdir, f"{save_title}_{now}")
     path = path_
 
     if type(fig) == matplotlib.figure.Figure:
         file_type = "Figure"
         save_types = "  & .".join(fig_save_types)
         for filetype in fig_save_types:
             i = 1
             while True:  # checks there isn't an existing figure with this name
-                if os.path.isfile(path + "." + filetype):
-                    path = path_ + "_" + str(i)
+                if os.path.isfile(f"{path}.{filetype}"):
+                    path = f"{path_}_{i}"
                     i += 1
                 elif i >= 100:
                     break
                 else:
                     break
-            fig.savefig(path + "." + filetype, bbox_inches="tight")
+            fig.savefig(f"{path}.{filetype}", bbox_inches="tight")
 
     elif type(fig) == matplotlib.animation.FuncAnimation:
         file_type = "Animation"
         save_types = "  & .".join(anim_save_types)
         for filetype in anim_save_types:
             i = 1
             while True:
-                if os.path.isfile(path + "." + filetype):
-                    path = path_ + "_" + str(i)
+                if os.path.isfile(f"{path}.{filetype}"):
+                    path = f"{path_}_{i}"
                     i += 1
                 elif i >= 100:
                     break
                 else:
                     break
-            fig.save(path + "." + filetype)
+            fig.save(f"{path}.{filetype}")
 
     print(f"{file_type} saved to {os.path.abspath(path)}.{save_types}")
 
     return path
 
 
 def save_animation(*args, **kwargs):
     """Saves an animation. This function just passes the animation object to utils.save_figure() where it is then saved. We only include this function for semantic consistency (you could just use save_figure directly. Takes exactly the same args are save_figure() and just passes the animation over there"""
     return save_figure(*args, **kwargs)
 
 
-"""Other"""
+"""High-level functions"""
 
 
-def update_class_params(Class, params: dict):
+def update_class_params(Class, params: dict, get_all_defaults=False):
     """Updates parameters from a dictionary.
     All parameters found in params will be updated to new value
     Args:
         params (dict): dictionary of parameters to change
         initialise (bool, optional): [description]. Defaults to False.
     """
+
+    if get_all_defaults:
+        all_default_params = collect_all_default_params(Class.__class__)
+        all_default_params.update(params)
+        params = all_default_params
+
     for key, value in params.items():
         setattr(Class, key, value)
 
 
+def collect_all_default_params(obj_class, keys_only=False):
+    """Collects all the default_params dictionaries from the current class, including those inherited from its parent classes.
+
+    Args:
+        obj_class (class): object class for which to collect the default_params dictionaries
+        keys_only (bool, optional): If True, only returns the keys of the default_params dictionaries. Defaults to False.
+
+    Returns:
+        dict or list: 
+            If keys_only == False, returns a dictionary of all the default_params values from the current class, including those inherited from its parent classes.
+            If keys_only == True, returns a list of all the keys of the default_params dictionaries from  the current class and its parent classes.
+    """
+
+    if not inspect.isclass(obj_class):
+        raise ValueError("obj_class must be a class object.")
+
+    if not "default_params" in obj_class.__dict__:
+        warnings.warn(
+            f"Cannot collect the default params dictionaries, as {obj_class} does not "
+            "have a class attribute 'default_params' defined in its preamble. "
+            "(Can be just an empty dictionary, i.e.: default_params = dict().)"
+        )
+        return
+
+    if keys_only:
+        all_default_param_keys = list()
+    else:
+        all_default_params_dicts = list()
+        all_default_params = dict()
+    
+    while hasattr(obj_class, "default_params"):
+        if keys_only:
+            all_default_param_keys.extend(obj_class.default_params.keys())
+        else:
+            all_default_params_dicts.append(obj_class.default_params)
+        if len(obj_class.__bases__):
+            obj_class = obj_class.__bases__[0]
+        else:
+            break
+    
+    if keys_only:
+        all_default_param_keys = sorted(set(all_default_param_keys))
+        return all_default_param_keys
+    
+    for default_params_dict in all_default_params_dicts[::-1]: # update in reverse (from parents to child class)
+        all_default_params.update(default_params_dict)
+
+    return all_default_params
+
+
+def check_params(Obj, param_keys):
+    """Given an object and a list of keys, checks whether the keys are all in 
+    the object's default_params dictionary.
+
+    Args:
+        Obj (object): object to check
+        param_keys (list): list of keys to check
+    
+    Returns:
+        list: list of keys in param_keys that weren't expected based on the default parameters of Obj
+    """
+
+    if inspect.isclass(Obj):
+        raise ValueError("Obj must be an instance of a class, not a class object.")
+
+    obj_class = Obj.__class__
+    if not "default_params" in obj_class.__dict__:
+        warnings.warn(
+            f"Cannot check the keys in the params dictionary, as {obj_class} does not "
+            "have a class attribute 'default_params' defined in its preamble. "
+            "(Can be just an empty dictionary, i.e.: default_params = dict().)"
+        )
+        return
+
+    all_default_param_keys = collect_all_default_params(obj_class, keys_only=True)
+    
+    unexpected_keys = [
+        key for key in param_keys if key not in all_default_param_keys
+    ]
+    
+    if len(unexpected_keys):
+        num = len(unexpected_keys)
+        unexpected_keys = ", ".join(
+            [f"'{attr}'" for attr in unexpected_keys]
+            )
+        object_name = str(Obj)
+        if hasattr(Obj, "name"):
+            object_name = f"{object_name} ('{Obj.name}')"
+
+        warnings.warn(
+            f"Found {num} unexpected params key(s) while initializing "
+            f"{object_name}: {unexpected_keys}"
+            )
+    
+    return unexpected_keys
+
+
 def activate(x, activation="sigmoid", deriv=False, other_args={}):
     """Activation function function
 
     Args:
         x (the input (vector))
         activation: which type of fucntion to use (this is overwritten by 'activation' key in other_args)
         deriv (bool, optional): Whether it return f(x) or df(x)/dx. Defaults to False.
```

### Comparing `ratinabox-1.4.2/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.5.0/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.2
+Version: 1.5.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.4.2/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.5.0/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/setup.cfg` & `ratinabox-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.4.2
+version = 1.5.0
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.4.2/tests/test_advanced.py` & `ratinabox-1.5.0/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.2/tests/test_environment.py` & `ratinabox-1.5.0/tests/test_environment.py`

 * *Files identical despite different names*

