# Comparing `tmp/ratinabox-1.5.0.tar.gz` & `tmp/ratinabox-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.5.0.tar", last modified: Fri Apr 21 10:47:30 2023, max compression
+gzip compressed data, was "ratinabox-1.5.1.tar", last modified: Fri Apr 21 16:39:02 2023, max compression
```

## Comparing `ratinabox-1.5.0.tar` & `ratinabox-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.766506 ratinabox-1.5.0/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.5.0/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 10:47:30.766679 ratinabox-1.5.0/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.5.0/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.5.0/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.758424 ratinabox-1.5.0/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41178 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31941 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    80998 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.5.0/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.5.0/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.760956 ratinabox-1.5.0/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8805 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5787 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3935 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.5.0/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.5.0/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15034 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7275 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.5.0/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.762472 ratinabox-1.5.0/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.5.0/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.5.0/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.5.0/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.5.0/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.5.0/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34227 2023-04-21 10:42:12.000000 ratinabox-1.5.0/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.759321 ratinabox-1.5.0/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-21 10:47:30.000000 ratinabox-1.5.0/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-21 10:47:30.767187 ratinabox-1.5.0/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.5.0/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 10:47:30.766344 ratinabox-1.5.0/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.5.0/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.5.0/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.5.0/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.5.0/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.128712 ratinabox-1.5.1/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.5.1/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 16:39:02.128826 ratinabox-1.5.1/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.5.1/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.5.1/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.122072 ratinabox-1.5.1/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41547 2023-04-21 16:30:58.000000 ratinabox-1.5.1/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32289 2023-04-21 16:31:04.000000 ratinabox-1.5.1/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    81263 2023-04-21 16:29:55.000000 ratinabox-1.5.1/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.5.1/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.5.1/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.124333 ratinabox-1.5.1/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.5.1/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.5.1/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-04-21 14:28:51.000000 ratinabox-1.5.1/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7270 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.5.1/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.125370 ratinabox-1.5.1/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.5.1/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.5.1/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.5.1/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.5.1/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.5.1/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34247 2023-04-21 16:38:02.000000 ratinabox-1.5.1/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.122836 ratinabox-1.5.1/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-21 16:39:02.129134 ratinabox-1.5.1/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.5.1/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.128611 ratinabox-1.5.1/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.5.1/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.5.1/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.5.1/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.5.1/tests/test_neurons.py
```

### Comparing `ratinabox-1.5.0/LICENSE` & `ratinabox-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/PKG-INFO` & `ratinabox-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.5.0
+Version: 1.5.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.5.0/README.md` & `ratinabox-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/Agent.py` & `ratinabox-1.5.1/ratinabox/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 
 import copy
+import pprint
 import numpy as np
 import os
 import matplotlib
 from matplotlib import pyplot as plt
 
 
 from ratinabox import utils
@@ -72,15 +73,15 @@
         Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
         self.Environment = Environment
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
         # initialise history dataframes
         self.history = {}
@@ -122,14 +123,22 @@
                 Use Ag.update() to move the Agent.
                 Positions and velocities are saved into the Agent.history dictionary.
                 Import external trajectory data using Ag.import_trajectory(). Plot trajectory using Ag.plot_trajectory().
                 Other plotting functions are available."""
             )
         return
 
+    @classmethod
+    def get_all_default_params(cls, verbose=False):
+        """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
+        all_default_params = utils.collect_all_default_params(cls)
+        if verbose:
+            pprint.pprint(all_default_params)
+        return all_default_params
+
     def update(self, dt=None, drift_velocity=None, drift_to_random_strength_ratio=1):
         """Movement policy update.
         In principle this does a very simple thing:
         • updates time by dt
         • updates velocity (speed and direction) according to a movement policy
         • updates position along the velocity direction
         In reality it's a complex function as the policy requires checking for immediate or upcoming collisions with all walls at each step as well as
```

### Comparing `ratinabox-1.5.0/ratinabox/Environment.py` & `ratinabox-1.5.1/ratinabox/Environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 
 import copy
+import pprint
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import shapely
 
 import warnings
 
@@ -60,15 +61,15 @@
     def __init__(self, params={}):
         """Initialise Environment, takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
         if self.dimensionality == "1D":
             self.D = 1
