# Comparing `tmp/regularizepsf-0.1.0.tar.gz` & `tmp/regularizepsf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regularizepsf-0.1.0.tar", last modified: Mon Feb  6 00:09:05 2023, max compression
+gzip compressed data, was "regularizepsf-0.2.0.tar", last modified: Fri Apr 21 16:41:13 2023, max compression
```

## Comparing `regularizepsf-0.1.0.tar` & `regularizepsf-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-06 00:09:05.101217 regularizepsf-0.1.0/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1070 2022-10-21 22:04:30.000000 regularizepsf-0.1.0/LICENSE
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2319 2023-02-06 00:09:05.100824 regularizepsf-0.1.0/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1968 2023-02-06 00:07:31.000000 regularizepsf-0.1.0/README.md
--rw-r--r--   0 jhughes  (1624782681) 1567826318      126 2022-12-02 19:38:08.000000 regularizepsf-0.1.0/pyproject.toml
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-06 00:09:05.095062 regularizepsf-0.1.0/regularizepsf/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      204 2022-12-29 00:17:46.000000 regularizepsf-0.1.0/regularizepsf/__init__.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318    11810 2023-02-05 19:10:59.000000 regularizepsf-0.1.0/regularizepsf/corrector.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318      348 2022-10-23 02:35:32.000000 regularizepsf-0.1.0/regularizepsf/exceptions.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318    16787 2023-02-05 23:03:23.000000 regularizepsf-0.1.0/regularizepsf/fitter.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318   400911 2023-02-05 23:05:21.000000 regularizepsf-0.1.0/regularizepsf/helper.c
--rw-r--r--   0 jhughes  (1624782681) 1567826318     4154 2022-11-04 22:29:59.000000 regularizepsf-0.1.0/regularizepsf/helper.pyx
--rw-r--r--   0 jhughes  (1624782681) 1567826318     5529 2022-12-29 00:17:46.000000 regularizepsf-0.1.0/regularizepsf/psf.py
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-06 00:09:05.100025 regularizepsf-0.1.0/regularizepsf.egg-info/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2319 2023-02-06 00:09:05.000000 regularizepsf-0.1.0/regularizepsf.egg-info/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318      399 2023-02-06 00:09:05.000000 regularizepsf-0.1.0/regularizepsf.egg-info/SOURCES.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2023-02-06 00:09:05.000000 regularizepsf-0.1.0/regularizepsf.egg-info/dependency_links.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318      102 2023-02-06 00:09:05.000000 regularizepsf-0.1.0/regularizepsf.egg-info/requires.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       14 2023-02-06 00:09:05.000000 regularizepsf-0.1.0/regularizepsf.egg-info/top_level.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       38 2023-02-06 00:09:05.101344 regularizepsf-0.1.0/setup.cfg
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1111 2023-02-06 00:08:39.000000 regularizepsf-0.1.0/setup.py
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-04-21 16:41:13.188407 regularizepsf-0.2.0/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     1070 2022-10-21 22:04:30.000000 regularizepsf-0.2.0/LICENSE
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     2383 2023-04-21 16:41:13.188075 regularizepsf-0.2.0/PKG-INFO
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     2032 2023-04-21 16:19:55.000000 regularizepsf-0.2.0/README.md
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      924 2023-03-12 01:49:56.000000 regularizepsf-0.2.0/pyproject.toml
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-04-21 16:41:13.182010 regularizepsf-0.2.0/regularizepsf/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      394 2023-04-21 16:34:43.000000 regularizepsf-0.2.0/regularizepsf/__init__.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318    12905 2023-04-21 16:19:55.000000 regularizepsf-0.2.0/regularizepsf/corrector.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      348 2023-03-12 01:59:58.000000 regularizepsf-0.2.0/regularizepsf/exceptions.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318    22919 2023-04-21 16:34:43.000000 regularizepsf-0.2.0/regularizepsf/fitter.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318   413887 2023-04-21 16:41:02.000000 regularizepsf-0.2.0/regularizepsf/helper.c
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     5030 2023-04-21 16:34:43.000000 regularizepsf-0.2.0/regularizepsf/helper.pyx
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     6080 2023-03-12 01:59:58.000000 regularizepsf-0.2.0/regularizepsf/psf.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318    13358 2023-04-21 16:34:43.000000 regularizepsf-0.2.0/regularizepsf/visualize.py
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-04-21 16:41:13.184643 regularizepsf-0.2.0/regularizepsf.egg-info/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     2383 2023-04-21 16:41:13.000000 regularizepsf-0.2.0/regularizepsf.egg-info/PKG-INFO
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      489 2023-04-21 16:41:13.000000 regularizepsf-0.2.0/regularizepsf.egg-info/SOURCES.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2023-04-21 16:41:13.000000 regularizepsf-0.2.0/regularizepsf.egg-info/dependency_links.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      124 2023-04-21 16:41:13.000000 regularizepsf-0.2.0/regularizepsf.egg-info/requires.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318       14 2023-04-21 16:41:13.000000 regularizepsf-0.2.0/regularizepsf.egg-info/top_level.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318       38 2023-04-21 16:41:13.188506 regularizepsf-0.2.0/setup.cfg
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     1139 2023-04-21 16:35:59.000000 regularizepsf-0.2.0/setup.py
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-04-21 16:41:13.187062 regularizepsf-0.2.0/tests/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     8223 2023-04-21 16:19:55.000000 regularizepsf-0.2.0/tests/test_corrector.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     9825 2023-04-21 16:19:55.000000 regularizepsf-0.2.0/tests/test_fitter.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     3845 2023-03-12 01:49:21.000000 regularizepsf-0.2.0/tests/test_psf.py
```

### Comparing `regularizepsf-0.1.0/LICENSE` & `regularizepsf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regularizepsf-0.1.0/regularizepsf/corrector.py` & `regularizepsf-0.2.0/regularizepsf/corrector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 import abc
 from pathlib import Path
-from typing import Any
+from typing import Any, Tuple
 
+import deepdish as dd
 import dill
 import numpy as np
 from numpy.fft import fft2, ifft2, ifftshift
-import deepdish as dd
 
-from regularizepsf.exceptions import InvalidSizeError, EvaluatedModelInconsistentSizeError, UnevaluatedPointError
-from regularizepsf.psf import VariedPSF, SimplePSF, PointSpreadFunctionABC
+from regularizepsf.exceptions import (
+    EvaluatedModelInconsistentSizeError,
+    InvalidSizeError,
+    UnevaluatedPointError,
+)
 from regularizepsf.helper import _correct_image, _precalculate_ffts
+from regularizepsf.psf import PointSpreadFunctionABC, SimplePSF, VariedPSF
 
 
 class CorrectorABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def save(self, path: str | Path) -> None:
         """Save the model to a file.
 
@@ -50,17 +54,19 @@
         """PSF correct an image according to the model
 
         Parameters
         ----------
         image : 2D float np.ndarray
             image to be corrected
         size : int
-            how big to make the patches when correcting an image, only used for FunctionalCorrector
+            how big to make the patches when correcting an image, 
+            only used for FunctionalCorrector
         alpha : float
-            controls the “hardness” of the transition from amplification to attenuation, see notes
+            controls the “hardness” of the transition from amplification 
+            to attenuation, see notes
         epsilon : float
             controls the maximum of the amplification, see notes
 
         Returns
         -------
         np.ndarray
             a image that has been PSF corrected
@@ -81,18 +87,19 @@
             an image with the PSF applied
         """
 
 
 class FunctionalCorrector(CorrectorABC):
     """
     A version of the PSF corrector that stores the model as a set of functions.
-    For the actual correction, the functions must first be evaluated to an ArrayCorrector.
+    For the actual correction, the functions must first 
+    be evaluated to an ArrayCorrector.
     """
     def __init__(self, psf: PointSpreadFunctionABC,
-                 target_model: SimplePSF | None):
+                 target_model: SimplePSF | None) -> None:
         """Initialize a FunctionalCorrector
 
         Parameters
         ----------
         psf : SimplePSF or VariedPSF
             the model describing the psf for each patch of the image
         target_model : SimplePSF or None
@@ -104,19 +111,23 @@
 
     @property
     def is_variable(self) -> bool:
         """
         Returns
         -------
         bool
-            True if the PSF model is varied (changes across the field-of-view) and False otherwise
+            True if the PSF model is varied (changes across the field-of-view) 
+            and False otherwise
         """
         return self._variable
 
-    def evaluate_to_array_form(self, x: np.ndarray, y: np.ndarray, size: int) -> ArrayCorrector:
+    def evaluate_to_array_form(self, 
+                               x: np.ndarray,
+                               y: np.ndarray, 
+                               size: int) -> ArrayCorrector:
         """Evaluates a FunctionalCorrector to an ArrayCorrector
 
         Parameters
         ----------
         x : np.ndarray
             the first dimension coordinates to evaluate over
         y : np.ndarray
@@ -129,38 +140,39 @@
         ArrayCorrector
             an array evaluated form of this PSF corrector
         """
         if size % 2 != 0:
             raise InvalidSizeError(f"size must be even. Found size={size}.")
 
         image_x, image_y = np.meshgrid(np.arange(size), np.arange(size))
-        evaluations = dict()
+        evaluations = {}
         for xx in x:
             for yy in y:
                 evaluations[(xx, yy)] = self._psf(image_x, image_y)
 
-        if self._target_model:
-            target_evaluation = self._target_model(image_x, image_y)
-        else:
-            target_evaluation = np.ones((size, size))
+        target_evaluation = self._target_model(image_x, image_y) if self._target_model else np.ones((size, size))
         return ArrayCorrector(evaluations, target_evaluation)
 
     def correct_image(self, image: np.ndarray, size: int,
                       alpha: float = 0.5, epsilon: float = 0.05) -> np.ndarray:
         corners = calculate_covering(image.shape, size)
-        array_corrector = self.evaluate_to_array_form(corners[:, 0], corners[:, 1], size)
-        return array_corrector.correct_image(image, size=size, alpha=alpha, epsilon=epsilon)
+        array_corrector = self.evaluate_to_array_form(corners[:, 0], 
+                                                      corners[:, 1], size)
+        return array_corrector.correct_image(image, 
+                                             size=size, 
+                                             alpha=alpha, 
+                                             epsilon=epsilon)
 
-    def save(self, path):
-        with open(path, 'wb') as f:
+    def save(self, path: str) -> None:
+        with open(path, "wb") as f:
             dill.dump(self, f)
 
     @classmethod
-    def load(cls, path):
-        with open(path, 'rb') as f:
+    def load(cls, path: str) -> FunctionalCorrector:
+        with open(path, "rb") as f:
             return dill.load(f)
 
 
     def simulate_observation(self, image: np.ndarray, size: int) -> np.ndarray:
         """Simulates on a star field what an observation using this PSF looks like
 
         Parameters
@@ -172,111 +184,130 @@
 
         Returns
         -------
         np.ndarray
             an image with the PSF applied
         """
         corners = calculate_covering(image.shape, size)
-        array_corrector = self.evaluate_to_array_form(corners[:, 0], corners[:, 1], size)
+        array_corrector = self.evaluate_to_array_form(corners[:, 0], 
+                                                      corners[:, 1], 
+                                                      size)
         return array_corrector.simulate_observation(image)
 
 
 class ArrayCorrector(CorrectorABC):
     """ A PSF corrector that is evaluated as array patches
     """
-    def __init__(self, evaluations: dict[Any, np.ndarray], target_evaluation: np.ndarray):
+    def __init__(self, evaluations: dict[Any, np.ndarray], 
+                 target_evaluation: np.ndarray) -> None:
         """Initialize an ArrayCorrector
 
         Parameters
         ----------
         evaluations : dict
-            evaluated version of the PSF as they vary over the image, keys should be (x, y) of the lower left
-                pixel of each patch. values should be the `np.ndarray` that corresponds to that patch
+            evaluated version of the PSF as they vary over the image, 
+                keys should be (x, y) of the lower left
+                pixel of each patch. values should be the `np.ndarray` 
+                that corresponds to that patch
         target_evaluation : np.ndarray
             evaluated version of the target PSF
         """
         self._evaluation_points: list[Any] = list(evaluations.keys())
 
         if not isinstance(evaluations[self._evaluation_points[0]], np.ndarray):
