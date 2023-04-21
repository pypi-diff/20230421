# Comparing `tmp/awesom-0.1.2.post1.tar.gz` & `tmp/awesom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesom-0.1.2.post1.tar", max compression
+gzip compressed data, was "awesom-0.1.4.tar", max compression
```

## Comparing `awesom-0.1.2.post1.tar` & `awesom-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1521 2022-10-26 10:01:25.402992 awesom-0.1.2.post1/LICENSE
--rw-r--r--   0        0        0      832 2022-12-24 08:30:56.622538 awesom-0.1.2.post1/README.md
--rw-r--r--   0        0        0     1578 2022-12-24 08:33:08.886286 awesom-0.1.2.post1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-24 08:30:56.623432 awesom-0.1.2.post1/src/awesom/__init__.py
--rw-r--r--   0        0        0     1480 2022-12-24 08:30:56.623850 awesom-0.1.2.post1/src/awesom/datasets.py
--rw-r--r--   0        0        0      113 2022-12-24 08:30:56.624138 awesom-0.1.2.post1/src/awesom/defaults.py
--rw-r--r--   0        0        0     1906 2022-12-24 08:30:56.624400 awesom-0.1.2.post1/src/awesom/grid.py
--rw-r--r--   0        0        0     3429 2022-12-24 08:30:56.624683 awesom-0.1.2.post1/src/awesom/neighbors.py
--rw-r--r--   0        0        0     7018 2022-12-24 08:30:56.625370 awesom-0.1.2.post1/src/awesom/plot.py
--rw-r--r--   0        0        0    10724 2022-12-24 08:30:56.626599 awesom-0.1.2.post1/src/awesom/som.py
--rw-r--r--   0        0        0      379 2022-12-24 08:30:56.627665 awesom-0.1.2.post1/src/awesom/typealias.py
--rw-r--r--   0        0        0     9220 2022-12-24 08:30:56.628549 awesom-0.1.2.post1/src/awesom/utilities.py
--rw-r--r--   0        0        0     1629 1970-01-01 00:00:00.000000 awesom-0.1.2.post1/setup.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 awesom-0.1.2.post1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2022-10-26 10:01:25.402992 awesom-0.1.4/LICENSE
+-rw-r--r--   0        0        0      832 2022-12-24 08:30:56.622538 awesom-0.1.4/README.md
+-rw-r--r--   0        0        0     1577 2023-04-21 09:20:18.055030 awesom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-16 21:19:15.345043 awesom-0.1.4/src/awesom/__init__.py
+-rw-r--r--   0        0        0     1520 2023-04-21 09:20:18.056887 awesom-0.1.4/src/awesom/datasets.py
+-rw-r--r--   0        0        0      113 2023-01-16 21:19:15.349342 awesom-0.1.4/src/awesom/defaults.py
+-rw-r--r--   0        0        0      124 2023-04-21 09:20:18.057494 awesom-0.1.4/src/awesom/exceptions.py
+-rw-r--r--   0        0        0     2358 2023-04-21 09:56:58.015789 awesom-0.1.4/src/awesom/grid.py
+-rw-r--r--   0        0        0     4337 2023-04-21 09:35:31.292197 awesom-0.1.4/src/awesom/neighbors.py
+-rw-r--r--   0        0        0     7240 2023-04-21 09:20:18.059089 awesom-0.1.4/src/awesom/plot.py
+-rw-r--r--   0        0        0    10392 2023-04-21 09:52:18.013839 awesom-0.1.4/src/awesom/som.py
+-rw-r--r--   0        0        0      534 2023-04-21 09:46:36.463319 awesom-0.1.4/src/awesom/typing.py
+-rw-r--r--   0        0        0     6944 2023-04-21 09:20:18.060821 awesom-0.1.4/src/awesom/utilities.py
+-rw-r--r--   0        0        0     3461 2023-04-21 09:20:18.061514 awesom-0.1.4/src/awesom/weights.py
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 awesom-0.1.4/setup.py
+-rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 awesom-0.1.4/PKG-INFO
```

### Comparing `awesom-0.1.2.post1/LICENSE` & `awesom-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awesom-0.1.2.post1/README.md` & `awesom-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `awesom-0.1.2.post1/pyproject.toml` & `awesom-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awesom"
-version = "0.1.2-post1"
+version = "0.1.4"
 description = "Self-organizing map framework for Python"
 authors = ["Michael Blaß <mblass@posteo.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Teagum/awesom"
 classifiers = [
     "Programming Language :: Python :: 3.10",
@@ -51,14 +51,14 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "matplotlib.*"
 ignore_missing_imports = true
 
 [tool.pylint.basic]
-good-names = ["i", "j", "k", "t", "x", "y", "_", "ax", "dx", "dy", "dw", "ix", "iy"]
+good-names = ["i", "j", "k", "n", "t", "x", "y", "_", "ax", "dx", "dy", "dw", "ix", "iy"]
 
 [tool.pylint.typecheck]
 ignored-argument-names = "_.*|data"
 
 [tool.pylint.design]
 max-locals = 20
```