@@ -159,14 +160,22 @@
         if ratinabox.verbose is True:
             print(
                 f"\nAn Environment has been initialised with parameters: {self.params}. Use Env.add_wall() to add a wall into the Environment. Plot Environment using Env.plot_environment()."
             )
 
         return
 
+    @classmethod
+    def get_all_default_params(cls, verbose=False):
+        """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
+        all_default_params = utils.collect_all_default_params(cls)
+        if verbose:
+            pprint.pprint(all_default_params)
+        return all_default_params
+
     def add_wall(self, wall):
         """Add a wall to the (2D) environment.
         Extends self.walls array to include one new wall.
         Args:
             wall (np.array): 2x2 array [[x1,y1],[x2,y2]]
         """
         assert self.dimensionality == "2D", "can only add walls into a 2D environment"
@@ -295,15 +304,15 @@
                     solid_capstyle="round",
                     zorder=2,
                 )
 
             # plot objects
             if self.plot_objects == True:
                 object_cmap = matplotlib.colormaps[self.object_colormap]
-                for (i, object) in enumerate(self.objects["objects"]):
+                for i, object in enumerate(self.objects["objects"]):
                     object_color = object_cmap(
                         self.objects["object_types"][i]
                         / (self.n_object_types - 1 + 1e-8)
                     )
                     ax.scatter(
                         object[0],
                         object[1],
@@ -315,15 +324,15 @@
                     )
 
             ax.set_aspect("equal")
             ax.grid(False)
             ax.axis("off")
             ax.set_xlim(left=extent[0] - 0.03, right=extent[1] + 0.03)
             ax.set_ylim(bottom=extent[2] - 0.03, top=extent[3] + 0.03)
-        
+
         ratinabox.utils.save_figure(fig, "Environment", save=autosave)
 
         return fig, ax
 
     def sample_positions(self, n=10, method="uniform_jitter"):
         """Scatters 'n' locations across the environment which can act as, for example, the centres of gaussian place fields, or as a random starting position.
         If method == "uniform" an evenly spaced grid of locations is returned.  If method == "uniform_jitter" these locations are jittered slightly (i.e. random but span the space). Note; if n doesn't uniformly divide the size (i.e. n is not a square number in a square environment) then the largest number that can be scattered uniformly are found, the remaining are randomly placed.
@@ -345,15 +354,14 @@
                 if method[7:] == "_jitter":
                     positions += np.random.uniform(
                         -0.45 * dx, 0.45 * dx, positions.shape
                     )
             return positions
 
         elif self.dimensionality == "2D":