-            raise ValueError(f"Individual evaluations must be numpy arrays. "
+            raise TypeError(f"Individual evaluations must be numpy arrays. "
                              f"Found {type(evaluations[self._evaluation_points[0]])}.")
         if len(evaluations[self._evaluation_points[0]].shape) != 2:
-            raise InvalidSizeError(f"PSF evaluations must be 2-D numpy arrays.")
+            raise InvalidSizeError("PSF evaluations must be 2-D numpy arrays.")
         self._size = evaluations[self._evaluation_points[0]].shape[0]
         if self._size % 2 != 0:
             raise InvalidSizeError(f"Size must be even. Found {self._size}")
 
         self._evaluations: dict[Any, np.ndarray] = evaluations
         for (x, y), evaluation in self._evaluations.items():
             if evaluation.shape != (self._size, self._size):
-                raise EvaluatedModelInconsistentSizeError(f"Expected evaluated model to have shapes of "
-                                                          f"{(self._size, self._size)}. Found {evaluation.shape} "
-                                                          f"at {(x, y)}.")
+                msg = ("Expected evaluated model to have shapes of "
+                       f"{(self._size, self._size)}."
+                       f"Found {evaluation.shape} at {(x, y)}.")
+                raise EvaluatedModelInconsistentSizeError(msg)
 
         self._target_evaluation = target_evaluation
         if self._target_evaluation.shape != (self._size, self._size):
-            raise EvaluatedModelInconsistentSizeError("The target and evaluations must have the same shape.")
+            msg = "The target and evaluations must have the same shape."
+            raise EvaluatedModelInconsistentSizeError(msg)
 
-        values = np.array([v for v in self._evaluations.values()], dtype=float)
-        self.target_fft, self.psf_i_fft = _precalculate_ffts(self._target_evaluation, values)
+        normalized_values = np.array(
+                [v / v.sum() for v in self._evaluations.values()], dtype=float)
+        normalized_target = target_evaluation / target_evaluation.sum()
+        self.target_fft, self.psf_i_fft = _precalculate_ffts(
+                normalized_target, normalized_values)
 
-    def correct_image(self, image: np.ndarray, size: int = None,
+    def correct_image(self, image: np.ndarray, size: int = None,  # noqa: ARG002, size used in FunctionalCorrector
                       alpha: float = 0.5, epsilon: float = 0.05) -> np.ndarray:
-        if not all(img_dim_i >= psf_dim_i for img_dim_i, psf_dim_i in zip(image.shape, (self._size, self._size))):
-            raise InvalidSizeError("The image must be at least as large as the PSFs in all dimensions")
-
-        x = np.array([x for x, _ in self._evaluations.keys()], dtype=int)
-        y = np.array([y for _, y in self._evaluations.keys()], dtype=int)
-
-        return _correct_image(image, self.target_fft, x, y, self.psf_i_fft,  alpha, epsilon)
+        if not all(img_dim_i >= psf_dim_i for img_dim_i, psf_dim_i in zip(image.shape, 
+                                                                          (self._size, 
+                                                                           self._size))):
+            msg = "The image must be at least as large as the PSFs in all dimensions"
+            raise InvalidSizeError(msg)
+
+        x = np.array([x for x, _ in self._evaluations], dtype=int)
+        y = np.array([y for _, y in self._evaluations], dtype=int)
+
+        return _correct_image(image, 
+                              self.target_fft, 
+                              x, y, 
+                              self.psf_i_fft,  alpha, epsilon)
 
-    def __getitem__(self, xy) -> np.ndarray:
+    def __getitem__(self, xy: Tuple[int, int]) -> np.ndarray:
         if xy in self._evaluation_points:
             return self._evaluations[xy]
         else:
             raise UnevaluatedPointError(f"Model not evaluated at {xy}.")
 
-    def save(self, path):
+    def save(self, path: str) -> None:
         dd.io.save(path, (self._evaluations, self._target_evaluation))
 
     @classmethod
-    def load(cls, path):
+    def load(cls, path: str) -> ArrayCorrector:
         evaluations, target_evaluation = dd.io.load(path)
         return cls(evaluations, target_evaluation)
 
     def simulate_observation(self, image: np.ndarray) -> np.ndarray:
         psf_shape = (self._size, self._size)
         pad_shape = psf_shape
         img_shape = image.shape
 
         xarr, yarr = np.meshgrid(np.arange(psf_shape[0]), np.arange(psf_shape[1]))
         apodization_window = np.sin((xarr + 0.5) * (np.pi / psf_shape[0])) * np.sin(
             (yarr + 0.5) * (np.pi / psf_shape[1]))
 
-        img_p = np.pad(image, psf_shape, mode='constant')
+        img_p = np.pad(image, psf_shape, mode="constant")
 
         observation_synthetic = np.zeros(img_shape)
         observation_synthetic_p = np.pad(observation_synthetic, pad_shape)
 
-        def get_img_i(x, y):
-            xs, xe, ys, ye = x + psf_shape[0], x + 2 * psf_shape[0], y + psf_shape[1], y + 2 * psf_shape[1]
+        def get_img_i(x: int, y: int) -> np.ndarray:
+            xs, xe = x + psf_shape[0], x + 2 * psf_shape[0]
+            ys, ye = y + psf_shape[1], y + 2 * psf_shape[1]
             return img_p[xs:xe, ys:ye]
 
-        def set_synthetic_p(x, y, image):
-            xs, xe, ys, ye = x + psf_shape[0], x + 2 * psf_shape[0], y + psf_shape[1], y + 2 * psf_shape[1]
-            observation_synthetic_p[xs:xe, ys:ye] = np.nansum([image, observation_synthetic_p[xs:xe, ys:ye]], axis=0)
+        def set_synthetic_p(x: int, y: int, image: np.ndarray) -> None:
+            xs, xe = x + psf_shape[0], x + 2 * psf_shape[0]
+            ys, ye = y + psf_shape[1], y + 2 * psf_shape[1]
+            observation_synthetic_p[xs:xe, ys:ye] = np.nansum(
+                [image, observation_synthetic_p[xs:xe, ys:ye]], axis=0)
 
         for (x, y), psf_i in self._evaluations.items():
             img_i = get_img_i(x, y)
-            out_i = np.real(ifftshift(ifft2(fft2(img_i * apodization_window) * fft2(psf_i)))) * apodization_window
+            out_i = np.real(ifftshift(ifft2(fft2(img_i * apodization_window) 
+                                            * fft2(psf_i)))) * apodization_window
             set_synthetic_p(x, y, out_i)
 
-        observation = observation_synthetic_p[psf_shape[0]:img_shape[0] + psf_shape[0],
+        return observation_synthetic_p[psf_shape[0]:img_shape[0] + psf_shape[0],
                       psf_shape[1]:img_shape[1] + psf_shape[1]]
-        return observation
 
 
 def calculate_covering(image_shape: tuple[int, int], size: int) -> np.ndarray:
     """Determines the grid of overlapping neighborhood patches.
 
     Parameters
     ----------
@@ -284,15 +315,16 @@
         shape of the image we plan to correct
     size : int
         size of the square patches we want to create
 
     Returns
     -------
     np.ndarray
-        an array of shape Nx2 where return[:, 0] are the x coordinate and return[:, 1] are the y coordinates
+        an array of shape Nx2 where return[:, 0] 
+        are the x coordinate and return[:, 1] are the y coordinates
 
     """
     half_size = np.ceil(size / 2).astype(int)
 
     x1 = np.arange(0, image_shape[0], size)
     y1 = np.arange(0, image_shape[1], size)
```

### Comparing `regularizepsf-0.1.0/regularizepsf/fitter.py` & `regularizepsf-0.2.0/regularizepsf/fitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from __future__ import annotations
 
 import abc
 import warnings
-from typing import Any
 from collections import namedtuple
+from collections.abc import Callable
 from numbers import Real
+from typing import Any, Dict, Generator, List, Optional, Tuple
 
-import numpy as np
 import deepdish as dd
-from lmfit import Parameters, minimize
-from lmfit.minimizer import MinimizerResult
+import numpy as np
 import sep
 from astropy.io import fits
+from lmfit import Parameters, minimize
+from lmfit.minimizer import MinimizerResult
 from scipy.interpolate import RectBivariateSpline
 from skimage.transform import downscale_local_mean
 
-from regularizepsf.psf import SimplePSF, PointSpreadFunctionABC
+from regularizepsf.corrector import ArrayCorrector, calculate_covering
 from regularizepsf.exceptions import InvalidSizeError
-from regularizepsf.corrector import calculate_covering, ArrayCorrector
+from regularizepsf.psf import PointSpreadFunctionABC, SimplePSF
 
 
 class PatchCollectionABC(metaclass=abc.ABCMeta):
-    def __init__(self, patches: dict[Any, np.ndarray]):
-        self._patches = patches
+    def __init__(self, patches: dict[Any, np.ndarray], counts: Optional[dict[Any, int]] = None) -> None:
+        self.patches = patches
+        self.counts = counts
         if patches:
             shape = next(iter(patches.values())).shape
             # TODO: check that the patches are square
-            self._size = shape[0]
+            self.size = shape[0]
         else:
-            self._size = None
+            self.size = None
 
-    def __len__(self):
-        return len(self._patches)
+    def __len__(self) -> int:
+        return len(self.patches)
 
     @classmethod
     @abc.abstractmethod
-    def extract(cls, images: list[np.ndarray], coordinates: list, size: int) -> PatchCollectionABC:
-        """Construct a PatchCollection from a set of images using the specified coordinates and patch size
+    def extract(cls, 
+                images: list[np.ndarray], 
+                coordinates: list, 
+                size: int) -> PatchCollectionABC:
+        """Construct a PatchCollection from a set of images 
+        using the specified coordinates and patch size
 
         Parameters
         ----------
         images : list of np.ndarrays
             the images loaded
         coordinates : list
-            A list of coordinates for the lower left pixel of each patch, specified in each type of PatchCollection
+            A list of coordinates for the lower left pixel of each patch, 
+                specified in each type of PatchCollection
         size : int
             size of one side of the square patches extracted
 
         Returns
         -------
         np.ndarray
             the square patches extracted into a PatchCollection
@@ -55,68 +62,86 @@
 
     def __getitem__(self, identifier: Any) -> np.ndarray:
         """Access a patch with square brackets
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, specifically implemented for each PatchCollection
+            identifier for a given patch, specifically implemented 
+            for each PatchCollection
 
         Returns
         -------
         np.ndarray
             a patch's data
         """
-        if identifier in self._patches:
-            return self._patches[identifier]
+        if identifier in self.patches:
+            return self.patches[identifier]
         else:
-            raise IndexError(f"{identifier} is not used to identify a patch in this collection.")
+            msg = f"{identifier} is not used to identify a patch in this collection."
+            raise IndexError(msg)
 
     def __contains__(self, identifier: Any) -> bool:
         """Determines if a patch is in the collection
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, specifically implemented for each PatchCollection
+            identifier for a given patch, 
+                specifically implemented for each PatchCollection
 
         Returns
         -------
         bool
-            True if patch with specified identifier is in the collection, False otherwise
+            True if patch with specified identifier is in the collection, 
+                False otherwise
         """
-        return identifier in self._patches
+        return identifier in self.patches
 
-    def add(self, identifier: Any, patch: np.ndarray) -> None:
+    def add(self,
+            identifier: Any,
+            patch: np.ndarray,
+            count: Optional[int] = None) -> None:
         """Add a new patch to the collection
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, specifically implemented for each PatchCollection
-
+            identifier for a given patch, 
+                specifically implemented for each PatchCollection
         patch : np.ndarray
             the data for a specific patch
+        count : int
+            Optionally, a corresponding item to add to the `counts` dictionary
 
         Returns
         -------
         None
         """
-        if identifier in self._patches:
+        if identifier in self.patches:
             # TODO: improve warning
-            warnings.warn(f"{identifier} is being overwritten in this collection.", Warning)
-        self._patches[identifier] = patch
+            warnings.warn(f"{identifier} is being overwritten in this collection.",
+                           Warning, stacklevel=2)
+        self.patches[identifier] = patch
 
-        if self._size is None:
-            self._size = patch.shape[0]
+        if count is not None:
+            self.counts[identifier] = count
+
+        if self.size is None:
+            self.size = patch.shape[0]
             # TODO : enforce square constraint
 
     @abc.abstractmethod
-    def average(self, corners: np.ndarray, step: int, size: int, mode: str) -> PatchCollectionABC:
-        """Construct a new PatchCollection where patches lying inside a new grid are averaged together
+    def average(self, 
+                corners: np.ndarray, 
+                step: int, 
+                size: int,
+                mode: str) -> PatchCollectionABC:
+        """Construct a new PatchCollection where patches 
+        lying inside a new grid are averaged together
 
         Parameters
         ----------
         corners : np.ndarray
             an Nx2 `np.ndarray` of the lower left corners of the new patch grid
         step : int
             how far apart each corner patch is
@@ -128,15 +153,17 @@
         Returns
         -------
         PatchCollectionABC
             a PatchCollection where data is sampled at the new grid
         """
 
     @abc.abstractmethod
-    def fit(self, base_psf: SimplePSF, is_varied: bool = False) -> PointSpreadFunctionABC:
+    def fit(self, 
+            base_psf: SimplePSF, 
+            is_varied: bool = False) -> PointSpreadFunctionABC:
         """
 
         Parameters
         ----------
         base_psf
         is_varied
 
@@ -153,49 +180,47 @@
         path : str
             where to save the patch collection
 
         Returns
         -------
         None
         """
-        dd.io.save(path, self._patches)
+        dd.io.save(path, self.patches)
 
     @classmethod
-    def load(cls, path) -> PatchCollectionABC:
+    def load(cls, path: str) -> PatchCollectionABC:
         """Load a PatchCollection from a file
 
         Parameters
         ----------
         path : str
             file path to load from
 
         Returns
         -------
         PatchCollectionABC
             the new patch collection
         """
         return cls(dd.io.load(path))
 
-    def keys(self):
+    def keys(self) -> List:
         """Gets identifiers for all patches"""
-        return self._patches.keys()
+        return self.patches.keys()
 
-    def values(self):
+    def values(self) -> List:
         """Gets values of all patches"""
-        return self._patches.values()
+        return self.patches.values()
 
-    def items(self):
+    def items(self) -> Dict:
         """A dictionary like iterator over the patches"""
-        return self._patches.items()
-
-    def __next__(self):
-        # TODO: implement
-        pass
+        return self.patches.items()
 
-    def _fit_lmfit(self, base_psf: SimplePSF, initial_guesses: dict[str, Real]) -> dict[Any, MinimizerResult]:
+    def _fit_lmfit(self, 
+                   base_psf: SimplePSF, 
+                   initial_guesses: dict[str, Real]) -> dict[Any, MinimizerResult]:
         """Fit a patch using lmfit
 
         Parameters
         ----------
         base_psf : SimplePSF
             the PSF model to use in fitting
         initial_guesses : dict[str, Real]
@@ -206,206 +231,325 @@
         dict
             keys are the identifiers, values are the `MinimizerResults` from lmfit
         """
         initial = Parameters()
         for parameter in base_psf.parameters:
             initial.add(parameter, value=initial_guesses[parameter])
 
-        xx, yy = np.meshgrid(np.arange(self._size), np.arange(self._size))
+        xx, yy = np.meshgrid(np.arange(self.size), np.arange(self.size))
 
-        results = dict()
-        for identifier, patch in self._patches.items():
+        results = {}
+        for identifier, patch in self.patches.items():
             results[identifier] = minimize(
-                lambda current_parameters, x, y, data: data - base_psf(x, y, **current_parameters.valuesdict()),
+                lambda current_parameters, x, y, data:
+                    data - base_psf(x, y, **current_parameters.valuesdict()),
                 initial,
                 args=(xx, yy, patch))
         return results
 
 
 CoordinateIdentifier = namedtuple("CoordinateIdentifier", "image_index, x, y")
 
 
 class CoordinatePatchCollection(PatchCollectionABC):
-    """A representation of a PatchCollection that operates on pixel coordinates from a set of images"""
+    """A representation of a PatchCollection that operates 
+    on pixel coordinates from a set of images"""
     @classmethod
     def extract(cls, images: list[np.ndarray],
                 coordinates: list[CoordinateIdentifier],
                 size: int) -> PatchCollectionABC:
-        out = cls(dict())
+        out = cls({})
 
         # pad in case someone selects a region on the edge of the image
         padding_shape = ((size, size), (size, size))
-        padded_images = [np.pad(image, padding_shape, mode='constant') for image in images]
+        padded_images = [np.pad(image, padding_shape, mode="constant") 
+                         for image in images]
 
         # TODO: prevent someone from selecting a region completing outside of the image
         for coordinate in coordinates:
             patch = padded_images[coordinate.image_index][coordinate.x+size:coordinate.x+2*size,
                                                           coordinate.y+size:coordinate.y+2*size]
             out.add(coordinate, patch)
         return out
 
     @classmethod
-    def find_stars_and_average(cls, image_paths: list[str],
+    def find_stars_and_average(cls, 
+                               images: list[str] | np.ndarray | Generator,
                                psf_size: int,
                                patch_size: int,
                                interpolation_scale: int = 1,
                                average_mode: str = "median",
-                               star_threshold: int = 3, hdu_choice=0):
-        """Loads a series of images, finds stars in each, and builds a CoordinatePatchCollection with averaged stars
+                               percentile: float = 10,
+                               star_threshold: int = 3,
+                               star_mask: Optional[list[str] | np.ndarray | Generator] = None,
+                               hdu_choice: int=0) -> CoordinatePatchCollection:
+        """Loads a series of images, finds stars in each, 
+            and builds a CoordinatePatchCollection with averaged stars
 
         Parameters
         ----------
-        image_paths : List[str]
-            location of FITS files to load
+        images : List[str] or np.ndarray or Generator
+            The images to be processed. Can be a list of FITS filenames, a
+            numpy array of shape (n_images, ny, nx), or a Generator that yields
+            each data array in turn.
         psf_size : int
             size of the PSF model to use
         patch_size : int
             square size that each PSF model applies to
         interpolation_scale : int
-            if >1, the image are first scaled by this factor. This results in stars being aligned at a subpixel scale
+            if >1, the image are first scaled by this factor. 
+                This results in stars being aligned at a subpixel scale
         average_mode : str
-            "median" or "mean" determines how patches are combined
+            "median", "percentile", or "mean": determines how patches are
+            combined
+        percentile : float
+            If `average_mode` is `"percentile"`, use this percentile value
+            (from 0 to 100)
         star_threshold : int
-            SEP's threshold for finding stars. See `threshold` in https://sep.readthedocs.io/en/v1.1.x/api/sep.extract.html#sep-extract
+            SEP's threshold for finding stars. See `threshold`
+                in https://sep.readthedocs.io/en/v1.1.x/api/sep.extract.html#sep-extract
+        star_mask : List[str] or np.ndarray or Generator
+            Masks to apply during star-finding. Can be a list of FITS filenames, a
+            numpy array of shape (n_images, ny, nx), or a Generator that yields
+            each mask array in turn. Where the mask pixel is `True`, the
+            corresponding data array pixel will not be selected as a star. See
+            `mask` in
+            https://sep.readthedocs.io/en/v1.1.x/api/sep.extract.html#sep-extract
+            for more details.
         hdu_choice : int
-            Which HDU from each image will be used, default of 0 is most common but could be 1 for compressed images
+            Which HDU from each image will be used, 
+                default of 0 is most common but could be 1 for compressed images
 
         Returns
         -------
         CoordinatePatchCollection
             An averaged star model built from the provided images
 
         Notes
         ------
-        Using an `interpolation_scale` other than 1 for large images can dramatically slow down the execution.
+        Using an `interpolation_scale` other than 1 
+            for large images can dramatically slow down the execution.
         """
-        # Load the first image to determine the image shape, assumed to be the same for all images
-        with fits.open(image_paths[0]) as hdul:
-            image_shape = hdul[hdu_choice].data.shape
+        if isinstance(images, Generator):
+            data_iterator = images
+        elif isinstance(images, np.ndarray):
+            if len(images.shape) == 3:
+                def generator():
+                    for image in images:
+                        yield image
+                data_iterator = generator()
+            else:
+                raise ValueError("Image data array must be 3D")
+        elif isinstance(images, List) and isinstance(images[0], str):
+            def generator():
+                for image_path in images:
+                    with fits.open(image_path) as hdul:
+                        yield hdul[hdu_choice].data.astype(float)
+            data_iterator = generator()
+        else:
+            raise ValueError("Unsupported type for `images`")
+
+        if star_mask is None:
+            def generator():
+                while True:
+                    yield None
+            star_mask_iterator = generator()
+        elif isinstance(star_mask, Generator):
+            star_mask_iterator = star_mask
+        elif isinstance(star_mask, np.ndarray):
+            if len(star_mask.shape) == 3:
+                def generator():
+                    for mask in star_mask:
+                        yield mask
+                star_mask_iterator = generator()
+            else:
+                raise ValueError("Star mask array must be 3D")
+        elif isinstance(star_mask, List) and isinstance(star_mask[0], str):
+            def generator():
+                for mask_path in star_mask:
+                    with fits.open(mask_path) as hdul:
+                        yield hdul[hdu_choice].data.astype(bool)
+            star_mask_iterator = generator()
+        else:
+            raise ValueError("Unsupported type for `star_mask`")
 
         # the output collection to return
-        this_collection = cls(dict())
+        this_collection = cls({})
+
+        # We'll store the first image's shape, and then make sure the others
+        # match.
+        image_shape = None
 
         # for each image do the magic
-        for i, image_path in enumerate(image_paths):
-            with fits.open(image_path) as hdul:
-                image = hdul[hdu_choice].data.astype(float)
-            if image.shape != image_shape:
-                raise ValueError(f"Images must all be the same shape. Found both {image_shape} and {image.shape}.")
+        for i, (image, star_mask) in enumerate(zip(data_iterator, star_mask_iterator)):
+            if image_shape is None:
+                image_shape = image.shape
+            elif image.shape != image_shape:
+                msg = ("Images must all be the same shape."
+                      f"Found both {image_shape} and {image.shape}.")
+                raise ValueError(msg)
 
             # if the image should be scaled then, do the scaling before anything else
             if interpolation_scale != 1:
-                interpolator = RectBivariateSpline(np.arange(image.shape[0]), np.arange(image.shape[1]), image)
-                image = interpolator(np.linspace(0, image.shape[0], image.shape[0] * interpolation_scale),
-                                     np.linspace(0, image.shape[1], image.shape[1] * interpolation_scale))
+                interpolator = RectBivariateSpline(np.arange(image.shape[0]), 
+                                                   np.arange(image.shape[1]), 
+                                                   image)
+                image = interpolator(np.linspace(0,
+                                                 image.shape[0] - 1,
+                                                 1 + (image.shape[0] - 1) * interpolation_scale),
+                                     np.linspace(0,
+                                                 image.shape[1] - 1,
+                                                 1 + (image.shape[1] - 1) * interpolation_scale))
 
             # find stars using SEP
             background = sep.Background(image)
             image_background_removed = image - background
-            image_star_coords = sep.extract(image_background_removed, star_threshold, err=background.globalrms)
+            image_star_coords = sep.extract(image_background_removed, 
+                                            star_threshold, 
+                                            err=background.globalrms,
+                                            mask=star_mask)
 
             coordinates = [CoordinateIdentifier(i,
-                                                int(y - psf_size * interpolation_scale / 2),
-                                                int(x - psf_size * interpolation_scale / 2))
-                           for x, y in zip(image_star_coords['x'], image_star_coords['y'])]
+                                                int(round(y - psf_size * interpolation_scale / 2)),
+                                                int(round(x - psf_size * interpolation_scale / 2)))
+                           for x, y in zip(image_star_coords["x"], image_star_coords["y"])]
 
             # pad in case someone selects a region on the edge of the image
             padding_shape = ((psf_size * interpolation_scale, psf_size * interpolation_scale),
                              (psf_size * interpolation_scale, psf_size * interpolation_scale))