### Comparing `awesom-0.1.2.post1/src/awesom/datasets.py` & `awesom-0.1.4/src/awesom/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Function for generating test and illustration data sets.
 """
 
-from typing import Optional, Tuple
-
 import numpy as np
 from scipy import stats
 
+from awesom.typing import IntArray, FloatArray
+
 
 def norm_circle(n_classes: int, n_per_class: int, class_std: int,
-                center: Tuple[int, int] = (0, 0), radius: int = 5,
-                seed: Optional[int] = None):
+                center: tuple[int, int] = (0, 0), radius: int = 5,
+                seed: int | None = None) -> tuple[FloatArray, IntArray]:
     # pylint: disable = too-many-arguments
     """Generate ``n_per_class`` samples from ``n_classes`` bivariate normal
     distributions, each with standard deviation ``class_std``. The means
     are equidistantly placed on a circle with radius ``radius``.
 
     Args:
         n_classes:    Number of classes.
```

### Comparing `awesom-0.1.2.post1/src/awesom/grid.py` & `awesom-0.1.4/src/awesom/grid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Grid for Self-organizing maps
 """
+from typing import Generator
+
 import numpy as np
 from scipy.spatial import cKDTree
 
-from . typealias import Array, Shape
+from awesom.typing import IntArray, DistFunc, Shape, FloatArray
 
 
 class SomGrid:
     """Rectangular SOM grid
     """
     def __init__(self, shape: Shape) -> None:
         if not all(isinstance(val, int) and val >= 1 for val in shape):
             raise ValueError("Dimensions must be integer > 0.")
         self.shape = shape
         self.pos = np.asarray(list(np.ndindex(shape)), dtype=int)
         self.tree = cKDTree(self.pos)
         self.rows, self.cols = np.indices(shape)
+        self.dists = np.empty((self.pos.shape[0], 1), dtype=np.float64)
 
-    def nhb_idx(self, radius: float, points: Array | None = None) -> Array:
+    def nhb_idx(self, radius: float, points: IntArray | None = None) -> IntArray:
         """Compute the neighbourhood unit indices within ``radius``
 
         If ``points`` is given, return the neighbourhood around each unit in
         ``points``. Otherwise, return the neighbourhodd for each unit on the
         grid.
 
         Args:
@@ -32,15 +35,15 @@
         Returns:
             Array of indices of neighbours.
         """
         if points is None:
             points = self.pos
         return np.asarray(self.tree.query_ball_point(points, radius, np.inf))
 
-    def nhb(self, radius: float, points: Array | None = None) -> Array:
+    def nhb(self, radius: float, points: IntArray | None = None) -> IntArray:
         """Compute neighbourhood within ``radius``
 
         If ``points`` is given, return the neighbourhood around each unit in
         ``points``. Otherwise, return the neighbourhodd for each unit on the
         grid.
 
         Args:
@@ -51,10 +54,15 @@
             Array of positions of neighbours.
         """
         if points is None:
             points = self.pos
         idx = self.nhb_idx(radius, points)
         return self.pos[idx]
 
-    def __iter__(self):
+    def neighbourhood_distances(self, center: FloatArray, radius: float,
+                                distance_func: DistFunc) -> FloatArray:
+        """Compute distances given ``distance_func``"""
+        return distance_func(self.pos, center, radius, self.dists)
+
+    def __iter__(self) -> Generator[tuple[int, int], None, None]:
         for row, col in zip(self.rows.flat, self.cols.flat):
             yield row, col
```

### Comparing `awesom-0.1.2.post1/src/awesom/plot.py` & `awesom-0.1.4/src/awesom/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Plotting functions for SOMs.
 """
 
-from typing import Callable, Optional, Union
+from typing import Any, Callable
 
 import numpy as np
 import numpy.typing as npt
 
+from awesom.typing import FloatArray, IntArray, Axis
 from . import utilities as utils
-from . typealias import Array, Axis
+from . som import SomBase
 
 
-def umatrix(ax: Axis, som, outline: bool = False, **kwargs) -> None:
+def umatrix(ax: Axis, som: SomBase, outline: bool = False, **kwargs: Any
+            ) -> None:
     """Plot the U-matrix.
 
     Args:
         ax:   Axis subplot.
         som:  SOM instance.
 
     Note:
@@ -24,15 +26,15 @@
     props = {
         'cmap': "terrain",
         'levels': 20}
     props.update(kwargs)
     _generic_contour(ax, som.umatrix(), outline, **props)
 
 
-def umatrix3d(ax: Axis, som, **kwargs) -> None:
+def umatrix3d(ax: Axis, som: SomBase, **kwargs: Any) -> None:
     """Plot the U-matrix in three dimensions.
 
     Args:
         ax:   Axis subplot.
         som:  SOM instance.
 
     Note:
@@ -41,16 +43,16 @@
     props = {
         'cmap': "terrain",
         }
     props.update(kwargs)
     ax.plot_surface(*np.mgrid[:som.dx, :som.dy], som.umatrix(), **props)
 
 
