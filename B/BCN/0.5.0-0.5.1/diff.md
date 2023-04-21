# Comparing `tmp/BCN-0.5.0.tar.gz` & `tmp/BCN-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BCN-0.5.0.tar", last modified: Sun Sep 25 17:03:20 2022, max compression
+gzip compressed data, was "dist/BCN-0.5.1.tar", last modified: Fri Apr 21 19:39:55 2023, max compression
```

## Comparing `BCN-0.5.0.tar` & `BCN-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.475719 BCN-0.5.0/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.470083 BCN-0.5.0/BCN/
--rw-r--r--   0 t          (501) staff       (20)     4967 2022-09-25 15:50:07.000000 BCN-0.5.0/BCN/BCNClassifier.py
--rw-r--r--   0 t          (501) staff       (20)     4638 2022-09-25 15:50:21.000000 BCN-0.5.0/BCN/BCNRegressor.py
--rw-r--r--   0 t          (501) staff       (20)      252 2022-09-25 15:49:05.000000 BCN-0.5.0/BCN/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.472750 BCN-0.5.0/BCN.egg-info/
--rw-r--r--   0 t          (501) staff       (20)      763 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      354 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/SOURCES.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/dependency_links.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/not-zip-safe
--rw-r--r--   0 t          (501) staff       (20)      257 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/requires.txt
--rw-r--r--   0 t          (501) staff       (20)        4 2022-09-25 17:03:20.000000 BCN-0.5.0/BCN.egg-info/top_level.txt
--rw-r--r--   0 t          (501) staff       (20)     1455 2022-08-12 14:12:40.000000 BCN-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 t          (501) staff       (20)      318 2022-08-18 09:42:24.000000 BCN-0.5.0/HISTORY.rst
--rw-r--r--   0 t          (501) staff       (20)     1690 2022-08-09 13:17:37.000000 BCN-0.5.0/LICENSE
--rw-r--r--   0 t          (501) staff       (20)      242 2022-08-09 13:17:37.000000 BCN-0.5.0/MANIFEST.in
--rw-r--r--   0 t          (501) staff       (20)      763 2022-09-25 17:03:20.475888 BCN-0.5.0/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)     2917 2022-08-18 09:42:24.000000 BCN-0.5.0/README.rst
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.460893 BCN-0.5.0/docs/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.461018 BCN-0.5.0/docs/site/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.473044 BCN-0.5.0/docs/site/img/
--rw-r--r--   0 t          (501) staff       (20)     1458 2022-08-18 15:42:37.000000 BCN-0.5.0/docs/site/img/grid.png
--rw-r--r--   0 t          (501) staff       (20)      375 2022-09-25 17:03:20.476575 BCN-0.5.0/setup.cfg
--rw-r--r--   0 t          (501) staff       (20)     1767 2022-09-25 15:48:57.000000 BCN-0.5.0/setup.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-09-25 17:03:20.474853 BCN-0.5.0/tests/
--rw-r--r--   0 t          (501) staff       (20)       33 2022-08-09 13:17:37.000000 BCN-0.5.0/tests/__init__.py
--rw-r--r--   0 t          (501) staff       (20)      367 2022-08-09 13:17:37.000000 BCN-0.5.0/tests/test_BCN.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.320455 BCN-0.5.1/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.312237 BCN-0.5.1/BCN/
+-rw-r--r--   0 t          (501) staff       (20)     5946 2023-04-21 19:36:22.000000 BCN-0.5.1/BCN/BCNClassifier.py
+-rw-r--r--   0 t          (501) staff       (20)     5647 2023-04-21 19:36:12.000000 BCN-0.5.1/BCN/BCNRegressor.py
+-rw-r--r--   0 t          (501) staff       (20)      252 2023-04-21 19:37:10.000000 BCN-0.5.1/BCN/__init__.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.316614 BCN-0.5.1/BCN.egg-info/
+-rw-r--r--   0 t          (501) staff       (20)      763 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)      354 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/not-zip-safe
+-rw-r--r--   0 t          (501) staff       (20)      139 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/requires.txt
+-rw-r--r--   0 t          (501) staff       (20)        4 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/top_level.txt
+-rw-r--r--   0 t          (501) staff       (20)     1455 2022-08-12 14:12:40.000000 BCN-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 t          (501) staff       (20)      318 2022-08-18 09:42:24.000000 BCN-0.5.1/HISTORY.rst
+-rw-r--r--   0 t          (501) staff       (20)     1690 2022-08-09 13:17:37.000000 BCN-0.5.1/LICENSE
+-rw-r--r--   0 t          (501) staff       (20)      242 2022-08-09 13:17:37.000000 BCN-0.5.1/MANIFEST.in
+-rw-r--r--   0 t          (501) staff       (20)      763 2023-04-21 19:39:55.320747 BCN-0.5.1/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)     2917 2022-08-18 09:42:24.000000 BCN-0.5.1/README.rst
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.303765 BCN-0.5.1/docs/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.303934 BCN-0.5.1/docs/site/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.317222 BCN-0.5.1/docs/site/img/
+-rw-r--r--   0 t          (501) staff       (20)     1458 2022-10-04 06:04:46.000000 BCN-0.5.1/docs/site/img/grid.png
+-rw-r--r--   0 t          (501) staff       (20)      375 2023-04-21 19:39:55.321925 BCN-0.5.1/setup.cfg
+-rw-r--r--   0 t          (501) staff       (20)     1767 2023-04-21 19:19:50.000000 BCN-0.5.1/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.319347 BCN-0.5.1/tests/
+-rw-r--r--   0 t          (501) staff       (20)       33 2022-08-09 13:17:37.000000 BCN-0.5.1/tests/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)      367 2022-08-09 13:17:37.000000 BCN-0.5.1/tests/test_BCN.py
```

### Comparing `BCN-0.5.0/BCN/BCNClassifier.py` & `BCN-0.5.1/BCN/BCNClassifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import os
 import numpy as np
 import rpy2.robjects.packages as rpackages
 
 from rpy2.robjects.packages import importr