-            padded_image = np.pad(image, padding_shape, mode='constant', constant_values=np.median(image))
+            padded_image = np.pad(image_background_removed,
+                                  padding_shape, 
+                                  mode="constant", 
+                                  constant_values=np.median(image))
 
             for coordinate in coordinates:
                 patch = padded_image[coordinate.x+interpolation_scale*psf_size:
                                      coordinate.x+2*interpolation_scale*psf_size,
                                      coordinate.y + interpolation_scale * psf_size:
                                      coordinate.y + 2 * interpolation_scale * psf_size]
                 this_collection.add(coordinate, patch)
 
-        corners = calculate_covering((image_shape[0] * interpolation_scale, image_shape[1] * interpolation_scale),
-                                     patch_size * interpolation_scale)
-        averaged = this_collection.average(corners, patch_size * interpolation_scale, psf_size * interpolation_scale,
-                                           mode=average_mode)
+        corners = calculate_covering((image_shape[0] * interpolation_scale, 
+                                      image_shape[1] * interpolation_scale),
+                                      patch_size * interpolation_scale)
+        averaged = this_collection.average(corners, 
+                                           patch_size * interpolation_scale, psf_size * interpolation_scale,
+                                           mode=average_mode, percentile=percentile)
 
         if interpolation_scale != 1:
-            for coordinate, patch in averaged.items():
-                averaged._patches[coordinate] = downscale_local_mean(averaged._patches[coordinate],
-                                                                     (interpolation_scale, interpolation_scale))
+            for coordinate, _ in averaged.items():
+                averaged.patches[coordinate] = downscale_local_mean(averaged.patches[coordinate],
+                                                                    (interpolation_scale, interpolation_scale))
 
-            averaged._size = psf_size
+            averaged.size = psf_size
 
-        output = CoordinatePatchCollection(dict())
+        output = CoordinatePatchCollection({}, counts={})
         for key, patch in averaged.items():
-            output._patches[CoordinateIdentifier(key.image_index, key.x // interpolation_scale, key.y // interpolation_scale)] = patch
+            count = averaged.counts[key]
+            output.add(CoordinateIdentifier(key.image_index,
+                                            key.x // interpolation_scale,
+                                            key.y // interpolation_scale),
+                       patch,
+                       count=count)
 
         return output
 
-    def average(self, corners: np.ndarray, patch_size: int, psf_size: int,
-                mode: str = "median") -> PatchCollectionABC:
-        CoordinatePatchCollection._validate_average_mode(mode)
-        pad_shape = self._calculate_pad_shape(patch_size)
+    def average(self, corners: np.ndarray, patch_size: int, psf_size: int,  # noqa: ARG002, kept for consistency
+                mode: str = "median", percentile: float = 10) -> PatchCollectionABC:
+        CoordinatePatchCollection._validate_average_mode(mode, percentile)
 
         if mode == "mean":
-            mean_stack = {tuple(corner): np.zeros((patch_size, patch_size)) for corner in corners}
-            counts = {tuple(corner): 0 for corner in corners}
-        elif mode == "median":
-            median_stack = {tuple(corner): [] for corner in corners}
+            mean_stack = {tuple(corner): np.zeros((psf_size, psf_size))
+                          for corner in corners}
+            mean_counts = {tuple(corner): np.zeros((psf_size, psf_size))
+                          for corner in corners}
+        else:
+            # n.b. If mode is 'median', we could set mode='percentile'
+            # and percentile=50 to simplify parts of this function, but
+            # np.nanpercentile(x, 50) seems to be about half as fast as
+            # np.nanmedian(x), so let's keep a speedy special case for medians.
+            stack = {tuple(corner): [] for corner in corners}
+        counts = {tuple(corner): 0 for corner in corners}
 
         corners_x, corners_y = corners[:, 0], corners[:, 1]
         x_bounds = np.stack([corners_x, corners_x + patch_size], axis=-1)
         y_bounds = np.stack([corners_y, corners_y + patch_size], axis=-1)
 
-        for identifier, patch in self._patches.items():
-            # pad patch with zeros
-            padded_patch = np.pad(patch / np.max(patch), pad_shape, mode='constant')
+        for identifier, patch in self.patches.items():
+            # Normalize the patch
+            patch = patch / np.max(patch)
 
             # Determine which average region it belongs to
-            center_x = identifier.x + self._size // 2
-            center_y = identifier.y + self._size // 2
+            center_x = identifier.x + self.size // 2
+            center_y = identifier.y + self.size // 2
             x_matches = (x_bounds[:, 0] <= center_x) * (center_x < x_bounds[:, 1])
             y_matches = (y_bounds[:, 0] <= center_y) * (center_y < y_bounds[:, 1])
             match_indices = np.where(x_matches * y_matches)[0]
 
             # add to averages and increment count
             for match_index in match_indices:
                 match_corner = tuple(corners[match_index])
                 if mode == "mean":
-                    mean_stack[match_corner] = np.nansum([mean_stack[match_corner], padded_patch], axis=0)
-                    counts[match_corner] += 1
-                elif mode == "median":
-                    median_stack[match_corner].append(padded_patch)
+                    mean_stack[match_corner] = np.nansum([mean_stack[match_corner], 
+                                                          patch], axis=0)
+                    mean_counts[match_corner] += np.isfinite(patch)
+                else:
+                    stack[match_corner].append(patch)
+                counts[match_corner] += 1
 
         if mode == "mean":
-            averages = {CoordinateIdentifier(None, corner[0], corner[1]): mean_stack[corner]/counts[corner]
+            averages = {CoordinateIdentifier(None, corner[0], corner[1]): 
+                        mean_stack[corner] / mean_counts[corner]
                         for corner in mean_stack}
         elif mode == "median":
             averages = {CoordinateIdentifier(None, corner[0], corner[1]):
-                            np.nanmedian(median_stack[corner], axis=0)
-                                if len(median_stack[corner]) > 0 else np.zeros((patch_size, patch_size))
-                        for corner in median_stack}
-        return CoordinatePatchCollection(averages)
+                            np.nanmedian(stack[corner], axis=0)
+                                if len(stack[corner]) > 0 else
+                                np.zeros((psf_size, psf_size))
+                        for corner in stack}
+        elif mode == "percentile":
+            averages = {CoordinateIdentifier(None, corner[0], corner[1]):
+                            np.nanpercentile(stack[corner],
+                                             percentile,
+                                             axis=0)
+                                if len(stack[corner]) > 0 else
+                                np.zeros((psf_size, psf_size))
+                        for corner in stack}
+        counts = {CoordinateIdentifier(None, corner[0], corner[1]): count
+                  for corner, count in counts.items()}
+        # Now that we have our combined patches, pad them as appropriate
+        pad_shape = self._calculate_pad_shape(patch_size)
+        for key, patch in averages.items():
+            averages[key] = np.pad(patch, pad_shape, mode="constant")
+        return CoordinatePatchCollection(averages, counts=counts)
 
     @staticmethod
-    def _validate_average_mode(mode: str):
+    def _validate_average_mode(mode: str, percentile: float) -> None:
         """Determine if the average_mode is a valid kind"""
-        valid_modes = ['median', 'mean']
+        valid_modes = ["median", "mean", "percentile"]
         if mode not in valid_modes:
-            raise ValueError(f"Found a mode of {mode} but it must be in the list {valid_modes}.")
+            msg = f"Found a mode of {mode} but it must be in the list {valid_modes}."
+            raise ValueError(msg)
+        if mode == "percentile" and not (0 <= percentile <= 100):
+            raise ValueError("`percentile` must be between 0 and 100, inclusive")
 
-    def _calculate_pad_shape(self, size):
-        pad_amount = size - self._size
+    def _calculate_pad_shape(self, size: int) -> Tuple[int, int]:
+        pad_amount = size - self.size
         if pad_amount < 0:
             raise InvalidSizeError(f"The average window size (found {size})" 
-                                   f"must be larger than the existing patch size (found {self._size}).")
+                                   "must be larger than the existing patch size"
+                                   f"(found {self.size}).")
         if pad_amount % 2 != 0:
             raise InvalidSizeError(f"The average window size (found {size})" 
-                                   f"must be the same parity as the existing patch size (found {self._size}).")
-        pad_shape = ((pad_amount//2, pad_amount//2), (pad_amount//2, pad_amount//2))
-        return pad_shape
+                                   "must be the same parity as the existing patch size"
+                                   f"(found {self.size}).")
+        return ((pad_amount//2, pad_amount//2), (pad_amount//2, pad_amount//2))
 
-    def fit(self, base_psf: SimplePSF, is_varied: bool = False) -> PointSpreadFunctionABC:
+    def fit(self, base_psf: SimplePSF, 
+            is_varied: bool = False) -> PointSpreadFunctionABC:
         raise NotImplementedError("TODO")
 
     def to_array_corrector(self, target_evaluation: np.array) -> ArrayCorrector:
         """Converts a patch collection that has been averaged into an ArrayCorrector
 
         Parameters
         ----------
@@ -413,16 +557,15 @@
             the evaluation of the Target PSF
 
         Returns
         -------
         ArrayCorrector
             An array corrector that can be used to correct PSFs
         """
-        evaluation_dictionary = dict()
-        for identifier, patch in self._patches.items():
+        evaluation_dictionary = {}
+        for identifier, patch in self.patches.items():
             corrected_patch = patch.copy()
             corrected_patch[np.isnan(corrected_patch)] = 0
             evaluation_dictionary[(identifier.x, identifier.y)] = corrected_patch
 
-        array_corrector = ArrayCorrector(evaluation_dictionary, target_evaluation)
-        return array_corrector
+        return ArrayCorrector(evaluation_dictionary, target_evaluation)
```

### Comparing `regularizepsf-0.1.0/regularizepsf/helper.c` & `regularizepsf-0.2.0/regularizepsf/helper.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.32 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/core/include"
+            "/Users/jhughes/Desktop/repos/regularizepsf/venv/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "regularizepsf.helper",
         "sources": [
             "regularizepsf/helper.pyx"
         ]
     },
     "module_name": "regularizepsf.helper"
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,15 +105,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -570,35 +570,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_READY(op)       (0)
+  #if defined(PyUnicode_IS_READY)
+  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                              0 : _PyUnicode_Ready((PyObject *)(op)))
   #else
-    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #define __Pyx_PyUnicode_READY(op)       (0)
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
   #else
-    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-    #else
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-    #endif
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1001,16 +1001,16 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
   "regularizepsf/helper.pyx",
-  "__init__.pxd",
-  "type.pxd",
+  "venv/lib/python3.10/site-packages/numpy/__init__.pxd",
+  "venv/lib/python3.10/site-packages/Cython/Includes/cpython/type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
@@ -1041,195 +1041,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1265,42 +1265,42 @@
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1424,26 +1424,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
+#define __Pyx_GetModuleGlobalName(var, name)  {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
+}
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
+}
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1689,42 +1689,14 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* BufferStructDeclare.proto */
-typedef struct {
-  Py_ssize_t shape, strides, suboffsets;
-} __Pyx_Buf_DimInfo;
-typedef struct {
-  size_t refcount;
-  Py_buffer pybuffer;
-} __Pyx_Buffer;
-typedef struct {
-  __Pyx_Buffer *rcbuffer;
-  char *data;
-  __Pyx_Buf_DimInfo diminfo[8];
-} __Pyx_LocalBuf_ND;
-
-#if PY_MAJOR_VERSION < 3
-    static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags);
-    static void __Pyx_ReleaseBuffer(Py_buffer *view);
-#else
-    #define __Pyx_GetBuffer PyObject_GetBuffer
-    #define __Pyx_ReleaseBuffer PyBuffer_Release
-#endif
-
-
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
     #define __Pyx_CREAL(z) (__real__(z))