-def component(ax: Axis, som, comp: int, outline: bool = False,
-              **kwargs) -> None:
+def component(ax: Axis, som: SomBase, comp: int, outline: bool = False,
+              **kwargs: Any) -> None:
     """Plot a component plane.
 
     Args:
         ax:    Axis subplot.
         som:   SOM instance.
         comp:  Component number.
     """
@@ -58,15 +60,16 @@
         'cmap': "magma",
         'levels': 20,}
     props.update(kwargs)
     _generic_contour(ax, som.weights[:, comp].reshape(som.shape), outline,
                      **props)
 
 
-def label_target(ax: Axis, som, data: Array, target: Array, **kwargs) -> None:
+def label_target(ax: Axis, som: SomBase, data: FloatArray, target: IntArray, **kwargs: Any
+                 ) -> None:
     """Add target labels for each bmu.
 
     Args:
         ax:      Axis subplot.
         som:     SOM instance.
         data:    Input data.
         target:  Target labels.
@@ -80,26 +83,26 @@
 
     bmu = som.match(data)
     bmu_xy = np.fliplr(np.atleast_2d(bmu)).T
     for x, y, t in zip(*bmu_xy, target):
         ax.text(x, y, t, fontdict=props)
 
 
-def qerror(ax: Axis, som, **kwargs) -> None:
+def qerror(ax: Axis, som: SomBase, **kwargs: Any) -> None:
     """Plot quantization error."""
     props = {
         'lw': 3,
         'alpha': .8,
         }
     props.update(kwargs)
     ax.plot(som.quantization_error, **props)
 
 
-def cluster_by(ax: Axis, som, data: Array, target: Array,
-               **kwargs) -> None:
+def cluster_by(ax: Axis, som: SomBase, data: FloatArray, target: IntArray, **kwargs: Any
+               ) -> None:
     """Plot bmu colored by ``traget``.
 
     Args:
         ax:      Axis subplot.
         som:     SOM instance.
         data:    Input data.
         target:  Target labels.
@@ -111,16 +114,17 @@
             }
     props.update(kwargs)
     bmu = som.match(data)
     bmu_xy = np.fliplr(np.atleast_2d(bmu)).T
     ax.scatter(*bmu_xy, **props)
 
 
-def hit_counts(ax: Axis, som, transform: Optional[Callable] = None,
-               **kwargs) -> None:
+def hit_counts(ax: Axis, som: SomBase,
+               transform: Callable[[IntArray], IntArray] | None = None
+               , **kwargs: Any) -> None:
     """Plot the winner histogram.
 
     Each unit is colored according to the number of times it was bmu.
 
     Args:
         ax:    Axis subplot.
         som:   SOM instance.
@@ -134,20 +138,18 @@
     props.update(kwargs)
     data = som.hit_counts.reshape(som.shape)
     if transform is not None:
         data = transform(data)
     ax.imshow(data, **props)
 
 
-def wire(ax: Axis, som,
-         unit_size: Union[float, Array] = 100.0,
-         line_width: float = 1.0,
-         highlight: Optional[Array] = None, labels: bool = False,
-         unit_color: str = 'k',
-         **kwargs) -> None:
+def wire(ax: Axis, som: SomBase,
+         unit_size: float | FloatArray = 100.0, line_width: float = 1.0,
+         highlight: FloatArray | None = None, labels: bool = False,
+         unit_color: str = 'k', **kwargs: Any) -> None:
     # pylint: disable = too-many-locals, too-many-arguments
     """Plot the weight vectors of a SOM with two-dimensional feature space.
 
     Neighbourhood relations are indicate by connecting lines.
 
     Args:
         ax:          The axis subplot.
@@ -221,16 +223,15 @@
 
     if labels is True:
         for (sw_x, sw_y), (ix, iy) in zip(som.weights, np.ndindex(som.shape)):
             ax.text(sw_x+1.3, sw_y, f"({ix}, {iy})", font, bbox=bbox, zorder=13)
     ax.set_aspect("equal")
 
 
