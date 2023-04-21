# Comparing `tmp/satvis-0.2.0.tar.gz` & `tmp/satvis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satvis-0.2.0.tar", last modified: Tue Apr 18 19:48:25 2023, max compression
+gzip compressed data, was "satvis-0.2.1.tar", last modified: Fri Apr 21 15:16:33 2023, max compression
```

## Comparing `satvis-0.2.0.tar` & `satvis-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1069 2022-11-14 19:16:32.000000 satvis-0.2.0/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-18 19:48:25.243433 satvis-0.2.0/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    12667 2022-11-16 20:21:06.000000 satvis-0.2.0/README.md
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1569 2023-04-18 19:46:26.000000 satvis-0.2.0/pyproject.toml
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/satvis/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2022-11-15 17:08:14.000000 satvis-0.2.0/satvis/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3791 2022-12-16 19:14:03.000000 satvis-0.2.0/satvis/int_tree_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     9374 2022-12-16 19:13:58.000000 satvis-0.2.0/satvis/schedule_plots.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3967 2022-12-16 19:16:52.000000 satvis-0.2.0/satvis/vis_history.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    11166 2023-04-18 19:45:28.000000 satvis-0.2.0/satvis/visibility_func.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/satvis.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      449 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2022-11-15 16:58:33.000000 satvis-0.2.0/satvis.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      269 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        7 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-04-18 19:48:25.243433 satvis-0.2.0/setup.cfg
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1480 2022-12-16 19:13:45.000000 satvis-0.2.0/tests/test_int_tree_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3660 2022-12-16 19:22:11.000000 satvis-0.2.0/tests/test_schedule_plots.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1407 2022-12-16 19:13:36.000000 satvis-0.2.0/tests/test_vis_history.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     7959 2023-04-18 19:42:38.000000 satvis-0.2.0/tests/test_visibility_func.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-21 15:16:33.882266 satvis-0.2.1/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1069 2022-11-14 19:16:32.000000 satvis-0.2.1/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-21 15:16:33.882266 satvis-0.2.1/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    12667 2022-11-16 20:21:06.000000 satvis-0.2.1/README.md
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1569 2023-04-21 15:15:09.000000 satvis-0.2.1/pyproject.toml
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-21 15:16:33.882266 satvis-0.2.1/satvis/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2022-11-15 17:08:14.000000 satvis-0.2.1/satvis/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3791 2022-12-16 19:14:03.000000 satvis-0.2.1/satvis/int_tree_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     9374 2022-12-16 19:13:58.000000 satvis-0.2.1/satvis/schedule_plots.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3967 2022-12-16 19:16:52.000000 satvis-0.2.1/satvis/vis_history.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    11863 2023-04-21 15:14:15.000000 satvis-0.2.1/satvis/visibility_func.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-21 15:16:33.882266 satvis-0.2.1/satvis.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-21 15:16:33.000000 satvis-0.2.1/satvis.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      449 2023-04-21 15:16:33.000000 satvis-0.2.1/satvis.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-04-21 15:16:33.000000 satvis-0.2.1/satvis.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2022-11-15 16:58:33.000000 satvis-0.2.1/satvis.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      269 2023-04-21 15:16:33.000000 satvis-0.2.1/satvis.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        7 2023-04-21 15:16:33.000000 satvis-0.2.1/satvis.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-04-21 15:16:33.882266 satvis-0.2.1/setup.cfg
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-21 15:16:33.882266 satvis-0.2.1/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1480 2022-12-16 19:13:45.000000 satvis-0.2.1/tests/test_int_tree_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3660 2022-12-16 19:22:11.000000 satvis-0.2.1/tests/test_schedule_plots.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1407 2022-12-16 19:13:36.000000 satvis-0.2.1/tests/test_vis_history.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     8610 2023-04-21 15:03:37.000000 satvis-0.2.1/tests/test_visibility_func.py
```

### Comparing `satvis-0.2.0/LICENSE` & `satvis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/PKG-INFO` & `satvis-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satvis
-Version: 0.2.0
+Version: 0.2.1
 Summary: Satellite LOS visibility calculator
 Author-email: Dylan Penn <dylanrpenn@vt.edu>
 License: MIT License
         
         Copyright (c) 2022 Dylan R. Penn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `satvis-0.2.0/README.md` & `satvis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/pyproject.toml` & `satvis-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satvis"
-version = "0.2.0"
+version = "0.2.1"
 description = "Satellite LOS visibility calculator"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=2.8.5"
 classifiers = [
     "Programming Language :: Python :: 2",
     "License :: OSI Approved :: MIT License",
```