@@ -1777,17 +1749,50 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* BufferStructDeclare.proto */
+typedef struct {
+  Py_ssize_t shape, strides, suboffsets;
+} __Pyx_Buf_DimInfo;
+typedef struct {
+  size_t refcount;
+  Py_buffer pybuffer;
+} __Pyx_Buffer;
+typedef struct {
+  __Pyx_Buffer *rcbuffer;
+  char *data;
+  __Pyx_Buf_DimInfo diminfo[8];
+} __Pyx_LocalBuf_ND;
+
+#if PY_MAJOR_VERSION < 3
+    static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags);
+    static void __Pyx_ReleaseBuffer(Py_buffer *view);
+#else
+    #define __Pyx_GetBuffer PyObject_GetBuffer
+    #define __Pyx_ReleaseBuffer PyBuffer_Release
+#endif
+
+
 /* FromPy.proto */
 static __pyx_t_double_complex __Pyx_PyComplex_As___pyx_t_double_complex(PyObject*);
 
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* ToPy.proto */
+#define __pyx_PyComplex_FromComplex(z)\
+        PyComplex_FromDoubles((double)__Pyx_CREAL(z),\
+                              (double)__Pyx_CIMAG(z))
+
 /* Arithmetic.proto */
 #if CYTHON_CCOMPLEX
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
@@ -1892,26 +1897,30 @@
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'regularizepsf.helper' */
 static PyObject *__pyx_f_13regularizepsf_6helper__correct_image(PyArrayObject *, PyArrayObject *, PyArrayObject *, PyArrayObject *, PyArrayObject *, float, float, int __pyx_skip_dispatch); /*proto*/
+static __pyx_t_double_complex __pyx_f_13regularizepsf_6helper__regularize_value(__pyx_t_double_complex, float, float, __pyx_t_double_complex, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_13regularizepsf_6helper__regularize_array(PyArrayObject *, float, float, PyArrayObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_13regularizepsf_6helper__precalculate_ffts(PyArrayObject *, PyArrayObject *, int __pyx_skip_dispatch); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float_t = { "float_t", NULL, sizeof(__pyx_t_5numpy_float_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo___pyx_t_double_complex = { "double complex", NULL, sizeof(__pyx_t_double_complex), { 0 }, 0, 'C', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t = { "DTYPE_t", NULL, sizeof(__pyx_t_13regularizepsf_6helper_DTYPE_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "regularizepsf.helper"
 extern int __pyx_module_is_main_regularizepsf__helper;
 int __pyx_module_is_main_regularizepsf__helper = 0;
 
 /* Implementation of 'regularizepsf.helper' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ImportError;
+static const char __pyx_k_A[] = "A";
+static const char __pyx_k_P[] = "P";
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k_y[] = "y";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_pi[] = "pi";
 static const char __pyx_k_pad[] = "pad";
 static const char __pyx_k_sin[] = "sin";
 static const char __pyx_k_fft2[] = "fft2";
@@ -1919,47 +1928,45 @@
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_real[] = "real";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_alpha[] = "alpha";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
-static const char __pyx_k_float[] = "float";
 static const char __pyx_k_ifft2[] = "ifft2";
 static const char __pyx_k_image[] = "image";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_square[] = "square";
 static const char __pyx_k_values[] = "values";
-static const char __pyx_k_complex[] = "complex";
 static const char __pyx_k_epsilon[] = "epsilon";
 static const char __pyx_k_constant[] = "constant";
 static const char __pyx_k_meshgrid[] = "meshgrid";
 static const char __pyx_k_numpy_fft[] = "numpy.fft";
 static const char __pyx_k_target_fft[] = "target_fft";
 static const char __pyx_k_values_fft[] = "values_fft";
 static const char __pyx_k_zeros_like[] = "zeros_like";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_target_evaluation[] = "target_evaluation";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static PyObject *__pyx_n_s_A;
 static PyObject *__pyx_n_s_ImportError;
+static PyObject *__pyx_n_s_P;
 static PyObject *__pyx_n_s_alpha;
 static PyObject *__pyx_n_s_arange;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_complex;
 static PyObject *__pyx_n_u_constant;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_epsilon;
 static PyObject *__pyx_n_s_fft2;
-static PyObject *__pyx_n_s_float;
 static PyObject *__pyx_n_s_ifft2;
 static PyObject *__pyx_n_s_image;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_meshgrid;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
@@ -1979,15 +1986,17 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_s_values_fft;
 static PyObject *__pyx_n_s_x;
 static PyObject *__pyx_n_s_y;
 static PyObject *__pyx_n_s_zeros_like;
 static PyObject *__pyx_pf_13regularizepsf_6helper__correct_image(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_image, PyArrayObject *__pyx_v_target_fft, PyArrayObject *__pyx_v_x, PyArrayObject *__pyx_v_y, PyArrayObject *__pyx_v_values_fft, float __pyx_v_alpha, float __pyx_v_epsilon); /* proto */
-static PyObject *__pyx_pf_13regularizepsf_6helper_2_precalculate_ffts(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_target_evaluation, PyArrayObject *__pyx_v_values); /* proto */
+static PyObject *__pyx_pf_13regularizepsf_6helper_2_regularize_value(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_double_complex __pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, __pyx_t_double_complex __pyx_v_P); /* proto */
+static PyObject *__pyx_pf_13regularizepsf_6helper_4_regularize_array(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, PyArrayObject *__pyx_v_P); /* proto */
+static PyObject *__pyx_pf_13regularizepsf_6helper_6_precalculate_ffts(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_target_evaluation, PyArrayObject *__pyx_v_values); /* proto */
 static PyObject *__pyx_float_0_5;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 /* Late includes */
 
 /* "regularizepsf/helper.pyx":11
  * @cython.wraparound(False)
@@ -2010,15 +2019,14 @@
   int __pyx_v_this_x_prime;
   int __pyx_v_this_y_prime;
   PyArrayObject *__pyx_v_img_i = 0;
   CYTHON_UNUSED PyArrayObject *__pyx_v_psf_i = 0;
   PyArrayObject *__pyx_v_corrected_i = 0;
   PyArrayObject *__pyx_v_padded_img = 0;
   PyArrayObject *__pyx_v_result_img = 0;
-  float __pyx_v_psf_i_hat_abs;
   PyArrayObject *__pyx_v_psf_i_hat_norm = 0;
   PyArrayObject *__pyx_v_img_i_hat = 0;
   PyArrayObject *__pyx_v_temp = 0;
   PyArrayObject *__pyx_v_apodization_window = 0;
   PyObject *__pyx_v_xarr = NULL;
   PyObject *__pyx_v_yarr = NULL;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_apodization_window;
@@ -2051,18 +2059,18 @@
   __Pyx_Buffer __pyx_pybuffer_y;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
+  PyArrayObject *__pyx_t_5 = NULL;
   PyArrayObject *__pyx_t_6 = NULL;
   PyArrayObject *__pyx_t_7 = NULL;
-  PyArrayObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   PyArrayObject *__pyx_t_9 = NULL;
   PyArrayObject *__pyx_t_10 = NULL;
   PyArrayObject *__pyx_t_11 = NULL;
   PyArrayObject *__pyx_t_12 = NULL;
   PyArrayObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
@@ -2195,27 +2203,27 @@
   __pyx_v_size = (__pyx_v_values_fft->dimensions[1]);
 
   /* "regularizepsf/helper.pyx":21
  *     cdef int num_evaluations = x.shape[0]
  *     cdef int size = values_fft.shape[1]
  *     cdef int i = 0, j=0, xx = 0, yy = 0             # <<<<<<<<<<<<<<
  *     cdef int this_x, this_y, this_x_prime, this_y_prime
- *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=float)
  */
   __pyx_v_i = 0;
   __pyx_v_j = 0;
   __pyx_v_xx = 0;
   __pyx_v_yy = 0;
 
   /* "regularizepsf/helper.pyx":23
  *     cdef int i = 0, j=0, xx = 0, yy = 0
  *     cdef int this_x, this_y, this_x_prime, this_y_prime
- *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=np.float)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
@@ -2233,101 +2241,89 @@
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 23, __pyx_L1_error)
-  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_5 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_img_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_img_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_img_i = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_img_i.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 23, __pyx_L1_error)
     } else {__pyx_pybuffernd_img_i.diminfo[0].strides = __pyx_pybuffernd_img_i.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_img_i.diminfo[0].shape = __pyx_pybuffernd_img_i.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_img_i.diminfo[1].strides = __pyx_pybuffernd_img_i.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_img_i.diminfo[1].shape = __pyx_pybuffernd_img_i.rcbuffer->pybuffer.shape[1];
     }
   }
-  __pyx_t_6 = 0;
-  __pyx_v_img_i = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
+  __pyx_v_img_i = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "regularizepsf/helper.pyx":24
  *     cdef int this_x, this_y, this_x_prime, this_y_prime
- *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
-  __pyx_t_5 = 0;
+  __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psf_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psf_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_psf_i = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psf_i.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 24, __pyx_L1_error)
     } else {__pyx_pybuffernd_psf_i.diminfo[0].strides = __pyx_pybuffernd_psf_i.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_psf_i.diminfo[0].shape = __pyx_pybuffernd_psf_i.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_psf_i.diminfo[1].strides = __pyx_pybuffernd_psf_i.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_psf_i.diminfo[1].shape = __pyx_pybuffernd_psf_i.rcbuffer->pybuffer.shape[1];
     }
   }
-  __pyx_t_7 = 0;
+  __pyx_t_6 = 0;
   __pyx_v_psf_i = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "regularizepsf/helper.pyx":25
- *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),
  *                                                          mode="constant")
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -2347,116 +2343,110 @@
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_corrected_i = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 25, __pyx_L1_error)
     } else {__pyx_pybuffernd_corrected_i.diminfo[0].strides = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_corrected_i.diminfo[0].shape = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_corrected_i.diminfo[1].strides = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_corrected_i.diminfo[1].shape = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.shape[1];
     }
   }
-  __pyx_t_8 = 0;
-  __pyx_v_corrected_i = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_t_7 = 0;
+  __pyx_v_corrected_i = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "regularizepsf/helper.pyx":26
- *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),             # <<<<<<<<<<<<<<
  *                                                          mode="constant")
- *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_pad); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_pad); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
-  __pyx_t_5 = 0;
+  __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
-  __pyx_t_3 = 0;
-  __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
-  __pyx_t_2 = 0;
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1);
+  __pyx_t_3 = 0;
   __pyx_t_1 = 0;
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_8);
+  __pyx_t_2 = 0;
+  __pyx_t_8 = 0;
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(((PyObject *)__pyx_v_image));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_image));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_image));
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
-  __pyx_t_5 = 0;
+  PyTuple_SET_ITEM(__pyx_t_8, 0, ((PyObject *)__pyx_v_image));
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "regularizepsf/helper.pyx":27
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),
  *                                                          mode="constant")             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)
  *     cdef float psf_i_hat_abs
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_mode, __pyx_n_u_constant) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_mode, __pyx_n_u_constant) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
 
   /* "regularizepsf/helper.pyx":26
- *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)
- *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),             # <<<<<<<<<<<<<<
  *                                                          mode="constant")
- *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_padded_img.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_padded_img = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_padded_img.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 26, __pyx_L1_error)
@@ -2466,99 +2456,87 @@
   __pyx_t_9 = 0;
   __pyx_v_padded_img = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "regularizepsf/helper.pyx":28
  *     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),
  *                                                          mode="constant")
- *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)             # <<<<<<<<<<<<<<
  *     cdef float psf_i_hat_abs
- *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=np.complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=complex)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros_like); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros_like); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_v_padded_img));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_padded_img));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_padded_img));
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_10 = ((PyArrayObject *)__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_result_img.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_result_img = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_result_img.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 28, __pyx_L1_error)
     } else {__pyx_pybuffernd_result_img.diminfo[0].strides = __pyx_pybuffernd_result_img.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_result_img.diminfo[0].shape = __pyx_pybuffernd_result_img.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_result_img.diminfo[1].strides = __pyx_pybuffernd_result_img.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_result_img.diminfo[1].shape = __pyx_pybuffernd_result_img.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_10 = 0;
-  __pyx_v_result_img = ((PyArrayObject *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_v_result_img = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
 
   /* "regularizepsf/helper.pyx":30
- *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)
+ *     cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)
  *     cdef float psf_i_hat_abs
- *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=np.complex)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=np.complex)
- *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=np.complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=complex)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=complex)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
-  __pyx_t_3 = 0;
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+  __pyx_t_4 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyComplex_Type))) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 30, __pyx_L1_error)
   __pyx_t_11 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_psf_i_hat_norm = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 30, __pyx_L1_error)
@@ -2567,112 +2545,100 @@
   }
   __pyx_t_11 = 0;
   __pyx_v_psf_i_hat_norm = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "regularizepsf/helper.pyx":31
  *     cdef float psf_i_hat_abs
- *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=np.complex)
- *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=np.complex)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=np.complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=complex)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=complex)
  *     cdef np.ndarray[np.float_t, ndim=2] apodization_window
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
   __pyx_t_4 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
+  __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, ((PyObject *)(&PyComplex_Type))) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_t_12 = ((PyArrayObject *)__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_12 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer, (PyObject*)__pyx_t_12, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_img_i_hat = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 31, __pyx_L1_error)
     } else {__pyx_pybuffernd_img_i_hat.diminfo[0].strides = __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_img_i_hat.diminfo[0].shape = __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_img_i_hat.diminfo[1].strides = __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_img_i_hat.diminfo[1].shape = __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_12 = 0;
-  __pyx_v_img_i_hat = ((PyArrayObject *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_v_img_i_hat = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
 
   /* "regularizepsf/helper.pyx":32
- *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=np.complex)
- *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=np.complex)
- *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=np.complex)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=complex)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float_t, ndim=2] apodization_window
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
-  __pyx_t_3 = 0;
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+  __pyx_t_4 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyComplex_Type))) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 32, __pyx_L1_error)
   __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 32, __pyx_L1_error)
@@ -2686,62 +2652,62 @@
   /* "regularizepsf/helper.pyx":36
  * 
  * 
  *     xarr, yarr = np.meshgrid(np.arange(size), np.arange(size))             # <<<<<<<<<<<<<<
  *     apodization_window = np.square(np.sin((xarr + 0.5) * (np.pi / size))) * np.square(np.sin((yarr + 0.5) * (np.pi / size)))
  *     apodization_window = np.sin((xarr + 0.5) * (np.pi / size)) * np.sin((yarr + 0.5) * (np.pi / size))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_meshgrid); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_meshgrid); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_14);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_14, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
+  __pyx_t_1 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_14, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_arange); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_arange); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_1);
+  __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = NULL;
   __pyx_t_16 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_2);
@@ -2751,116 +2717,116 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_16 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_5, __pyx_t_3};
+    PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_1, __pyx_t_3};
     __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_5, __pyx_t_3};
+    PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_1, __pyx_t_3};
     __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_14) {
-      __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_14); __pyx_t_14 = NULL;
+      __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_14); __pyx_t_14 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_16, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_16, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_16, __pyx_t_3);
-    __pyx_t_5 = 0;
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_16, __pyx_t_3);
+    __pyx_t_1 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
     PyObject* sequence = __pyx_t_4;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
       __PYX_ERR(0, 36, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
+      __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
-      __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
+      __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_8);
     #else
     __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     #endif
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else {
     Py_ssize_t index = -1;
     __pyx_t_3 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_17 = Py_TYPE(__pyx_t_3)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_17(__pyx_t_3); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
-    index = 1; __pyx_t_1 = __pyx_t_17(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L3_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_1);
+    index = 1; __pyx_t_8 = __pyx_t_17(__pyx_t_3); if (unlikely(!__pyx_t_8)) goto __pyx_L3_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_8);
     if (__Pyx_IternextUnpackEndCheck(__pyx_t_17(__pyx_t_3), 2) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
     __pyx_t_17 = NULL;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_17 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 36, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_xarr = __pyx_t_2;
   __pyx_t_2 = 0;
-  __pyx_v_yarr = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_v_yarr = __pyx_t_8;
+  __pyx_t_8 = 0;
 
   /* "regularizepsf/helper.pyx":37
  * 
  *     xarr, yarr = np.meshgrid(np.arange(size), np.arange(size))
  *     apodization_window = np.square(np.sin((xarr + 0.5) * (np.pi / size))) * np.square(np.sin((yarr + 0.5) * (np.pi / size)))             # <<<<<<<<<<<<<<
  *     apodization_window = np.sin((xarr + 0.5) * (np.pi / size)) * np.sin((yarr + 0.5) * (np.pi / size))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_square); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_square); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyFloat_AddObjC(__pyx_v_xarr, __pyx_float_0_5, 0.5, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_pi); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
@@ -2872,50 +2838,50 @@
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = PyNumber_Multiply(__pyx_t_3, __pyx_t_18); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __pyx_t_18 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_5);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_18)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_18);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_18) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_18, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_14);
+  __pyx_t_8 = (__pyx_t_18) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_18, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_14);
   __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_5)) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_square); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_square); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_sin); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_t_14 = __Pyx_PyFloat_AddObjC(__pyx_v_yarr, __pyx_float_0_5, 0.5, 0, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
@@ -2940,42 +2906,42 @@
     if (likely(__pyx_t_19)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_18);
       __Pyx_INCREF(__pyx_t_19);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_18, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_19) ? __Pyx_PyObject_Call2Args(__pyx_t_18, __pyx_t_19, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_18, __pyx_t_3);
+  __pyx_t_8 = (__pyx_t_19) ? __Pyx_PyObject_Call2Args(__pyx_t_18, __pyx_t_19, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_18, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __pyx_t_18 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_5);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_18)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_18);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_18) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_18, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1);
+  __pyx_t_2 = (__pyx_t_18) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_18, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Multiply(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_Multiply(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 37, __pyx_L1_error)
-  __pyx_t_20 = ((PyArrayObject *)__pyx_t_5);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_20 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_apodization_window.rcbuffer->pybuffer);
     __pyx_t_16 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_apodization_window.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_16 < 0)) {
       PyErr_Fetch(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_apodization_window.rcbuffer->pybuffer, (PyObject*)__pyx_v_apodization_window, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
@@ -2986,16 +2952,16 @@
       }
       __pyx_t_21 = __pyx_t_22 = __pyx_t_23 = 0;
     }
     __pyx_pybuffernd_apodization_window.diminfo[0].strides = __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_apodization_window.diminfo[0].shape = __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_apodization_window.diminfo[1].strides = __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_apodization_window.diminfo[1].shape = __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.shape[1];
     if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
   }
   __pyx_t_20 = 0;
-  __pyx_v_apodization_window = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_v_apodization_window = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "regularizepsf/helper.pyx":38
  *     xarr, yarr = np.meshgrid(np.arange(size), np.arange(size))
  *     apodization_window = np.square(np.sin((xarr + 0.5) * (np.pi / size))) * np.square(np.sin((yarr + 0.5) * (np.pi / size)))
  *     apodization_window = np.sin((xarr + 0.5) * (np.pi / size)) * np.sin((yarr + 0.5) * (np.pi / size))             # <<<<<<<<<<<<<<
  * 
  *     for i in range(num_evaluations):
@@ -3003,66 +2969,66 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyFloat_AddObjC(__pyx_v_xarr, __pyx_float_0_5, 0.5, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_pi); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_pi); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_18, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_18, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1);
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_sin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyFloat_AddObjC(__pyx_v_yarr, __pyx_float_0_5, 0.5, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyFloat_AddObjC(__pyx_v_yarr, __pyx_float_0_5, 0.5, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_19 = __Pyx_PyNumber_Divide(__pyx_t_18, __pyx_t_2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_19);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_19); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_8, __pyx_t_19); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
   __pyx_t_19 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_19)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_19);
@@ -3072,17 +3038,17 @@
   }
   __pyx_t_4 = (__pyx_t_19) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_19, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_t_20 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_apodization_window.rcbuffer->pybuffer);
     __pyx_t_16 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_apodization_window.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
@@ -3199,26 +3165,26 @@
  *                 img_i[xx, yy] = apodization_window[xx, yy] * padded_img[this_x_prime + xx, this_y_prime + yy]
  *         img_i_hat = fft2(img_i)             # <<<<<<<<<<<<<<
  * 
  *         for xx in range(size):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_fft2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = NULL;
+    __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_5)) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((PyObject *)__pyx_v_img_i)) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)__pyx_v_img_i));
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, ((PyObject *)__pyx_v_img_i)) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)__pyx_v_img_i));
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 50, __pyx_L1_error)
     __pyx_t_12 = ((PyArrayObject *)__pyx_t_3);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
@@ -3242,91 +3208,87 @@
     __pyx_t_3 = 0;
 
     /* "regularizepsf/helper.pyx":52
  *         img_i_hat = fft2(img_i)
  * 
  *         for xx in range(size):             # <<<<<<<<<<<<<<
  *             for yy in range(size):
- *                 psf_i_hat_abs = abs(values_fft[i, xx, yy])
+ *                 psf_i_hat_norm[xx, yy] = _regularize_value(
  */
     __pyx_t_27 = __pyx_v_size;
     __pyx_t_28 = __pyx_t_27;
     for (__pyx_t_29 = 0; __pyx_t_29 < __pyx_t_28; __pyx_t_29+=1) {
       __pyx_v_xx = __pyx_t_29;
 
       /* "regularizepsf/helper.pyx":53
  * 
  *         for xx in range(size):
  *             for yy in range(size):             # <<<<<<<<<<<<<<
- *                 psf_i_hat_abs = abs(values_fft[i, xx, yy])
- *                 psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))
+ *                 psf_i_hat_norm[xx, yy] = _regularize_value(
+ *                         values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])
  */
       __pyx_t_30 = __pyx_v_size;
       __pyx_t_31 = __pyx_t_30;
       for (__pyx_t_32 = 0; __pyx_t_32 < __pyx_t_31; __pyx_t_32+=1) {
         __pyx_v_yy = __pyx_t_32;
 
-        /* "regularizepsf/helper.pyx":54
- *         for xx in range(size):
+        /* "regularizepsf/helper.pyx":55
  *             for yy in range(size):
- *                 psf_i_hat_abs = abs(values_fft[i, xx, yy])             # <<<<<<<<<<<<<<
- *                 psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))
+ *                 psf_i_hat_norm[xx, yy] = _regularize_value(
+ *                         values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])             # <<<<<<<<<<<<<<
  *                 temp[xx, yy] = img_i_hat[xx, yy] * psf_i_hat_norm[xx, yy] * target_fft[xx, yy]
+ *         corrected_i = np.real(ifft2(temp))
  */
         __pyx_t_35 = __pyx_v_i;
         __pyx_t_34 = __pyx_v_xx;
         __pyx_t_33 = __pyx_v_yy;
-        __pyx_v_psf_i_hat_abs = __Pyx_c_abs_double((*__Pyx_BufPtrStrided3d(__pyx_t_double_complex *, __pyx_pybuffernd_values_fft.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_values_fft.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_values_fft.diminfo[1].strides, __pyx_t_33, __pyx_pybuffernd_values_fft.diminfo[2].strides)));
+        __pyx_t_26 = __pyx_v_xx;
+        __pyx_t_37 = __pyx_v_yy;
 
-        /* "regularizepsf/helper.pyx":55
+        /* "regularizepsf/helper.pyx":54
+ *         for xx in range(size):
  *             for yy in range(size):
- *                 psf_i_hat_abs = abs(values_fft[i, xx, yy])
- *                 psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))             # <<<<<<<<<<<<<<
+ *                 psf_i_hat_norm[xx, yy] = _regularize_value(             # <<<<<<<<<<<<<<
+ *                         values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])
  *                 temp[xx, yy] = img_i_hat[xx, yy] * psf_i_hat_norm[xx, yy] * target_fft[xx, yy]
- *         corrected_i = np.real(ifft2(temp))
  */
-        __pyx_t_33 = __pyx_v_i;
-        __pyx_t_34 = __pyx_v_xx;
-        __pyx_t_35 = __pyx_v_yy;
-        __pyx_t_26 = __pyx_v_xx;
-        __pyx_t_37 = __pyx_v_yy;
         __pyx_t_36 = __pyx_v_xx;
         __pyx_t_38 = __pyx_v_yy;
-        *__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_psf_i_hat_norm.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_psf_i_hat_norm.diminfo[1].strides) = __Pyx_c_prod_double(__Pyx_c_quot_double(__Pyx_c_conj_double((*__Pyx_BufPtrStrided3d(__pyx_t_double_complex *, __pyx_pybuffernd_values_fft.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_values_fft.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_values_fft.diminfo[1].strides, __pyx_t_35, __pyx_pybuffernd_values_fft.diminfo[2].strides))), __pyx_t_double_complex_from_parts(__pyx_v_psf_i_hat_abs, 0)), __pyx_t_double_complex_from_parts((((double)powf(__pyx_v_psf_i_hat_abs, __pyx_v_alpha)) / (pow(((double)__pyx_v_psf_i_hat_abs), (__pyx_v_alpha + 1.0)) + pow((__pyx_v_epsilon * __Pyx_c_abs_double((*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_target_fft.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_target_fft.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_target_fft.diminfo[1].strides)))), (__pyx_v_alpha + 1.0)))), 0));
+        *__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_psf_i_hat_norm.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_psf_i_hat_norm.diminfo[1].strides) = __pyx_f_13regularizepsf_6helper__regularize_value((*__Pyx_BufPtrStrided3d(__pyx_t_double_complex *, __pyx_pybuffernd_values_fft.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_values_fft.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_values_fft.diminfo[1].strides, __pyx_t_33, __pyx_pybuffernd_values_fft.diminfo[2].strides)), __pyx_v_alpha, __pyx_v_epsilon, (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_target_fft.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_target_fft.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_target_fft.diminfo[1].strides)), 0);
 
         /* "regularizepsf/helper.pyx":56
- *                 psf_i_hat_abs = abs(values_fft[i, xx, yy])
- *                 psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))
+ *                 psf_i_hat_norm[xx, yy] = _regularize_value(
+ *                         values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])
  *                 temp[xx, yy] = img_i_hat[xx, yy] * psf_i_hat_norm[xx, yy] * target_fft[xx, yy]             # <<<<<<<<<<<<<<
  *         corrected_i = np.real(ifft2(temp))
  * 
  */
         __pyx_t_37 = __pyx_v_xx;
         __pyx_t_26 = __pyx_v_yy;
-        __pyx_t_35 = __pyx_v_xx;
-        __pyx_t_34 = __pyx_v_yy;
         __pyx_t_33 = __pyx_v_xx;
+        __pyx_t_34 = __pyx_v_yy;
+        __pyx_t_35 = __pyx_v_xx;
         __pyx_t_38 = __pyx_v_yy;
         __pyx_t_36 = __pyx_v_xx;
         __pyx_t_39 = __pyx_v_yy;
-        *__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_temp.diminfo[0].strides, __pyx_t_39, __pyx_pybuffernd_temp.diminfo[1].strides) = __Pyx_c_prod_double(__Pyx_c_prod_double((*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_img_i_hat.diminfo[0].strides, __pyx_t_26, __pyx_pybuffernd_img_i_hat.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_psf_i_hat_norm.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_psf_i_hat_norm.diminfo[1].strides))), (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_target_fft.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_target_fft.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_target_fft.diminfo[1].strides)));
+        *__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_temp.diminfo[0].strides, __pyx_t_39, __pyx_pybuffernd_temp.diminfo[1].strides) = __Pyx_c_prod_double(__Pyx_c_prod_double((*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_img_i_hat.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_img_i_hat.diminfo[0].strides, __pyx_t_26, __pyx_pybuffernd_img_i_hat.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_psf_i_hat_norm.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_psf_i_hat_norm.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_psf_i_hat_norm.diminfo[1].strides))), (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_target_fft.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_target_fft.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_target_fft.diminfo[1].strides)));
       }
     }
 
     /* "regularizepsf/helper.pyx":57
- *                 psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))
+ *                         values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])
  *                 temp[xx, yy] = img_i_hat[xx, yy] * psf_i_hat_norm[xx, yy] * target_fft[xx, yy]
  *         corrected_i = np.real(ifft2(temp))             # <<<<<<<<<<<<<<
  * 
  *         # add the corrected_i to the array
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_real); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_real); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ifft2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_19 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_19)) {
@@ -3338,49 +3300,49 @@
     }
     __pyx_t_4 = (__pyx_t_19) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_19, ((PyObject *)__pyx_v_temp)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_temp));
     __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
     if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
+    __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 57, __pyx_L1_error)
-    __pyx_t_8 = ((PyArrayObject *)__pyx_t_3);
+    __pyx_t_7 = ((PyArrayObject *)__pyx_t_3);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer);
-      __pyx_t_27 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
+      __pyx_t_27 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
       if (unlikely(__pyx_t_27 < 0)) {
         PyErr_Fetch(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrected_i.rcbuffer->pybuffer, (PyObject*)__pyx_v_corrected_i, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_23); Py_XDECREF(__pyx_t_22); Py_XDECREF(__pyx_t_21);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_23, __pyx_t_22, __pyx_t_21);
         }
         __pyx_t_23 = __pyx_t_22 = __pyx_t_21 = 0;
       }
       __pyx_pybuffernd_corrected_i.diminfo[0].strides = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_corrected_i.diminfo[0].shape = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_corrected_i.diminfo[1].strides = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_corrected_i.diminfo[1].shape = __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.shape[1];
       if (unlikely(__pyx_t_27 < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
     }
-    __pyx_t_8 = 0;
+    __pyx_t_7 = 0;
     __Pyx_DECREF_SET(__pyx_v_corrected_i, ((PyArrayObject *)__pyx_t_3));
     __pyx_t_3 = 0;
 
     /* "regularizepsf/helper.pyx":60
  * 
  *         # add the corrected_i to the array
  *         for xx in range(size):             # <<<<<<<<<<<<<<
@@ -3408,49 +3370,49 @@
  *         for xx in range(size):
  *             for yy in range(size):
  *                 result_img[this_x_prime+xx, this_y_prime+yy] = result_img[this_x_prime+xx, this_y_prime+yy] + (corrected_i[xx, yy] * apodization_window[xx, yy])             # <<<<<<<<<<<<<<
  * 
  *     return result_img[2 * size:image.shape[0] + 2 * size, 2 * size:image.shape[1] + 2 * size]
  */
         __pyx_t_38 = (__pyx_v_this_x_prime + __pyx_v_xx);