-def data_2d(ax: Axis, data: Array, colors: Array,
-            **kwargs) -> None:
+def data_2d(ax: Axis, data: FloatArray, colors: FloatArray, **kwargs: Any) -> None:
     """Scatter plot a data set with two-dimensional feature space.
 
     This just the usual scatter command with some reasonable defaults.
 
     Args:
         ax:      The axis subplot.
         data:    The data set.
@@ -245,16 +246,16 @@
         'cmap': "plasma",
         'edgecolors': "None",
         's': 10}
     props.update(kwargs)
     _ = ax.scatter(*data.T, **props)
 
 
-def _generic_contour(ax: Axis, data: Array, outline: bool = False,
-                     **kwargs) -> None:
+def _generic_contour(ax: Axis, data: FloatArray, outline: bool = False,
+                     **kwargs: Any) -> None:
     """Contour plot.
 
     Args:
         ax:    Axis subplot.
         data:  Two-dimensional array.
     """
     sdx, sdy = data.shape
```

### Comparing `awesom-0.1.2.post1/src/awesom/som.py` & `awesom-0.1.4/src/awesom/som.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 
 # pylint: disable = R0904, R0902, R0913
 
 import pathlib
 import pickle
 
 import numpy as np
+import numpy.typing as npt
 from scipy.spatial import distance
 
+from awesom.exceptions import NotCalibratedError
+from awesom.typing import FloatArray, IntArray, Metric, Shape, SomDims, FilePath
 from . import defaults
 from . import grid
 from . import neighbors
 from . import utilities as utils
-from . typealias import Array, Metric, Shape, SomDims, WeightInit, FilePath
+from . weights import Weights
 
 
 class SomBase:
     """Self-organizing map base class
     """
-    def __init__(self, dims: SomDims, n_iter: int, eta: float,
-                 nhr: float, nh_shape: str, init_weights: WeightInit,
-                 metric: Metric, seed: float | None = None):
+    def __init__(self, dims: SomDims, n_iter: int, eta: float, nhr: float,
+                 nh_shape: str, weights: Weights, metric: Metric = "euclidean",
+                 seed: int | IntArray | None = None):
 
         self._grid = grid.SomGrid(dims[:2])
         self.n_features = dims[2]
-        self._hit_counts = np.zeros(self.n_units)
+        self._hit_counts = np.zeros(self.n_units, dtype=np.int_)
         self.n_iter = n_iter
         self.metric = metric
         self._qrr = np.zeros(n_iter)
         self._trr = np.zeros(n_iter)
-        self._weights: Array | None = None
+        self._weights = weights
+        self._rng = np.random.default_rng(seed)
+        self._calibration: IntArray | None = None
 
         try:
             self._neighbourhood = getattr(neighbors, nh_shape)
         except AttributeError as err:
             raise AttributeError(f"Neighborhood shape {nh_shape} is unknown. "
                                  "Use one of `gaussian`, `mexican`, `rect`, or "
                                  "`star`") from err
@@ -47,26 +52,14 @@
                              "range [0, 1]")
 
         if nhr >= 1:
             self.init_nhr = nhr
         else:
             raise ValueError("Neighbourhood radius must be int > 0.")
 
-        if seed is not None:
-            np.random.seed(seed)
-
-        if isinstance(init_weights, str):
-            self.init_weights = utils.weight_initializer[init_weights]
-        elif callable(init_weights):
-            self.init_weights = init_weights
-        else:
-            msg = "Initializer must be string or callable."
-            raise ValueError(msg)
-
-        self._dists: Array | None = None
 
     @property
     def dims(self) -> SomDims:
         """Return the SOM dimensions."""
         return (*self._grid.shape, self.n_features)
 
     @property
@@ -96,55 +89,45 @@
 
     @property
     def grid(self) -> grid.SomGrid:
         """Return the grid."""
         return self._grid
 
     @property
-    def dists(self) -> Array | None:
-        """Return the distance matrix of the grid points."""
-        return self._dists
-
-    @property
-    def weights(self) -> Array | None:
+    def weights(self) -> FloatArray:
         """Return the weight vectors."""
-        return self._weights
+        return self._weights.vectors
 
     @property
-    def hit_counts(self) -> Array:
+    def hit_counts(self) -> IntArray:
         """Return total hit counts for each SOM unit."""
         return self._hit_counts
 
     @property
-    def quantization_error(self) -> Array:
+    def quantization_error(self) -> FloatArray:
         """Return quantization error."""
         return self._qrr
 
     @property
-    def topographic_error(self) -> Array:
+    def topographic_error(self) -> FloatArray:
         """Return topographic error."""
         return self._trr
 
-    def calibrate(self, data: Array, target: Array) -> Array:
+    def calibrate(self, data: FloatArray, target: IntArray) -> None:
         """Retrieve the target value of the best matching input data vector
         for each unit weight vector.
 
         Args:
             data:     Input data set.
             target:  Target labels.
-
-        Returns:
-            Array of target values.
         """
-        if self._weights is None:
-            raise ValueError("Weights not initialized")
-        bm_dv, _ = utils.best_match(data, self._weights, self.metric)
-        return target[bm_dv]
+        bm_dv, _ = utils.best_match(data, self.weights, self.metric)
+        self._calibration = target[bm_dv]
 
-    def distribute(self, data: Array) -> dict[int, list[int]]:
+    def distribute(self, data: FloatArray) -> dict[int, list[int]]:
         """Distribute the vectors of ``data`` on the SOM.
 
         Indices of vectors n ``data`` are mapped to the index of
         their best matching unit.
 
         Args:
             data:  Input data set.
