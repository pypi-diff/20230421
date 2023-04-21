# Comparing `tmp/pycalib-0.1.0.dev3.tar.gz` & `tmp/pycalib-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycalib-0.1.0.dev3.tar", last modified: Wed Nov 30 14:10:10 2022, max compression
+gzip compressed data, was "pycalib-0.1.0.dev4.tar", last modified: Fri Apr 21 12:36:12 2023, max compression
```

## Comparing `pycalib-0.1.0.dev3.tar` & `pycalib-0.1.0.dev4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/PKG-INFO
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5372 2022-11-29 17:05:41.000000 pycalib-0.1.0.dev3/README.md
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       27 2022-11-30 14:09:37.000000 pycalib-0.1.0.dev3/pycalib/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    22331 2022-11-29 16:53:42.000000 pycalib-0.1.0.dev3/pycalib/metrics.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/models/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29071 2022-11-29 16:56:53.000000 pycalib-0.1.0.dev3/pycalib/models/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9530 2021-03-24 17:40:54.000000 pycalib-0.1.0.dev3/pycalib/models/multiclass.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     2712 2021-03-24 17:08:37.000000 pycalib-0.1.0.dev3/pycalib/stats.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/tests/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-03-08 14:18:37.000000 pycalib-0.1.0.dev3/pycalib/tests/__init__.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/tests/models/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-08-04 09:25:58.000000 pycalib-0.1.0.dev3/pycalib/tests/models/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1964 2022-11-29 16:54:08.000000 pycalib-0.1.0.dev3/pycalib/tests/models/test_init.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5012 2021-03-24 17:23:05.000000 pycalib-0.1.0.dev3/pycalib/tests/test_metrics.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1994 2022-11-29 16:53:11.000000 pycalib-0.1.0.dev3/pycalib/utils.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/visualisations/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29080 2022-11-29 16:52:30.000000 pycalib-0.1.0.dev3/pycalib/visualisations/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9077 2021-03-24 17:07:10.000000 pycalib-0.1.0.dev3/pycalib/visualisations/barycentric.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     6653 2021-03-24 17:06:48.000000 pycalib-0.1.0.dev3/pycalib/visualisations/ternary.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib/visualisations/tests/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-04-13 10:23:56.000000 pycalib-0.1.0.dev3/pycalib/visualisations/tests/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     4975 2022-11-29 16:52:02.000000 pycalib-0.1.0.dev3/pycalib/visualisations/tests/test_init.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/pycalib.egg-info/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2022-11-30 14:10:10.000000 pycalib-0.1.0.dev3/pycalib.egg-info/PKG-INFO
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)      624 2022-11-30 14:10:10.000000 pycalib-0.1.0.dev3/pycalib.egg-info/SOURCES.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        1 2022-11-30 14:10:10.000000 pycalib-0.1.0.dev3/pycalib.egg-info/dependency_links.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       76 2022-11-30 14:10:10.000000 pycalib-0.1.0.dev3/pycalib.egg-info/requires.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        8 2022-11-30 14:10:10.000000 pycalib-0.1.0.dev3/pycalib.egg-info/top_level.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       79 2022-11-30 14:10:10.279254 pycalib-0.1.0.dev3/setup.cfg
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1215 2022-11-30 14:09:22.000000 pycalib-0.1.0.dev3/setup.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/PKG-INFO
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5372 2022-11-29 17:05:41.000000 pycalib-0.1.0.dev4/README.md
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       27 2023-04-21 12:32:27.000000 pycalib-0.1.0.dev4/pycalib/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    22331 2022-11-29 16:53:42.000000 pycalib-0.1.0.dev4/pycalib/metrics.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/models/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29071 2022-11-29 16:56:53.000000 pycalib-0.1.0.dev4/pycalib/models/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9530 2021-03-24 17:40:54.000000 pycalib-0.1.0.dev4/pycalib/models/multiclass.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     2712 2021-03-24 17:08:37.000000 pycalib-0.1.0.dev4/pycalib/stats.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/tests/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-03-08 14:18:37.000000 pycalib-0.1.0.dev4/pycalib/tests/__init__.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/tests/models/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-08-04 09:25:58.000000 pycalib-0.1.0.dev4/pycalib/tests/models/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1964 2022-11-29 16:54:08.000000 pycalib-0.1.0.dev4/pycalib/tests/models/test_init.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5012 2021-03-24 17:23:05.000000 pycalib-0.1.0.dev4/pycalib/tests/test_metrics.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1994 2022-11-29 16:53:11.000000 pycalib-0.1.0.dev4/pycalib/utils.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/visualisations/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29080 2022-11-29 16:52:30.000000 pycalib-0.1.0.dev4/pycalib/visualisations/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9555 2023-04-21 12:35:12.000000 pycalib-0.1.0.dev4/pycalib/visualisations/barycentric.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     6653 2021-03-24 17:06:48.000000 pycalib-0.1.0.dev4/pycalib/visualisations/ternary.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/visualisations/tests/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-04-13 10:23:56.000000 pycalib-0.1.0.dev4/pycalib/visualisations/tests/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     4975 2022-11-29 16:52:02.000000 pycalib-0.1.0.dev4/pycalib/visualisations/tests/test_init.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib.egg-info/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/PKG-INFO
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)      624 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        1 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       76 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/requires.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        8 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/top_level.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       79 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/setup.cfg
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1215 2022-11-30 14:09:22.000000 pycalib-0.1.0.dev4/setup.py
```

### Comparing `pycalib-0.1.0.dev3/PKG-INFO` & `pycalib-0.1.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycalib
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Python library with tools for classifier calibration.
 Home-page: https://classifier-calibration.github.io/PyCalib/
 Author: Miquel Perello Nieto, Hao Song, Telmo de Menezes e Silva Filho
 Author-email: perello.nieto@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev3.tar.gz
+Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev4.tar.gz
 Description: [![CI][ci:b]][ci]
         [![Documentation][documentation:b]][documentation]
         [![License BSD3][license:b]][license]
         ![Python3.8][python:b]
         [![pypi][pypi:b]][pypi]
         [![codecov][codecov:b]][codecov]
         [![DOI](https://zenodo.org/badge/280465805.svg)](https://zenodo.org/badge/latestdoi/280465805)
```

### Comparing `pycalib-0.1.0.dev3/README.md` & `pycalib-0.1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/metrics.py` & `pycalib-0.1.0.dev4/pycalib/metrics.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/models/__init__.py` & `pycalib-0.1.0.dev4/pycalib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/models/multiclass.py` & `pycalib-0.1.0.dev4/pycalib/models/multiclass.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/stats.py` & `pycalib-0.1.0.dev4/pycalib/stats.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/tests/models/test_init.py` & `pycalib-0.1.0.dev4/pycalib/tests/models/test_init.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/tests/test_metrics.py` & `pycalib-0.1.0.dev4/pycalib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/utils.py` & `pycalib-0.1.0.dev4/pycalib/utils.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/visualisations/__init__.py` & `pycalib-0.1.0.dev4/pycalib/visualisations/__init__.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/visualisations/barycentric.py` & `pycalib-0.1.0.dev4/pycalib/visualisations/barycentric.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,38 +110,50 @@
     '''
     corners = np.array([[0, 0], [1, 0], [0.5, 0.75**0.5]])
     triangle = tri.Triangulation(corners[:, 0], corners[:, 1])
 
     refiner = tri.UniformTriRefiner(triangle)
     trimesh = refiner.refine_triangulation(subdiv=subdiv)
 
-    pvals = np.array([func(xy2bc(xy)) for xy in zip(trimesh.x, trimesh.y)])
+    z = np.array([func(xy2bc(xy)) for xy in zip(trimesh.x, trimesh.y)])
 
     if fig is None:
         fig = plt.figure()
     if ax is None:
         ax = fig.add_subplot(111)
 
     # FIXME I would like the following line to work, but the max value is not
     # shown. I had to do create manually the levels and increase the max value
     # by an epsilon. This could be a major problem if the epsilon is not small
     # for the original range of values
-    # contour = ax.tricontourf(trimesh, pvals, nlevels, **kwargs)
-    # contour = ax.tricontourf(trimesh, pvals, nlevels, extend='both')
-    contour = ax.tricontourf(trimesh, pvals,
-                             levels=np.linspace(pvals.min(), pvals.max()+1e-9,
-                                                nlevels),
-                             **kwargs)
-
-    # Colorbar
-    cb = fig.colorbar(contour, ax=ax, fraction=0.1, orientation='horizontal')
-    tick_locator = ticker.MaxNLocator(nbins=5)
-    cb.locator = tick_locator
-    # cb.ax.xaxis.set_major_locator(ticker.AutoLocator())
-    cb.update_ticks()
+    # contour = ax.tricontourf(trimesh, z, nlevels, **kwargs)
+    # contour = ax.tricontourf(trimesh, z, nlevels, extend='both')
+    is_nan = ~np.isfinite(z)
+    #z[is_nan] = 0
+    nan_id = np.where(is_nan)[0]
+    triangles_mask = np.zeros(trimesh.triangles.shape[0])
+    for ni in nan_id:
+        for i in range(trimesh.triangles.shape[0]):
+            if ni in trimesh.triangles[i]:
+                triangles_mask[i] = 1
+    trimesh.set_mask(triangles_mask)
+    if not np.all(triangles_mask):
+        contour = ax.tricontourf(trimesh, z,
+                                 levels=np.linspace(z[~is_nan].min(),
+                                                    z[~is_nan].max()+1e-9,
+                                                    nlevels),
+                                 **kwargs)
+
+        # Colorbar
+        cb = fig.colorbar(contour, ax=ax, fraction=0.1,
+                          orientation='horizontal')
+        tick_locator = ticker.MaxNLocator(nbins=5)
+        cb.locator = tick_locator
+        # cb.ax.xaxis.set_major_locator(ticker.AutoLocator())
+        cb.update_ticks()
 
     if labels is not None:
         if labels == 'auto':
             labels = [r'$C_{}$'.format(i+1) for i in range(len(corners))]
         center = corners.mean(axis=0)
         for i, corner in enumerate(corners):
             text_x, text_y = corner - (center - corner)*0.1
```

### Comparing `pycalib-0.1.0.dev3/pycalib/visualisations/ternary.py` & `pycalib-0.1.0.dev4/pycalib/visualisations/ternary.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib/visualisations/tests/test_init.py` & `pycalib-0.1.0.dev4/pycalib/visualisations/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/pycalib.egg-info/PKG-INFO` & `pycalib-0.1.0.dev4/pycalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycalib
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Python library with tools for classifier calibration.
 Home-page: https://classifier-calibration.github.io/PyCalib/
 Author: Miquel Perello Nieto, Hao Song, Telmo de Menezes e Silva Filho
 Author-email: perello.nieto@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev3.tar.gz
+Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev4.tar.gz
 Description: [![CI][ci:b]][ci]
         [![Documentation][documentation:b]][documentation]
         [![License BSD3][license:b]][license]
         ![Python3.8][python:b]
         [![pypi][pypi:b]][pypi]
         [![codecov][codecov:b]][codecov]
         [![DOI](https://zenodo.org/badge/280465805.svg)](https://zenodo.org/badge/latestdoi/280465805)
```

### Comparing `pycalib-0.1.0.dev3/pycalib.egg-info/SOURCES.txt` & `pycalib-0.1.0.dev4/pycalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev3/setup.py` & `pycalib-0.1.0.dev4/setup.py`

 * *Files identical despite different names*