-from rpy2.robjects import IntVector
+from rpy2.robjects import ListVector
 from rpy2.robjects.vectors import StrVector
-from rpy2.robjects import numpy2ri, r
+from rpy2.robjects import numpy2ri, default_converter, r
+from rpy2.robjects.conversion import localconverter
 
 from sklearn.base import BaseEstimator
 from sklearn.base import ClassifierMixin
 
-numpy2ri.activate()
 
 r['options'](warn=-1)
 
 required_packages = ["bcn"]  # list of required R packages
 
 if all(rpackages.isinstalled(x) for x in required_packages):
     check_packages = True  # True if packages are already installed
@@ -54,15 +53,15 @@
       nu: float
           Learning rate.
       col_sample: float
           Percentage of columns (covariates) adjusted at each iteration of the algorithm.
       lam: float
           Defines lower and upper bounds neural networks weights.
       r: float
-          A constant usually > 0.9
+          With 0 < r < 1. Controls the convergence rate of residuals.
       tol: float
           Convergence tolerance for an early stopping
       type_optim: string
           Type of optimization procedure used for finding neural networks weights at each iteration ("nlminb", "nmkb", "hjkb", "bobyqa", "randomsearch")
       activation: string
           Activation function (must be bounded). Currently: "sigmoid", "tanh".
       hidden_layer_bias: boolean