-        __pyx_t_33 = (__pyx_v_this_y_prime + __pyx_v_yy);
+        __pyx_t_35 = (__pyx_v_this_y_prime + __pyx_v_yy);
         __pyx_t_34 = __pyx_v_xx;
-        __pyx_t_35 = __pyx_v_yy;
+        __pyx_t_33 = __pyx_v_yy;
         __pyx_t_26 = __pyx_v_xx;
         __pyx_t_37 = __pyx_v_yy;
         __pyx_t_39 = (__pyx_v_this_x_prime + __pyx_v_xx);
         __pyx_t_36 = (__pyx_v_this_y_prime + __pyx_v_yy);
-        *__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_result_img.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_result_img.diminfo[0].strides, __pyx_t_36, __pyx_pybuffernd_result_img.diminfo[1].strides) = ((*__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_result_img.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_result_img.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_result_img.diminfo[1].strides)) + ((*__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_corrected_i.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_corrected_i.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_apodization_window.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_apodization_window.diminfo[1].strides))));
+        *__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_result_img.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_result_img.diminfo[0].strides, __pyx_t_36, __pyx_pybuffernd_result_img.diminfo[1].strides) = ((*__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_result_img.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_result_img.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_result_img.diminfo[1].strides)) + ((*__Pyx_BufPtrStrided2d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_corrected_i.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_corrected_i.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_corrected_i.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_apodization_window.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_apodization_window.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_apodization_window.diminfo[1].strides))));
       }
     }
   }
 
   /* "regularizepsf/helper.pyx":64
  *                 result_img[this_x_prime+xx, this_y_prime+yy] = result_img[this_x_prime+xx, this_y_prime+yy] + (corrected_i[xx, yy] * apodization_window[xx, yy])
  * 
  *     return result_img[2 * size:image.shape[0] + 2 * size, 2 * size:image.shape[1] + 2 * size]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_3 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_long(((__pyx_v_image->dimensions[0]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PySlice_New(__pyx_t_3, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(((__pyx_v_image->dimensions[0]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = PySlice_New(__pyx_t_3, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyInt_From_long(((__pyx_v_image->dimensions[1]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PySlice_New(__pyx_t_5, __pyx_t_3, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_2 = PySlice_New(__pyx_t_1, __pyx_t_3, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
@@ -3473,15 +3435,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_18);
   __Pyx_XDECREF(__pyx_t_19);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
@@ -3762,20 +3724,560 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "regularizepsf/helper.pyx":70
  * @cython.wraparound(False)
  * @cython.cdivision(True)
+ * cpdef complex _regularize_value(             # <<<<<<<<<<<<<<
+ *         complex A,
+ *         float alpha,
+ */
+
+static PyObject *__pyx_pw_13regularizepsf_6helper_3_regularize_value(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static __pyx_t_double_complex __pyx_f_13regularizepsf_6helper__regularize_value(__pyx_t_double_complex __pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, __pyx_t_double_complex __pyx_v_P, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  float __pyx_v_A_abs;
+  __pyx_t_double_complex __pyx_v_R_A;
+  __pyx_t_double_complex __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_regularize_value", 0);
+
+  /* "regularizepsf/helper.pyx":76
+ *         complex P):
+ *     """Implements Eqn (6) of Hughes et al. (2023) for one Fourier-space pixel"""
+ *     cdef float A_abs = abs(A)             # <<<<<<<<<<<<<<
+ *     cdef complex R_A = (A.conjugate() / A_abs) * (A_abs**alpha / (A_abs**(alpha+1.0) + (epsilon * abs(P))**(alpha+1.0)))
+ *     return R_A
+ */
+  __pyx_v_A_abs = __Pyx_c_abs_double(__pyx_v_A);
+
+  /* "regularizepsf/helper.pyx":77
+ *     """Implements Eqn (6) of Hughes et al. (2023) for one Fourier-space pixel"""
+ *     cdef float A_abs = abs(A)
+ *     cdef complex R_A = (A.conjugate() / A_abs) * (A_abs**alpha / (A_abs**(alpha+1.0) + (epsilon * abs(P))**(alpha+1.0)))             # <<<<<<<<<<<<<<
+ *     return R_A
+ * 
+ */
+  __pyx_v_R_A = __Pyx_c_prod_double(__Pyx_c_quot_double(__Pyx_c_conj_double(__pyx_v_A), __pyx_t_double_complex_from_parts(__pyx_v_A_abs, 0)), __pyx_t_double_complex_from_parts((((double)powf(__pyx_v_A_abs, __pyx_v_alpha)) / (pow(((double)__pyx_v_A_abs), (__pyx_v_alpha + 1.0)) + pow((__pyx_v_epsilon * __Pyx_c_abs_double(__pyx_v_P)), (__pyx_v_alpha + 1.0)))), 0));
+
+  /* "regularizepsf/helper.pyx":78
+ *     cdef float A_abs = abs(A)
+ *     cdef complex R_A = (A.conjugate() / A_abs) * (A_abs**alpha / (A_abs**(alpha+1.0) + (epsilon * abs(P))**(alpha+1.0)))
+ *     return R_A             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_R_A;
+  goto __pyx_L0;
+
+  /* "regularizepsf/helper.pyx":70
+ * @cython.wraparound(False)
+ * @cython.cdivision(True)
+ * cpdef complex _regularize_value(             # <<<<<<<<<<<<<<
+ *         complex A,
+ *         float alpha,
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13regularizepsf_6helper_3_regularize_value(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_13regularizepsf_6helper_2_regularize_value[] = "Implements Eqn (6) of Hughes et al. (2023) for one Fourier-space pixel";
+static PyObject *__pyx_pw_13regularizepsf_6helper_3_regularize_value(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __pyx_t_double_complex __pyx_v_A;
+  float __pyx_v_alpha;
+  float __pyx_v_epsilon;
+  __pyx_t_double_complex __pyx_v_P;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_regularize_value (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_A,&__pyx_n_s_alpha,&__pyx_n_s_epsilon,&__pyx_n_s_P,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_A)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_alpha)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_value", 1, 4, 4, 1); __PYX_ERR(0, 70, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_epsilon)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_value", 1, 4, 4, 2); __PYX_ERR(0, 70, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_P)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_value", 1, 4, 4, 3); __PYX_ERR(0, 70, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_regularize_value") < 0)) __PYX_ERR(0, 70, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+    }
+    __pyx_v_A = __Pyx_PyComplex_As___pyx_t_double_complex(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L3_error)
+    __pyx_v_alpha = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_alpha == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
+    __pyx_v_epsilon = __pyx_PyFloat_AsFloat(values[2]); if (unlikely((__pyx_v_epsilon == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
+    __pyx_v_P = __Pyx_PyComplex_As___pyx_t_double_complex(values[3]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("_regularize_value", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 70, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("regularizepsf.helper._regularize_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_13regularizepsf_6helper_2_regularize_value(__pyx_self, __pyx_v_A, __pyx_v_alpha, __pyx_v_epsilon, __pyx_v_P);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13regularizepsf_6helper_2_regularize_value(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_double_complex __pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, __pyx_t_double_complex __pyx_v_P) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __pyx_t_double_complex __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_regularize_value", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_13regularizepsf_6helper__regularize_value(__pyx_v_A, __pyx_v_alpha, __pyx_v_epsilon, __pyx_v_P, 0);
+  __pyx_t_2 = __pyx_PyComplex_FromComplex(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("regularizepsf.helper._regularize_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "regularizepsf/helper.pyx":84
+ * @cython.wraparound(False)
+ * @cython.cdivision(True)
+ * cpdef _regularize_array(             # <<<<<<<<<<<<<<
+ *         np.ndarray[np.complex128_t, ndim=2] A,
+ *         float alpha,
+ */
+
+static PyObject *__pyx_pw_13regularizepsf_6helper_5_regularize_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_13regularizepsf_6helper__regularize_array(PyArrayObject *__pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, PyArrayObject *__pyx_v_P, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  int __pyx_v_size;
+  PyArrayObject *__pyx_v_output = 0;
+  int __pyx_v_xx;
+  int __pyx_v_yy;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_A;
+  __Pyx_Buffer __pyx_pybuffer_A;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_P;
+  __Pyx_Buffer __pyx_pybuffer_P;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_output;
+  __Pyx_Buffer __pyx_pybuffer_output;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyArrayObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  Py_ssize_t __pyx_t_13;
+  Py_ssize_t __pyx_t_14;
+  Py_ssize_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  Py_ssize_t __pyx_t_17;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_regularize_array", 0);
+  __pyx_pybuffer_output.pybuffer.buf = NULL;
+  __pyx_pybuffer_output.refcount = 0;
+  __pyx_pybuffernd_output.data = NULL;
+  __pyx_pybuffernd_output.rcbuffer = &__pyx_pybuffer_output;
+  __pyx_pybuffer_A.pybuffer.buf = NULL;
+  __pyx_pybuffer_A.refcount = 0;
+  __pyx_pybuffernd_A.data = NULL;
+  __pyx_pybuffernd_A.rcbuffer = &__pyx_pybuffer_A;
+  __pyx_pybuffer_P.pybuffer.buf = NULL;
+  __pyx_pybuffer_P.refcount = 0;
+  __pyx_pybuffernd_P.data = NULL;
+  __pyx_pybuffernd_P.rcbuffer = &__pyx_pybuffer_P;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_A.rcbuffer->pybuffer, (PyObject*)__pyx_v_A, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_A.diminfo[0].strides = __pyx_pybuffernd_A.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_A.diminfo[0].shape = __pyx_pybuffernd_A.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_A.diminfo[1].strides = __pyx_pybuffernd_A.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_A.diminfo[1].shape = __pyx_pybuffernd_A.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_P.rcbuffer->pybuffer, (PyObject*)__pyx_v_P, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_P.diminfo[0].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_P.diminfo[0].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_P.diminfo[1].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_P.diminfo[1].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[1];
+
+  /* "regularizepsf/helper.pyx":90
+ *         np.ndarray[np.complex128_t, ndim=2] P):
+ *     """Loops _regularize_value across a 2D array"""
+ *     cdef int size = A.shape[1]             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.complex128_t, ndim=2] output = np.empty((size, size), dtype=complex)
+ * 
+ */
+  __pyx_v_size = (__pyx_v_A->dimensions[1]);
+
+  /* "regularizepsf/helper.pyx":91
+ *     """Loops _regularize_value across a 2D array"""
+ *     cdef int size = A.shape[1]
+ *     cdef np.ndarray[np.complex128_t, ndim=2] output = np.empty((size, size), dtype=complex)             # <<<<<<<<<<<<<<
+ * 
+ *     for xx in range(size):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
+  __pyx_t_1 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, ((PyObject *)(&PyComplex_Type))) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_5 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+      __pyx_v_output = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_output.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 91, __pyx_L1_error)
+    } else {__pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_output.diminfo[1].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_output.diminfo[1].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[1];
+    }
+  }
+  __pyx_t_5 = 0;
+  __pyx_v_output = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "regularizepsf/helper.pyx":93
+ *     cdef np.ndarray[np.complex128_t, ndim=2] output = np.empty((size, size), dtype=complex)
+ * 
+ *     for xx in range(size):             # <<<<<<<<<<<<<<
+ *         for yy in range(size):
+ *             output[xx, yy] = _regularize_value(A[xx, yy], alpha, epsilon, P[xx, yy])
+ */
+  __pyx_t_6 = __pyx_v_size;
+  __pyx_t_7 = __pyx_t_6;
+  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
+    __pyx_v_xx = __pyx_t_8;
+
+    /* "regularizepsf/helper.pyx":94
+ * 
+ *     for xx in range(size):
+ *         for yy in range(size):             # <<<<<<<<<<<<<<
+ *             output[xx, yy] = _regularize_value(A[xx, yy], alpha, epsilon, P[xx, yy])
+ *     return output
+ */
+    __pyx_t_9 = __pyx_v_size;
+    __pyx_t_10 = __pyx_t_9;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+      __pyx_v_yy = __pyx_t_11;
+
+      /* "regularizepsf/helper.pyx":95
+ *     for xx in range(size):
+ *         for yy in range(size):
+ *             output[xx, yy] = _regularize_value(A[xx, yy], alpha, epsilon, P[xx, yy])             # <<<<<<<<<<<<<<
+ *     return output
+ * 
+ */
+      __pyx_t_12 = __pyx_v_xx;
+      __pyx_t_13 = __pyx_v_yy;
+      __pyx_t_14 = __pyx_v_xx;
+      __pyx_t_15 = __pyx_v_yy;
+      __pyx_t_16 = __pyx_v_xx;
+      __pyx_t_17 = __pyx_v_yy;
+      *__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_output.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_output.diminfo[1].strides) = __pyx_f_13regularizepsf_6helper__regularize_value((*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_A.diminfo[0].strides, __pyx_t_13, __pyx_pybuffernd_A.diminfo[1].strides)), __pyx_v_alpha, __pyx_v_epsilon, (*__Pyx_BufPtrStrided2d(__pyx_t_double_complex *, __pyx_pybuffernd_P.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_P.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_P.diminfo[1].strides)), 0);
+    }
+  }
+
+  /* "regularizepsf/helper.pyx":96
+ *         for yy in range(size):
+ *             output[xx, yy] = _regularize_value(A[xx, yy], alpha, epsilon, P[xx, yy])
+ *     return output             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_output));
+  __pyx_r = ((PyObject *)__pyx_v_output);
+  goto __pyx_L0;
+
+  /* "regularizepsf/helper.pyx":84
+ * @cython.wraparound(False)
+ * @cython.cdivision(True)
+ * cpdef _regularize_array(             # <<<<<<<<<<<<<<
+ *         np.ndarray[np.complex128_t, ndim=2] A,
+ *         float alpha,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_A.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("regularizepsf.helper._regularize_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_A.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_output);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13regularizepsf_6helper_5_regularize_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_13regularizepsf_6helper_4_regularize_array[] = "Loops _regularize_value across a 2D array";
+static PyObject *__pyx_pw_13regularizepsf_6helper_5_regularize_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyArrayObject *__pyx_v_A = 0;
+  float __pyx_v_alpha;
+  float __pyx_v_epsilon;
+  PyArrayObject *__pyx_v_P = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_regularize_array (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_A,&__pyx_n_s_alpha,&__pyx_n_s_epsilon,&__pyx_n_s_P,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_A)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_alpha)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_array", 1, 4, 4, 1); __PYX_ERR(0, 84, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_epsilon)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_array", 1, 4, 4, 2); __PYX_ERR(0, 84, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_P)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_regularize_array", 1, 4, 4, 3); __PYX_ERR(0, 84, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_regularize_array") < 0)) __PYX_ERR(0, 84, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+    }
+    __pyx_v_A = ((PyArrayObject *)values[0]);
+    __pyx_v_alpha = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_alpha == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_epsilon = __pyx_PyFloat_AsFloat(values[2]); if (unlikely((__pyx_v_epsilon == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L3_error)
+    __pyx_v_P = ((PyArrayObject *)values[3]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("_regularize_array", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 84, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("regularizepsf.helper._regularize_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_A), __pyx_ptype_5numpy_ndarray, 1, "A", 0))) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_P), __pyx_ptype_5numpy_ndarray, 1, "P", 0))) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13regularizepsf_6helper_4_regularize_array(__pyx_self, __pyx_v_A, __pyx_v_alpha, __pyx_v_epsilon, __pyx_v_P);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13regularizepsf_6helper_4_regularize_array(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_A, float __pyx_v_alpha, float __pyx_v_epsilon, PyArrayObject *__pyx_v_P) {
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_A;
+  __Pyx_Buffer __pyx_pybuffer_A;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_P;
+  __Pyx_Buffer __pyx_pybuffer_P;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_regularize_array", 0);
+  __pyx_pybuffer_A.pybuffer.buf = NULL;
+  __pyx_pybuffer_A.refcount = 0;
+  __pyx_pybuffernd_A.data = NULL;
+  __pyx_pybuffernd_A.rcbuffer = &__pyx_pybuffer_A;
+  __pyx_pybuffer_P.pybuffer.buf = NULL;
+  __pyx_pybuffer_P.refcount = 0;
+  __pyx_pybuffernd_P.data = NULL;
+  __pyx_pybuffernd_P.rcbuffer = &__pyx_pybuffer_P;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_A.rcbuffer->pybuffer, (PyObject*)__pyx_v_A, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_A.diminfo[0].strides = __pyx_pybuffernd_A.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_A.diminfo[0].shape = __pyx_pybuffernd_A.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_A.diminfo[1].strides = __pyx_pybuffernd_A.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_A.diminfo[1].shape = __pyx_pybuffernd_A.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_P.rcbuffer->pybuffer, (PyObject*)__pyx_v_P, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_P.diminfo[0].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_P.diminfo[0].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_P.diminfo[1].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_P.diminfo[1].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[1];
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_13regularizepsf_6helper__regularize_array(__pyx_v_A, __pyx_v_alpha, __pyx_v_epsilon, __pyx_v_P, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_A.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("regularizepsf.helper._regularize_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_A.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "regularizepsf/helper.pyx":102
+ * @cython.wraparound(False)
+ * @cython.cdivision(True)
  * cpdef _precalculate_ffts(np.ndarray[DTYPE_t, ndim=2] target_evaluation, np.ndarray[DTYPE_t, ndim=3] values):             # <<<<<<<<<<<<<<
  *     cdef int size = values.shape[1]
  *     cdef int num_patches = values.shape[0]
  */
 