@@ -152,109 +135,94 @@
         Returns:
             Dictionary with SOM unit indices as keys. Each key maps to a list
             that holds the indices of rows in ``data``, which best match this
             key.
         """
         return utils.distribute(self.match(data), self.n_units)
 
-    def match_flat(self, data: Array) -> Array:
+    def match_flat(self, data: FloatArray) -> IntArray:
         """Return the index of the best matching unit for each vector in
         ``data``.
 
         Args:
             data:  Input data set.
 
         Returns:
             Array of SOM unit indices.
         """
-        if self._weights is None:
-            raise ValueError("Weights not initialized")
-        bmu, _ = utils.best_match(self._weights, data, self.metric)
+        bmu, _ = utils.best_match(self.weights, data, self.metric)
         return bmu
 
-    def match(self, data: Array) -> Array:
+    def match(self, data: FloatArray) -> IntArray:
         """Return the multi index of the best matching unit for each vector in
         ``data``.
 
         Caution: This function returns the multi index into the array.
 
         Args:
             data:  Input data set.
 
         Returns:
             Array of SOM unit indices.
         """
         bmu = self.match_flat(data)
         return np.column_stack(np.unravel_index(bmu, self.shape))
 
-    def predict(self, data: Array) -> Array:
+    def predict(self, data: FloatArray) -> IntArray:
         """Predict the SOM index of the best matching unit
         for each item in ``data``.
 
         Args:
             data:  Input data. Rows are items, columns are features.
 
         Returns:
             One-dimensional array of indices.
         """
-        if self._weights is None:
-            raise ValueError("Weights not initialized")
-        bmi, _ = utils.best_match(self._weights, data, self.metric)
-        return bmi
+        if self._calibration is None:
+            raise NotCalibratedError("Cannot predict fromm not calibrated SOM")
+        bmi, _ = utils.best_match(self.weights, data, self.metric)
+        return self._calibration[bmi]
 
     def save(self, path: FilePath) -> None:
         """Save SOM object to pickle file
 
         Args:
             path: Save SOM to this path.
         """
         path = pathlib.Path(path)
         with path.open("wb") as file:
             pickle.dump(self, file)
 
-    def save_weights(self, path: FilePath) -> None:
-        """Save weights only as a portable `.npy` file
-
-        Args:
-            path:  File path
-        """
-        if self._weights is None:
-            raise ValueError("Weights not initialized")
-        np.save(path, self._weights, allow_pickle=False)
-
-    def transform(self, data: Array) -> Array:
+    def transform(self, data: FloatArray) -> FloatArray:
         """Transform each item in ``data`` to feature space.
 
         This, in principle, returns best matching unit's weight vectors.
 
         Args:
             data:  Input data. Rows are items, columns are features.
 
         Returns:
             Position of each data item in the feature space.
         """
-        bmi = self.predict(data)
-        if self._weights is None:
-            raise ValueError("Weights not initialized")
+        bmi = self.match_flat(data)
         return self._weights[bmi]
 
-    def umatrix(self, radius: int = 1, scale: bool = True, norm: bool = True):
+    def umatrix(self, radius: int = 1, scale: bool = True, norm: bool = True
+                ) -> FloatArray:
         """Compute U-matrix of SOM instance.
 
         Args:
             radius:   Map neighbourhood radius.
             scale:    If ``True``, scale each U-height by the number of the
                       associated unit's neighbours.
             norm:     Normalize U-matrix if ``True``.
 
         Returns:
             Unified distance matrix.
         """
-        if self._weights is None:
-            raise ValueError("Wrights not initialized")
         u_height = np.empty(self.n_units, dtype="float64")
         nhd_per_unit = self._grid.nhb_idx(radius)
         for i, nhd_idx in enumerate(nhd_per_unit):
             cwv = self._weights[[i]]
             nhd = self._weights[nhd_idx]
             u_height[i] = distance.cdist(cwv, nhd, self.metric).sum()
             if scale:
@@ -270,56 +238,70 @@
 
 class BatchMap(SomBase):
     """Self-organizing map with batch training
 
     The batch training updates the weight vectors once for all input vectors.
     """
     def __init__(self, dims: SomDims, n_iter: int, eta: float, nhr: float,
-                 nh_shape: str = "gaussian", init_weights: WeightInit  = "rnd",
+                 nh_shape: str = "gaussian", weights: Weights | None = None,
                  metric: Metric = "euclidean", seed: int | None = None):
 
-        super().__init__(dims, n_iter, eta, nhr, nh_shape, init_weights, metric,
+        if weights is None:
+            weights = Weights(*dims)
+            weights.init_pca()
+
+        super().__init__(dims, n_iter, eta, nhr, nh_shape, weights, metric,
                          seed=seed)
 
 
 class IncrementalMap(SomBase):
     """Self-organizing map with online learning algorithm
 
     The incremental, or online training updates the weight vectors for each
     input vector.
     """
     def __init__(self, dims: SomDims, n_iter: int, eta: float, nhr: float,
-                 nh_shape: str = "gaussian", init_weights: WeightInit = "rnd",
+                 nh_shape: str = "gaussian", weights: Weights | None = None,
                  metric: Metric = "euclidean", seed: int | None = None):
 
-        super().__init__(dims, n_iter, eta, nhr, nh_shape, init_weights, metric,
-                         seed=seed)
+        if weights is None:
+            weights = Weights(*dims)
+            weights.init_pca()
 
-    def fit(self, train_data, verbose=False, output_weights=False):
-        """Fit the SOM to the ``training_data``
+        super().__init__(dims, n_iter, eta, nhr, nh_shape, weights, metric,
+                         seed=seed)
 