### Comparing `satvis-0.2.0/satvis/int_tree_converter.py` & `satvis-0.2.1/satvis/int_tree_converter.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/satvis/schedule_plots.py` & `satvis-0.2.1/satvis/schedule_plots.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/satvis/vis_history.py` & `satvis-0.2.1/satvis/vis_history.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/satvis/visibility_func.py` & `satvis-0.2.1/satvis/visibility_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,28 @@
 
 # Standard Library Imports
 from typing import Tuple
 from warnings import warn
 
 # Third Party Imports
 from intervaltree import Interval, IntervalTree
-from numpy import append, arange, arccos, array, dot, isreal, nan, ndarray, sign
+from numpy import (
+    append,
+    arange,
+    arccos,
+    array,
+    dot,
+    float32,
+    isreal,
+    logical_and,
+    nan,
+    ndarray,
+    sign,
+    where,
+)
 from numpy.linalg import norm
 from numpy.polynomial import Polynomial
 
 
 # %% Visibility function
 def visibilityFunc(
     r1: ndarray,
@@ -117,15 +130,15 @@
 
 
 # %% Calculate visibility windows
 def zeroCrossingFit(
     v: ndarray,
     t: ndarray,
     id: object = None,
-) -> Tuple[ndarray[float], ndarray[float], IntervalTree]:
+) -> Tuple[ndarray[float], ndarray[int], IntervalTree]:
     """Interpolates visibility windows from sparse visibility data.
 
         Fit curves around zero-crossings of visibility function.
         Fit cubic polynomials to every 4 points, so loop through t[3] - t[end].
         Outputs interval tree object of visibility windows.
 
         Based on: Alfano, Salvatore, Negron, David Jr., Moore, Jennifer L.,
@@ -133,29 +146,29 @@
         Astronautical Sciences, Vol. 40, No. 2, 1992
     Args:
         v (`ndarray`): [1 x N] array of floats
         t (`ndarray`): [1 x N] array of floats
         id (`any`): (Optional) Identifier for interval tree
 
     Returns:
-        crossings (`ndarray`): [1 x M] array of times at which the
+        crossings (`ndarray[float]`): [1 x M] array of times at which the
             visibility function crosses 0
-        riseSet (`ndarray`): [1 x M] array of +-1 indicating if associated
+        riseSet (`ndarray[int]`): [1 x M] array of +-1 indicating if associated
             value in crossings is a rise point (+1) or set point (-1)
         tree (`IntervalTree`): Interval tree object of time bounds during
             which visibility function is >1
 
     Note that the ability to detect rise/set times within the first 2 steps
         of the beginning or end of `t` is sketchy due to the 4-point curve
         fit requirement. Workaround is in-place that does a 1st-order polyfit
         when t[0] and t[1] straddle v=0.
     """
     # initialize
-    crossings = []
-    riseSet = []
+    crossings = array([], dtype=float32)
+    riseSet = array([], dtype=int)
     tree = IntervalTree()
     crossIndx = -1
 
     # Special case: no-zero crossings, V is positive for all time
     if all(sign(v) == 1):
         temp = Interval(t[0], t[-1], id)
         tree.add(temp)
@@ -178,29 +191,30 @@
             tree.add(temp)
 
     # iterate through time vector for all other cases
     for i in arange(3, len(t)):
         # print('i =' + str(i))
         if i == 3:
             #  starting visibility sign (+1 or -1)
-            startV = sign(v[0])
+            startV = sign(v[1])
+
+        # print('i =' + str(i))
+        # grab 4 time values
+        tSnapshot = array([t[i - 3], t[i - 2], t[i - 1], t[i]])
+        # grab 4 v values
+        vSnapshot = array([v[i - 3], v[i - 2], v[i - 1], v[i]])
 
         # fit with 2 mid-points on either side of zero
-        if sign(v[i - 1]) != sign(v[i - 2]):
+        # if sign(v[i - 1]) != sign(v[i - 2]):
+        if sign(vSnapshot[1]) != sign(vSnapshot[2]):
             crossIndx += 1
 
-            # print('i =' + str(i))
-            # grab 4 time values
-            tSnapshot = array([t[i - 3], t[i - 2], t[i - 1], t[i]])
-            # grab 4 v values
-            vSnapshot = array([v[i - 3], v[i - 2], v[i - 1], v[i]])
-
             # Get new crossing.
             new_crossings = findCrossing(tSnapshot, vSnapshot, 3)