-static PyObject *__pyx_pw_13regularizepsf_6helper_3_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_13regularizepsf_6helper_7_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_13regularizepsf_6helper__precalculate_ffts(PyArrayObject *__pyx_v_target_evaluation, PyArrayObject *__pyx_v_values, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_size;
   int __pyx_v_num_patches;
   PyArrayObject *__pyx_v_psf_target_hat = 0;
   PyArrayObject *__pyx_v_psf_i_hat = 0;
   PyArrayObject *__pyx_v_holder = 0;
   int __pyx_v_patch_i;
@@ -3839,235 +4341,223 @@
   __pyx_pybuffernd_target_evaluation.rcbuffer = &__pyx_pybuffer_target_evaluation;
   __pyx_pybuffer_values.pybuffer.buf = NULL;
   __pyx_pybuffer_values.refcount = 0;
   __pyx_pybuffernd_values.data = NULL;
   __pyx_pybuffernd_values.rcbuffer = &__pyx_pybuffer_values;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer, (PyObject*)__pyx_v_target_evaluation, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer, (PyObject*)__pyx_v_target_evaluation, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 102, __pyx_L1_error)
   }
   __pyx_pybuffernd_target_evaluation.diminfo[0].strides = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_target_evaluation.diminfo[0].shape = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_target_evaluation.diminfo[1].strides = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_target_evaluation.diminfo[1].shape = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 102, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_values.diminfo[1].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_values.diminfo[1].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_values.diminfo[2].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_values.diminfo[2].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[2];
 