-        The method first initializes the weight vectors and then starts
-        training.
-        """
-        self._weights = self.init_weights(self.dims, train_data)
+    def fit(self, train_data: FloatArray, target: IntArray | None = None,
+            verbose: bool = False) -> None:
+        """Fit the SOM to the ``training_data``"""
         eta_ = utils.decrease_linear(self.init_eta, self.n_iter, defaults.FINAL_ETA)
         nhr_ = utils.decrease_expo(self.init_nhr, self.n_iter, defaults.FINAL_NHR)
 
-        np.random.seed(10)
+        _update_buffer = np.empty_like(self.weights)
         for (c_iter, c_eta, c_nhr) in zip(range(self.n_iter), eta_, nhr_):
             if verbose:
                 print(f"iter: {c_iter:2} -- eta: {np.round(c_eta, 4):<5} -- "
                       f"nh: {np.round(c_nhr, 5):<6}")
 
-            for i, fvect in enumerate(np.random.permutation(train_data)):
-                if output_weights:
-                    fname = f"weights/weights_{c_iter:05}_{i:05}.npy"
-                    with open(fname, "wb") as fobj:
-                        np.save(fobj, self._weights, allow_pickle=False)
+            for fvect in self._rng.permutation(train_data):
                 bmu, err = utils.best_match(self.weights, fvect, self.metric)
                 self._hit_counts[bmu] += 1
                 m_idx = np.atleast_2d(np.unravel_index(bmu, self.shape)).T
-                neighbourhood = self._neighbourhood(self._grid.pos, m_idx, c_nhr)
-                self._weights += c_eta * neighbourhood * (fvect - self._weights)
+                #self._neighbourhood(self._grid.pos, m_idx, c_nhr, self._grid._dists)
+                self._update_weights(fvect, m_idx, c_nhr, c_eta, _update_buffer)
 
             _, err = utils.best_match(self.weights, train_data, self.metric)
             self._qrr[c_iter] = err.sum() / train_data.shape[0]
+
+        if target is not None:
+            self.calibrate(train_data, target)
+
+    def _update_weights(self, vec: FloatArray, center: npt.ArrayLike, radius:
+                        float, eta: float, buffer: FloatArray) -> None:
+        #update = eta * neighbours * (vec - self._weights.vectors)
+        #self._weights.vectors += update
+        center = np.asarray(center).astype(np.float64)
+        self.grid.neighbourhood_distances(center, radius, self._neighbourhood)
+        np.subtract(vec, self._weights.vectors, out=buffer)
+        np.multiply(self.grid.dists, buffer, out=buffer)
+        np.multiply(eta, buffer, out=buffer)
+        np.add(buffer, self._weights.vectors, out=self._weights.vectors)
```

### Comparing `awesom-0.1.2.post1/src/awesom/utilities.py` & `awesom-0.1.4/src/awesom/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Utilities for self.organizing maps.
 """
 
 import itertools
-from typing import Iterable, Iterator
+from typing import cast, Iterable, Iterator
 
 import numpy as np
 from scipy.spatial import distance
 from scipy import stats
 
-from . typealias import Array, Metric, SomDims
+from awesom.typing import IntArray, FloatArray, Metric
 
 
 def grid_iter(n_rows: int, n_cols: int) -> Iterator[tuple[int, int]]:
     """Compute grid indices of an two-dimensional array.
 
     Args:
         n_rows:  Number of array rows.
@@ -21,25 +21,25 @@
 
     Returns:
         Multi-index iterator.
     """
     return itertools.product(range(n_rows), range(n_cols))
 
 
-def grid(n_rows: int, n_cols: int) -> Array:
+def grid(n_rows: int, n_cols: int) -> IntArray:
     """Compute grid indices of a two-dimensional array.
 
     Args:
         n_rows:  Number of array rows.
         n_cols:  Number of array columns.
 
     Returns:
         Two-dimensional array in which each row represents an multi-index.
     """
-    return np.array(list(grid_iter(n_rows, n_cols)))
+    return np.array(list(grid_iter(n_rows, n_cols)), dtype=int)
 
 
 def decrease_linear(start: float, step: float, stop: float = 1.0
                     ) -> Iterator[float]:
     """Linearily decrease ``start``  in ``step`` steps to ``stop``."""
     if step < 1 or not isinstance(step, int):
         raise ValueError("Param `step` must be int >= 1.")
@@ -60,16 +60,16 @@
         yield start
     else:
         coef = np.log(stop / start) / (step - 1)
         for stp in range(step):
             yield start * np.exp(coef*stp)
 
 
