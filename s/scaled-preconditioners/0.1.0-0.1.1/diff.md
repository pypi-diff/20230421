# Comparing `tmp/scaled_preconditioners-0.1.0.tar.gz` & `tmp/scaled_preconditioners-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaled_preconditioners-0.1.0.tar", max compression
+gzip compressed data, was "scaled_preconditioners-0.1.1.tar", max compression
```

## Comparing `scaled_preconditioners-0.1.0.tar` & `scaled_preconditioners-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2019-09-04 11:51:07.308628 scaled_preconditioners-0.1.0/LICENSE
--rw-r--r--   0        0        0     1634 2023-04-17 13:01:57.921716 scaled_preconditioners-0.1.0/README.md
--rw-r--r--   0        0        0     1124 2023-04-17 09:16:51.522490 scaled_preconditioners-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 07:55:47.392287 scaled_preconditioners-0.1.0/scaled_preconditioners/__init__.py
--rw-r--r--   0        0        0     2486 2023-04-17 12:32:25.104953 scaled_preconditioners-0.1.0/scaled_preconditioners/approximation.py
--rw-r--r--   0        0        0     2361 2023-04-17 12:39:20.742716 scaled_preconditioners-0.1.0/scaled_preconditioners/preconditioner.py
--rw-r--r--   0        0        0      184 2023-04-17 07:50:04.039146 scaled_preconditioners-0.1.0/scaled_preconditioners/utils.py
--rw-r--r--   0        0        0     2498 2023-04-17 13:15:54.189183 scaled_preconditioners-0.1.0/setup.py
--rw-r--r--   0        0        0     2301 2023-04-17 13:15:54.189345 scaled_preconditioners-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-21 13:30:51.037443 scaled_preconditioners-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1642 2023-04-21 13:30:51.037443 scaled_preconditioners-0.1.1/README.md
+-rw-r--r--   0        0        0     1124 2023-04-21 13:30:51.041443 scaled_preconditioners-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 13:30:51.041443 scaled_preconditioners-0.1.1/scaled_preconditioners/__init__.py
+-rw-r--r--   0        0        0     4598 2023-04-21 13:30:51.041443 scaled_preconditioners-0.1.1/scaled_preconditioners/approximation.py
+-rw-r--r--   0        0        0     2143 2023-04-21 13:30:51.041443 scaled_preconditioners-0.1.1/scaled_preconditioners/preconditioner.py
+-rw-r--r--   0        0        0      184 2023-04-21 13:30:51.041443 scaled_preconditioners-0.1.1/scaled_preconditioners/utils.py
+-rw-r--r--   0        0        0     2506 2023-04-21 13:31:55.206889 scaled_preconditioners-0.1.1/setup.py
+-rw-r--r--   0        0        0     2309 2023-04-21 13:31:55.207175 scaled_preconditioners-0.1.1/PKG-INFO
```

### Comparing `scaled_preconditioners-0.1.0/LICENSE` & `scaled_preconditioners-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scaled_preconditioners-0.1.0/README.md` & `scaled_preconditioners-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Build Status
 
 [![Tests](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml/badge.svg)](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml)
 
 ## Installation
 
-``pip install bregman_approx``
+``pip install scaled_preconditioners``
 
 ## A simple example
 
 #### Define some parameters
 ```
 dimension = 100
 psd_rank = 50
```