-  /* "regularizepsf/helper.pyx":71
+  /* "regularizepsf/helper.pyx":103
  * @cython.cdivision(True)
  * cpdef _precalculate_ffts(np.ndarray[DTYPE_t, ndim=2] target_evaluation, np.ndarray[DTYPE_t, ndim=3] values):
  *     cdef int size = values.shape[1]             # <<<<<<<<<<<<<<
  *     cdef int num_patches = values.shape[0]
  *     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)
  */
   __pyx_v_size = (__pyx_v_values->dimensions[1]);
 
-  /* "regularizepsf/helper.pyx":72
+  /* "regularizepsf/helper.pyx":104
  * cpdef _precalculate_ffts(np.ndarray[DTYPE_t, ndim=2] target_evaluation, np.ndarray[DTYPE_t, ndim=3] values):
  *     cdef int size = values.shape[1]
  *     cdef int num_patches = values.shape[0]             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)
- *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=np.complex)
+ *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=complex)
  */
   __pyx_v_num_patches = (__pyx_v_values->dimensions[0]);
 
-  /* "regularizepsf/helper.pyx":73
+  /* "regularizepsf/helper.pyx":105
  *     cdef int size = values.shape[1]
  *     cdef int num_patches = values.shape[0]
  *     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=np.complex)
- *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=complex)
+ *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=float)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fft2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fft2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_target_evaluation)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_target_evaluation));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 105, __pyx_L1_error)
   __pyx_t_4 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer, (PyObject*)__pyx_t_4, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_psf_target_hat = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 73, __pyx_L1_error)
+      __PYX_ERR(0, 105, __pyx_L1_error)
     } else {__pyx_pybuffernd_psf_target_hat.diminfo[0].strides = __pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_psf_target_hat.diminfo[0].shape = __pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_psf_target_hat.diminfo[1].strides = __pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_psf_target_hat.diminfo[1].shape = __pyx_pybuffernd_psf_target_hat.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_4 = 0;
   __pyx_v_psf_target_hat = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "regularizepsf/helper.pyx":74
+  /* "regularizepsf/helper.pyx":106
  *     cdef int num_patches = values.shape[0]
  *     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)
- *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=np.complex)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=np.float)
+ *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=complex)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=float)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_patches); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_patches); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_5);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, ((PyObject *)(&PyComplex_Type))) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 74, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_7 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo___pyx_t_double_complex, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_psf_i_hat = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 74, __pyx_L1_error)
+      __PYX_ERR(0, 106, __pyx_L1_error)
     } else {__pyx_pybuffernd_psf_i_hat.diminfo[0].strides = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_psf_i_hat.diminfo[0].shape = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_psf_i_hat.diminfo[1].strides = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_psf_i_hat.diminfo[1].shape = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_psf_i_hat.diminfo[2].strides = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_psf_i_hat.diminfo[2].shape = __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_7 = 0;
-  __pyx_v_psf_i_hat = ((PyArrayObject *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_v_psf_i_hat = ((PyArrayObject *)__pyx_t_3);
+  __pyx_t_3 = 0;
 
-  /* "regularizepsf/helper.pyx":75
+  /* "regularizepsf/helper.pyx":107
  *     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)
- *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=np.complex)
- *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=np.float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=complex)
+ *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=float)             # <<<<<<<<<<<<<<
  * 
  *     for patch_i in range(num_patches):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
-  __pyx_t_1 = 0;
+  __pyx_t_3 = 0;
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_holder.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_holder = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_holder.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 75, __pyx_L1_error)
+      __PYX_ERR(0, 107, __pyx_L1_error)
     } else {__pyx_pybuffernd_holder.diminfo[0].strides = __pyx_pybuffernd_holder.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_holder.diminfo[0].shape = __pyx_pybuffernd_holder.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_holder.diminfo[1].strides = __pyx_pybuffernd_holder.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_holder.diminfo[1].shape = __pyx_pybuffernd_holder.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_holder = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "regularizepsf/helper.pyx":77
- *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=np.float)
+  /* "regularizepsf/helper.pyx":109
+ *     cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=float)
  * 
  *     for patch_i in range(num_patches):             # <<<<<<<<<<<<<<
  *         for xx in range(size):
  *             for yy in range(size):
  */
   __pyx_t_9 = __pyx_v_num_patches;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_patch_i = __pyx_t_11;
 
-    /* "regularizepsf/helper.pyx":78
+    /* "regularizepsf/helper.pyx":110
  * 
  *     for patch_i in range(num_patches):
  *         for xx in range(size):             # <<<<<<<<<<<<<<
  *             for yy in range(size):
  *                 holder[xx, yy] = values[patch_i, xx, yy]
  */
     __pyx_t_12 = __pyx_v_size;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_xx = __pyx_t_14;
 
-      /* "regularizepsf/helper.pyx":79
+      /* "regularizepsf/helper.pyx":111
  *     for patch_i in range(num_patches):
  *         for xx in range(size):
  *             for yy in range(size):             # <<<<<<<<<<<<<<
  *                 holder[xx, yy] = values[patch_i, xx, yy]
  *         result = fft2(holder)
  */
       __pyx_t_15 = __pyx_v_size;
       __pyx_t_16 = __pyx_t_15;
       for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
         __pyx_v_yy = __pyx_t_17;
 
-        /* "regularizepsf/helper.pyx":80
+        /* "regularizepsf/helper.pyx":112
  *         for xx in range(size):
  *             for yy in range(size):
  *                 holder[xx, yy] = values[patch_i, xx, yy]             # <<<<<<<<<<<<<<
  *         result = fft2(holder)
  *         for xx in range(size):
  */
         __pyx_t_18 = __pyx_v_patch_i;
@@ -4075,115 +4565,115 @@
         __pyx_t_20 = __pyx_v_yy;
         __pyx_t_21 = __pyx_v_xx;
         __pyx_t_22 = __pyx_v_yy;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_holder.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_holder.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_holder.diminfo[1].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_13regularizepsf_6helper_DTYPE_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_values.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_values.diminfo[1].strides, __pyx_t_20, __pyx_pybuffernd_values.diminfo[2].strides));
       }
     }
 
-    /* "regularizepsf/helper.pyx":81
+    /* "regularizepsf/helper.pyx":113
  *             for yy in range(size):
  *                 holder[xx, yy] = values[patch_i, xx, yy]
  *         result = fft2(holder)             # <<<<<<<<<<<<<<
  *         for xx in range(size):
  *             for yy in range(size):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fft2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fft2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, ((PyObject *)__pyx_v_holder)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_holder));
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_result, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "regularizepsf/helper.pyx":82
+    /* "regularizepsf/helper.pyx":114
  *                 holder[xx, yy] = values[patch_i, xx, yy]
  *         result = fft2(holder)
  *         for xx in range(size):             # <<<<<<<<<<<<<<
  *             for yy in range(size):
  *                 psf_i_hat[patch_i, xx, yy] = result[xx, yy]
  */
     __pyx_t_12 = __pyx_v_size;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_xx = __pyx_t_14;
 
-      /* "regularizepsf/helper.pyx":83
+      /* "regularizepsf/helper.pyx":115
  *         result = fft2(holder)
  *         for xx in range(size):
  *             for yy in range(size):             # <<<<<<<<<<<<<<
  *                 psf_i_hat[patch_i, xx, yy] = result[xx, yy]
  *     return psf_target_hat, psf_i_hat
  */
       __pyx_t_15 = __pyx_v_size;
       __pyx_t_16 = __pyx_t_15;
       for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
         __pyx_v_yy = __pyx_t_17;
 
-        /* "regularizepsf/helper.pyx":84
+        /* "regularizepsf/helper.pyx":116
  *         for xx in range(size):
  *             for yy in range(size):
  *                 psf_i_hat[patch_i, xx, yy] = result[xx, yy]             # <<<<<<<<<<<<<<
  *     return psf_target_hat, psf_i_hat
  */
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_xx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_xx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_yy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_yy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_2);
         PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
         __pyx_t_3 = 0;
         __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_result, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_result, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_23 = __Pyx_PyComplex_As___pyx_t_double_complex(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L1_error)
+        __pyx_t_23 = __Pyx_PyComplex_As___pyx_t_double_complex(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_20 = __pyx_v_patch_i;
         __pyx_t_19 = __pyx_v_xx;
         __pyx_t_18 = __pyx_v_yy;
         *__Pyx_BufPtrStrided3d(__pyx_t_double_complex *, __pyx_pybuffernd_psf_i_hat.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_psf_i_hat.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_psf_i_hat.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_psf_i_hat.diminfo[2].strides) = __pyx_t_23;
       }
     }
   }
 
-  /* "regularizepsf/helper.pyx":85
+  /* "regularizepsf/helper.pyx":117
  *             for yy in range(size):
  *                 psf_i_hat[patch_i, xx, yy] = result[xx, yy]
  *     return psf_target_hat, psf_i_hat             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_v_psf_target_hat));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_psf_target_hat));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_psf_target_hat));
   __Pyx_INCREF(((PyObject *)__pyx_v_psf_i_hat));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_psf_i_hat));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_psf_i_hat));
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "regularizepsf/helper.pyx":70
+  /* "regularizepsf/helper.pyx":102
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * cpdef _precalculate_ffts(np.ndarray[DTYPE_t, ndim=2] target_evaluation, np.ndarray[DTYPE_t, ndim=3] values):             # <<<<<<<<<<<<<<
  *     cdef int size = values.shape[1]
  *     cdef int num_patches = values.shape[0]
  */
 
@@ -4220,16 +4710,16 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13regularizepsf_6helper_3_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_13regularizepsf_6helper_3_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13regularizepsf_6helper_7_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_13regularizepsf_6helper_7_precalculate_ffts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_target_evaluation = 0;
   PyArrayObject *__pyx_v_values = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4253,51 +4743,51 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_target_evaluation)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_precalculate_ffts", 1, 2, 2, 1); __PYX_ERR(0, 70, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_precalculate_ffts", 1, 2, 2, 1); __PYX_ERR(0, 102, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_precalculate_ffts") < 0)) __PYX_ERR(0, 70, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_precalculate_ffts") < 0)) __PYX_ERR(0, 102, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_target_evaluation = ((PyArrayObject *)values[0]);
     __pyx_v_values = ((PyArrayObject *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_precalculate_ffts", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 70, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_precalculate_ffts", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 102, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("regularizepsf.helper._precalculate_ffts", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_target_evaluation), __pyx_ptype_5numpy_ndarray, 1, "target_evaluation", 0))) __PYX_ERR(0, 70, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13regularizepsf_6helper_2_precalculate_ffts(__pyx_self, __pyx_v_target_evaluation, __pyx_v_values);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_target_evaluation), __pyx_ptype_5numpy_ndarray, 1, "target_evaluation", 0))) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13regularizepsf_6helper_6_precalculate_ffts(__pyx_self, __pyx_v_target_evaluation, __pyx_v_values);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13regularizepsf_6helper_2_precalculate_ffts(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_target_evaluation, PyArrayObject *__pyx_v_values) {
+static PyObject *__pyx_pf_13regularizepsf_6helper_6_precalculate_ffts(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_target_evaluation, PyArrayObject *__pyx_v_values) {
   __Pyx_LocalBuf_ND __pyx_pybuffernd_target_evaluation;
   __Pyx_Buffer __pyx_pybuffer_target_evaluation;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_values;
   __Pyx_Buffer __pyx_pybuffer_values;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -4311,24 +4801,24 @@
   __pyx_pybuffernd_target_evaluation.rcbuffer = &__pyx_pybuffer_target_evaluation;
   __pyx_pybuffer_values.pybuffer.buf = NULL;
   __pyx_pybuffer_values.refcount = 0;
   __pyx_pybuffernd_values.data = NULL;
   __pyx_pybuffernd_values.rcbuffer = &__pyx_pybuffer_values;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer, (PyObject*)__pyx_v_target_evaluation, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer, (PyObject*)__pyx_v_target_evaluation, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 102, __pyx_L1_error)
   }
   __pyx_pybuffernd_target_evaluation.diminfo[0].strides = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_target_evaluation.diminfo[0].shape = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_target_evaluation.diminfo[1].strides = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_target_evaluation.diminfo[1].shape = __pyx_pybuffernd_target_evaluation.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_13regularizepsf_6helper_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 102, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_values.diminfo[1].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_values.diminfo[1].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_values.diminfo[2].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_values.diminfo[2].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[2];
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_13regularizepsf_6helper__precalculate_ffts(__pyx_v_target_evaluation, __pyx_v_values, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_13regularizepsf_6helper__precalculate_ffts(__pyx_v_target_evaluation, __pyx_v_values, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4348,15 +4838,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_values.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4365,29 +4855,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4398,15 +4888,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4415,29 +4905,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4448,15 +4938,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4465,29 +4955,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4498,15 +4988,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4515,29 +5005,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4548,15 +5038,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4565,29 +5055,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4598,212 +5088,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4819,15 +5309,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4835,53 +5325,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4889,30 +5379,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4927,15 +5417,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4951,15 +5441,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4967,53 +5457,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -5021,30 +5511,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5059,15 +5549,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5083,15 +5573,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5099,53 +5589,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -5153,30 +5643,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5191,191 +5681,193 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 static PyMethodDef __pyx_methods[] = {
   {"_correct_image", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13regularizepsf_6helper_1_correct_image, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13regularizepsf_6helper__correct_image},
-  {"_precalculate_ffts", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13regularizepsf_6helper_3_precalculate_ffts, METH_VARARGS|METH_KEYWORDS, 0},
+  {"_regularize_value", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13regularizepsf_6helper_3_regularize_value, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13regularizepsf_6helper_2_regularize_value},
+  {"_regularize_array", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13regularizepsf_6helper_5_regularize_array, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13regularizepsf_6helper_4_regularize_array},
+  {"_precalculate_ffts", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13regularizepsf_6helper_7_precalculate_ffts, METH_VARARGS|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec_helper(PyObject* module); /*proto*/
@@ -5413,25 +5905,25 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_n_s_A, __pyx_k_A, sizeof(__pyx_k_A), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+  {&__pyx_n_s_P, __pyx_k_P, sizeof(__pyx_k_P), 0, 0, 1, 1},
   {&__pyx_n_s_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 0, 1, 1},
   {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_complex, __pyx_k_complex, sizeof(__pyx_k_complex), 0, 0, 1, 1},
   {&__pyx_n_u_constant, __pyx_k_constant, sizeof(__pyx_k_constant), 0, 1, 0, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_epsilon, __pyx_k_epsilon, sizeof(__pyx_k_epsilon), 0, 0, 1, 1},
   {&__pyx_n_s_fft2, __pyx_k_fft2, sizeof(__pyx_k_fft2), 0, 0, 1, 1},
-  {&__pyx_n_s_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 0, 1, 1},
   {&__pyx_n_s_ifft2, __pyx_k_ifft2, sizeof(__pyx_k_ifft2), 0, 0, 1, 1},
   {&__pyx_n_s_image, __pyx_k_image, sizeof(__pyx_k_image), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_meshgrid, __pyx_k_meshgrid, sizeof(__pyx_k_meshgrid), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
@@ -5464,26 +5956,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -5493,15 +5985,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float_0_5 = PyFloat_FromDouble(0.5); if (unlikely(!__pyx_float_0_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -5783,15 +6275,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_regularizepsf__helper) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5865,15 +6357,15 @@
  * from numpy.fft import fft2, ifft2
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../private/var/folders/w3/c3fpftqj0cn3zdjqpnn7ds31hdhdts/T/pip-build-env-5kubech5/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6883,16 +7375,18 @@
 
 /* UnpackItemEndCheck */
   static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
+    } else {
+        return __Pyx_IterFinish();
     }
-    return __Pyx_IterFinish();
+    return 0;
 }
 
 /* PyFloatBinop */
   #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyFloat_AddObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check) {
     const double b = floatval;
     double a, result;
@@ -7060,15 +7554,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
     #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr = NULL;
+    PyObject *runerr;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -7729,15 +8223,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
     #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -7956,56 +8450,14 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-#if PY_MAJOR_VERSION < 3
-static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
-    if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
-    return -1;
-}
-static void __Pyx_ReleaseBuffer(Py_buffer *view) {
-    PyObject *obj = view->obj;
-    if (!obj) return;
-    if (PyObject_CheckBuffer(obj)) {
-        PyBuffer_Release(view);
-        return;
-    }
-    if ((0)) {}
-    view->obj = NULL;
-    Py_DECREF(obj);
-}
-#endif
-
-
-    /* CIntFromPyVerify */
-    #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
 /* Declarations */
     #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
@@ -8127,15 +8579,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if ((b.imag == 0) && (a.real >= 0)) {
+                } else if (b.imag == 0) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -8152,28 +8604,70 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* FromPy */
+#if PY_MAJOR_VERSION < 3
+static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
+    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    return -1;
+}
+static void __Pyx_ReleaseBuffer(Py_buffer *view) {
+    PyObject *obj = view->obj;
+    if (!obj) return;
+    if (PyObject_CheckBuffer(obj)) {
+        PyBuffer_Release(view);
+        return;
+    }
+    if ((0)) {}
+    view->obj = NULL;
+    Py_DECREF(obj);
+}
+#endif
+
+
+    /* FromPy */
     static __pyx_t_double_complex __Pyx_PyComplex_As___pyx_t_double_complex(PyObject* o) {
     Py_complex cval;
 #if !CYTHON_COMPILING_IN_PYPY
     if (PyComplex_CheckExact(o))
         cval = ((PyComplexObject *)o)->cval;
     else
 #endif
         cval = PyComplex_AsCComplex(o);
     return __pyx_t_double_complex_from_parts(
                (double)cval.real,
                (double)cval.imag);
 }
 
+/* CIntFromPyVerify */
+    #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* Declarations */
     #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -8295,15 +8789,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if ((b.imag == 0) && (a.real >= 0)) {
+                } else if (b.imag == 0) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
```

### Comparing `regularizepsf-0.1.0/regularizepsf/helper.pyx` & `regularizepsf-0.2.0/regularizepsf/helper.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -16,24 +16,24 @@
                      float alpha,
                      float epsilon):
     """Core Cython code to actually correct an image"""
     cdef int num_evaluations = x.shape[0]
     cdef int size = values_fft.shape[1]
     cdef int i = 0, j=0, xx = 0, yy = 0
     cdef int this_x, this_y, this_x_prime, this_y_prime