-def best_match(weights: Array, inp: Array, metric: Metric
-               ) -> tuple[Array, Array]:
+def best_match(weights: FloatArray, inp: FloatArray, metric: Metric,
+               out: FloatArray | None = None) -> tuple[IntArray, FloatArray]:
     """Compute the best matching unit of ``weights`` for each
     element in ``inp``.
 
     If several elemets in ``weights`` have the same distance to the
     current element of ``inp``, the first element of ``weights`` is
     choosen to be the best matching unit.
 
@@ -95,125 +95,68 @@
         raise ValueError(msg)
 
     inp = np.atleast_2d(inp)
     if inp.ndim > 2:
         msg = (f"Array ``inp`` has {weights.ndim} dimensions, it "
                "has to have one or two dimensions.")
         raise ValueError(msg)
-
-    dists = distance.cdist(weights, inp, metric)
+    dists = distance.cdist(weights, inp, metric, out=out)
     return dists.argmin(axis=0), dists.min(axis=0)
 
 
-def sample_pca(dims: SomDims, data: Array | None = None, **kwargs) -> Array:
-    """Compute initial SOM weights by sampling from the first two principal
-    components of the input data.
-
-    Args:
-        dims:   Dimensions of SOM.
-        data:   Input data set.
-        adapt:  If ``True``, the largest value of ``shape`` is applied to the
-                principal component with the largest sigular value. This
-                orients the map, such that map dimension with the most units
-                coincides with principal component with the largest variance.
-
-    Returns:
-        Array of SOM weights.
-    """
-    n_rows, n_cols, n_feats = dims
-
-    if data is None:
-        data = np.random.randint(-100, 100, (300, n_feats))
-    _, vects, trans_data = pca(data, 2)
-    data_min = trans_data.min(axis=0)
-    data_max = trans_data.max(axis=0)
-    if "adapt" in kwargs and kwargs['adapt'] is True:
-        shape = tuple(sorted((n_rows, n_cols), reverse=True))
-    else:
-        shape = (n_rows, n_cols)
-    dim_x = np.linspace(data_min[0], data_max[0], shape[0])
-    dim_y = np.linspace(data_min[1], data_max[1], shape[1])
-    grid_x, grid_y = np.meshgrid(dim_x, dim_y)
-    points = np.vstack((grid_x.ravel(), grid_y.ravel()))
-    weights = points.T @ vects + data.mean(axis=0)
-    return weights
-
+def sample_st_matrix(n_mat: int, size: int) -> FloatArray:
+    """Sample stochastic matrices from Dirichlet distribution
 
-def sample_rnd(dims: SomDims, data: Array | None = None) -> Array:
-    """Compute initial SOM weights by sampling uniformly from the data space.
+    The distribution is configured to place five times more probability mass on
+    the main diagonal than on the remaining elements.
 
     Args:
-        dims:  Dimensions of SOM.
-        data:  Input data set. If ``None``, sample from [-10, 10].
+        n_mat:  Number of matrices
+        size:   Number of matirx row/cols
 
     Returns:
-        Array of SOM weights.
+        Two-dimensional array. Each row corresponds to a flattened matrix.
     """
-    n_rows, n_cols, n_feats = dims
-    n_units = n_rows * n_cols
-    if data is not None:
-        data_limits = np.column_stack((data.min(axis=0), data.max(axis=0)))
-    else:
-        data_limits = np.random.randint(-10, 10, (n_feats, 2))
-        data_limits.sort()
-    weights = [np.random.uniform(dmin, dmax, n_units)
-               for (dmin, dmax) in data_limits]
-    return np.column_stack(weights)
-
-
-def sample_stm(dims: SomDims, data: Array | None = None) -> Array:
-    """Compute initial SOM weights by sampling stochastic matrices from
-    Dirichlet distribution.
-
-    The rows of each n by n stochastic matrix are sampes drawn from the
-    Dirichlet distribution, where n is the number of rows and cols of the
-    matrix. The diagonal elemets of the matrices are set to twice the
-    probability of the remaining elements.
-    The square root of the weight vectors' size must be a real integer.
+    if n_mat < 1:
+        raise ValueError("n_mat < 1")
 
-    Args:
-        dims:  Dimensions of SOM.
-        data:  Input data set.
+    if size < 2:
+        raise ValueError("size < 2")
 
-    Returns:
-        Array of SOM weights.
+    pfact = 5.0
+    alpha = np.ones((size, size), dtype=np.float64)
+    np.fill_diagonal(alpha, pfact)
 
-    Notes:
-        Each row of the output array is to be considered a flattened
-        stochastic matrix, such that each ``N = sqrt(data.shape[1])`` values
-        are a discrete probability distribution forming the ``N`` th row of
-        the matrix.
-    """
-    n_rows, n_cols, n_feats = dims
-    n_states = np.sqrt(n_feats)
-    if bool(n_states - int(n_states)):
-        msg = (f"Weight vector with {n_feats} elements is not "
-               "reshapeable to square matrix.")
-        raise ValueError(msg)
+    samples = [stats.dirichlet(a).rvs(n_mat) for a in alpha]
+    return np.hstack(samples, dtype=np.float64)
 
-    n_states = int(n_states)
-    n_units = n_rows * n_cols
-    alpha = np.random.randint(1, 10, (n_states, n_states))
-    st_matrix = np.hstack([stats.dirichlet(a).rvs(size=n_units)
-                           for a in alpha])
-    return st_matrix
 