-            single_crossing = trimCrossings(new_crossings)
+            single_crossing = trimCrossings(new_crossings, tSnapshot)
             crossings = append(crossings, single_crossing)
 
             # determine if zero-crossing was a rise or set time and assign
             # val to vector
             riseSet = append(riseSet, riseOrSet(v[i - 1]))
 
             # Construct interval tree for times when v > 0 (visibility
@@ -225,26 +239,43 @@
             if crossIndx >= 0 and sign(v[i]) == 1:
                 temp = Interval(crossings[crossIndx], t[i], id)
                 tree.add(temp)
 
     return crossings, riseSet, tree
 
 
-def trimCrossings(crossings: ndarray) -> ndarray:
-    """Trim extra (false) crossings from array."""
+def trimCrossings(crossings: ndarray, time_snapshot: ndarray) -> ndarray:
+    """Trim extra (false) crossings from array.
+
+    Args:
+        crossings (`ndarray`): An array of crossing times.
+        time_snapshot (`ndarray`): A 4-element array of times encompassing crossings
+            (i.e. min(time_snapshot) < min(crossings) and
+            max(time_snapshot) > max(crossings)).
+
+    Returns:
+        `ndarray`: A single time from crossing that is in between time_snapshot[1]
+            and time_snapshot[2].
+    """
+    assert len(time_snapshot) == 4
 
     # Get new crossing; grab single element from new_crossings in case
-    # multiple crossings are returned. This happens in edge case where
-    # crossings occur between i=0/1 and i=1/2 or i=0/1, 1/2, and 2/3
+    # multiple crossings are returned.
     if len(crossings) == 1:
         # Single crossing detected, return input
         c = crossings[0]
-    elif len(crossings) in [2, 3]:
-        # 2 or 3 crossings detected, return the 1st entry.
-        c = crossings[1]
+    else:
+        # c = crossings[1]
+        lower_bound = time_snapshot[1]
+        upper_bound = time_snapshot[2]
+        indx = where(
+            logical_and(crossings <= upper_bound, crossings >= lower_bound)
+        )
+        assert len(indx) == 1
+        c = crossings[indx]
 
     return c
 
 
 def findCrossing(
     t: ndarray,
     v: ndarray,
```

### Comparing `satvis-0.2.0/satvis.egg-info/PKG-INFO` & `satvis-0.2.1/satvis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satvis
-Version: 0.2.0
+Version: 0.2.1
 Summary: Satellite LOS visibility calculator
 Author-email: Dylan Penn <dylanrpenn@vt.edu>
 License: MIT License
         
         Copyright (c) 2022 Dylan R. Penn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `satvis-0.2.0/tests/test_int_tree_converter.py` & `satvis-0.2.1/tests/test_int_tree_converter.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/tests/test_schedule_plots.py` & `satvis-0.2.1/tests/test_schedule_plots.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/tests/test_vis_history.py` & `satvis-0.2.1/tests/test_vis_history.py`

 * *Files identical despite different names*

### Comparing `satvis-0.2.0/tests/test_visibility_func.py` & `satvis-0.2.1/tests/test_visibility_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for `visibility_func.py`."""
 # %% Imports
 from __future__ import annotations
 
 # Third Party Imports
 from matplotlib import pyplot as plt
-from numpy import array, linspace, sin, zeros
+from numpy import arange, array, linspace, sin, zeros
 
 # satvis Imports
 from satvis.visibility_func import visibilityFunc, zeroCrossingFit
 
 # %% Test visibilityFunc
 print("\n visibilityFunc simple tests...")
 RE = 6378
@@ -184,14 +184,30 @@
 # Triple-crossing in a window up-down-up  (-+-++)
 vis_a = array([-1, 0.2, -0.5, 4, 2])
 [crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
 print("\n triple crossing (-+-++)")
 print(f"crossings={crossings} \nriseSet={riseSet}")
 print(f"tree={visTree}")
 
+# More than 1 frame, double-crossing, up-down (...-+--)
+vis_a = array([-1, -1, -1, -1, -0.2, +0.5, -4, -2])
+t = arange(0, len(vis_a))
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n >1 frame, double-crossing (...-+--)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
+# More than 1 frame, double-crossing, down-up (...+-++)
+vis_a = array([1, 1, 1, 1, 0.2, -0.5, 4, 2])
+t = arange(0, len(vis_a))
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n >1 frame, double-crossing (...+-++)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
 
 # %% Long time vector
 print("\nLong tests \n")
 tLong = linspace(0, 30, num=100)
 # multiple crossings, ends not visible
 vis5 = sin(tLong)
 [crossings, riseSet, visTree] = zeroCrossingFit(vis5, tLong, "der")
```