-    cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=np.float)
-    cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=np.float)
-    cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=np.float)
+    cdef np.ndarray[np.float_t, ndim=2] img_i = np.empty((size, size), dtype=float)
+    cdef np.ndarray[DTYPE_t, ndim=2] psf_i = np.empty((size, size), dtype=float)
+    cdef np.ndarray[DTYPE_t, ndim=2] corrected_i = np.empty((size, size), dtype=float)
     cdef np.ndarray[DTYPE_t, ndim=2] padded_img = np.pad(image, ((2 * size, 2* size), (2*size, 2*size)),
                                                          mode="constant")
-    cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=np.float)
+    cdef np.ndarray[DTYPE_t, ndim=2] result_img = np.zeros_like(padded_img, dtype=float)
     cdef float psf_i_hat_abs
-    cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=np.complex)
-    cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=np.complex)
-    cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=np.complex)
+    cdef np.ndarray[np.complex128_t, ndim=2] psf_i_hat_norm = np.empty((size, size), dtype=complex)
+    cdef np.ndarray[np.complex128_t, ndim=2] img_i_hat = np.empty((size, size), dtype=complex)
+    cdef np.ndarray[np.complex128_t, ndim=2] temp = np.empty((size, size), dtype=complex)
     cdef np.ndarray[np.float_t, ndim=2] apodization_window
 
 
     xarr, yarr = np.meshgrid(np.arange(size), np.arange(size))
     apodization_window = np.square(np.sin((xarr + 0.5) * (np.pi / size))) * np.square(np.sin((yarr + 0.5) * (np.pi / size)))
     apodization_window = np.sin((xarr + 0.5) * (np.pi / size)) * np.sin((yarr + 0.5) * (np.pi / size))
 
@@ -47,39 +47,71 @@
         for xx in range(size):
             for yy in range(size):
                 img_i[xx, yy] = apodization_window[xx, yy] * padded_img[this_x_prime + xx, this_y_prime + yy]
         img_i_hat = fft2(img_i)
 
         for xx in range(size):
             for yy in range(size):
-                psf_i_hat_abs = abs(values_fft[i, xx, yy])
-                psf_i_hat_norm[xx, yy] = (values_fft[i, xx, yy].conjugate() / psf_i_hat_abs) * ((psf_i_hat_abs**alpha) / ((psf_i_hat_abs**(alpha+1.0)) + (epsilon * abs(target_fft[xx, yy]))**(alpha+1.0)))
+                psf_i_hat_norm[xx, yy] = _regularize_value(
+                        values_fft[i, xx, yy], alpha, epsilon, target_fft[xx, yy])
                 temp[xx, yy] = img_i_hat[xx, yy] * psf_i_hat_norm[xx, yy] * target_fft[xx, yy]
         corrected_i = np.real(ifft2(temp))
 
         # add the corrected_i to the array
         for xx in range(size):
             for yy in range(size):
                 result_img[this_x_prime+xx, this_y_prime+yy] = result_img[this_x_prime+xx, this_y_prime+yy] + (corrected_i[xx, yy] * apodization_window[xx, yy])
 
     return result_img[2 * size:image.shape[0] + 2 * size, 2 * size:image.shape[1] + 2 * size]
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.cdivision(True)
+cpdef complex _regularize_value(
+        complex A,
+        float alpha,
+        float epsilon,
+        complex P):
+    """Implements Eqn (6) of Hughes et al. (2023) for one Fourier-space pixel"""
+    cdef float A_abs = abs(A)
+    cdef complex R_A = (A.conjugate() / A_abs) * (A_abs**alpha / (A_abs**(alpha+1.0) + (epsilon * abs(P))**(alpha+1.0)))
+    return R_A
+
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+@cython.cdivision(True)
+cpdef _regularize_array(
+        np.ndarray[np.complex128_t, ndim=2] A,
+        float alpha,
+        float epsilon,
+        np.ndarray[np.complex128_t, ndim=2] P):
+    """Loops _regularize_value across a 2D array"""
+    cdef int size = A.shape[1]
+    cdef np.ndarray[np.complex128_t, ndim=2] output = np.empty((size, size), dtype=complex)
+
+    for xx in range(size):
+        for yy in range(size):
+            output[xx, yy] = _regularize_value(A[xx, yy], alpha, epsilon, P[xx, yy])
+    return output
+
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+@cython.cdivision(True)
 cpdef _precalculate_ffts(np.ndarray[DTYPE_t, ndim=2] target_evaluation, np.ndarray[DTYPE_t, ndim=3] values):
     cdef int size = values.shape[1]
     cdef int num_patches = values.shape[0]
     cdef np.ndarray[np.complex128_t, ndim=2] psf_target_hat = fft2(target_evaluation)
-    cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=np.complex)
-    cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=np.float)
+    cdef np.ndarray[np.complex128_t, ndim=3] psf_i_hat = np.empty((num_patches, size, size), dtype=complex)
+    cdef np.ndarray[np.float_t, ndim=2] holder = np.empty((size, size), dtype=float)
 
     for patch_i in range(num_patches):
         for xx in range(size):
             for yy in range(size):
                 holder[xx, yy] = values[patch_i, xx, yy]
         result = fft2(holder)
         for xx in range(size):
             for yy in range(size):
                 psf_i_hat[patch_i, xx, yy] = result[xx, yy]
-    return psf_target_hat, psf_i_hat
+    return psf_target_hat, psf_i_hat
```

### Comparing `regularizepsf-0.1.0/regularizepsf/psf.py` & `regularizepsf-0.2.0/regularizepsf/psf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
-from typing import Callable, Any, cast
-from numbers import Real
+import abc
 import inspect
 from functools import partial
-import abc
+from numbers import Real
+from typing import Any, Callable, Dict, List, cast
 
 import numpy as np
 
-from regularizepsf.exceptions import (PSFParameterValidationError,
-                                      VariedPSFParameterMismatchError)
+from regularizepsf.exceptions import (
+    PSFParameterValidationError,
+    VariedPSFParameterMismatchError,
+)
 
 
 class PointSpreadFunctionABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def __call__(self, x: Real | np.ndarary, y: Real | np.ndarray) -> Real | np.ndarray:
         """Evaluation of the point spread function
 
@@ -28,117 +30,134 @@
         -------
         real number or `np.ndarray`
             the value of the point spread function at (x,y)
         """
 
     @property
     @abc.abstractmethod
-    def parameters(self):
+    def parameters(self) -> List:
         """Varying parameters of the model."""
 
 
 class SimplePSF(PointSpreadFunctionABC):
     """Model for a simple PSF"""
 
-    def __init__(self, function: Callable):
+    def __init__(self, function: Callable) -> None:
         """Creates a PSF object
 
         Parameters
         ----------
         function
-            Python function representing the PSF, first two parameters must be x and y and must return an numpy array
+            Python function representing the PSF,
+                first two parameters must be x and y and must return an numpy array
         """
         self._f: Callable = function
         self._signature: inspect.Signature = inspect.signature(function)
         self._parameters: set[str] = set()
 
         if len(self._signature.parameters) < 2:
-            raise PSFParameterValidationError("x and y must be the first two arguments in your model equation.")
+            msg = "x and y must be the first two arguments in your model equation."
+            raise PSFParameterValidationError(msg)
 
         for i, variable in enumerate(self._signature.parameters):
             if i == 0 and variable != "x":
-                raise PSFParameterValidationError("x must be the first arguments in your model equation.")
+                msg = "x must be the first arguments in your model equation."
+                raise PSFParameterValidationError(msg)
             elif i == 1 and variable != "y":
-                raise PSFParameterValidationError("y must be the second arguments in your model equation")
+                msg = "y must be the second arguments in your model equation"
+                raise PSFParameterValidationError(msg)
             if i >= 2:
                 self._parameters.add(variable)
 
-    def __call__(self, x, y, **kwargs) -> Real | np.ndarray:
+    def __call__(self, 
+                 x: Real | np.ndarray,
+                 y: Real | np.ndarray, 
+                 **kwargs: Dict[str, Any]) -> Real | np.ndarray:
         return self._f(x, y, **kwargs)
 
     @property
     def parameters(self) -> set[str]:
         return self._parameters
 
 
-def simple_psf(arg=None) -> SimplePSF:
+def simple_psf(arg: Any=None) -> SimplePSF:
     if callable(arg):
         return SimplePSF(arg)
     else:
-        raise Exception("psf decorator must have no arguments.")
+        raise TypeError("psf decorator must have no arguments.")
 
 
 class VariedPSF(PointSpreadFunctionABC):
     """Model for a PSF that varies over the field of view"""
 
-    def __init__(self, vary_function: Callable, base_psf: SimplePSF, validate_at_call: bool = True):
+    def __init__(self, 
+                 vary_function: Callable,
+                 base_psf: SimplePSF, 
+                 validate_at_call: bool = True) -> None:
         self._vary_function = vary_function
         self._base_psf = base_psf
         self.validate_at_call = validate_at_call
 
         self.parameterization_signature = inspect.signature(vary_function)
         if len(self.parameterization_signature.parameters) < 2:
-            raise PSFParameterValidationError(f"Found {len(self.parameterization_signature.parameters)}")
+            msg = f"Found {len(self.parameterization_signature.parameters)}"
+            raise PSFParameterValidationError(msg)
 
         if len(self.parameterization_signature.parameters) > 2:
-            raise PSFParameterValidationError(
-                f"Found function requiring {len(self.parameterization_signature.parameters)} arguments."
-                "Expected 2, only `x` and `y`.")
+            msg = ("Found function requiring"
+                   f"{len(self.parameterization_signature.parameters)}"
+                   "arguments. Expected 2, only `x` and `y`.")
+            raise PSFParameterValidationError(msg)
 
         for i, variable in enumerate(self.parameterization_signature.parameters):
             if i == 0 and variable != "x":
-                raise PSFParameterValidationError("x must be the first argument in your parameterization equation.")
+                msg = "x must be the first argument in your parameterization equation."
+                raise PSFParameterValidationError(msg)
             elif i == 1 and variable != "y":
-                raise PSFParameterValidationError("y must be the second argument in your parameterization equation")
+                msg = "y must be the second argument in your parameterization equation"
+                raise PSFParameterValidationError(msg)
 
         # check the parameters at the origin
         origin_evaluation: dict[str, Any] = vary_function(0, 0)
         self._origin_parameters: set[str] = set(origin_evaluation.keys())
         if self._base_psf.parameters != self._origin_parameters:
             msg = (f"The base PSF model has parameters {self._base_psf.parameters} "
-                   f"while the varied psf supplies {self._origin_parameters} at the origin. These must match.")
+                   f"while the varied psf supplies {self._origin_parameters}" 
+                   "at the origin. These must match.")
             raise VariedPSFParameterMismatchError(msg)
 
-    def __call__(self, x, y):
+    def __call__(self, x: Real | np.ndarray, y: Real | np.ndarray) -> Real | np.ndarray:
         variance = self._vary_function(x, y)
-        if self.validate_at_call:
-            if set(variance.keys()) != self.parameters:
-                raise VariedPSFParameterMismatchError(f"At (x, y) the varying parameters were {set(variance.keys())}"
-                                                      f" when the parameters were expected as {self.parameters}.")
+        if self.validate_at_call and set(variance.keys()) != self.parameters:
+                msg = (f"At (x, y) the varying parameters were {set(variance.keys())}"
+                       f" when the parameters were expected as {self.parameters}.")
+                raise VariedPSFParameterMismatchError(msg)
         return self._base_psf(x, y, **variance)
 
     @property
-    def parameters(self):
+    def parameters(self) -> List:
         return self._base_psf.parameters
 
 
-def _varied_psf(base_psf: SimplePSF):
+def _varied_psf(base_psf: SimplePSF) -> VariedPSF:
     if base_psf is None:
-        raise Exception("A base_psf must be provided to the varied_psf decorator.")
+        raise TypeError("A base_psf must be provided to the varied_psf decorator.")
 
-    def inner(__fn=None, *, check_at_call: bool = True):
+    def inner(__fn: Callable=None, *, check_at_call: bool = True) -> Callable:
         if __fn:
             return VariedPSF(__fn, base_psf, validate_at_call=check_at_call)
         else:
             return partial(inner, check_at_call=check_at_call)
 
     return inner
 
 
-def varied_psf(base_psf: SimplePSF = None):
+def varied_psf(base_psf: SimplePSF = None) -> VariedPSF:
     if isinstance(base_psf, SimplePSF):
         return cast(VariedPSF, _varied_psf(base_psf))
     else:
         if callable(base_psf):
-            raise Exception("varied_psf decorator must be called with an argument for the base_psf.")
+            raise TypeError("varied_psf decorator must be called"
+                            "with an argument for the base_psf.")
         else:
-            raise Exception("varied_psf decorator expects exactly one argument of type PSF.")
+            raise TypeError("varied_psf decorator expects exactly"
+                            "one argument of type PSF.")
```

### Comparing `regularizepsf-0.1.0/setup.py` & `regularizepsf-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 ext_modules = [Extension('regularizepsf.helper',
                          sources=['regularizepsf/helper.pyx'],
                          include_dirs=[numpy.get_include()])]
 
 setup(
     name='regularizepsf',
-    version='0.1.0',
+    version='0.2.0',
     description='Point spread function modeling and regularization',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['regularizepsf'],
     url='https://github.com/punch-mission/regularizepsf',
     license='MIT',
     author='J. Marcus Hughes',
     author_email='hughes.jmb@gmail.com',
     ext_modules=cythonize(ext_modules, annotate=True, compiler_directives={'language_level': 3}),
-    install_requires=["numpy", "dill", "deepdish", "lmfit", "sep", "cython", "astropy", "scipy", "scikit-image"],
+    install_requires=["numpy", "dill", "deepdish", "lmfit", "sep", "cython", "astropy", "scipy", "scikit-image", "matplotlib"],
     package_data={"regularizepsf": ["helper.pyx"]},
     setup_requires=["cython"],
-    extras_require={"test": ['pytest', 'coverage', 'pytest-runner']}
+    extras_require={"test": ['pytest', 'coverage', 'pytest-runner', 'pytest-mpl']}
 )
```