+def sample_st_vector(n_vectors: int, size: int) -> FloatArray:
+    """Sample stochastic vectors
 
-def sample_hist(dims: SomDims, data: Array | None = None) -> Array:
-    """Sample sum-normalized histograms.
+    Sample random stochastic vectors with uniformly distributed probability
+    mass. The sum of each vector equals 1.0 and each element is a number
+    between 0.0 and 1.0.
 
     Args:
-        dims:  Dimensions of SOM.
-        data:  Input data set.
+        n_vectors: Number of vectors
+        size:      Vector size
 
     Returns:
-        Two-dimensional array in which each row is a historgram.
+        Two-dimensional array, whose rows correspond to vectors
     """
-    n_rows, n_cols, n_feats = dims
-    return stats.dirichlet(np.ones(n_feats)).rvs(n_rows*n_cols)
+    if n_vectors < 1:
+        raise ValueError("``n_vectors < 0")
+
+    if size < 1:
+        raise ValueError("``size`` < 1")
+
+    alpha = np.ones(size, dtype=np.float64)
+    samples = stats.dirichlet(alpha).rvs(n_vectors)
+    return np.asanyarray(samples, dtype=np.float64)
 
 
 def distribute(bmu_idx: Iterable[int], n_units: int
                ) -> dict[int, list[int]]:
     """List training data matches per SOM unit.
 
     This method assumes that the ith element of ``bmu_idx`` corresponds to the
@@ -232,15 +175,16 @@
     """
     unit_matches: dict[int, list[int]] = {i: [] for i in range(n_units)}
     for data_idx, bmu in enumerate(bmu_idx):
         unit_matches[bmu].append(data_idx)
     return unit_matches
 
 
-def pca(data: Array, n_comps: int = 2) -> tuple[Array, Array, Array]:
+def pca(data: FloatArray, n_comps: int = 2
+        ) -> tuple[FloatArray, FloatArray, FloatArray]:
     """Perfom principal component analysis
 
     Interanlly, ``data`` will be centered but not scaled.
 
     Args:
         data:     Data set
         n_comps:  Number of principal components
@@ -255,16 +199,16 @@
 
     ord_idx = np.flip(vals.argsort())[:n_comps]
     vals = vals[ord_idx]
     vects = vects[ord_idx]
     return vals, vects, data_centered @ vects.T
 
 
-def scale(arr: Array, new_min: int = 0, new_max: int = 1, axis: int = -1
-          ) -> Array:
+def scale(arr: FloatArray, new_min: int = 0, new_max: int = 1, axis: int = -1
+          ) -> FloatArray:
     """Scale ``arr`` between ``new_min`` and ``new_max``
 
     Args:
         arr:        Array to be scaled.
         new_min:    Lower bound.
         new_max:    Upper bound.
 
@@ -273,15 +217,8 @@
     """
     xmax = arr.max(axis=axis, keepdims=True)
     xmin = arr.min(axis=axis, keepdims=True)
 
     fact = (arr-xmin) / (xmax - xmin)
     out = fact * (new_max - new_min) + new_min
 
-    return out
-
-
-weight_initializer = {
-    'rnd': sample_rnd,
-    'stm': sample_stm,
-    'pca': sample_pca,
-    'hist': sample_hist}
+    return cast(FloatArray, out)
```

### Comparing `awesom-0.1.2.post1/setup.py` & `awesom-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.1,<4.0.0', 'numpy>=1.23.4,<2.0.0', 'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'awesom',
-    'version': '0.1.2.post1',
+    'version': '0.1.4',
     'description': 'Self-organizing map framework for Python',
     'long_description': '[![mypy](https://github.com/Teagum/blossom/actions/workflows/mypy.yml/badge.svg)](https://github.com/Teagum/blossom/actions/workflows/mypy.yml)\n[![pylint](https://github.com/Teagum/blossom/actions/workflows/pylint.yml/badge.svg)](https://github.com/Teagum/blossom/actions/workflows/pylint.yml)\n\n# Awesom\nSelf-organizing map framework for Python\n\n\n```python\nimport matplotlib.pyplot as plt\n\nfrom awesom import datasets\nfrom awesom import plot as asp\nfrom awesom.som import IncrementalMap\n\n\nX, y = datasets.norm_circle(5, 500, 1, radius=4)\n\nsom = IncrementalMap((7, 7, X.shape[1]), 100, 0.04, 4)\nsom.fit(X)\n\nfig, ax = plt.subplots(1, 1)\nasp.data_2d(ax, X, y)\nasp.wire(ax, som)\n```\n\n![SOM wire plot](https://user-images.githubusercontent.com/11088297/209104159-958cfbef-15f5-4259-9c15-bfebcb76058e.png "Input dataspce with wire plot")\n',
     'author': 'Michael Blaß',
     'author_email': 'mblass@posteo.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Teagum/awesom',
```

### Comparing `awesom-0.1.2.post1/PKG-INFO` & `awesom-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awesom
-Version: 0.1.2.post1
+Version: 0.1.4
 Summary: Self-organizing map framework for Python
 Home-page: https://github.com/Teagum/awesom
 License: BSD-3-Clause
 Author: Michael Blaß
 Author-email: mblass@posteo.net
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Education
```