-
             if method == "random":
                 positions = np.zeros((n, 2))
                 positions[:, 0] = np.random.uniform(
                     self.extent[0], self.extent[1], size=n
                 )
                 positions[:, 1] = np.random.uniform(
                     self.extent[2], self.extent[3], size=n
@@ -375,15 +383,15 @@
                     positions_remaining = self.sample_positions(
                         n=n_remaining, method="random"
                     )
                     positions = np.vstack((positions, positions_remaining))
 
             if (self.is_rectangular is False) or (self.has_holes is True):
                 # in this case, the positions you have sampled within the extent of the environment may not actually fall within it's legal area (i.e. they could be outside the polygon boundary or inside a hole). Brute force this by randomly resampling these points until all fall within the env.
-                for (i, pos) in enumerate(positions):
+                for i, pos in enumerate(positions):
                     if self.check_if_position_is_in_environment(pos) == False:
                         pos = self.sample_positions(n=1, method="random").reshape(
                             -1
                         )  # this recursive call must pass eventually, assuming the env is sufficiently large. this is why we don't need a while loop
                         positions[i] = pos
             return positions
```

### Comparing `ratinabox-1.5.0/ratinabox/Neurons.py` & `ratinabox-1.5.1/ratinabox/Neurons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 
 import copy
+import pprint
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import scipy
 from scipy import stats as stats
 
 from ratinabox import utils
@@ -33,21 +34,21 @@
 
     The unique function in each child classes is get_state(). Whenever Neurons.update() is called Neurons.get_state() is then called to calculate and return the firing rate of the cells at the current moment in time. This is then saved. In order to make your own Neuron subclass you will need to write a class with the following mandatory structure:
 
     ============================================================================================
     MyNeuronClass(Neurons):
 
         default_params = {'a_default_param":3.14159} # default params dictionary is defined in the preamble, as a class attribute. Note its values are passed upwards and used in all the parents classes of your class.
-    
+
         def __init__(self,
                      Agent,
                      params={}): #<-- do not change these
 
 
-            self.params = copy.deepcopy(self.__class__.default_params) # it is best to retrieve the default param dictionary as self.__class__. Then, make sure to deepcopy it, as only making a shallow copy can have unintended consequences (i.e., any modifications to it would be propagated to ALL instances of this class!).
+            self.params = copy.deepcopy(__class__.default_params) # to get the default param dictionary of the current class, defined in the preamble, use __class__. Then, make sure to deepcopy it, as only making a shallow copy can have unintended consequences (i.e., any modifications to it would be propagated to ALL instances of this class!).
             self.params.update(params)
 
             super().__init__(Agent,self.params)
 
         def get_state(self,
                       evaluate_at='agent',
                       **kwargs) #<-- do not change these
@@ -100,15 +101,15 @@
             params (dict, optional). Defaults to {}.
 
         Typically you will not actually initialise a Neurons() class, instead you will initialised by one of it's subclasses.
         """
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
         self.firingrate = np.zeros(self.n)
         self.noise = np.zeros(self.n)
@@ -119,14 +120,22 @@
         self.history["spikes"] = []
 
         if ratinabox.verbose is True:
             print(
                 f"\nA Neurons() class has been initialised with parameters f{self.params}. Use Neurons.update() to update the firing rate of the Neurons to correspond with the Agent.Firing rates and spikes are saved into the Agent.history dictionary. Plot a timeseries of the rate using Neurons.plot_rate_timeseries(). Plot a rate map of the Neurons using Neurons.plot_rate_map()."
             )
 
+    @classmethod
+    def get_all_default_params(cls, verbose=False):
+        """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
+        all_default_params = utils.collect_all_default_params(cls)
+        if verbose:
+            pprint.pprint(all_default_params)
+        return all_default_params
+
     def update(self):
         # update noise vector
         dnoise = utils.ornstein_uhlenbeck(
             dt=self.Agent.dt,
             x=self.noise,
             drift=0,
             noise_scale=self.noise_std,
@@ -666,17 +675,17 @@
 
         Args:
             params (dict, optional). Defaults to {}.
         """
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
-        
+
         super().__init__(Agent, self.params)
 
         if self.place_cell_centres is None:
             self.place_cell_centres = self.Agent.Environment.sample_positions(
                 n=self.n, method="uniform_jitter"
             )
         elif type(self.place_cell_centres) is str:
@@ -836,24 +845,23 @@
         "random_gridscales": True,
         "random_phase_offsets": True,
         "min_fr": 0,
         "max_fr": 1,
         "name": "GridCells",
     }
 
-
     def __init__(self, Agent, params={}):
         """Initialise GridCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)      
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         super().__init__(Agent, self.params)
 
         # Initialise grid cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
@@ -984,15 +992,15 @@
         """Initialise BoundaryVectorCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         super().__init__(Agent, self.params)
 
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "boundary cells only possible in 2D"
@@ -1268,20 +1276,18 @@
         "pref_object_dist": 0.25,
         "xi": 0.08,
         "beta": 12,
         "max_fr": 1,
         "min_fr": 0,
     }
 
-
     def __init__(self, Agent, params={}):
-
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "object vector cells only possible in 2D"
 
         super().__init__(Agent, self.params)
@@ -1458,15 +1464,15 @@
     def __init__(self, Agent, params={}):
         """Initialise HeadDirectionCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         if self.Agent.Environment.dimensionality == "2D":
             self.n = self.params["n"]
             self.preferred_angles = np.linspace(0, 2 * np.pi, self.n + 1)[:-1]
             # self.preferred_directions = np.array([np.cos(angles),np.sin(angles)]).T #n HDCs even spaced on unit circle
             self.angular_tunings = np.array(
@@ -1581,15 +1587,15 @@
 
     def __init__(self, Agent, params={}):
         """Initialise VelocityCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         self.one_sigma_speed = self.Agent.speed_mean + self.Agent.speed_std
 
         super().__init__(Agent, self.params)
 
         if ratinabox.verbose is True:
@@ -1633,15 +1639,15 @@
     def __init__(self, Agent, params={}):
         """Initialise SpeedCell(), takes as input a parameter dictionary, 'params'. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         super().__init__(Agent, self.params)
         self.n = 1
         self.one_sigma_speed = self.Agent.speed_mean + self.Agent.speed_std
 
         if ratinabox.verbose is True:
@@ -1709,18 +1715,17 @@
         "input_layers": [],  # a list of input layers, or add one by one using self.add_inout
         "activation_params": {"activation": "linear"},
         "name": "FeedForwardLayer",
         "biases": None,  # an array of biases, one for each neuron
     }
 
     def __init__(self, Agent, params={}):
-
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         super().__init__(Agent, self.params)
 
         self.inputs = {}
         for input_layer in self.input_layers:
             self.add_input(input_layer)
```

### Comparing `ratinabox-1.5.0/ratinabox/README.md` & `ratinabox-1.5.1/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/__init__.py` & `ratinabox-1.5.1/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.5.1/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ],  # angluar FoV in degrees (will be symmetric on both sides, so give range in 0 (forwards) to 180 (backwards)
         "spatial_resolution": 0.04,  # resolution of each BVC tiling FoV
         "cell_type": "BVC",  # FoV neurons can either respond to local boundaries ("BVC") or objects ("OVC")
     }
 
     def __init__(self, Agent, params={}):
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         # tile FoV within angular and distance specifications given as params
         self.FoV_angles_radians = [a * np.pi / 180 for a in self.params["FoV_angles"]]
         dx = self.params["spatial_resolution"]
         radii = np.arange(
             max(0.01, self.params["FoV_distance"][0]),
```

### Comparing `ratinabox-1.5.0/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.5.1/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         """Initialise PhasePrecessingPlaceCell(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         super().__init__(Agent, self.params)
         self.sigma = np.sqrt(1 / self.kappa)
 
         assert self.description in [
             "gaussian",
```

### Comparing `ratinabox-1.5.0/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.5.1/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """Initialise PlaneWaveNeurons(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}."""
 
         self.Agent = Agent
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         super().__init__(Agent, self.params)
 
         # Initialise  cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
```

### Comparing `ratinabox-1.5.0/ratinabox/contribs/README.md` & `ratinabox-1.5.1/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.5.1/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.5.1/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "dt": 0.001,
     }
 
     def __init__(self, Environment, params={}):
 
         self.Environment = Environment
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         super().__init__(Environment, self.params)
 
         # ground truth Agent
         self.TrueAgent = Agent(self.Environment, self.params)
         self.TrueAgent.history[
```

### Comparing `ratinabox-1.5.0/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.5.1/ratinabox/contribs/ValueNeuron.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "L2": 0.001,  # L2 regularisation
         "activation_params": {"activation": "relu"},  # non-linearity for
         "n": 1,  # how many rewards there will be and thus how many Values function (each represented by one ValueNeuron) there are
     }
 
     def __init__(self, Agent, params={}):
 
-        self.params = copy.deepcopy(self.__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
         self.params["input_layers"] = [self.params["input_layer"]]
         super().__init__(Agent, self.params)  # initialise parent class
 
         if self.tau_e == None:
             self.tau_e = self.tau / 2
```

### Comparing `ratinabox-1.5.0/ratinabox/data/README.md` & `ratinabox-1.5.1/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/data/rat.png` & `ratinabox-1.5.1/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/data/sargolini.npz` & `ratinabox-1.5.1/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/data/tanni.npz` & `ratinabox-1.5.1/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/ratinabox/utils.py` & `ratinabox-1.5.1/ratinabox/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,22 +663,22 @@
         params = all_default_params
 
     for key, value in params.items():
         setattr(Class, key, value)
 
 
 def collect_all_default_params(obj_class, keys_only=False):
-    """Collects all the default_params dictionaries from the current class, including those inherited from its parent classes.
+    """Collects all the default_params dictionaries from the current class, including those inherited from its parent classes and its parents parents etc.
 
     Args:
         obj_class (class): object class for which to collect the default_params dictionaries
         keys_only (bool, optional): If True, only returns the keys of the default_params dictionaries. Defaults to False.
 
     Returns:
-        dict or list: 
+        dict or list:
             If keys_only == False, returns a dictionary of all the default_params values from the current class, including those inherited from its parent classes.
             If keys_only == True, returns a list of all the keys of the default_params dictionaries from  the current class and its parent classes.
     """
 
     if not inspect.isclass(obj_class):
         raise ValueError("obj_class must be a class object.")
 
@@ -691,43 +691,45 @@
         return
 
     if keys_only:
         all_default_param_keys = list()
     else:
         all_default_params_dicts = list()
         all_default_params = dict()
-    
+
     while hasattr(obj_class, "default_params"):
         if keys_only:
             all_default_param_keys.extend(obj_class.default_params.keys())
         else:
             all_default_params_dicts.append(obj_class.default_params)
         if len(obj_class.__bases__):
             obj_class = obj_class.__bases__[0]
         else:
             break
-    
+
     if keys_only:
         all_default_param_keys = sorted(set(all_default_param_keys))
         return all_default_param_keys
-    
-    for default_params_dict in all_default_params_dicts[::-1]: # update in reverse (from parents to child class)
+
+    for default_params_dict in all_default_params_dicts[
+        ::-1
+    ]:  # update in reverse (from parents to child class)
         all_default_params.update(default_params_dict)
 
     return all_default_params
 
 
 def check_params(Obj, param_keys):
-    """Given an object and a list of keys, checks whether the keys are all in 
+    """Given an object and a list of keys, checks whether the keys are all in
     the object's default_params dictionary.
 
     Args:
         Obj (object): object to check
         param_keys (list): list of keys to check
-    
+
     Returns:
         list: list of keys in param_keys that weren't expected based on the default parameters of Obj
     """
 
     if inspect.isclass(Obj):
         raise ValueError("Obj must be an instance of a class, not a class object.")
 
@@ -737,33 +739,26 @@
             f"Cannot check the keys in the params dictionary, as {obj_class} does not "
             "have a class attribute 'default_params' defined in its preamble. "
             "(Can be just an empty dictionary, i.e.: default_params = dict().)"
         )
         return
 
     all_default_param_keys = collect_all_default_params(obj_class, keys_only=True)
-    
-    unexpected_keys = [
-        key for key in param_keys if key not in all_default_param_keys
-    ]
-    
+
+    unexpected_keys = [key for key in param_keys if key not in all_default_param_keys]
+
     if len(unexpected_keys):
         num = len(unexpected_keys)
-        unexpected_keys = ", ".join(
-            [f"'{attr}'" for attr in unexpected_keys]
-            )
-        object_name = str(Obj)
-        if hasattr(Obj, "name"):
-            object_name = f"{object_name} ('{Obj.name}')"
+        unexpected_keys = ", ".join([f"'{attr}'" for attr in unexpected_keys])
 
         warnings.warn(
             f"Found {num} unexpected params key(s) while initializing "
-            f"{object_name}: {unexpected_keys}"
-            )
-    
+            f"{obj_class.__name__} object: {unexpected_keys}.\nIf you intended to set this parameter, ignore this message. To see all default parameters for this class call {obj_class.__name__}.get_all_default_params()."
+        )
+
     return unexpected_keys
 
 
 def activate(x, activation="sigmoid", deriv=False, other_args={}):
     """Activation function function
 
     Args:
```

### Comparing `ratinabox-1.5.0/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.5.1/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.5.0
+Version: 1.5.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.5.0/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.5.1/ratinabox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ratinabox.egg-info/requires.txt
 ratinabox.egg-info/top_level.txt
 ratinabox/contribs/FieldOfViewNeurons.py
 ratinabox/contribs/PhasePrecessingPlaceCells.py
 ratinabox/contribs/PlaneWaveNeurons.py
 ratinabox/contribs/README.md
 ratinabox/contribs/STDPFeedForwardLayer.py
+ratinabox/contribs/SuccessorFeatures.py
 ratinabox/contribs/ThetaSequenceAgent.py
 ratinabox/contribs/ValueNeuron.py
 ratinabox/contribs/__init__.py
 ratinabox/data/README.md
 ratinabox/data/__init__.py
 ratinabox/data/rat.png
 ratinabox/data/sargolini.npz
```

### Comparing `ratinabox-1.5.0/setup.cfg` & `ratinabox-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.5.0
+version = 1.5.1
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.5.0/tests/test_advanced.py` & `ratinabox-1.5.1/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.0/tests/test_environment.py` & `ratinabox-1.5.1/tests/test_environment.py`

 * *Files identical despite different names*