@@ -108,17 +107,26 @@
         X: {ndarray} of shape (n_samples, n_features)
             Training data.
 
         y: ndarray of shape (n_samples,) 
             Target values.
 
     """
-    X_r = base.matrix(X, nrow=X.shape[0], ncol=X.shape[1])
-    y_r = IntVector(y) 
-    self.obj = bcn.bcn(x = X_r, y = y_r, 
+
+    # cf. https://rpy2.github.io/doc/latest/html/numpy.html
+    # Create a converter that starts with rpy2's default converter
+    # to which the numpy conversion rules are added.
+    np_cv_rules = localconverter(default_converter + numpy2ri.converter)
+
+    with np_cv_rules:
+        # Anything here and until the `with` block is exited
+        # will use our numpy converter whenever objects are
+        # passed to R or are returned by R while calling
+        # rpy2.robjects functions.
+        self.obj = bcn.bcn(x = X, y = y, 
                        B = self.B, 
                        nu = self.nu,
                        col_sample = self.col_sample,
                        lam = self.lam,
                        r = self.r,
                        tol = self.tol,
                        type_optim = self.type_optim,
@@ -126,28 +134,40 @@
                        hidden_layer_bias = self.hidden_layer_bias,
                        verbose = self.verbose,
                        show_progress = self.show_progress,
                        seed = self.seed                       
                        )
     return self
 
-  def predict_proba(self, X, **kwargs): 
+  def predict_proba(self, X): 
     """Predict probabilities using BCN (Boosted Configuration Networks) classification model
 
     Parameters:
 
         X: array-like, shape (n_samples, n_features)
             Training data.
     """           
     assert self.obj is not None, "you must call `fit` before trying to predict"    
-    X_r = base.matrix(X, nrow=X.shape[0], ncol=X.shape[1])
-    return bcn.predict_bcn(self.obj, X_r, type="probs")
 
-  def predict(self, X, **kwargs):
+    # cf. https://rpy2.github.io/doc/latest/html/numpy.html
+    # Create a converter that starts with rpy2's default converter
+    # to which the numpy conversion rules are added.
+    np_cv_rules = localconverter(default_converter + numpy2ri.converter)
+
+    with np_cv_rules:
+        # Anything here and until the `with` block is exited
+        # will use our numpy converter whenever objects are
+        # passed to R or are returned by R while calling
+        # rpy2.robjects functions.
+        r_obj = ListVector(self.obj)
+        r_obj.do_slot_assign("class", StrVector(["bcn"]))
+        return bcn.predict_bcn(r_obj, X, type="probs")
+
+  def predict(self, X):
     """Predict using BCN (Boosted Configuration Networks) classification model
 
     Parameters:
 
         X: array-like, shape (n_samples, n_features)
             Test data.
     """           
-    return np.argmax(self.predict_proba(X, **kwargs), axis=1)
+    return np.argmax(self.predict_proba(X), axis=1)
```

### Comparing `BCN-0.5.0/BCN.egg-info/PKG-INFO` & `BCN-0.5.1/BCN.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCN
-Version: 0.5.0
+Version: 0.5.1
 Summary: Boosted Configuration Networks
 Home-page: https://github.com/Techtonique/bcn_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD license
 Keywords: BCN,Machine Learning,Statistical Learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `BCN-0.5.0/CONTRIBUTING.rst` & `BCN-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `BCN-0.5.0/LICENSE` & `BCN-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BCN-0.5.0/PKG-INFO` & `BCN-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCN
-Version: 0.5.0
+Version: 0.5.1
 Summary: Boosted Configuration Networks
 Home-page: https://github.com/Techtonique/bcn_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD license
 Keywords: BCN,Machine Learning,Statistical Learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `BCN-0.5.0/README.rst` & `BCN-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `BCN-0.5.0/docs/site/img/grid.png` & `BCN-0.5.1/docs/site/img/grid.png`

 * *Files identical despite different names*

### Comparing `BCN-0.5.0/setup.py` & `BCN-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     include_package_data=True,
     keywords=['BCN', 'Machine Learning', 'Statistical Learning'],
     name='BCN',
     packages=find_packages(include=['BCN', 'BCN.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Techtonique/bcn_python',
-    version='0.5.0',
+    version='0.5.1',
     zip_safe=False,
 )
```