### Comparing `scaled_preconditioners-0.1.0/pyproject.toml` & `scaled_preconditioners-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaled_preconditioners"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Andreas Bock <aasbo@dtu.dk>"]
 readme = "README.md"
 packages = [{include = "scaled_preconditioners"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <3.12"
```

### Comparing `scaled_preconditioners-0.1.0/scaled_preconditioners/preconditioner.py` & `scaled_preconditioners-0.1.1/scaled_preconditioners/preconditioner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,69 @@
-import functools
-
 import numpy as np
 import scipy.sparse
 from scipy.sparse import identity as sparse_identity
 from scipy.sparse.linalg import LinearOperator
 
-from scaled_preconditioners.approximation import approximate
+from scaled_preconditioners.approximation import Factor, approximate
 
-__all__ = ["compute_preconditioner"]
+__all__ = ["compute_preconditioner", "Factor"]
 
 
 def compute_preconditioner(
-    factor,
-    B,
+    factor: Factor,
+    psd_term: LinearOperator,
     algorithm: str,
     rank_approx: int,
     n_oversamples: int = 1,
     n_power_iter: int = 0,
     random_state: int = 0,
 ) -> LinearOperator:
     """
-    For a matrix S = A + B, this method computes the preconditioner:
+    For a Hermitian matrix S = A + B, this method computes the preconditioner:
 
         P = Q(I + X)Q^*,
 
     where X is a low rank approximation G = Q^{-1} B Q^{-*}. The preconditioner
-    is provided as a `LinearOperator`.
+    is provided as a `LinearOperator`. The type of approximation is given by the
+    `algorithm` parameter.
 
     Args:
-        factor: {array-like, sparse matrix} of shape (n, n)
-            Factor of A.
-        B: {array-like, sparse matrix} of shape (n, n)
-            Positive semidefinite matrix.
+        factor: a Factor object.
+        psd_term: a Symmetric positive semidefinite matrix as a LinearOperator.
         algorithm: Can be either 'truncated_svd', 'randomized' or 'nystrom'.
         rank_approx: rank of the approximation (must be less than rank(X)).
-        n_oversamples: Oversampling parameter.
+        n_oversamples: Oversampling parameter. Not currently supported for
+            algorithm="nystrom".
         n_power_iter: Number of power iterations used in range finding.
         random_state: Seed.
 
     Returns:
-        A low rank approximation of `X`.
-
-    Raises:
-        ValueError: If `factor` is sparse and `B` is not, or vice versa.
+        A low rank approximation of `X` as a LinearOperator.
     """
-    is_sparse = scipy.sparse.issparse(factor)
-    if is_sparse ^ scipy.sparse.issparse(B):
-        raise ValueError(
-            f"Type mismatch between inputs. Factor is {type(factor)}"
-            f" but PSD matrix is {type(B)}. Both need to be either"
-            f" dense or CSR matrices."
-        )
-    if is_sparse:
-        _solve_fn = scipy.sparse.linalg.spsolve
-    else:
-        _solve_fn = scipy.linalg.solve
-
-    right_inv = _solve_fn(factor, B.T).T
-    G = _solve_fn(factor, right_inv)
-
-    factors_approx = approximate(
-        G,
+    scaled_psd_term = factor.inv() @  psd_term @ factor.inv().T
+    f, ft = approximate(
+        scaled_psd_term,
         algorithm,
         rank_approx=rank_approx,
         n_oversamples=n_oversamples,
         n_power_iter=n_power_iter,
         random_state=random_state,
     )
-    prod = functools.reduce(lambda a, b: a @ b, factors_approx)
-    if is_sparse:
-        inner = sparse_identity(factor.shape[0]) + prod
-    else:
-        inner = np.eye(factor.shape[0]) + prod
+    inner = sparse_identity(rank_approx) + ft @ f
+
+    def apply_inner(vector):
+        # v -> f.T v
+        w = ft.dot(vector)
+
+        # w -> (I_r + f.T f)^{1} w
+        u = scipy.linalg.solve(inner, w)
+
+        # action of  I_r - f(I_r + f.T @ f)^{1} f.T
+        return vector - np.dot(f, u)
 
     def action(vector):
-        return _solve_fn(factor @ inner @ factor.T, vector)
+        vector = factor.solve(vector)
+        vector = apply_inner(vector)
+        vector = factor.rsolve(vector)
+        return vector
 
     return LinearOperator(factor.shape, matvec=action)
```

### Comparing `scaled_preconditioners-0.1.0/setup.py` & `scaled_preconditioners-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'nox-poetry>=1.0.2,<2.0.0',
  'pytest>=7.3.0,<8.0.0',
  'scikit-learn>=1.2.2,<2.0.0',
  'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'scaled-preconditioners',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# Preconditioner Design via Bregman Divergences\n\nThis package implements the preconditioners in [1]. A simple use case\nis demonstrated below. See `examples/example_pcg.py` for a demo of all the \npreconditioners defined in this package.\n\n[1] TODO\n\n## Build Status\n\n[![Tests](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml/badge.svg)](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml)\n\n## Installation\n\n``pip install bregman_approx``\n\n## A simple example\n\n#### Define some parameters\n```\ndimension = 100\npsd_rank = 50\n```\n\n#### Construct S = A + B\n```\nF = csc_matrix(np.random.rand(dimension, psd_rank))\nB = F @ F.T\nQ = csc_matrix(np.random.rand(dimension, dimension))\nS = Q @ Q.T + B\n```\n\n#### Construct the preconditioner\nHere we use a randomised SVD, other options include truncated SVD, the\nNyström approximation. There is support for oversampling and power iteration\nschemes.\n```\nrank_approx = 15\npc = compute_preconditioner(\n    Q,\n    B,\n    algorithm="randomized",\n    rank_approx=rank_approx,\n    n_oversamples=4,\n    n_power_iter=0,\n)\n```\n\n#### Set up a right-hand side\n\n```\nrhs = np.random.rand(dimension)\ncounter = ConjugateGradientCounter()\n```\n\n#### Solve `Sx=b` with and without a preconditioner \n```\n_, info = linalg.cg(S, rhs, callback=counter)\nprint("No preconditioner:")\nprint(f"\\t Converged: {info == 0}")\nprint(f"\\t Iterations: {counter.n_iter}\\n")\n\ncounter.reset()\n_, info = linalg.cg(S, rhs, M=rsvd_pc, callback=counter)\nprint("Randomised SVD preconditioner:")\nprint(f"\\t Converged: {info == 0}")\nprint(f"\\t Iterations: {counter.n_iter}\\n")\n```',
+    'long_description': '# Preconditioner Design via Bregman Divergences\n\nThis package implements the preconditioners in [1]. A simple use case\nis demonstrated below. See `examples/example_pcg.py` for a demo of all the \npreconditioners defined in this package.\n\n[1] TODO\n\n## Build Status\n\n[![Tests](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml/badge.svg)](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml)\n\n## Installation\n\n``pip install scaled_preconditioners``\n\n## A simple example\n\n#### Define some parameters\n```\ndimension = 100\npsd_rank = 50\n```\n\n#### Construct S = A + B\n```\nF = csc_matrix(np.random.rand(dimension, psd_rank))\nB = F @ F.T\nQ = csc_matrix(np.random.rand(dimension, dimension))\nS = Q @ Q.T + B\n```\n\n#### Construct the preconditioner\nHere we use a randomised SVD, other options include truncated SVD, the\nNyström approximation. There is support for oversampling and power iteration\nschemes.\n```\nrank_approx = 15\npc = compute_preconditioner(\n    Q,\n    B,\n    algorithm="randomized",\n    rank_approx=rank_approx,\n    n_oversamples=4,\n    n_power_iter=0,\n)\n```\n\n#### Set up a right-hand side\n\n```\nrhs = np.random.rand(dimension)\ncounter = ConjugateGradientCounter()\n```\n\n#### Solve `Sx=b` with and without a preconditioner \n```\n_, info = linalg.cg(S, rhs, callback=counter)\nprint("No preconditioner:")\nprint(f"\\t Converged: {info == 0}")\nprint(f"\\t Iterations: {counter.n_iter}\\n")\n\ncounter.reset()\n_, info = linalg.cg(S, rhs, M=rsvd_pc, callback=counter)\nprint("Randomised SVD preconditioner:")\nprint(f"\\t Converged: {info == 0}")\nprint(f"\\t Iterations: {counter.n_iter}\\n")\n```',
     'author': 'Andreas Bock',
     'author_email': 'aasbo@dtu.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `scaled_preconditioners-0.1.0/PKG-INFO` & `scaled_preconditioners-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaled-preconditioners
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Andreas Bock
 Author-email: aasbo@dtu.dk
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 
 ## Build Status
 
 [![Tests](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml/badge.svg)](https://github.com/andreasbock/scaled_preconditioners/actions/workflows/tests.yml)
 
 ## Installation
 
-``pip install bregman_approx``
+``pip install scaled_preconditioners``
 
 ## A simple example
 
 #### Define some parameters
 ```
 dimension = 100
 psd_rank = 50
```

