# Comparing `tmp/shgo-0.5.1.tar.gz` & `tmp/shgo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shgo-0.5.1.tar", last modified: Tue May  4 18:26:57 2021, max compression
+gzip compressed data, was "shgo-1.0.0.tar", last modified: Fri Apr 21 10:27:43 2023, max compression
```

## Comparing `shgo-0.5.1.tar` & `shgo-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 18:26:57.660554 shgo-0.5.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2017-09-22 09:04:45.000000 shgo-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3416 2021-05-04 18:26:57.660554 shgo-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2003 2020-10-27 10:36:08.000000 shgo-0.5.1/README.rst
--rw-r--r--   0 root         (0) root         (0)       66 2021-05-04 18:26:57.660554 shgo-0.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1869 2021-05-04 18:26:09.000000 shgo-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 18:26:57.650554 shgo-0.5.1/shgo/
--rw-r--r--   0 root         (0) root         (0)      128 2020-09-02 11:29:33.000000 shgo-0.5.1/shgo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63265 2021-05-04 18:06:38.000000 shgo-0.5.1/shgo/_shgo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 18:26:57.657221 shgo-0.5.1/shgo/_shgo_lib/
--rw-r--r--   0 root         (0) root         (0)        0 2018-12-09 11:33:58.000000 shgo-0.5.1/shgo/_shgo_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46090 2021-05-04 14:13:05.000000 shgo-0.5.1/shgo/_shgo_lib/_complex.py
--rw-r--r--   0 root         (0) root         (0)    13965 2021-05-04 18:05:39.000000 shgo-0.5.1/shgo/_shgo_lib/_vertex.py
--rw-r--r--   0 root         (0) root         (0)    12466 2019-07-03 06:05:20.000000 shgo-0.5.1/shgo/_shgo_lib/sobol_seq.py
--rwxr-xr-x   0 root         (0) root         (0)   295548 2018-12-09 11:33:58.000000 shgo-0.5.1/shgo/_shgo_lib/sobol_vec.gz
--rw-r--r--   0 root         (0) root         (0)    26925 2018-12-09 11:33:58.000000 shgo-0.5.1/shgo/_shgo_lib/triangulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 18:26:57.657221 shgo-0.5.1/shgo/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2017-10-22 13:11:28.000000 shgo-0.5.1/shgo/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31765 2021-05-04 18:23:37.000000 shgo-0.5.1/shgo/tests/test__shgo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 18:26:57.653887 shgo-0.5.1/shgo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3416 2021-05-04 18:26:57.000000 shgo-0.5.1/shgo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      450 2021-05-04 18:26:57.000000 shgo-0.5.1/shgo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-04 18:26:57.000000 shgo-0.5.1/shgo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2017-10-17 11:26:50.000000 shgo-0.5.1/shgo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2021-05-04 18:26:57.000000 shgo-0.5.1/shgo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-05-04 18:26:57.000000 shgo-0.5.1/shgo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:27:43.374665 shgo-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2017-09-22 09:04:45.000000 shgo-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-21 10:27:43.374665 shgo-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2003 2020-10-27 10:36:08.000000 shgo-1.0.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-21 10:27:43.377998 shgo-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-21 10:27:40.000000 shgo-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:27:43.371332 shgo-1.0.0/shgo/
+-rw-r--r--   0 root         (0) root         (0)      128 2020-09-02 11:29:33.000000 shgo-1.0.0/shgo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61265 2023-02-11 21:48:20.000000 shgo-1.0.0/shgo/_shgo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:27:43.374665 shgo-1.0.0/shgo/_shgo_lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-12-09 11:33:58.000000 shgo-1.0.0/shgo/_shgo_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50374 2023-02-11 09:02:48.000000 shgo-1.0.0/shgo/_shgo_lib/_complex.py
+-rw-r--r--   0 root         (0) root         (0)    13911 2023-02-11 09:02:57.000000 shgo-1.0.0/shgo/_shgo_lib/_vertex.py
+-rw-r--r--   0 root         (0) root         (0)    12466 2019-07-03 06:05:20.000000 shgo-1.0.0/shgo/_shgo_lib/sobol_seq.py
+-rwxr-xr-x   0 root         (0) root         (0)   295548 2018-12-09 11:33:58.000000 shgo-1.0.0/shgo/_shgo_lib/sobol_vec.gz
+-rw-r--r--   0 root         (0) root         (0)    26925 2018-12-09 11:33:58.000000 shgo-1.0.0/shgo/_shgo_lib/triangulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:27:43.374665 shgo-1.0.0/shgo/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2017-10-22 13:11:28.000000 shgo-1.0.0/shgo/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37024 2023-02-11 09:06:13.000000 shgo-1.0.0/shgo/tests/test__shgo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:27:43.374665 shgo-1.0.0/shgo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-21 10:27:43.000000 shgo-1.0.0/shgo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-21 10:27:43.000000 shgo-1.0.0/shgo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 10:27:43.000000 shgo-1.0.0/shgo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2017-10-17 11:26:50.000000 shgo-1.0.0/shgo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-21 10:27:43.000000 shgo-1.0.0/shgo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-21 10:27:43.000000 shgo-1.0.0/shgo.egg-info/top_level.txt
```

### Comparing `shgo-0.5.1/LICENSE` & `shgo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shgo-0.5.1/PKG-INFO` & `shgo-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 Metadata-Version: 2.1
 Name: shgo
-Version: 0.5.1
+Version: 1.0.0
 Summary: Simplicial homology global optimisation
 Home-page: https://github.com/stefan-endres/shgo
 Author: Stefan Endres, Carl Sandrock
 Author-email: stefan.c.endres@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/Stefan-Endres/shgo.svg?branch=master
-            :target: https://travis-ci.org/Stefan-Endres/shgo
-        .. image:: https://coveralls.io/repos/github/Stefan-Endres/shgo/badge.png?branch=master
-            :target: https://coveralls.io/github/Stefan-Endres/shgo?branch=master
-        
-        Repository: https://github.com/Stefan-Endres/shgo
-        
-        Description
-        -----------
-        
-        Finds the global minimum of a function using simplicial homology global
-        optimisation (shgo_). Appropriate for solving general purpose NLP and blackbox
-        optimisation problems to global optimality (low dimensional problems).
-        The general form of an optimisation problem is given by:
-        
-        .. _shgo: https://stefan-endres.github.io/shgo/
-        
-        ::
-        
-            minimize f(x) subject to
-        
-            g_i(x) >= 0,  i = 1,...,m
-            h_j(x)  = 0,  j = 1,...,p
-        
-        where x is a vector of one or more variables. ``f(x)`` is the objective
-        function ``R^n -> R``, ``g_i(x)`` are the inequality constraints.
-        ``h_j(x)`` are the equality constrains.
-        
-        
-        Installation
-        ------------
-        Stable:
-        
-        .. code::
-        
-            $ pip install shgo
-            
-        Latest:
-        
-        .. code::
-        
-            $ git clone https://github.com/Stefan-Endres/shgo
-            $ cd shgo
-            $ python setup.py install
-            $ python setup.py test
-        
-        Documentation
-        -------------
-        The project website https://stefan-endres.github.io/shgo/ contains more detailed examples, notes and performance profiles.
-        
-        Quick example
-        -------------
-        
-        Consider the problem of minimizing the Rosenbrock function. This function is implemented in ``rosen`` in ``scipy.optimize``
-        
-        .. code:: python
-        
-            >>> from scipy.optimize import rosen
-            >>> from shgo import shgo
-            >>> bounds = [(0,2), (0, 2), (0, 2), (0, 2), (0, 2)]
-            >>> result = shgo(rosen, bounds)
-            >>> result.x, result.fun
-            (array([ 1.,  1.,  1.,  1.,  1.]), 2.9203923741900809e-18)
-        
-        Note that bounds determine the dimensionality of the objective function and is therefore a required input, however you can specify empty bounds using ``None`` or objects like numpy.inf which will be converted to large float numbers.
-        
-        
 Keywords: optimization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/Stefan-Endres/shgo.svg?branch=master
+    :target: https://travis-ci.org/Stefan-Endres/shgo
+.. image:: https://coveralls.io/repos/github/Stefan-Endres/shgo/badge.png?branch=master
+    :target: https://coveralls.io/github/Stefan-Endres/shgo?branch=master
+
+Repository: https://github.com/Stefan-Endres/shgo
+
+Description
+-----------
+
+Finds the global minimum of a function using simplicial homology global
+optimisation (shgo_). Appropriate for solving general purpose NLP and blackbox
+optimisation problems to global optimality (low dimensional problems).
+The general form of an optimisation problem is given by:
+
+.. _shgo: https://stefan-endres.github.io/shgo/
+
+::
+
+    minimize f(x) subject to
+
+    g_i(x) >= 0,  i = 1,...,m
+    h_j(x)  = 0,  j = 1,...,p
+
+where x is a vector of one or more variables. ``f(x)`` is the objective
+function ``R^n -> R``, ``g_i(x)`` are the inequality constraints.
+``h_j(x)`` are the equality constrains.
+
+
+Installation
+------------
+Stable:
+
+.. code::
+
+    $ pip install shgo
+    
+Latest:
+
+.. code::
+
+    $ git clone https://github.com/Stefan-Endres/shgo
+    $ cd shgo
+    $ python setup.py install
+    $ python setup.py test
+
+Documentation
+-------------
+The project website https://stefan-endres.github.io/shgo/ contains more detailed examples, notes and performance profiles.
+
+Quick example
+-------------
+
+Consider the problem of minimizing the Rosenbrock function. This function is implemented in ``rosen`` in ``scipy.optimize``
+
+.. code:: python
+
+    >>> from scipy.optimize import rosen
+    >>> from shgo import shgo
+    >>> bounds = [(0,2), (0, 2), (0, 2), (0, 2), (0, 2)]
+    >>> result = shgo(rosen, bounds)
+    >>> result.x, result.fun
+    (array([ 1.,  1.,  1.,  1.,  1.]), 2.9203923741900809e-18)
+
+Note that bounds determine the dimensionality of the objective function and is therefore a required input, however you can specify empty bounds using ``None`` or objects like numpy.inf which will be converted to large float numbers.
+
```

### Comparing `shgo-0.5.1/README.rst` & `shgo-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `shgo-0.5.1/setup.py` & `shgo-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Get the long description from the README file
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 
 setup(name='shgo',
-      version='0.5.1',
+      version='1.0.0',
       description='Simplicial homology global optimisation',
       url='https://github.com/stefan-endres/shgo',
       author='Stefan Endres, Carl Sandrock',
       author_email='stefan.c.endres@gmail.com',
       license='MIT',
       packages=['shgo', 'shgo._shgo_lib', 'shgo.tests'],
       package_data={'shgo._shgo_lib': ['sobol_vec.gz']},
@@ -39,15 +39,11 @@
           'Topic :: Scientific/Engineering :: Mathematics',
 
           # Pick your license as you wish (should match "license" above)
           'License :: OSI Approved :: MIT License',
 
           # Specify the Python versions you support here. In particular, ensure
           # that you indicate whether you support Python 2, Python 3 or both.
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3'
       ],
       test_suite='shgo.tests.test__shgo',
       zip_safe=False)
```

### Comparing `shgo-0.5.1/shgo/_shgo.py` & `shgo-1.0.0/shgo/_shgo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-"""
-shgo: The simplicial homology global optimisation algorithm
-"""
-
-# Std. library imports
-from __future__ import division, print_function, absolute_import
+"""shgo: The simplicial homology global optimisation algorithm."""
 from collections import namedtuple
 import time
 import logging
 import warnings
-
 import sys
 
-# Scientific python imports
 import numpy as np
+
 from scipy import spatial
-from scipy.optimize import OptimizeResult, minimize#, MemoizeJac
-# Library imports
-from shgo._shgo_lib import sobol_seq
-from shgo._shgo_lib._complex import Complex
-__all__ = ['shgo', 'SHGO']
+from scipy.optimize import OptimizeResult, minimize, Bounds
+from scipy.optimize._optimize import MemoizeJac
+from scipy.optimize._constraints import new_bounds_to_old
+from scipy._lib._util import _FunctionWrapper
+
+#from scipy.optimize._shgo_lib._complex import Complex
+from ._shgo_lib._complex import Complex
 
-#TODO: Add symmetry contraints for the random sampling (?)
+__all__ = ['shgo', 'SHGO']
 
 
-def shgo(func, bounds, args=(), constraints=None, n=100, iters=1, callback=None,
-         minimizer_kwargs=None, options=None, sampling_method='simplicial',
-         workers=None):
+def shgo(
+    func, bounds, args=(), constraints=None, n=100, iters=1, callback=None,
+    minimizer_kwargs=None, options=None, sampling_method='simplicial', *,
+    workers=1
+):
     """
     Finds the global minimum of a function using SHG optimization.
 
     SHGO stands for "simplicial homology global optimization".
 
     Parameters
     ----------
     func : callable
         The objective function to be minimized.  Must be in the form
         ``f(x, *args)``, where ``x`` is the argument in the form of a 1-D array
         and ``args`` is a tuple of any additional fixed parameters needed to
         completely specify the function.
-    bounds : sequence
-        Bounds for variables.  ``(min, max)`` pairs for each element in ``x``,
-        defining the lower and upper bounds for the optimizing argument of
-        `func`. It is required to have ``len(bounds) == len(x)``.
-        ``len(bounds)`` is used to determine the number of parameters in ``x``.
-        Use ``None`` for one of min or max when there is no bound in that
-        direction. By default bounds are ``(None, None)``.
+    bounds : sequence or `Bounds`
+        Bounds for variables. There are two ways to specify the bounds:
+
+        1. Instance of `Bounds` class.
+        2. Sequence of ``(min, max)`` pairs for each element in `x`.
+
     args : tuple, optional
         Any additional fixed parameters needed to completely specify the
         objective function.
     constraints : dict or sequence of dict, optional
         Constraints definition.
         Function(s) ``R**n`` in the form::
 
@@ -81,43 +78,49 @@
            means that ``constraints`` will not be added so if equality
            constraints and so forth need to be added then the inequality
            functions in ``constraints`` need to be added to
            ``minimizer_kwargs`` too).
 
     n : int, optional
         Number of sampling points used in the construction of the simplicial
-        complex. Note that this argument is only used for ``sobol`` and other
-        arbitrary `sampling_methods`.
+        complex. For the default ``simplicial`` sampling method 2**dim + 1
+        sampling points are generated instead of the default `n=100`. For all
+        other specified values `n` sampling points are generated. For
+        ``sobol``, ``halton`` and other arbitrary `sampling_methods` `n=100` or
+         another speciefied number of sampling points are generated.
     iters : int, optional
-        Number of iterations used in the construction of the simplicial complex.
+        Number of iterations used in the construction of the simplicial
+        complex. Default is 1.
     callback : callable, optional
         Called after each iteration, as ``callback(xk)``, where ``xk`` is the
         current parameter vector.
     minimizer_kwargs : dict, optional
         Extra keyword arguments to be passed to the minimizer
         ``scipy.optimize.minimize`` Some important options could be:
 
             * method : str
-                The minimization method (e.g. ``SLSQP``).
+                The minimization method. If not given, chosen to be one of
+                BFGS, L-BFGS-B, SLSQP, depending on whether or not the
+                problem has constraints or bounds.
             * args : tuple
                 Extra arguments passed to the objective function (``func``) and
                 its derivatives (Jacobian, Hessian).
             * options : dict, optional
                 Note that by default the tolerance is specified as
                 ``{ftol: 1e-12}``
 
     options : dict, optional
         A dictionary of solver options. Many of the options specified for the
         global routine are also passed to the scipy.optimize.minimize routine.
         The options that are also passed to the local routine are marked with
         "(L)".
 
         Stopping criteria, the algorithm will terminate if any of the specified
-        criteria are met. However, the default algorithm does not require any to
-        be specified:
+        criteria are met. However, the default algorithm does not require any
+        to be specified:
 
         * maxfev : int (L)
             Maximum number of function evaluations in the feasible domain.
             (Note only methods that support this option will terminate
             the routine at precisely exact specified value. Otherwise the
             criterion will only terminate during a global iteration)
         * f_min
@@ -142,26 +145,44 @@
             function (after adequate sampling points each of these subdomains
             contain a unique global minimum). If the difference in the hgr is 0
             between iterations for ``maxhgrd`` specified iterations the
             algorithm will terminate.
 
         Objective function knowledge:
 
-        * symmetry : list or None
-            Specify True if the objective function contains symmetric variables.
-            The search space (and therefore performance) is decreased by O(n!).
+        * symmetry : list or bool
+            Specify if the objective function contains symmetric variables.
+            The search space (and therefore performance) is decreased by up to
+            O(n!) times in the fully symmetric case. If `True` is specified
+            then all variables will be set symmetric to the first variable.
+            Default
+            is set to False.
+
+            E.g.  f(x) = (x_1 + x_2 + x_3) + (x_4)**2 + (x_5)**2 + (x_6)**2
+
+            In this equation x_2 and x_3 are symmetric to x_1, while x_5 and
+            x_6 are symmetric to x_4, this can be specified to the solver as:
+
+            symmetry = [0,  # Variable 1
+                        0,  # symmetric to variable 1
+                        0,  # symmetric to variable 1
+                        3,  # Variable 4
+                        3,  # symmetric to variable 4
+                        3,  # symmetric to variable 4
+                        ]
 
         * jac : bool or callable, optional
             Jacobian (gradient) of objective function. Only for CG, BFGS,
             Newton-CG, L-BFGS-B, TNC, SLSQP, dogleg, trust-ncg. If ``jac`` is a
-            boolean and is True, ``fun`` is assumed to return the gradient along
-            with the objective function. If False, the gradient will be
+            boolean and is True, ``fun`` is assumed to return the gradient
+            along with the objective function. If False, the gradient will be
             estimated numerically. ``jac`` can also be a callable returning the
             gradient of the objective. In this case, it must accept the same
-            arguments as ``fun``. (Passed to `scipy.optimize.minmize` automatically)
+            arguments as ``fun``. (Passed to `scipy.optimize.minmize`
+            automatically)
 
         * hess, hessp : callable, optional
             Hessian (matrix of second-order derivatives) of objective function
             or Hessian of objective function times an arbitrary vector p.
             Only for Newton-CG, dogleg, trust-ncg. Only one of ``hessp`` or
             ``hess`` needs to be given. If ``hess`` is provided, then
             ``hessp`` will be ignored. If neither ``hess`` nor ``hessp`` is
@@ -170,48 +191,48 @@
             times an arbitrary vector. (Passed to `scipy.optimize.minmize`
             automatically)
 
         Algorithm settings:
 
         * minimize_every_iter : bool
             If True then promising global sampling points will be passed to a
-            local minimisation routine every iteration. If False then only the
-            final minimiser pool will be run. Defaults to False.
+            local minimization routine every iteration. If True then only the
+            final minimizer pool will be run. Defaults to True.
         * local_iter : int
-            Only evaluate a few of the best minimiser pool candidates every
+            Only evaluate a few of the best minimizer pool candidates every
             iteration. If False all potential points are passed to the local
-            minimisation routine.
-        * infty_constraints: bool
+            minimization routine.
+        * infty_constraints : bool
             If True then any sampling points generated which are outside will
             the feasible domain will be saved and given an objective function
             value of ``inf``. If False then these points will be discarded.
             Using this functionality could lead to higher performance with
             respect to function evaluations before the global minimum is found,
             specifying False will use less memory at the cost of a slight
             decrease in performance. Defaults to True.
 
         Feedback:
 
         * disp : bool (L)
             Set to True to print convergence messages.
 
     sampling_method : str or function, optional
-        Current built in sampling method options are ``sobol`` and
-        ``simplicial``. The default ``simplicial`` uses less memory and provides
-        the theoretical guarantee of convergence to the global minimum in finite
-        time. The ``sobol`` method is faster in terms of sampling point
-        generation at the cost of higher memory resources and the loss of
+        Current built in sampling method options are ``halton``, ``sobol`` and
+        ``simplicial``. The default ``simplicial`` provides
+        the theoretical guarantee of convergence to the global minimum in
+        finite time. ``halton`` and ``sobol`` method are faster in terms of
+        sampling point generation at the cost of the loss of
         guaranteed convergence. It is more appropriate for most "easier"
         problems where the convergence is relatively fast.
         User defined sampling functions must accept two arguments of ``n``
         sampling points of dimension ``dim`` per call and output an array of
         sampling points with shape `n x dim`.
 
     workers : int  optional
-        Uses `multiprocessing.Pool <multiprocessing>`) to sample and run the 
+        Uses `multiprocessing.Pool <multiprocessing>`) to sample and run the
         local serial minimizatons in parrallel.
 
     Returns
     -------
     res : OptimizeResult
         The optimization result represented as a `OptimizeResult` object.
         Important attributes are:
@@ -221,22 +242,22 @@
         ``funl`` the function output at the corresponding local solutions,
         ``success`` a Boolean flag indicating if the optimizer exited
         successfully,
         ``message`` which describes the cause of the termination,
         ``nfev`` the total number of objective function evaluations including
         the sampling calls,
         ``nlfev`` the total number of objective function evaluations
-        culminating from all local search optimisations,
+        culminating from all local search optimizations,
         ``nit`` number of iterations performed by the global routine.
 
     Notes
     -----
-    Global optimization using simplicial homology global optimisation [1]_.
-    Appropriate for solving general purpose NLP and blackbox optimisation
-    problems to global optimality (low dimensional problems).
+    Global optimization using simplicial homology global optimization [1]_.
+    Appropriate for solving general purpose NLP and blackbox optimization
+    problems to global optimality (low-dimensional problems).
 
     In general, the optimization problems are of the form::
 
         minimize f(x) subject to
 
         g_i(x) >= 0,  i = 1,...,m
         h_j(x)  = 0,  j = 1,...,p
@@ -245,149 +266,146 @@
     function ``R^n -> R``, ``g_i(x)`` are the inequality constraints, and
     ``h_j(x)`` are the equality constraints.
 
     Optionally, the lower and upper bounds for each element in x can also be
     specified using the `bounds` argument.
 
     While most of the theoretical advantages of SHGO are only proven for when
-    ``f(x)`` is a Lipschitz smooth function. The algorithm is also proven to
+    ``f(x)`` is a Lipschitz smooth function, the algorithm is also proven to
     converge to the global optimum for the more general case where ``f(x)`` is
     non-continuous, non-convex and non-smooth, if the default sampling method
     is used [1]_.
 
     The local search method may be specified using the ``minimizer_kwargs``
-    parameter which is passed on to ``scipy.optimize.minimize``. By default
-    the ``SLSQP`` method is used. In general it is recommended to use the
+    parameter which is passed on to ``scipy.optimize.minimize``. By default,
+    the ``SLSQP`` method is used. In general, it is recommended to use the
     ``SLSQP`` or ``COBYLA`` local minimization if inequality constraints
     are defined for the problem since the other methods do not use constraints.
 
-    The ``sobol`` method points are generated using the Sobol (1967) [2]_
-    sequence. The primitive polynomials and various sets of initial direction
-    numbers for generating Sobol sequences is provided by [3]_ by Frances Kuo
-    and Stephen Joe. The original program sobol.cc (MIT) is available and
-    described at http://web.maths.unsw.edu.au/~fkuo/sobol/ translated to
-    Python 3 by Carl Sandrock 2016-03-31.
+    The ``halton`` and ``sobol`` method points are generated using
+    `scipy.stats.qmc`. Any other QMC method could be used.
 
     References
     ----------
     .. [1] Endres, SC, Sandrock, C, Focke, WW (2018) "A simplicial homology
-           algorithm for lipschitz optimisation", Journal of Global Optimization.
-    .. [2] Sobol, IM (1967) "The distribution of points in a cube and the
-           approximate evaluation of integrals", USSR Comput. Math. Math. Phys.
-           7, 86-112.
-    .. [3] Joe, SW and Kuo, FY (2008) "Constructing Sobol sequences with
+           algorithm for lipschitz optimisation", Journal of Global
+           Optimization.
+    .. [2] Joe, SW and Kuo, FY (2008) "Constructing Sobol' sequences with
            better  two-dimensional projections", SIAM J. Sci. Comput. 30,
            2635-2654.
-    .. [4] Hoch, W and Schittkowski, K (1981) "Test examples for nonlinear
-           programming codes", Lecture Notes in Economics and mathematical
+    .. [3] Hock, W and Schittkowski, K (1981) "Test examples for nonlinear
+           programming codes", Lecture Notes in Economics and Mathematical
            Systems, 187. Springer-Verlag, New York.
            http://www.ai7.uni-bayreuth.de/test_problem_coll.pdf
-    .. [5] Wales, DJ (2015) "Perspective: Insight into reaction coordinates and
+    .. [4] Wales, DJ (2015) "Perspective: Insight into reaction coordinates and
            dynamics from the potential energy landscape",
            Journal of Chemical Physics, 142(13), 2015.
 
     Examples
     --------
     First consider the problem of minimizing the Rosenbrock function, `rosen`:
 
     >>> from scipy.optimize import rosen, shgo
     >>> bounds = [(0,2), (0, 2), (0, 2), (0, 2), (0, 2)]
     >>> result = shgo(rosen, bounds)
     >>> result.x, result.fun
-    (array([ 1.,  1.,  1.,  1.,  1.]), 2.9203923741900809e-18)
+    (array([1., 1., 1., 1., 1.]), 2.920392374190081e-18)
 
     Note that bounds determine the dimensionality of the objective
     function and is therefore a required input, however you can specify
     empty bounds using ``None`` or objects like ``np.inf`` which will be
     converted to large float numbers.
 
     >>> bounds = [(None, None), ]*4
     >>> result = shgo(rosen, bounds)
     >>> result.x
-    array([ 0.99999851,  0.99999704,  0.99999411,  0.9999882 ])
+    array([0.99999851, 0.99999704, 0.99999411, 0.9999882 ])
 
-    Next we consider the Eggholder function, a problem with several local
+    Next, we consider the Eggholder function, a problem with several local
     minima and one global minimum. We will demonstrate the use of arguments and
     the capabilities of `shgo`.
     (https://en.wikipedia.org/wiki/Test_functions_for_optimization)
 
+    >>> import numpy as np
     >>> def eggholder(x):
     ...     return (-(x[1] + 47.0)
     ...             * np.sin(np.sqrt(abs(x[0]/2.0 + (x[1] + 47.0))))
     ...             - x[0] * np.sin(np.sqrt(abs(x[0] - (x[1] + 47.0))))
     ...             )
     ...
     >>> bounds = [(-512, 512), (-512, 512)]
 
-    `shgo` has two built-in low discrepancy sampling sequences.  First we will
-    input 30 initial sampling points of the Sobol sequence:
+    `shgo` has built-in low discrepancy sampling sequences. First, we will
+    input 64 initial sampling points of the *Sobol'* sequence:
 
-    >>> result = shgo(eggholder, bounds, n=30, sampling_method='sobol')
+    >>> result = shgo(eggholder, bounds, n=64, sampling_method='sobol')
     >>> result.x, result.fun
-    (array([ 512.        ,  404.23180542]), -959.64066272085051)
+    (array([512.        , 404.23180824]), -959.6406627208397)
 
     `shgo` also has a return for any other local minima that was found, these
     can be called using:
 
     >>> result.xl
-    array([[ 512.        ,  404.23180542],
-           [ 283.07593402, -487.12566542],
+    array([[ 512.        ,  404.23180824],
+           [ 283.0759062 , -487.12565635],
            [-294.66820039, -462.01964031],
-           [-105.87688985,  423.15324143],
-           [-242.97923629,  274.38032063],
+           [-105.87688911,  423.15323845],
+           [-242.97926   ,  274.38030925],
            [-506.25823477,    6.3131022 ],
-           [-408.71981195, -156.10117154],
-           [ 150.23210485,  301.31378508],
-           [  91.00922754, -391.28375925],
-           [ 202.8966344 , -269.38042147],
-           [ 361.66625957, -106.96490692],
-           [-219.40615102, -244.06022436],
-           [ 151.59603137, -100.61082677]])
+           [-408.71980731, -156.10116949],
+           [ 150.23207937,  301.31376595],
+           [  91.00920901, -391.283763  ],
+           [ 202.89662724, -269.38043241],
+           [ 361.66623976, -106.96493868],
+           [-219.40612786, -244.06020508]])
 
     >>> result.funl
     array([-959.64066272, -718.16745962, -704.80659592, -565.99778097,
            -559.78685655, -557.36868733, -507.87385942, -493.9605115 ,
-           -426.48799655, -421.15571437, -419.31194957, -410.98477763,
-           -202.53912972])
+           -426.48799655, -421.15571437, -419.31194957, -410.98477763])
 
     These results are useful in applications where there are many global minima
     and the values of other global minima are desired or where the local minima
     can provide insight into the system (for example morphologies
-    in physical chemistry [5]_).
+    in physical chemistry [4]_).
 
     If we want to find a larger number of local minima, we can increase the
     number of sampling points or the number of iterations. We'll increase the
-    number of sampling points to 60 and the number of iterations from the
-    default of 1 to 5. This gives us 60 x 5 = 300 initial sampling points.
+    number of sampling points to 64 and the number of iterations from the
+    default of 1 to 3. Using ``simplicial`` this would have given us
+    64 x 3 = 192 initial sampling points.
 
-    >>> result_2 = shgo(eggholder, bounds, n=60, iters=5, sampling_method='sobol')
+    >>> result_2 = shgo(eggholder,
+    ...                 bounds, n=64, iters=3, sampling_method='sobol')
     >>> len(result.xl), len(result_2.xl)
-    (13, 39)
+    (12, 20)
 
-    Note the difference between, e.g., ``n=180, iters=1`` and ``n=60, iters=3``.
+    Note the difference between, e.g., ``n=192, iters=1`` and ``n=64,
+    iters=3``.
     In the first case the promising points contained in the minimiser pool
-    is processed only once. In the latter case it is processed every 60 sampling
-    points for a total of 3 times.
+    are processed only once. In the latter case it is processed every 64
+    sampling points for a total of 3 times.
 
     To demonstrate solving problems with non-linear constraints consider the
-    following example from Hock and Schittkowski problem 73 (cattle-feed) [4]_::
+    following example from Hock and Schittkowski problem 73 (cattle-feed)
+    [3]_::
 
         minimize: f = 24.55 * x_1 + 26.75 * x_2 + 39 * x_3 + 40.50 * x_4
 
-        subject to: 2.3 * x_1 + 5.6 * x_2 + 11.1 * x_3 + 1.3 * x_4 - 5     >= 0,
+        subject to: 2.3 * x_1 + 5.6 * x_2 + 11.1 * x_3 + 1.3 * x_4 - 5    >= 0,
 
                     12 * x_1 + 11.9 * x_2 + 41.8 * x_3 + 52.1 * x_4 - 21
                         -1.645 * sqrt(0.28 * x_1**2 + 0.19 * x_2**2 +
-                                      20.5 * x_3**2 + 0.62 * x_4**2)       >= 0,
+                                      20.5 * x_3**2 + 0.62 * x_4**2)      >= 0,
 
-                    x_1 + x_2 + x_3 + x_4 - 1                              == 0,
+                    x_1 + x_2 + x_3 + x_4 - 1                             == 0,
 
                     1 >= x_i >= 0 for all i
 
-    The approximate answer given in [4]_ is::
+    The approximate answer given in [3]_ is::
 
         f([0.6355216, -0.12e-11, 0.3127019, 0.05177655]) = 29.894378
 
     >>> def f(x):  # (cattle-feed)
     ...     return 24.55*x[0] + 26.75*x[1] + 39*x[2] + 40.50*x[3]
     ...
     >>> def g1(x):
@@ -402,94 +420,103 @@
     >>> def h1(x):
     ...     return x[0] + x[1] + x[2] + x[3] - 1  # == 0
     ...
     >>> cons = ({'type': 'ineq', 'fun': g1},
     ...         {'type': 'ineq', 'fun': g2},
     ...         {'type': 'eq', 'fun': h1})
     >>> bounds = [(0, 1.0),]*4
-    >>> res = shgo(f, bounds, iters=3, constraints=cons)
+    >>> res = shgo(f, bounds, n=150, constraints=cons)
     >>> res
+     message: Optimization terminated successfully.
+     success: True
          fun: 29.894378159142136
-        funl: array([29.89437816])
-     message: 'Optimization terminated successfully.'
-        nfev: 119
-         nit: 3
-       nlfev: 40
-       nlhev: 0
+        funl: [ 2.989e+01]
+           x: [ 6.355e-01  1.137e-13  3.127e-01  5.178e-02]
+          xl: [[ 6.355e-01  1.137e-13  3.127e-01  5.178e-02]]
+         nit: 1
+        nfev: 142
+       nlfev: 35
        nljev: 5
-     success: True
-           x: array([6.35521569e-01, 1.13700270e-13, 3.12701881e-01, 5.17765506e-02])
-          xl: array([[6.35521569e-01, 1.13700270e-13, 3.12701881e-01, 5.17765506e-02]])
+       nlhev: 0
+
+
 
     >>> g1(res.x), g2(res.x), h1(res.x)
-    (-5.0626169922907138e-14, -2.9594104944408173e-12, 0.0)
+    (-5.062616992290714e-14, -2.9594104944408173e-12, 0.0)
 
     """
+    # if necessary, convert bounds class to old bounds
+    if isinstance(bounds, Bounds):
+        bounds = new_bounds_to_old(bounds.lb, bounds.ub, len(bounds.lb))
+
     # Initiate SHGO class
     shc = SHGO(func, bounds, args=args, constraints=constraints, n=n,
                iters=iters, callback=callback,
                minimizer_kwargs=minimizer_kwargs,
                options=options, sampling_method=sampling_method,
                workers=workers)
 
     # Run the algorithm, process results and test success
     shc.iterate_all()
 
     if not shc.break_routine:
         if shc.disp:
-            print("Successfully completed construction of complex.")
+            logging.info("Successfully completed construction of complex.")
 
     # Test post iterations success
     if len(shc.LMC.xl_maps) == 0:
         # If sampling failed to find pool, return lowest sampled point
         # with a warning
         shc.find_lowest_vertex()
         shc.break_routine = True
-        shc.fail_routine(mes="Failed to find a feasible minimiser point. "
+        shc.fail_routine(mes="Failed to find a feasible minimizer point. "
                              "Lowest sampling point = {}".format(shc.f_lowest))
         shc.res.fun = shc.f_lowest
         shc.res.x = shc.x_lowest
         shc.res.nfev = shc.fn
         shc.res.tnev = shc.n_sampled
+    else:
+        # Test that the optimal solutions do not violate any constraints
+        pass  # TODO
 
     # Confirm the routine ran successfully
     if not shc.break_routine:
         shc.res.message = 'Optimization terminated successfully.'
         shc.res.success = True
 
     # Return the final results
     return shc.res
 
 
-class SHGO(object):
+class SHGO:
     def __init__(self, func, bounds, args=(), constraints=None, n=None,
                  iters=None, callback=None, minimizer_kwargs=None,
                  options=None, sampling_method='simplicial', workers=1):
-
+        from scipy.stats import qmc
         # Input checks
-        methods = ['sobol', 'simplicial']
+        methods = ['halton', 'sobol', 'simplicial']
         if isinstance(sampling_method, str) and sampling_method not in methods:
             raise ValueError(("Unknown sampling_method specified."
                               " Valid methods: {}").format(', '.join(methods)))
 
-        # Initiate class
-        
         # Split obj func if given with Jac
         try:
-            if ((minimizer_kwargs['jac'] is True) and 
-               (not callable(minimizer_kwargs['jac']))):
+            if ((minimizer_kwargs['jac'] is True) and
+                    (not callable(minimizer_kwargs['jac']))):
                 self.func = MemoizeJac(func)
                 jac = self.func.derivative
                 minimizer_kwargs['jac'] = jac
-                func = self.func  #.fun
+                func = self.func  # .fun
             else:
                 self.func = func  # Normal definition of objective function
         except (TypeError, KeyError):
             self.func = func  # Normal definition of objective function
 
+        # Initiate class
+        self.func = _FunctionWrapper(func, args)
         self.bounds = bounds
         self.args = args
         self.callback = callback
 
         # Bounds
         abound = np.array(bounds, float)
         self.dim = np.shape(abound)[0]  # Dimensionality of problem
@@ -510,16 +537,16 @@
         # Constraints
         # Process constraint dict sequence:
         self.constraints = constraints
         if constraints is not None:
             self.min_cons = constraints
             self.g_cons = []
             self.g_args = []
-            if (not isinstance(constraints, tuple)) and (not
-            isinstance(constraints, list)):
+            if (type(constraints) is not tuple) and (type(constraints)
+                                                     is not list):
                 constraints = (constraints,)
 
             for cons in constraints:
                 if cons['type'] == 'ineq':
                     self.g_cons.append(cons['fun'])
                     try:
                         self.g_args.append(cons['args'])
@@ -529,16 +556,15 @@
             self.g_args = tuple(self.g_args)
         else:
             self.g_cons = None
             self.g_args = None
 
         # Define local minimization keyword arguments
         # Start with defaults
-        self.minimizer_kwargs = {'args': self.args,
-                                 'method': 'SLSQP',
+        self.minimizer_kwargs = {'method': 'SLSQP',
                                  'bounds': self.bounds,
                                  'options': {},
                                  'callback': self.callback
                                  }
         if minimizer_kwargs is not None:
             # Overwrite with supplied values
             self.minimizer_kwargs.update(minimizer_kwargs)
@@ -594,14 +620,15 @@
             'tnc': ['jac', 'bounds'],
             'cobyla': ['constraints'],
             'slsqp': ['jac', 'bounds', 'constraints'],
             'dogleg': ['jac', 'hess'],
             'trust-ncg': ['jac', 'hess', 'hessp'],
             'trust-krylov': ['jac', 'hess', 'hessp'],
             'trust-exact': ['jac', 'hess'],
+            'trust-constr': ['jac', 'hess', 'hessp'],
         }
         method = self.minimizer_kwargs['method']
         self.min_solver_args += solver_args[method.lower()]
 
         # Only retain the known arguments
         def _restrict_to_keys(dictionary, goodkeys):
             """Remove keys from dictionary if not in goodkeys - inplace"""
@@ -621,65 +648,78 @@
         self.iters_done = 0  # Iterations completed
         self.n = n  # Sampling points per iteration
         self.nc = 0  # n  # Sampling points to sample in current iteration
         self.n_prc = 0  # Processed points (used to track Delaunay iters)
         self.n_sampled = 0  # To track no. of sampling points already generated
         self.fn = 0  # Number of feasible sampling points evaluations performed
         self.hgr = 0  # Homology group rank
+        # Initially attempt to build the triangulation incrementally:
+        self.qhull_incremental = True
 
         # Default settings if no sampling criteria.
-        if (self.n is None) and (self.iters is None):
-            self.n = 100
+        if (self.n is None) and (self.iters is None) \
+                and (sampling_method == 'simplicial'):
+            self.n = 2 ** self.dim + 1
             self.nc = 0  # self.n
         if self.iters is None:
             self.iters = 1
         if (self.n is None) and not (sampling_method == 'simplicial'):
-            self.n = 100
+            self.n = self.n = 100
             self.nc = 0  # self.n
+        if (self.n == 100) and (sampling_method == 'simplicial'):
+            self.n = 2 ** self.dim + 1
 
         if not ((self.maxiter is None) and (self.maxfev is None) and (
                 self.maxev is None)
                 and (self.minhgrd is None) and (self.f_min_true is None)):
             self.iters = None
 
         # Set complex construction mode based on a provided stopping criteria:
         # Initialise sampling Complex and function cache
+        # Note that sfield_args=() since args are already wrapped in self.func
+        # using the_FunctionWrapper class.
         self.HC = Complex(dim=self.dim, domain=self.bounds,
-                          sfield=self.func, sfield_args=self.args,
+                          sfield=self.func, sfield_args=(),
                           symmetry=self.symmetry,
                           constraints=self.constraints,
-                          # constraints=self.g_cons,
-                          constraints_args=self.g_args,
                           workers=workers)
 
         # Choose complex constructor
         if sampling_method == 'simplicial':
             self.iterate_complex = self.iterate_hypercube
             self.sampling_method = sampling_method
 
-        elif sampling_method == 'sobol' or not isinstance(sampling_method, str):
+        elif sampling_method in ['halton', 'sobol'] or \
+                not isinstance(sampling_method, str):
             self.iterate_complex = self.iterate_delaunay
             # Sampling method used
-            if sampling_method == 'sobol':
-                self.sampling_method = sampling_method
-                self.sampling = self.sampling_sobol
-                self.Sobol = sobol_seq.Sobol()  # Init Sobol class
-                if self.dim < 40:
-                    self.sobol_points = self.sobol_points_40
+            if sampling_method in ['halton', 'sobol']:
+                if sampling_method == 'sobol':
+                    self.n = int(2 ** np.ceil(np.log2(self.n)))
+                    # self.n #TODO: Should always be self.n, this is
+                    # unacceptable for shgo, check that nfev behaves as
+                    # expected.
+                    self.nc = 0
+                    self.sampling_method = 'sobol'
+                    self.qmc_engine = qmc.Sobol(d=self.dim, scramble=False,
+                                                seed=0)
                 else:
-                    self.sobol_points = self.sobol_points_10k
+                    self.sampling_method = 'halton'
+                    self.qmc_engine = qmc.Halton(d=self.dim, scramble=True,
+                                                 seed=0)
+
+                def sampling_method(n, d):
+                    return self.qmc_engine.random(n)
+
             else:
                 # A user defined sampling method:
-                # self.sampling_points = sampling_method
-                self.sampling = self.sampling_custom
-                self.sampling_function = sampling_method  # F(n, d)
                 self.sampling_method = 'custom'
 
-            # QHull options
-            self.qhull_incremental = True
+            self.sampling = self.sampling_custom
+            self.sampling_function = sampling_method  # F(n, d)
 
         # Local controls
         self.stop_l_iter = False  # Local minimisation iterations
         self.stop_complex_iter = False  # Sampling iterations
 
         # Initiate storage objects used in algorithm classes
         self.minimizer_pool = []
@@ -706,15 +746,25 @@
         options : dict
 
         Returns
         -------
         None
 
         """
+        # Update 'options' dict passed to optimize.minimize
+        # Do this first so we don't mutate `options` below.
         self.minimizer_kwargs['options'].update(options)
+
+        # Ensure that 'jac', 'hess', and 'hessp' are passed directly to
+        # `minimize` as keywords, not as part of its 'options' dictionary.
+        for opt in ['jac', 'hess', 'hessp']:
+            if opt in self.minimizer_kwargs['options']:
+                self.minimizer_kwargs[opt] = (
+                    self.minimizer_kwargs['options'].pop(opt))
+
         # Default settings:
         self.minimize_every_iter = options.get('minimize_every_iter', True)
 
         # Algorithm limits
         # Maximum number of iterations to perform.
         self.maxiter = options.get('maxiter', None)
         # Maximum number of function evaluations in the feasible domain
@@ -731,154 +781,157 @@
             self.f_tol = options.get('f_tol', 1e-4)
         else:
             self.f_min_true = None
 
         self.minhgrd = options.get('minhgrd', None)
 
         # Objective function knowledge
-        self.symmetry = options.get('symmetry', None)
-
+        self.symmetry = options.get('symmetry', False)
+        if self.symmetry:
+            self.symmetry = [0, ]*len(self.bounds)
+        else:
+            self.symmetry = None
         # Algorithm functionality
         # Only evaluate a few of the best candiates
         self.local_iter = options.get('local_iter', False)
-
         self.infty_cons_sampl = options.get('infty_constraints', True)
 
         # Feedback
         self.disp = options.get('disp', False)
 
+    def __exit__(self, *args):
+        return self.HC.V._mapwrapper.__exit__(*args)
+
     # Iteration properties
     # Main construction loop:
     def iterate_all(self):
         """
-        Iterate for `self.iters` iterations.
+        Construct for `iters` iterations.
 
         If uniform sampling is used, every iteration adds 'n' sampling points.
 
-        Stop iterations if a stopping criteria (ex. sampling points or
+        Iterations if a stopping criteria (e.g., sampling points or
         processing time) has been met.
 
         """
         if self.disp:
-            print('Splitting first generation')
+            logging.info('Splitting first generation')
 
         while not self.stop_global:
             if self.break_routine:
                 break
             # Iterate complex, process minimisers
             self.iterate()
             self.stopping_criteria()
 
         # Build minimiser pool
-        # Final iteration only needed if pools weren't minimised every iteration
+        # Final iteration only needed if pools weren't minimised every
+        # iteration
         if not self.minimize_every_iter:
             if not self.break_routine:
-                # TODO: Improve or document ignore_globals (otherwise only the
-                #       first entry in the pool is processed)
-                self.find_minima(ignore_globals=True)
+                self.find_minima()
 
         self.res.nit = self.iters_done  # + 1
         self.fn = self.HC.V.nfev
 
-    def find_minima(self, ignore_globals=False):
+    def find_minima(self):
         """
-        Construct the minimiser pool, map the minimisers to local minima
+        Construct the minimizer pool, map the minimizers to local minima
         and sort the results into a global return object.
         """
         if self.disp:
-            print('Search for minimiser pool')
+            logging.info('Searching for minimizer pool...')
 
         self.minimizers()
-        logging.info(f'self.X_min = {self.X_min}')
+
         if len(self.X_min) != 0:
-            # Minimise the pool of minimisers with local minimisation methods
+            # Minimize the pool of minimizers with local minimization methods
             # Note that if Options['local_iter'] is an `int` instead of default
-            # value False then only that number of candidates will be minimised
-            self.minimise_pool(self.local_iter, ignore_globals)
+            # value False then only that number of candidates will be minimized
+            self.minimise_pool(self.local_iter)
             # Sort results and build the global return object
             self.sort_result()
 
             # Lowest values used to report in case of failures
             self.f_lowest = self.res.fun
             self.x_lowest = self.res.x
         else:
             self.find_lowest_vertex()
 
         if self.disp:
-            logging.info(
-                "Minimiser pool = SHGO.X_min = {}".format(self.X_min))
-            print("Minimiser pool = SHGO.X_min = {}".format(self.X_min))
-
+            logging.info(f"Minimiser pool = SHGO.X_min = {self.X_min}")
 
     def find_lowest_vertex(self):
         # Find the lowest objective function value on one of
         # the vertices of the simplicial complex
         self.f_lowest = np.inf
         for x in self.HC.V.cache:
-            logging.info(f'self.HC.V[x].f = {self.HC.V[x].f}')
             if self.HC.V[x].f < self.f_lowest:
-                logging.info(f'self.HC.V[x].f = {self.HC.V[x].f}')
+                if self.disp:
+                    logging.info(f'self.HC.V[x].f = {self.HC.V[x].f}')
                 self.f_lowest = self.HC.V[x].f
                 self.x_lowest = self.HC.V[x].x_a
-        # TODO: TEMPORARY CHECK, FIX:
         for lmc in self.LMC.cache:
             if self.LMC[lmc].f_min < self.f_lowest:
                 self.f_lowest = self.LMC[lmc].f_min
                 self.x_lowest = self.LMC[lmc].x_l
 
         if self.f_lowest == np.inf:  # no feasible point
             self.f_lowest = None
             self.x_lowest = None
 
-
     # Stopping criteria functions:
     def finite_iterations(self):
         mi = min(x for x in [self.iters, self.maxiter] if x is not None)
-        logging.info(f'Iterations done = {self.iters_done} / {mi}')
-
+        if self.disp:
+            logging.info(f'Iterations done = {self.iters_done} / {mi}')
         if self.iters is not None:
             if self.iters_done >= (self.iters):
                 self.stop_global = True
 
         if self.maxiter is not None:  # Stop for infeasible sampling
             if self.iters_done >= (self.maxiter):
                 self.stop_global = True
         return self.stop_global
 
     def finite_fev(self):
         # Finite function evals in the feasible domain
-        logging.info(f'Function evaluations done = {self.fn} / {self.maxfev}')
+        if self.disp:
+            logging.info(f'Function evaluations done = {self.fn} / {self.maxfev}')
         if self.fn >= self.maxfev:
             self.stop_global = True
         return self.stop_global
 
     def finite_ev(self):
         # Finite evaluations including infeasible sampling points
-        logging.info(f'Sampling evaluations done = {self.n_sampled} '
-                     f'/ {self.maxev}')
+        if self.disp:
+            logging.info(f'Sampling evaluations done = {self.n_sampled} '
+                         f'/ {self.maxev}')
         if self.n_sampled >= self.maxev:
             self.stop_global = True
 
     def finite_time(self):
-        logging.info(f'Time elapsed = {time.time() - self.init} '
-                     f'/ {self.maxtime}')
+        if self.disp:
+            logging.info(f'Time elapsed = {time.time() - self.init} '
+                         f'/ {self.maxtime}')
         if (time.time() - self.init) >= self.maxtime:
             self.stop_global = True
 
     def finite_precision(self):
         """
         Stop the algorithm if the final function value is known
 
         Specify in options (with ``self.f_min_true = options['f_min']``)
         and the tolerance with ``f_tol = options['f_tol']``
         """
-        # If no minimiser has been found use the lowest sampling value
+        # If no minimizer has been found use the lowest sampling value
         self.find_lowest_vertex()
-        logging.info(f'Lowest function evaluation = {self.f_lowest}')
-        logging.info(f'Specified minimum = {self.f_min_true}')
+        if self.disp:
+            logging.info(f'Lowest function evaluation = {self.f_lowest}')
+            logging.info(f'Specified minimum = {self.f_min_true}')
         # If no feasible point was return from test
         if self.f_lowest is None:
             return self.stop_global
 
         # Function to stop algorithm at specified percentage error:
         if self.f_min_true == 0.0:
             if self.f_lowest <= self.f_tol:
@@ -886,34 +939,36 @@
         else:
             pe = (self.f_lowest - self.f_min_true) / abs(self.f_min_true)
             if self.f_lowest <= self.f_min_true:
                 self.stop_global = True
                 # 2if (pe - self.f_tol) <= abs(1.0 / abs(self.f_min_true)):
                 if abs(pe) >= 2 * self.f_tol:
                     warnings.warn("A much lower value than expected f* =" +
-                                  " {} than".format(self.f_min_true) +
+                                  f" {self.f_min_true} than" +
                                   " the was found f_lowest =" +
-                                  "{} ".format(self.f_lowest))
+                                  f"{self.f_lowest} ")
             if pe <= self.f_tol:
                 self.stop_global = True
 
         return self.stop_global
 
     def finite_homology_growth(self):
-
+        """
+        Stop the algorithm if homology group rank did not grow in iteration.
+        """
         if self.LMC.size == 0:
             return  # pass on no reason to stop yet.
         self.hgrd = self.LMC.size - self.hgr
 
         self.hgr = self.LMC.size
         if self.hgrd <= self.minhgrd:
             self.stop_global = True
-
-        logging.info(f'Current homology growth = {self.hgrd} '
-                     f' (minimum growth = {self.minhgrd})')
+        if self.disp:
+            logging.info(f'Current homology growth = {self.hgrd} '
+                         f' (minimum growth = {self.minhgrd})')
         return self.stop_global
 
     def stopping_criteria(self):
         """
         Various stopping criteria ran every iteration
 
         Returns
@@ -930,146 +985,163 @@
             self.finite_ev()
         if self.maxtime is not None:
             self.finite_time()
         if self.f_min_true is not None:
             self.finite_precision()
         if self.minhgrd is not None:
             self.finite_homology_growth()
+        return self.stop_global
 
     def iterate(self):
         self.iterate_complex()
 
-        # Build minimiser pool
+        # Build minimizer pool
         if self.minimize_every_iter:
             if not self.break_routine:
-                self.find_minima()  # Process minimiser pool
+                self.find_minima()  # Process minimizer pool
 
         # Algorithm updates
         self.iters_done += 1
 
     def iterate_hypercube(self):
         """
         Iterate a subdivision of the complex
 
         Note: called with ``self.iterate_complex()`` after class initiation
         """
         # Iterate the complex
         if self.disp:
-            print('Constructing and refining simplicial complex graph '
-                  'structure')
+            logging.info('Constructing and refining simplicial complex graph '
+                         'structure')
         if self.n is None:
             self.HC.refine_all()
             self.n_sampled = self.HC.V.size()  # nevs counted
         else:
             self.HC.refine(self.n)
             self.n_sampled += self.n
 
         if self.disp:
-            print('Triangulation completed, evaluating all contraints and o'
-                  'bjective function values.')
+            logging.info('Triangulation completed, evaluating all contraints '
+                         'and objective function values.')
+
+        # Readd minimisers to complex
+        if len(self.LMC.xl_maps) > 0:
+            for xl in self.LMC.cache:
+                v = self.HC.V[xl]
+                v_near = v.star()
+                for v in v.nn:
+                    v_near = v_near.union(v.nn)
+                # Reconnect vertices to complex
+                # if self.HC.connect_vertex_non_symm(tuple(self.LMC[xl].x_l),
+                #                                   near=v_near):
+                #    continue
+                # else:
+                    # If failure to find in v_near, then search all vertices
+                    # (very expensive operation:
+                #    self.HC.connect_vertex_non_symm(tuple(self.LMC[xl].x_l)
+                #                                    )
 
         # Evaluate all constraints and functions
         self.HC.V.process_pools()
         if self.disp:
-            print('Evaluations completed.')
+            logging.info('Evaluations completed.')
 
         # feasible sampling points counted by the triangulation.py routines
         self.fn = self.HC.V.nfev
         return
 
     def iterate_delaunay(self):
         """
         Build a complex of Delaunay triangulated points
 
         Note: called with ``self.iterate_complex()`` after class initiation
         """
-        self.nc += self.n  # TODO: IS THIS CORRECT?
+        self.nc += self.n
         self.sampled_surface(infty_cons_sampl=self.infty_cons_sampl)
 
         # Add sampled points to a triangulation, construct self.Tri
         if self.disp:
-            print('Constructing and refining simplicial complex graph '
-                  'structure from sampling points.')
+            logging.info(f'self.n = {self.n}')
+            logging.info(f'self.nc = {self.nc}')
+            logging.info('Constructing and refining simplicial complex graph '
+                         'structure from sampling points.')
 
-        #TODO: Find another solution for triangulating 1D,
         if self.dim < 2:
             self.Ind_sorted = np.argsort(self.C, axis=0)
             self.Ind_sorted = self.Ind_sorted.flatten()
             tris = []
             for ind, ind_s in enumerate(self.Ind_sorted):
                 if ind > 0:
                     tris.append(self.Ind_sorted[ind - 1:ind + 1])
-                    #print(f'B[ind - 1:ind + 1] = {B[ind - 1:ind + 1]}')
 
             tris = np.array(tris)
             # Store 1D triangulation:
             self.Tri = namedtuple('Tri', ['points', 'simplices'])(self.C, tris)
             self.points = {}
         else:
             if self.C.shape[0] > self.dim + 1:  # Ensure a simplex can be built
                 self.delaunay_triangulation(n_prc=self.n_prc)
             self.n_prc = self.C.shape[0]
 
         if self.disp:
-            print('Triangulation completed, evaluating all contraints and o'
-                  'bjective function values.')
+            logging.info('Triangulation completed, evaluating all '
+                         'contraints and objective function values.')
 
-        # self.delaunay_minimizers()
         if hasattr(self, 'Tri'):
-            #TODO: PURGE OLD COMPLEX VERTICES! OR RECOMPUTE POOLS ?!
             self.HC.vf_to_vv(self.Tri.points, self.Tri.simplices)
-        #self.C
-        #self.Tri.simplices
 
         # Process all pools
-        #self.n_sampled = self.nc
         # Evaluate all constraints and functions
         if self.disp:
-            print('Triangulation completed, evaluating all contraints and o'
-                  'bjective function values.')
+            logging.info('Triangulation completed, evaluating all contraints '
+                         'and objective function values.')
 
         # Evaluate all constraints and functions
         self.HC.V.process_pools()
         if self.disp:
-            print('Evaluations completed.')
+            logging.info('Evaluations completed.')
 
         # feasible sampling points counted by the triangulation.py routines
         self.fn = self.HC.V.nfev
-        self.n_sampled = self.nc#self.HC.V.size()  # nevs counted in triangulation.py
-        #print(f'self.Tri.points= {self.Tri.points}')
-        #print(f'self.Tri.simplices = {self.Tri.simplices}')
+        self.n_sampled = self.nc  # nevs counted in triangulation
         return
 
     # Hypercube minimizers
     def minimizers(self):
         """
         Returns the indexes of all minimizers
         """
         self.minimizer_pool = []
         # Note: Can implement parallelization here
         for x in self.HC.V.cache:
+            in_LMC = False
+            if len(self.LMC.xl_maps) > 0:
+                for xlmi in self.LMC.xl_maps:
+                    if np.all(np.array(x) == np.array(xlmi)):
+                        in_LMC = True
+            if in_LMC:
+                continue
+
             if self.HC.V[x].minimiser():
                 if self.disp:
                     logging.info('=' * 60)
-                    logging.info(
-                        'v.x = {} is minimiser'.format(self.HC.V[x].x_a))
-                    logging.info('v.f = {} is minimiser'.format(self.HC.V[x].f))
+                    logging.info(f'v.x = {self.HC.V[x].x_a} is minimizer')
+                    logging.info(f'v.f = {self.HC.V[x].f} is minimizer')
                     logging.info('=' * 30)
 
                 if self.HC.V[x] not in self.minimizer_pool:
                     self.minimizer_pool.append(self.HC.V[x])
 
                 if self.disp:
-                    logging.info('Neighbours:')
+                    logging.info('Neighbors:')
                     logging.info('=' * 30)
                     for vn in self.HC.V[x].nn:
-                        logging.info('x = {} || f = {}'.format(vn.x, vn.f))
+                        logging.info(f'x = {vn.x} || f = {vn.f}')
 
                     logging.info('=' * 60)
-
         self.minimizer_pool_F = []
         self.X_min = []
         # normalized tuple in the Vertex cache
         self.X_min_cache = {}  # Cache used in hypercube sampling
 
         for v in self.minimizer_pool:
             self.X_min.append(v.x_a)
@@ -1082,78 +1154,60 @@
         # TODO: Only do this if global mode
         self.sort_min_pool()
 
         return self.X_min
 
     # Local minimisation
     # Minimiser pool processing
-    def minimise_pool(self, force_iter=False, ignore_globals=False):
+    def minimise_pool(self, force_iter=False):
         """
         This processing method can optionally minimise only the best candidate
         solutions in the minimiser pool
 
         Parameters
         ----------
         force_iter : int
-                     Number of starting minimisers to process (can be sepcified
+                     Number of starting minimizers to process (can be sepcified
                      globally or locally)
 
         """
         # Find first local minimum
         # NOTE: Since we always minimize this value regardless it is a waste to
         # build the topograph first before minimizing
         lres_f_min = self.minimize(self.X_min[0], ind=self.minimizer_pool[0])
-        logging.info(f'lres_f_min = {lres_f_min}')
-        # Trim minimised point from current minimiser set
+
+        # Trim minimized point from current minimizer set
         self.trim_min_pool(0)
 
         while not self.stop_l_iter:
-            logging.info(f'self.stop_l_iter = {self.stop_l_iter}')
             # Global stopping criteria:
-            logging.info(f'self.stop_global = {self.stop_global}')
-            logging.info(
-                f'self.stopping_criteria() = {self.stopping_criteria()}')
-            logging.info(f'self.stop_global = {self.stop_global}')
             self.stopping_criteria()
-            if not ignore_globals:
-                if self.stop_global:
-                    self.stop_l_iter = True
-                    break
-            if 0:
-                if self.f_min_true is not None:
-                    if (lres_f_min.fun - self.f_min_true) / abs(
-                            self.f_min_true) <= self.f_tol:
-                        self.stop_l_iter = True
-                        break
+
             # Note first iteration is outside loop:
             if force_iter:
-                if self.disp:
-                    logging.info(
-                        'SHGO.iters in function minimise_pool = {}'.format(
-                            loc_iter))
                 force_iter -= 1
                 if force_iter == 0:
                     self.stop_l_iter = True
                     break
 
             if np.shape(self.X_min)[0] == 0:
                 self.stop_l_iter = True
                 break
 
-            # Construct topograph from current minimiser set
-            # (NOTE: This is a very small topograph using only the miniser pool
+            # Construct topograph from current minimizer set
+            # (NOTE: This is a very small topograph using only the minizer pool
             #        , it might be worth using some graph theory tools instead.
             self.g_topograph(lres_f_min.x, self.X_min)
 
-            # Find local minimum at the miniser with the greatest euclidean
+            # Find local minimum at the miniser with the greatest Euclidean
             # distance from the current solution
             ind_xmin_l = self.Z[:, -1]
             lres_f_min = self.minimize(self.Ss[-1, :], self.minimizer_pool[-1])
-            logging.info(f'lres_f_min = {lres_f_min}')
-            # Trim minimised point from current minimiser set
+
+            # Trim minimised point from current minimizer set
             self.trim_min_pool(ind_xmin_l)
 
         # Reset controls
         self.stop_l_iter = False
         return
 
     def sort_min_pool(self):
@@ -1192,20 +1246,21 @@
     def construct_lcb_simplicial(self, v_min):
         """
         Construct locally (approximately) convex bounds
 
         Parameters
         ----------
         v_min : Vertex object
-                The minimiser vertex
+                The minimizer vertex
 
         Returns
         -------
         cbounds : list of lists
-            List of size dim with length-2 list of bounds for each dimension
+            List of size dimension with length-2 list of bounds for each
+            dimension.
 
         """
         cbounds = [[x_b_i[0], x_b_i[1]] for x_b_i in self.bounds]
         # Loop over all bounds
         for vn in v_min.nn:
             for i, x_i in enumerate(vn.x_a):
                 # Lower bound
@@ -1213,279 +1268,184 @@
                     cbounds[i][0] = x_i
 
                 # Upper bound
                 if (x_i > v_min.x_a[i]) and (x_i < cbounds[i][1]):
                     cbounds[i][1] = x_i
 
         if self.disp:
-            logging.info('cbounds found for v_min.x_a = {}'.format(v_min.x_a))
-            logging.info('cbounds = {}'.format(cbounds))
+            logging.info(f'cbounds found for v_min.x_a = {v_min.x_a}')
+            logging.info(f'cbounds = {cbounds}')
 
         return cbounds
 
     def construct_lcb_delaunay(self, v_min, ind=None):
         """
         Construct locally (approximately) convex bounds
 
         Parameters
         ----------
         v_min : Vertex object
-                The minimiser vertex
+                The minimizer vertex
 
         Returns
         -------
         cbounds : list of lists
-            List of size dim with length-2 list of bounds for each dimension
+            List of size dimension with length-2 list of bounds for each
+            dimension.
         """
         cbounds = [[x_b_i[0], x_b_i[1]] for x_b_i in self.bounds]
 
         return cbounds
 
     # Minimize a starting point locally
     def minimize(self, x_min, ind=None):
         """
         This function is used to calculate the local minima using the specified
         sampling point as a starting value.
 
         Parameters
         ----------
         x_min : vector of floats
-            Current starting point to minimise.
+            Current starting point to minimize.
 
         Returns
         -------
         lres : OptimizeResult
             The local optimization result represented as a `OptimizeResult`
             object.
         """
         # Use minima maps if vertex was already run
         if self.disp:
-            logging.info('Vertex minimiser maps = {}'.format(self.LMC.v_maps))
+            logging.info(f'Vertex minimiser maps = {self.LMC.v_maps}')
 
         if self.LMC[x_min].lres is not None:
+            logging.info(f'Found self.LMC[x_min].lres = '
+                         f'{self.LMC[x_min].lres}')
             return self.LMC[x_min].lres
 
-        # TODO: Check discarded bound rules
-
         if self.callback is not None:
-            print('Callback for '
+            logging.info('Callback for '
                   'minimizer starting at {}:'.format(x_min))
 
         if self.disp:
-            print('--- Starting '
+            logging.info('Starting '
                   'minimization at {}...'.format(x_min))
 
         if self.sampling_method == 'simplicial':
             x_min_t = tuple(x_min)
             # Find the normalized tuple in the Vertex cache:
             x_min_t_norm = self.X_min_cache[tuple(x_min_t)]
-
             x_min_t_norm = tuple(x_min_t_norm)
-
             g_bounds = self.construct_lcb_simplicial(self.HC.V[x_min_t_norm])
             if 'bounds' in self.min_solver_args:
                 self.minimizer_kwargs['bounds'] = g_bounds
+                logging.info(self.minimizer_kwargs['bounds'])
 
         else:
             g_bounds = self.construct_lcb_delaunay(x_min, ind=ind)
             if 'bounds' in self.min_solver_args:
                 self.minimizer_kwargs['bounds'] = g_bounds
+                logging.info(self.minimizer_kwargs['bounds'])
 
         if self.disp and 'bounds' in self.minimizer_kwargs:
-            print('bounds in kwarg:')
-            print(self.minimizer_kwargs['bounds'])
+            logging.info('bounds in kwarg:')
+            logging.info(self.minimizer_kwargs['bounds'])
 
         # Local minimization using scipy.optimize.minimize:
         lres = minimize(self.func, x_min, **self.minimizer_kwargs)
 
         if self.disp:
-            print('lres = {}'.format(lres))
+            logging.info(f'lres = {lres}')
 
-        # Local function evals for all minimisers
+        # Local function evals for all minimizers
         self.res.nlfev += lres.nfev
         if 'njev' in lres:
             self.res.nljev += lres.njev
         if 'nhev' in lres:
             self.res.nlhev += lres.nhev
 
-        try:  # Needed because of the brain dead 1x1 numpy arrays
+        try:  # Needed because of the brain dead 1x1 NumPy arrays
             lres.fun = lres.fun[0]
         except (IndexError, TypeError):
             lres.fun
 
         # Append minima maps
         self.LMC[x_min]
         self.LMC.add_res(x_min, lres, bounds=g_bounds)
 
         return lres
 
-    # Post local minimisation processing
+    # Post local minimization processing
     def sort_result(self):
         """
         Sort results and build the global return object
         """
         # Sort results in local minima cache
         results = self.LMC.sort_cache_result()
         self.res.xl = results['xl']
         self.res.funl = results['funl']
         self.res.x = results['x']
         self.res.fun = results['fun']
 
         # Add local func evals to sampling func evals
         # Count the number of feasible vertices and add to local func evals:
         self.res.nfev = self.fn + self.res.nlfev
-        self.res.tnev = self.n_sampled + self.res.nlfev
         return self.res
 
     # Algorithm controls
     def fail_routine(self, mes=("Failed to converge")):
         self.break_routine = True
         self.res.success = False
         self.X_min = [None]
         self.res.message = mes
 
     def sampled_surface(self, infty_cons_sampl=False):
         """
         Sample the function surface.
-        
+
         There are 2 modes, if ``infty_cons_sampl`` is True then the sampled
         points that are generated outside the feasible domain will be
         assigned an ``inf`` value in accordance with SHGO rules.
-        This guarantees convergence and usually requires less objective function
-        evaluations at the computational costs of more Delaunay triangulation
-        points.
-
-        If ``infty_cons_sampl`` is False then the infeasible points are discarded
-        and only a subspace of the sampled points are used. This comes at the
-        cost of the loss of guaranteed convergence and usually requires more
-        objective function evaluations.
+        This guarantees convergence and usually requires less objective
+        function evaluations at the computational costs of more Delaunay
+        triangulation points.
+
+        If ``infty_cons_sampl`` is False, then the infeasible points are
+        discarded and only a subspace of the sampled points are used. This
+        comes at the cost of the loss of guaranteed convergence and usually
+        requires more objective function evaluations.
         """
         # Generate sampling points
         if self.disp:
-            print('Generating sampling points')
+            logging.info('Generating sampling points')
         self.sampling(self.nc, self.dim)
-        #print(f'self.sampling(self.nc, self.dim) = {self.sampling(self.nc, self.dim)}')
-        # Append minimizer points
-        #TODO: n_prc needs to add len(self.LMC.xl_maps) for self.delaunay_triangulation
         if len(self.LMC.xl_maps) > 0:
             self.C = np.vstack((self.C, np.array(self.LMC.xl_maps)))
         if not infty_cons_sampl:
             # Find subspace of feasible points
             if self.g_cons is not None:
                 self.sampling_subspace()
 
         # Sort remaining samples
         self.sorted_samples()
 
         # Find objective function references
-        #self.fun_ref()
-
         self.n_sampled = self.nc
 
-    def sobol_points_40(self, n, d, skip=0):
-        """
-        Wrapper for ``sobol_seq.i4_sobol_generate``
-
-        Generate N sampling points in D dimensions
-        """
-        points = self.Sobol.i4_sobol_generate(d, n, skip=0)
-
-        return points
-
-    def sobol_points_10k(self, N, D):
-        """
-        sobol.cc by Frances Kuo and Stephen Joe translated to Python 3 by
-        Carl Sandrock 2016-03-31
-
-        The original program is available and described at
-        http://web.maths.unsw.edu.au/~fkuo/sobol/
-        """
-        import gzip
-        import os
-        path = os.path.join(os.path.dirname(__file__), '_shgo_lib',
-                            'sobol_vec.gz')
-        f = gzip.open(path, 'rb')
-        unsigned = "uint64"
-        # swallow header
-        next(f)
-
-        L = int(np.log(N) // np.log(2.0)) + 1
-
-        C = np.ones(N, dtype=unsigned)
-        for i in range(1, N):
-            value = i
-            while value & 1:
-                value >>= 1
-                C[i] += 1
-
-        points = np.zeros((N, D), dtype='double')
-
-        # XXX: This appears not to set the first element of V
-        V = np.empty(L + 1, dtype=unsigned)
-        for i in range(1, L + 1):
-            V[i] = 1 << (32 - i)
-
-        X = np.empty(N, dtype=unsigned)
-        X[0] = 0
-        for i in range(1, N):
-            X[i] = X[i - 1] ^ V[C[i - 1]]
-            points[i, 0] = X[i] / 2 ** 32
-
-        for j in range(1, D):
-            F_int = [int(item) for item in next(f).strip().split()]
-            (d, s, a), m = F_int[:3], [0] + F_int[3:]
-
-            if L <= s:
-                for i in range(1, L + 1):
-                    V[i] = m[i] << (32 - i)
-            else:
-                for i in range(1, s + 1):
-                    V[i] = m[i] << (32 - i)
-                for i in range(s + 1, L + 1):
-                    V[i] = V[i - s] ^ (
-                            V[i - s] >> np.array(s, dtype=unsigned))
-                    for k in range(1, s):
-                        V[i] ^= np.array(
-                            (((a >> (s - 1 - k)) & 1) * V[i - k]),
-                            dtype=unsigned)
-
-            X[0] = 0
-            for i in range(1, N):
-                X[i] = X[i - 1] ^ V[C[i - 1]]
-                points[i, j] = X[i] / 2 ** 32  # *** the actual points
-
-        f.close()
-        return points
-
-    def sampling_sobol(self, n, dim):
+    def sampling_custom(self, n, dim):
         """
         Generates uniform sampling points in a hypercube and scales the points
         to the bound limits.
         """
         # Generate sampling points.
         # Generate uniform sample points in [0, 1]^m \subset R^m
         if self.n_sampled == 0:
-            self.C = self.sobol_points(n, dim)
+            self.C = self.sampling_function(n, dim)
         else:
-            self.C = self.sobol_points(n, dim, skip=self.n_sampled)
-        # Distribute over bounds
-        for i in range(len(self.bounds)):
-            self.C[:, i] = (self.C[:, i] *
-                            (self.bounds[i][1] - self.bounds[i][0])
-                            + self.bounds[i][0])
-        return self.C
-
-    def sampling_custom(self, n, dim):
-        """
-        Generates uniform sampling points in a hypercube and scales the points
-        to the bound limits.
-        """
-        # Generate sampling points.
-        # Generate uniform sample points in [0, 1]^m \subset R^m
-        self.C = self.sampling_function(n, dim)
+            self.C = self.sampling_function(n, dim)
         # Distribute over bounds
         for i in range(len(self.bounds)):
             self.C[:, i] = (self.C[:, i] *
                             (self.bounds[i][1] - self.bounds[i][0])
                             + self.bounds[i][0])
         return self.C
 
@@ -1494,17 +1454,17 @@
         # Subspace of feasible points.
         for ind, g in enumerate(self.g_cons):
             self.C = self.C[g(self.C.T, *self.g_args[ind]) >= 0.0]
             if self.C.size == 0:
                 self.res.message = ('No sampling point found within the '
                                     + 'feasible set. Increasing sampling '
                                     + 'size.')
-                # sampling correctly for both 1D and >1D cases
+                # sampling correctly for both 1-D and >1-D cases
                 if self.disp:
-                    print(self.res.message)
+                    logging.info(self.res.message)
 
     def sorted_samples(self):  # Validated
         """Find indexes of the sorted sampling points"""
         self.Ind_sorted = np.argsort(self.C, axis=0)
         self.Xs = self.C[self.Ind_sorted]
         return self.Ind_sorted, self.Xs
 
@@ -1514,30 +1474,33 @@
             # in self.sampled_surface
             self.Tri.add_points(self.C[n_prc:, :])
         else:
             try:
                 self.Tri = spatial.Delaunay(self.C,
                                             incremental=self.qhull_incremental,
                                             )
-            except:
+            except spatial.QhullError:
                 if str(sys.exc_info()[1])[:6] == 'QH6239':
                     logging.warning('QH6239 Qhull precision error detected, '
-                        'this usually occurs when no bounds are specified, '
-                        'Qhull can only run with the "Qz" option on for '
-                        'handling cocircular/cospherical points and in this '
-                        'case incremental mode is switched off. The performance'
-                        ' of shgo will be reduced in this mode.')
+                                    'this usually occurs when no bounds are '
+                                    'specified, Qhull can only run with '
+                                    'handling cocircular/cospherical points'
+                                    ' and in this case incremental mode is '
+                                    'switched off. The performance of shgo '
+                                    'will be reduced in this mode.')
                     self.qhull_incremental = False
                     self.Tri = spatial.Delaunay(self.C,
-                                   incremental=self.qhull_incremental)
+                                                incremental=
+                                                self.qhull_incremental)
                 else:
                     raise
 
         return self.Tri
 
+
 class LMap:
     def __init__(self, v):
         self.v = v
         self.x_l = None
         self.lres = None
         self.f_min = None
         self.lbounds = []
@@ -1601,43 +1564,14 @@
 
         # Save ordered list of minima
         results['xl'] = self.xl_maps[ind_sorted]  # Ordered x vals
         self.f_maps = np.array(self.f_maps)
         results['funl'] = self.f_maps[ind_sorted]
         results['funl'] = results['funl'].T
 
-        # Find global of all minimisers
+        # Find global of all minimizers
         results['x'] = self.xl_maps[ind_sorted[0]]  # Save global minima
         results['fun'] = self.f_maps[ind_sorted[0]]  # Save global fun value
 
         self.xl_maps = np.ndarray.tolist(self.xl_maps)
         self.f_maps = np.ndarray.tolist(self.f_maps)
         return results
-
-# TODO: In scipy version delete this
-class MemoizeJac(object):
-    """ Decorator that caches the return values of a function returning `(fun, grad)`
-        each time it is called. """
-
-    def __init__(self, fun):
-        self.fun = fun
-        self.jac = None
-        self._value = None
-        self.x = None
-
-    def _compute_if_needed(self, x, *args):
-        if not np.all(x == self.x) or self._value is None or self.jac is None:
-            self.x = np.asarray(x).copy()
-            fg = self.fun(x, *args)
-            self.jac = fg[1]
-            self._value = fg[0]
-
-    def __call__(self, x, *args):
-        """ returns the the function value """
-        self._compute_if_needed(x, *args)
-        return self._value
-
-    def derivative(self, x, *args):
-        self._compute_if_needed(x, *args)
-        return self.jac
-    
-
```

### Comparing `shgo-0.5.1/shgo/_shgo_lib/_complex.py` & `shgo-1.0.0/shgo/_shgo_lib/_complex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,133 @@
-"""
-Base classes for low memory simplicial complex structures.
-"""
-# Std. Library
+"""Base classes for low memory simplicial complex structures."""
 import copy
-import collections
 import logging
-import os
 import itertools
-import json
 import decimal
-from functools import lru_cache  # For Python 3 only
-from abc import ABC, abstractmethod
-# Required modules:
+from functools import lru_cache
+
 import numpy
 
-# Module specific imports
-from ._vertex import VertexCacheField
+from ._vertex import (VertexCacheField, VertexCacheIndex)
 
 
-# Main complex class:
 class Complex:
+    """
+    Base class for a simplicial complex described as a cache of vertices
+    together with their connections.
+
+    Important methods:
+        Domain triangulation:
+                Complex.triangulate, Complex.split_generation
+        Triangulating arbitrary points (must be traingulable,
+            may exist outside domain):
+                Complex.triangulate(sample_set)
+        Converting another simplicial complex structure data type to the
+            structure used in Complex (ex. OBJ wavefront)
+                Complex.convert(datatype, data)
+
+    Important objects:
+        HC.V: The cache of vertices and their connection
+        HC.H: Storage structure of all vertex groups
+
+    Parameters
+    ----------
+    dim : int
+        Spatial dimensionality of the complex R^dim
+    domain : list of tuples, optional
+        The bounds [x_l, x_u]^dim of the hyperrectangle space
+        ex. The default domain is the hyperrectangle [0, 1]^dim
+        Note: The domain must be convex, non-convex spaces can be cut
+              away from this domain using the non-linear
+              g_cons functions to define any arbitrary domain
+              (these domains may also be disconnected from each other)
+    sfield :
+        A scalar function defined in the associated domain f: R^dim --> R
+    sfield_args : tuple
+        Additional arguments to be passed to `sfield`
+    vfield :
+        A scalar function defined in the associated domain
+                       f: R^dim --> R^m
+                   (for example a gradient function of the scalar field)
+    vfield_args : tuple
+        Additional arguments to be passed to vfield
+    symmetry : None or list
+            Specify if the objective function contains symmetric variables.
+            The search space (and therefore performance) is decreased by up to
+            O(n!) times in the fully symmetric case.
+
+            E.g.  f(x) = (x_1 + x_2 + x_3) + (x_4)**2 + (x_5)**2 + (x_6)**2
+
+            In this equation x_2 and x_3 are symmetric to x_1, while x_5 and
+             x_6 are symmetric to x_4, this can be specified to the solver as:
+
+            symmetry = [0,  # Variable 1
+                        0,  # symmetric to variable 1
+                        0,  # symmetric to variable 1
+                        3,  # Variable 4
+                        3,  # symmetric to variable 4
+                        3,  # symmetric to variable 4
+                        ]
+
+    constraints : dict or sequence of dict, optional
+        Constraints definition.
+        Function(s) ``R**n`` in the form::
+
+            g(x) <= 0 applied as g : R^n -> R^m
+            h(x) == 0 applied as h : R^n -> R^p
+
+        Each constraint is defined in a dictionary with fields:
+
+            type : str
+                Constraint type: 'eq' for equality, 'ineq' for inequality.
+            fun : callable
+                The function defining the constraint.
+            jac : callable, optional
+                The Jacobian of `fun` (only for SLSQP).
+            args : sequence, optional
+                Extra arguments to be passed to the function and Jacobian.
+
+        Equality constraint means that the constraint function result is to
+        be zero whereas inequality means that it is to be
+        non-negative.constraints : dict or sequence of dict, optional
+        Constraints definition.
+        Function(s) ``R**n`` in the form::
+
+            g(x) <= 0 applied as g : R^n -> R^m
+            h(x) == 0 applied as h : R^n -> R^p
+
+        Each constraint is defined in a dictionary with fields:
+
+            type : str
+                Constraint type: 'eq' for equality, 'ineq' for inequality.
+            fun : callable
+                The function defining the constraint.
+            jac : callable, optional
+                The Jacobian of `fun` (unused).
+            args : sequence, optional
+                Extra arguments to be passed to the function and Jacobian.
+
+        Equality constraint means that the constraint function result is to
+        be zero whereas inequality means that it is to be non-negative.
+
+    workers : int  optional
+        Uses `multiprocessing.Pool <multiprocessing>`) to compute the field
+         functions in parrallel.
+    """
     def __init__(self, dim, domain=None, sfield=None, sfield_args=(),
-                 symmetry=None, constraints=None,
-                 constraints_args=None, #TODO: Add
-                 workers=None):
-        """
-        A base class for a simplicial complex described as a cache of vertices
-        together with their connections.
-
-        Important methods:
-            Domain triangulation:
-                    Complex.triangulate, Complex.split_generation
-            Triangulating arbitrary points (must be traingulable,
-                may exist outside domain):
-                    Complex.triangulate(sample_set)  #TODO
-            Converting another simplicial complex structure data type to the
-                structure used in Complex (ex. OBJ wavefront)
-                    Complex.convert(datatype, data)  #TODO
-            Convert the structure in the Complex to other data type:
-                    #TODO
-
-        Important objects:
-            HC.V: The cache of vertices and their connection
-            HC.H: Storage structure of all vertex groups
-
-        :param dim: int, Spatial dimensionality of the complex R^dim
-        :param domain: list of tuples, optional
-                The bounds [x_l, x_u]^dim of the hyperrectangle space
-                ex. The default domain is the hyperrectangle [0, 1]^dim
-                Note: The domain must be convex, non-convex spaces can be cut
-                      away from this domain using the non-linear
-                      g_cons functions to define any arbitrary domain
-                      (these domains may also be disconnected from each other)
-        :param sfield: A scalar function defined in the associated domain
-                           f: R^dim --> R
-        :param sfield_args: tuple, Additional arguments to be passed to sfield
-        :param vfield: A scalar function defined in the associated domain
-                           f: R^dim --> R^m
-                       (for example a gradient function of the scalar field)
-        :param vfield_args: tuple, Additional arguments to be passed to sfield
-        :param symmetry: If all the variables in the field are symmetric this
-                option will reduce complexity of the triangulation by O(n!)
-
-        constraints : dict or sequence of dict, optional
-            Constraints definition.
-            Function(s) ``R**n`` in the form::
-
-                g(x) <= 0 applied as g : R^n -> R^m
-                h(x) == 0 applied as h : R^n -> R^p
-
-            Each constraint is defined in a dictionary with fields:
-
-                type : str
-                    Constraint type: 'eq' for equality, 'ineq' for inequality.
-                fun : callable
-                    The function defining the constraint.
-                jac : callable, optional
-                    The Jacobian of `fun` (only for SLSQP).
-                args : sequence, optional
-                    Extra arguments to be passed to the function and Jacobian.
-
-            Equality constraint means that the constraint function result is to
-            be zero whereas inequality means that it is to be non-negative.constraints : dict or sequence of dict, optional
-            Constraints definition.
-            Function(s) ``R**n`` in the form::
-
-                g(x) <= 0 applied as g : R^n -> R^m
-                h(x) == 0 applied as h : R^n -> R^p
-
-            Each constraint is defined in a dictionary with fields:
-
-                type : str
-                    Constraint type: 'eq' for equality, 'ineq' for inequality.
-                fun : callable
-                    The function defining the constraint.
-                jac : callable, optional
-                    The Jacobian of `fun` (unused).
-                args : sequence, optional
-                    Extra arguments to be passed to the function and Jacobian.
-
-            Equality constraint means that the constraint function result is to
-            be zero whereas inequality means that it is to be non-negative.
-
-        workers : int  optional
-            Uses `multiprocessing.Pool <multiprocessing>`) to compute the field
-             functions in parrallel.
-        """
+                 symmetry=None, constraints=None, workers=1):
         self.dim = dim
 
         # Domains
         self.domain = domain
         if domain is None:
             self.bounds = [(float(0), float(1.0)), ] * dim
         else:
-            self.bounds = domain  # TODO: Assert that len(domain) is dim
-        self.symmetry = symmetry  # TODO: Define the functions to be used
+            self.bounds = domain
+        self.symmetry = symmetry
         #      here in init to avoid if checks
 
         # Field functions
         self.sfield = sfield
         self.sfield_args = sfield_args
 
         # Process constraints
@@ -150,60 +159,67 @@
         self.perm_cycle = 0
 
         # Every cell is stored in a list of its generation,
         # ex. the initial cell is stored in self.H[0]
         # 1st get new cells are stored in self.H[1] etc.
         # When a cell is sub-generated it is removed from this list
 
-        self.H = []  # Storage structure of vertex groups #TODO: Dated?
+        self.H = []  # Storage structure of vertex groups
 
         # Cache of all vertices
-        # Initiate a vertex cache and an associated field cache, note that
-        # the field case is always initiated inside the vertex cache if an
-        # associated field scalar field is defined:
-        if sfield is not None:
-            self.V = VertexCacheField(field=sfield, field_args=sfield_args,
-                                      g_cons=self.g_cons,
-                                      g_cons_args=self.g_args,
-                                      workers=workers)
-        self.V_non_symm = []  # List of non-symmetric vertices
+        if (sfield is not None) or (self.g_cons is not None):
+            # Initiate a vertex cache and an associated field cache, note that
+            # the field case is always initiated inside the vertex cache if an
+            # associated field scalar field is defined:
+            if sfield is not None:
+                self.V = VertexCacheField(field=sfield, field_args=sfield_args,
+                                          g_cons=self.g_cons,
+                                          g_cons_args=self.g_args,
+                                          workers=workers)
+            elif self.g_cons is not None:
+                self.V = VertexCacheField(field=sfield, field_args=sfield_args,
+                                          g_cons=self.g_cons,
+                                          g_cons_args=self.g_args,
+                                          workers=workers)
+        else:
+            self.V = VertexCacheIndex()
 
+        self.V_non_symm = []  # List of non-symmetric vertices
 
     def __call__(self):
         return self.H
 
     # %% Triangulation methods
-    def cyclic_product(self, bounds, origin, supremum, centroid=True,
-                       printout=False):
-        #TODO: Connect every vertex with the supremum before yielding
-        #TODO: Change self.origin and self. supremum to local origin
+    def cyclic_product(self, bounds, origin, supremum, centroid=True):
+        """Generate initial triangulation using cyclic product"""
+        # Define current hyperrectangle
         vot = tuple(origin)
         vut = tuple(supremum)  # Hyperrectangle supremum
         self.V[vot]
         vo = self.V[vot]
         yield vo.x
         self.V[vut].connect(self.V[vot])
         yield vut
         # Cyclic group approach with second x_l --- x_u operation.
 
         # These containers store the "lower" and "upper" vertices
         # corresponding to the origin or supremum of every C2 group.
         # It has the structure of `dim` times embedded lists each containing
         # these vertices as the entire complex grows. Bounds[0] has to be done
         # outside the loops before we have symmetric containers.
-        #NOTE: This means that bounds[0][1] must always exist
+        # NOTE: This means that bounds[0][1] must always exist
         C0x = [[self.V[vot]]]
         a_vo = copy.copy(list(origin))
         a_vo[0] = vut[0]  # Update aN Origin
         a_vo = self.V[tuple(a_vo)]
-        #self.V[vot].connect(self.V[tuple(a_vo)])
+        # self.V[vot].connect(self.V[tuple(a_vo)])
         self.V[vot].connect(a_vo)
         yield a_vo.x
         C1x = [[a_vo]]
-        #C1x = [[self.V[tuple(a_vo)]]]
+        # C1x = [[self.V[tuple(a_vo)]]]
         ab_C = []  # Container for a + b operations
 
         # Loop over remaining bounds
         for i, x in enumerate(bounds[1:]):
             # Update lower and upper containers
             C0x.append([])
             C1x.append([])
@@ -257,15 +273,14 @@
                         # Yield new points
                         yield a_vu.x
 
                 # Try to connect aN lower source of previous a + b
                 # operation with a aN vertex
                 ab_Cc = copy.copy(ab_C)
 
-                #TODO: SHOULD THIS BE MOVED OUTSIDE THE try ?
                 for vp in ab_Cc:
                     b_v = list(vp[0].x)
                     ab_v = list(vp[1].x)
                     b_v[i + 1] = vut[i + 1]
                     ab_v[i + 1] = vut[i + 1]
                     b_v = self.V[tuple(b_v)]  # b + vl
                     ab_v = self.V[tuple(ab_v)]  # b + a_vl
@@ -274,69 +289,50 @@
                     b_v.connect(ab_v)  # s-s
 
                     # Add new list of cross pairs
                     ab_C.append((vp[0], ab_v))
                     ab_C.append((b_v, ab_v))
 
             except IndexError:
-                #TODO: The above routine works for symm inits, so maybe test if
-                # vl exists and then work from there?
-                # Copy lists for iteration
-                # cC0x = [x[:] for x in C0x[:i + 1]]
                 cC0x = C0x[i]
                 cC1x = C1x[i]
                 VL, VU = cC0x, cC1x
                 for k, (vl, vu) in enumerate(zip(VL, VU)):
                     # Build aN vertices for each lower-upper pair in N:
                     a_vu = list(vu.x)
                     a_vu[i + 1] = vut[i + 1]
-
                     # Connect vertices in N to corresponding vertices
                     # in aN:
                     a_vu = self.V[tuple(a_vu)]
                     # Connect vertices in N to corresponding vertices
                     # in aN:
                     vu.connect(a_vu)
                     # Connect new vertex pair in aN:
                     # a_vl.connect(a_vu)
                     # Connect lower pair to upper (triangulation
                     # operation of a + b (two arbitrary operations):
                     vl.connect(a_vu)
                     ab_C.append((vl, a_vu))
-
-                    # Update the containers
                     C0x[i + 1].append(vu)
                     C1x[i + 1].append(a_vu)
-
-                    # Update old containers
                     # Yield new points
                     a_vu.connect(self.V[vut])
                     yield a_vu.x
                     ab_Cc = copy.copy(ab_C)
                     for vp in ab_Cc:
                         if vp[1].x[i] == vut[i]:
                             ab_v = list(vp[1].x)
                             ab_v[i + 1] = vut[i + 1]
                             ab_v = self.V[tuple(ab_v)]  # b + a_vl
                             # Note o---o is already connected
                             vp[0].connect(ab_v)  # o-s
-                        #    b_v.connect(ab_v)  # s-s
 
                             # Add new list of cross pairs
                             ab_C.append((vp[0], ab_v))
 
-            # Printing
-            if printout:
-                print("=" * 19)
-                print("Current symmetry group:")
-                print("=" * 19)
-                for v in self.V.cache:
-                    self.V[v].print_out()
-                print("=" * 19)
-
         # Clean class trash
         try:
             del C0x
             del cC0x
             del C1x
             del cC1x
             del ab_C
@@ -348,46 +344,45 @@
         if centroid:
             vo = self.V[vot]
             vs = self.V[vut]
             # Disconnect the origin and supremum
             vo.disconnect(vs)
             # Build centroid
             vc = self.split_edge(vot, vut)
-            # TODO: If not initial triangulation, we'll need to use a different
-            # container
             for v in vo.nn:
                 v.connect(vc)
             yield vc.x
             return vc.x
         else:
             yield vut
             return vut
 
-
-    def triangulate(self, n=None, symmetry=None, centroid=True, printout=False):
+    def triangulate(self, n=None, symmetry=None, centroid=True,
+                    printout=False):
         """
         Triangulate the initial domain, if n is not None then a limited number
         of points will be generated
 
-        :param n:
-        :param symmetry:
+        Parameters
+        ----------
+        n : int, Number of points to be sampled.
+        symmetry :
 
             Ex. Dictionary/hashtable
             f(x) = (x_1 + x_2 + x_3) + (x_4)**2 + (x_5)**2 + (x_6)**2
 
             symmetry = symmetry[0]: 0,  # Variable 1
                        symmetry[1]: 0,  # symmetric to variable 1
                        symmetry[2]: 0,  # symmetric to variable 1
                        symmetry[3]: 3,  # Variable 4
                        symmetry[4]: 3,  # symmetric to variable 4
                        symmetry[5]: 3,  # symmetric to variable 4
                         }
-
-        :param printout:
-        :return:
+        centroid : bool, if True add a central point to the hypercube
+        printout : bool, if True print out results
 
         NOTES:
         ------
         Rather than using the combinatorial algorithm to connect vertices we
         make the following observation:
 
         The bound pairs are similar a C2 cyclic group and the structure is
@@ -409,75 +404,78 @@
         # Build origin and supremum vectors
         origin = [i[0] for i in self.bounds]
         self.origin = origin
         supremum = [i[1] for i in self.bounds]
 
         self.supremum = supremum
 
-        #TODO: Add check that len(symmetry) is equal to len(self.bounds)
         if symmetry is None:
             cbounds = self.bounds
         else:
             cbounds = copy.copy(self.bounds)
             for i, j in enumerate(symmetry):
                 if i is not j:
                     # pop second entry on second symmetry vars
                     cbounds[i] = [self.bounds[symmetry[i]][0]]
-                    # Sole (first) entry is the sup value and there is no origin
+                    # Sole (first) entry is the sup value and there is no
+                    # origin:
                     cbounds[i] = [self.bounds[symmetry[i]][1]]
-                    if self.bounds[symmetry[i]] is not self.bounds[symmetry[j]]:
+                    if (self.bounds[symmetry[i]] is not
+                            self.bounds[symmetry[j]]):
                         logging.warning(f"Variable {i} was specified as "
-                                        f"symmetetric to variable {j}, however,"
-                                        f"the bounds {i} ="
-                                        f" {self.bounds[symmetry[i]]} and {j} ="
+                                        f"symmetetric to variable {j}, however"
+                                        f", the bounds {i} ="
+                                        f" {self.bounds[symmetry[i]]} and {j}"
+                                        f" ="
                                         f" {self.bounds[symmetry[j]]} do not "
                                         f"match, the mismatch was ignored in "
                                         f"the initial triangulation.")
                         cbounds[i] = self.bounds[symmetry[j]]
 
-
         if n is None:
             # Build generator
-            self.cp = self.cyclic_product(cbounds, origin, supremum, centroid,
-                                          printout)
+            self.cp = self.cyclic_product(cbounds, origin, supremum, centroid)
             for i in self.cp:
                 i
 
             try:
                 self.triangulated_vectors.append((tuple(self.origin),
                                                   tuple(self.supremum)))
             except (AttributeError, KeyError):
                 self.triangulated_vectors = [(tuple(self.origin),
                                               tuple(self.supremum))]
 
         else:
-            #Check if generator already exists
+            # Check if generator already exists
             try:
                 self.cp
             except (AttributeError, KeyError):
                 self.cp = self.cyclic_product(cbounds, origin, supremum,
-                                              centroid, printout)
+                                              centroid)
 
             try:
                 while len(self.V.cache) < n:
                     next(self.cp)
             except StopIteration:
-                #TODO: We should maybe append and add the possibility of
-                #      of starting new triangulated domains on different
-                #      complexes
                 try:
                     self.triangulated_vectors.append((tuple(self.origin),
                                                       tuple(self.supremum)))
                 except (AttributeError, KeyError):
                     self.triangulated_vectors = [(tuple(self.origin),
                                                   tuple(self.supremum))]
+
+        if printout:
+            # for v in self.C0():
+            #   v.print_out()
+            for v in self.V.cache:
+                self.V[v].print_out()
+
         return
 
     def refine(self, n=1):
-        #TODO: Replace with while loop checking cache size instead?
         if n is None:
             try:
                 self.triangulated_vectors
                 self.refine_all()
                 return
             except AttributeError as ae:
                 if str(ae) == "'Complex' object has no attribute " \
@@ -486,73 +484,66 @@
                     return
                 else:
                     raise
 
         nt = len(self.V.cache) + n  # Target number of total vertices
         # In the outer while loop we iterate until we have added an extra `n`
         # vertices to the complex:
-        #TODO: We can reduce the number of exception handling and exceptions to
-        #  StopIteration if we try to generate the initial objects first and
-        #  then refine only have the first few while loop runs
         while len(self.V.cache) < nt:  # while loop 1
             try:  # try 1
                 # Try to access triangulated_vectors, this should only be
-                # defined if an initial triangulation has already been performed
+                # defined if an initial triangulation has already been
+                # performed:
                 self.triangulated_vectors
                 # Try a usual iteration of the current generator, if it
                 # does not exist or is exhausted then produce a new generator
                 try:  # try 2
-                    #next(self.rls)
-                    #print(f'next(self.rls) = {next(self.rls)}')
                     next(self.rls)
                 except (AttributeError, StopIteration, KeyError):
                     vp = self.triangulated_vectors[0]
-                    #print(f'vp = {vp}')
                     self.rls = self.refine_local_space(*vp, bounds=self.bounds)
-                    # next(self.rls)
-                    #print(f'next(self.rls) = {next(self.rls)}')
                     next(self.rls)
 
             except (AttributeError, KeyError):
                 # If an initial triangulation has not been completed, then
                 # we start/continue the initial triangulation targeting `nt`
-                # vertices, if nt is greater than the initial number of vertices
-                # then the refine routine will move back to try 1.
+                # vertices, if nt is greater than the initial number of
+                # vertices then the `refine` routine will move back to try 1.
                 self.triangulate(nt, self.symmetry)
         return
 
     def refine_all(self, centroids=True):
-        """
-        Refine the entire domain of the current complex
-        :return:
-        """
-
+        """Refine the entire domain of the current complex."""
         try:
             self.triangulated_vectors
             tvs = copy.copy(self.triangulated_vectors)
             for i, vp in enumerate(tvs):
-                #self.rls =self.refine_local_space_c(*vp, vpool=vn_pool_sets[i])
                 self.rls = self.refine_local_space(*vp, bounds=self.bounds)
                 for i in self.rls:
                     i
         except AttributeError as ae:
             if str(ae) == "'Complex' object has no attribute " \
                           "'triangulated_vectors'":
                 self.triangulate(symmetry=self.symmetry, centroid=centroids)
             else:
                 raise
 
+        # This adds a centroid to every new sub-domain generated and defined
+        # by self.triangulated_vectors, in addition the vertices ! to complete
+        # the triangulation
         return
 
-    def refine_local_space(self, origin, supremum, bounds, centroid=1,
-                              printout=0):
+    def refine_local_space(self, origin, supremum, bounds, centroid=1):
         # Copy for later removal
         origin_c = copy.copy(origin)
         supremum_c = copy.copy(supremum)
 
+        # Initiate local variables redefined in later inner `for` loop:
+        vl, vu, a_vu = None, None, None
+
         # Change the vector orientation so that it is only increasing
         s_ov = list(origin)
         s_origin = list(origin)
         s_sv = list(supremum)
         s_supremum = list(supremum)
         for i, vi in enumerate(s_origin):
             if s_ov[i] > s_sv[i]:
@@ -572,15 +563,15 @@
         # Cyclic group approach with second x_l --- x_u operation.
 
         # These containers store the "lower" and "upper" vertices
         # corresponding to the origin or supremum of every C2 group.
         # It has the structure of `dim` times embedded lists each containing
         # these vertices as the entire complex grows. Bounds[0] has to be done
         # outside the loops before we have symmetric containers.
-        #NOTE: This means that bounds[0][1] must always exist
+        # NOTE: This means that bounds[0][1] must always exist
 
         a_vl = copy.copy(list(vot))
         a_vl[0] = vut[0]  # Update aN Origin
         if tuple(a_vl) not in self.V.cache:
             vo = self.V[vot]  # initiate if doesn't exist yet
             vs = self.V[vut]
             # Start by finding the old centroid of the new space:
@@ -623,24 +614,25 @@
                 # Try to connect aN lower source of previous a + b
                 # operation with a aN vertex
                 ab_Cc = copy.copy(ab_C)  # NOTE: We append ab_C in the
                 # (VL, VC, VU) for-loop, but we use the copy of the list in the
                 # ab_Cc for-loop.
                 s_ab_Cc = copy.copy(s_ab_C)
 
-                #%%
                 # Early try so that we don't have to copy the cache before
                 # moving on to next C1/C2: Try to add the operation of a new
                 # C2 product by accessing the upper bound
                 if tuple(t_a_vl) not in self.V.cache:
-                    raise IndexError  # Raise error to continue symmetric refine
+                    # Raise error to continue symmetric refine
+                    raise IndexError
                 t_a_vu = list(vut)
                 t_a_vu[i + 1] = vut[i + 1]
                 if tuple(t_a_vu) not in self.V.cache:
-                    raise IndexError  # Raise error to continue symmetric refine
+                    # Raise error to continue symmetric refine:
+                    raise IndexError
 
                 for vectors in s_ab_Cc:
                     # s_ab_C.append([c_vc, vl, vu, a_vu])
                     bc_vc = list(vectors[0].x)
                     b_vl = list(vectors[1].x)
                     b_vu = list(vectors[2].x)
                     ba_vu = list(vectors[3].x)
@@ -661,41 +653,37 @@
                     d_bc_vc.connect(vectors[2])  # Connect all to centroid
                     d_bc_vc.connect(vectors[3])  # Connect all to centroid
                     yield d_bc_vc.x
                     b_vl = self.V[tuple(b_vl)]
                     bc_vc.connect(b_vl)  # Connect aN cross pairs
                     d_bc_vc.connect(b_vl)  # Connect all to centroid
 
-
                     yield b_vl
                     b_vu = self.V[tuple(b_vu)]
                     bc_vc.connect(b_vu)  # Connect aN cross pairs
                     d_bc_vc.connect(b_vu)  # Connect all to centroid
 
-                    #TODO: Should be done in the cyclical loop somehow?
                     b_vl_c = self.split_edge(b_vu.x, b_vl.x)
                     bc_vc.connect(b_vl_c)
-                    ###
 
                     yield b_vu
                     ba_vu = self.V[tuple(ba_vu)]
                     bc_vc.connect(ba_vu)  # Connect aN cross pairs
                     d_bc_vc.connect(ba_vu)  # Connect all to centroid
 
                     # Split the a + b edge of the initial triangulation:
                     os_v = self.split_edge(vectors[1].x, ba_vu.x)  # o-s
                     ss_v = self.split_edge(b_vl.x, ba_vu.x)  # s-s
-
-                    #TODO: Should be done in the cyclical loop somehow?
                     b_vu_c = self.split_edge(b_vu.x, ba_vu.x)
                     bc_vc.connect(b_vu_c)
                     yield os_v.x  # often equal to vco, but not always
                     yield ss_v.x  # often equal to bc_vu, but not always
                     yield ba_vu
-                    # Split remaining to centre, call this centre group "d = 0.5*a"
+                    # Split remaining to centre, call this centre group
+                    # "d = 0.5*a"
                     d_bc_vc = self.split_edge(vectors[0].x, bc_vc.x)
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     yield d_bc_vc.x
                     d_b_vl = self.split_edge(vectors[1].x, b_vl.x)
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     d_bc_vc.connect(d_b_vl)  # Connect dN cross pairs
                     yield d_b_vl.x
@@ -712,19 +700,16 @@
                     #       bc_vc, b_vl, b_vu, ba_vl, ba_vu]
                     comb = [vl, vu, a_vu,
                             b_vl, b_vu, ba_vu]
                     comb_iter = itertools.combinations(comb, 2)
                     for vecs in comb_iter:
                         self.split_edge(vecs[0].x, vecs[1].x)
                     # Add new list of cross pairs
-                    #ab_C.append((bc_vc, b_vl, b_vu, ba_vl, ba_vu))
-                    #ab_C.append((d_bc_vc, d_b_vl, d_b_vu, d_ba_vl, d_ba_vu))
                     ab_C.append((d_bc_vc, vectors[1], b_vl, a_vu, ba_vu))
                     ab_C.append((d_bc_vc, vl, b_vl, a_vu, ba_vu))  # = prev
-                    #ab_C.append((d_bc_vc, vu, b_vu, a_vl, ba_vl))
 
                 for vectors in ab_Cc:
                     bc_vc = list(vectors[0].x)
                     b_vl = list(vectors[1].x)
                     b_vu = list(vectors[2].x)
                     ba_vl = list(vectors[3].x)
                     ba_vu = list(vectors[4].x)
@@ -763,15 +748,16 @@
                     d_bc_vc.connect(ba_vu)  # Connect all to centroid
                     # Split the a + b edge of the initial triangulation:
                     os_v = self.split_edge(vectors[1].x, ba_vu.x)  # o-s
                     ss_v = self.split_edge(b_vl.x, ba_vu.x)  # s-s
                     yield os_v.x  # often equal to vco, but not always
                     yield ss_v.x  # often equal to bc_vu, but not always
                     yield ba_vu
-                    # Split remaining to centre, call this centre group "d = 0.5*a"
+                    # Split remaining to centre, call this centre group
+                    # "d = 0.5*a"
                     d_bc_vc = self.split_edge(vectors[0].x, bc_vc.x)
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     yield d_bc_vc.x
                     d_b_vl = self.split_edge(vectors[1].x, b_vl.x)
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     d_bc_vc.connect(d_b_vl)  # Connect dN cross pairs
                     yield d_b_vl.x
@@ -783,17 +769,14 @@
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     d_bc_vc.connect(d_ba_vl)  # Connect dN cross pairs
                     yield d_ba_vl
                     d_ba_vu = self.split_edge(vectors[4].x, ba_vu.x)
                     d_bc_vc.connect(vco)  # NOTE: Unneeded?
                     d_bc_vc.connect(d_ba_vu)  # Connect dN cross pairs
                     yield d_ba_vu
-
-                    #ab_C.append((c_vc, vl, vu, a_vl, a_vu))  # CHECK
-
                     c_vc, vl, vu, a_vl, a_vu = vectors
 
                     comb = [vl, vu, a_vl, a_vu,
                             b_vl, b_vu, ba_vl, ba_vu]
                     comb_iter = itertools.combinations(comb, 2)
                     for vecs in comb_iter:
                         self.split_edge(vecs[0].x, vecs[1].x)
@@ -820,24 +803,25 @@
                         # Build cN vertices for each lower-upper C3 group in N:
                         c_vc.connect(vco)
                         c_vc.connect(vc)
                         c_vc.connect(vl)  # Connect c + ac operations
                         c_vc.connect(vu)  # Connect c + ac operations
                         c_vc.connect(a_vl)  # Connect c + ac operations
                         c_vc.connect(a_vu)  # Connect c + ac operations
-                        yield(c_vc.x)
+                        yield c_vc.x
                         c_vl = self.split_edge(vl.x, a_vl.x)
                         c_vl.connect(vco)
                         c_vc.connect(c_vl)  # Connect cN group vertices
-                        yield(c_vl.x)
-                        c_vu = self.split_edge(vu.x, a_vu.x) # yield at end of loop
+                        yield c_vl.x
+                        # yield at end of loop:
+                        c_vu = self.split_edge(vu.x, a_vu.x)
                         c_vu.connect(vco)
                         # Connect remaining cN group vertices
                         c_vc.connect(c_vu)  # Connect cN group vertices
-                        yield (c_vu.x)
+                        yield c_vu.x
 
                         a_vc = self.split_edge(a_vl.x, a_vu.x)  # is (a + vc) ?
                         a_vc.connect(vco)
                         a_vc.connect(c_vc)
 
                         # Storage for connecting c + ac operations:
                         ab_C.append((c_vc, vl, vu, a_vl, a_vu))
@@ -858,109 +842,110 @@
                         Cox[j].append(a_vl)
                         Ccx[j].append(c_vc)  # !
                         Ccx[j].append(a_vc)  # !
                         Cux[j].append(c_vu)  # !
                         Cux[j].append(a_vu)
 
                         # Yield new points
-                        yield(a_vc.x)
+                        yield a_vc.x
 
             except IndexError:
-                # TODO: The above routine works for symm inits, so maybe test if
-                # vl exists and then work from there?
                 for vectors in ab_Cc:
                     ba_vl = list(vectors[3].x)
                     ba_vu = list(vectors[4].x)
                     ba_vl[i + 1] = vut[i + 1]
                     ba_vu[i + 1] = vut[i + 1]
                     ba_vu = self.V[tuple(ba_vu)]
                     yield ba_vu
-                    # Split the a + b edge of the initial triangulation:
                     d_bc_vc = self.split_edge(vectors[1].x, ba_vu.x)  # o-s
                     yield ba_vu
                     d_bc_vc.connect(vectors[1])  # Connect all to centroid
                     d_bc_vc.connect(vectors[2])  # Connect all to centroid
                     d_bc_vc.connect(vectors[3])  # Connect all to centroid
                     d_bc_vc.connect(vectors[4])  # Connect all to centroid
                     yield d_bc_vc.x
                     ba_vl = self.V[tuple(ba_vl)]
                     yield ba_vl
-
-                    # Split remaining to centre, call this centre group "d = 0.5*a"
                     d_ba_vl = self.split_edge(vectors[3].x, ba_vl.x)
                     d_ba_vu = self.split_edge(vectors[4].x, ba_vu.x)
                     d_ba_vc = self.split_edge(d_ba_vl.x, d_ba_vu.x)
                     yield d_ba_vl
                     yield d_ba_vu
                     yield d_ba_vc
                     c_vc, vl, vu, a_vl, a_vu = vectors
-                    comb = [vl, vu, a_vl, a_vu, ba_vl, ba_vu]
+                    comb = [vl, vu, a_vl, a_vu,
+                            ba_vl,
+                            ba_vu]
                     comb_iter = itertools.combinations(comb, 2)
                     for vecs in comb_iter:
                         self.split_edge(vecs[0].x, vecs[1].x)
 
-            # Copy lists for iteration
-            cCox = Cox[i]
-            cCcx = Ccx[i]
-            cCux = Cux[i]
-            VL, VC, VU = cCox, cCcx, cCux
-            for k, (vl, vc, vu) in enumerate(zip(VL, VC, VU)):
-                # Build aN vertices for each lower-upper pair in N:
-                a_vu = list(vu.x)
-                a_vu[i + 1] = vut[i + 1]
-
-                # Connect vertices in N to corresponding vertices
-                # in aN:
-                a_vu = self.V[tuple(a_vu)]
-                yield a_vl.x
-                # Split the a + b edge of the initial triangulation:
-                c_vc = self.split_edge(vl.x, a_vu.x)
-                self.split_edge(vl.x, vu.x)  # Equal to vc
-                c_vc.connect(vco)
-                c_vc.connect(vc)
-                c_vc.connect(vl)  # Connect c + ac operations
-                c_vc.connect(vu)  # Connect c + ac operations
-                c_vc.connect(a_vu)  # Connect c + ac operations
-                yield (c_vc.x)
-                # yield at end of loop
-                c_vu = self.split_edge(vu.x, a_vu.x)
-                c_vu.connect(vco)
-                # Connect remaining cN group vertices
-                c_vc.connect(c_vu)  # Connect cN group vertices
-                yield (c_vu.x)
-                Cox[i + 1].append(vu)
-                Ccx[i + 1].append(c_vu)
-                Cux[i + 1].append(a_vu)
-                s_ab_C.append([c_vc, vl, vu, a_vu])
-                yield a_vu.x
+                # Copy lists for iteration
+                cCox = Cox[i]
+                cCcx = Ccx[i]
+                cCux = Cux[i]
+                VL, VC, VU = cCox, cCcx, cCux
+                for k, (vl, vc, vu) in enumerate(zip(VL, VC, VU)):
+                    # Build aN vertices for each lower-upper pair in N:
+                    a_vu = list(vu.x)
+                    a_vu[i + 1] = vut[i + 1]
+
+                    # Connect vertices in N to corresponding vertices
+                    # in aN:
+                    a_vu = self.V[tuple(a_vu)]
+                    yield a_vl.x
+                    # Split the a + b edge of the initial triangulation:
+                    c_vc = self.split_edge(vl.x, a_vu.x)
+                    self.split_edge(vl.x, vu.x)  # Equal to vc
+                    c_vc.connect(vco)
+                    c_vc.connect(vc)
+                    c_vc.connect(vl)  # Connect c + ac operations
+                    c_vc.connect(vu)  # Connect c + ac operations
+                    c_vc.connect(a_vu)  # Connect c + ac operations
+                    yield (c_vc.x)
+                    c_vu = self.split_edge(vu.x,
+                                           a_vu.x)  # yield at end of loop
+                    c_vu.connect(vco)
+                    # Connect remaining cN group vertices
+                    c_vc.connect(c_vu)  # Connect cN group vertices
+                    yield (c_vu.x)
+
+                    # Update the containers
+                    Cox[i + 1].append(vu)
+                    Ccx[i + 1].append(c_vu)
+                    Cux[i + 1].append(a_vu)
+
+                    # Update old containers
+                    s_ab_C.append([c_vc, vl, vu, a_vu])
+
+                    yield a_vu.x
+
         # Clean class trash
         try:
-            del C0x
-            del cC0x
-            del C1x
-            del cC1x
+            del Cox
+            del Ccx
+            del Cux
             del ab_C
             del ab_Cc
         except UnboundLocalError:
             pass
 
         try:
             self.triangulated_vectors.remove((tuple(origin_c),
                                               tuple(supremum_c)))
         except ValueError:
-            pass # Turn this into a logging warning?
-
+            # Turn this into a logging warning?
+            pass
         # Add newly triangulated vectors:
         for vs in sup_set:
             self.triangulated_vectors.append((tuple(vco.x), tuple(vs.x)))
 
         # Extra yield to ensure that the triangulation is completed
         if centroid:
             vcn_set = set()
-            vcn_list = []
             c_nn_lists = []
             for vs in sup_set:
                 # Build centroid
                 c_nn = self.vpool(vco.x, vs.x)
                 try:
                     c_nn.remove(vcn_set)
                 except KeyError:
@@ -987,52 +972,44 @@
         else:
             pass
 
         yield vut
         return
 
     def refine_star(self, v):
-        """
-        Refine the star domain of a vertex v
-        :param v: Vertex object
-        """
+        """Refine the star domain of a vertex `v`."""
         # Copy lists before iteration
         vnn = copy.copy(v.nn)
         v1nn = []
         d_v0v1_set = set()
         for v1 in vnn:
             v1nn.append(copy.copy(v1.nn))
 
         for v1, v1nn in zip(vnn, v1nn):
-            print('-')
-            print(f'v1.x = {v1.x}')
             vnnu = v1nn.intersection(vnn)
-            print(f'vnnu = {vnnu}')
 
             d_v0v1 = self.split_edge(v.x, v1.x)
             for o_d_v0v1 in d_v0v1_set:
                 d_v0v1.connect(o_d_v0v1)
             d_v0v1_set.add(d_v0v1)
             for v2 in vnnu:
-                print(f'v2 = {v2}')
                 d_v1v2 = self.split_edge(v1.x, v2.x)
                 d_v0v1.connect(d_v1v2)
         return
 
     @lru_cache(maxsize=None)
     def split_edge(self, v1, v2):
         v1 = self.V[v1]
         v2 = self.V[v2]
         # Destroy original edge, if it exists:
         v1.disconnect(v2)
         # Compute vertex on centre of edge:
         try:
             vct = (v2.x_a - v1.x_a) / 2.0 + v1.x_a
         except TypeError:  # Allow for decimal operations
-            #TODO: Only except float
             vct = (v2.x_a - v1.x_a) / decimal.Decimal(2.0) + v1.x_a
 
         vc = self.V[tuple(vct)]
         # Connect to original 2 vertices to the new centre vertex
         vc.connect(v1)
         vc.connect(v2)
         return vc
@@ -1051,16 +1028,14 @@
         bu = list(vst)
         for i, (voi, vsi) in enumerate(zip(vot, vst)):
             if bl[i] > vsi:
                 bl[i] = vsi
             if bu[i] < voi:
                 bu[i] = voi
 
-        # TODO: These for loops can easily be replaced by numpy operations,
-        #      tests should be run to determine which method is faster.
         #      NOTE: This is mostly done with sets/lists because we aren't sure
         #            how well the numpy arrays will scale to thousands of
         #             dimensions.
         vn_pool = set()
         vn_pool.update(vo.nn)
         vn_pool.update(vs.nn)
         cvn_pool = copy.copy(vn_pool)
@@ -1075,22 +1050,177 @@
                         pass  # NOTE: Not all neigbouds are in initial pool
         return vn_pool
 
     def vf_to_vv(self, vertices, simplices):
         """
         Convert a vertex-face mesh to a vertex-vertex mesh used by this class
 
-        :param vertices: list of vertices
-        :param simplices: list of simplices
-        :return:
+        Parameters
+        ----------
+        vertices : list
+            Vertices
+        simplices : list
+            Simplices
         """
         if self.dim > 1:
             for s in simplices:
                 edges = itertools.combinations(s, self.dim)
                 for e in edges:
                     self.V[tuple(vertices[e[0]])].connect(
                         self.V[tuple(vertices[e[1]])])
         else:
             for e in simplices:
                 self.V[tuple(vertices[e[0]])].connect(
                     self.V[tuple(vertices[e[1]])])
         return
+
+    def connect_vertex_non_symm(self, v_x, near=None):
+        """
+        Adds a vertex at coords v_x to the complex that is not symmetric to the
+        initial triangulation and sub-triangulation.
+
+        If near is specified (for example; a star domain or collections of
+        cells known to contain v) then only those simplices containd in near
+        will be searched, this greatly speeds up the process.
+
+        If near is not specified this method will search the entire simplicial
+        complex structure.
+
+        Parameters
+        ----------
+        v_x : tuple
+            Coordinates of non-symmetric vertex
+        near : set or list
+            List of vertices, these are points near v to check for
+        """
+        if near is None:
+            star = self.V
+        else:
+            star = near
+        # Create the vertex origin
+        if tuple(v_x) in self.V.cache:
+            if self.V[v_x] in self.V_non_symm:
+                pass
+            else:
+                return
+
+        self.V[v_x]
+        found_nn = False
+        S_rows = []
+        for v in star:
+            S_rows.append(v.x)
+
+        S_rows = numpy.array(S_rows)
+        A = numpy.array(S_rows) - numpy.array(v_x)
+        # Iterate through all the possible simplices of S_rows
+        for s_i in itertools.combinations(range(S_rows.shape[0]),
+                                          r=self.dim + 1):
+            # Check if connected, else s_i is not a simplex
+            valid_simplex = True
+            for i in itertools.combinations(s_i, r=2):
+                # Every combination of vertices must be connected, we check of
+                # the current iteration of all combinations of s_i are
+                # connected we break the loop if it is not.
+                if ((self.V[tuple(S_rows[i[1]])] not in
+                        self.V[tuple(S_rows[i[0]])].nn)
+                    and ((self.V[tuple(S_rows[i[0]])] not in
+                         self.V[tuple(S_rows[i[1]])].nn))):
+                    valid_simplex = False
+                    break
+
+            S = S_rows[tuple([s_i])]
+            if valid_simplex:
+                if self.deg_simplex(S, proj=None):
+                    valid_simplex = False
+
+            # If s_i is a valid simplex we can test if v_x is inside si
+            if valid_simplex:
+                # Find the A_j0 value from the precalculated values
+                A_j0 = A[tuple([s_i])]
+                if self.in_simplex(S, v_x, A_j0):
+                    found_nn = True
+                    # breaks the main for loop, s_i is the target simplex:
+                    break
+
+        # Connect the simplex to point
+        if found_nn:
+            for i in s_i:
+                self.V[v_x].connect(self.V[tuple(S_rows[i])])
+        # Attached the simplex to storage for all non-symmetric vertices
+        self.V_non_symm.append(self.V[v_x])
+        # this bool value indicates a successful connection if True:
+        return found_nn
+
+    def in_simplex(self, S, v_x, A_j0=None):
+        """Check if a vector v_x is in simplex `S`.
+
+        Parameters
+        ----------
+        S : array_like
+            Array containing simplex entries of vertices as rows
+        v_x :
+            A candidate vertex
+        A_j0 : array, optional,
+            Allows for A_j0 to be pre-calculated
+
+        Returns
+        -------
+        res : boolean
+            True if `v_x` is in `S`
+        """
+        A_11 = numpy.delete(S, 0, 0) - S[0]
+
+        sign_det_A_11 = numpy.sign(numpy.linalg.det(A_11))
+        if sign_det_A_11 == 0:
+            # NOTE: We keep the variable A_11, but we loop through A_jj
+            # ind=
+            # while sign_det_A_11 == 0:
+            #    A_11 = numpy.delete(S, ind, 0) - S[ind]
+            #    sign_det_A_11 = numpy.sign(numpy.linalg.det(A_11))
+
+            sign_det_A_11 = -1  # TODO: Choose another det of j instead?
+            # TODO: Unlikely to work in many cases
+
+        if A_j0 is None:
+            A_j0 = S - v_x
+
+        for d in range(self.dim + 1):
+            det_A_jj = (-1)**d * sign_det_A_11
+            # TODO: Note that scipy might be faster to add as an optional
+            #       dependency
+            sign_det_A_j0 = numpy.sign(numpy.linalg.det(numpy.delete(A_j0, d,
+                                                                     0)))
+            # TODO: Note if sign_det_A_j0 == then the point is coplanar to the
+            #       current simplex facet, so perhaps return True and attach?
+            if det_A_jj == sign_det_A_j0:
+                continue
+            else:
+                return False
+
+        return True
+
+    def deg_simplex(self, S, proj=None):
+        """Test a simplex S for degeneracy (linear dependence in R^dim).
+
+        Parameters
+        ----------
+        S : np.array
+            Simplex with rows as vertex vectors
+        proj : array, optional,
+            If the projection S[1:] - S[0] is already
+            computed it can be added as an optional argument.
+        """
+        # Strategy: we test all combination of faces, if any of the
+        # determinants are zero then the vectors lie on the same face and is
+        # therefore linearly dependent in the space of R^dim
+        if proj is None:
+            proj = S[1:] - S[0]
+
+        # TODO: Is checking the projection of one vertex against faces of other
+        #       vertices sufficient? Or do we need to check more vertices in
+        #       dimensions higher than 2?
+        # TODO: Literature seems to suggest using proj.T, but why is this
+        #       needed?
+        if numpy.linalg.det(proj) == 0.0:  # TODO: Repalace with tolerance?
+            return True  # Simplex is degenerate
+        else:
+            return False  # Simplex is not degenerate
```

### Comparing `shgo-0.5.1/shgo/_shgo_lib/_vertex.py` & `shgo-1.0.0/shgo/_shgo_lib/_vertex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import collections
 from abc import ABC, abstractmethod
-import logging
-import copy
+
 import numpy as np
-from functools import partial
-import multiprocessing as mp
 
-#from hyperct._field import *
+from scipy._lib._util import MapWrapper
+
 
-"""Vertex objects"""
 class VertexBase(ABC):
     """
     Base class for a vertex.
     """
     def __init__(self, x, nn=None, index=None):
         """
         Initiation of a vertex object.
@@ -43,79 +40,85 @@
         if item not in ['x_a']:
             raise AttributeError(f"{type(self)} object has no attribute "
                                  f"'{item}'")
         if item == 'x_a':
             self.x_a = np.array(self.x)
             return self.x_a
 
-
     @abstractmethod
     def connect(self, v):
         raise NotImplementedError("This method is only implemented with an "
                                   "associated child of the base class.")
 
     @abstractmethod
     def disconnect(self, v):
         raise NotImplementedError("This method is only implemented with an "
                                   "associated child of the base class.")
 
-    def print_out(self):
-        print("Vertex: {}".format(self.x))
-        constr = 'Connections: '
-        for vc in self.nn:
-            constr += '{} '.format(vc.x)
-
-        print(constr)
-
     def star(self):
-        """
-        Returns the star domain st(v) of the vertex.
+        """Returns the star domain ``st(v)`` of the vertex.
 
-        :param v: The vertex v in st(v)
-        :return: st, a set containing all the vertices in st(v)
+        Parameters
+        ----------
+        v :
+            The vertex ``v`` in ``st(v)``
+
+        Returns
+        -------
+        st : set
+            A set containing all the vertices in ``st(v)``
         """
         self.st = self.nn
         self.st.add(self)
         return self.st
 
+
 class VertexScalarField(VertexBase):
-    """Add homology properties of a scalar field f: R^n --> R associated with
-    the geometry built from the VertexBase class"""
+    """
+    Add homology properties of a scalar field f: R^n --> R associated with
+    the geometry built from the VertexBase class
+    """
 
     def __init__(self, x, field=None, nn=None, index=None, field_args=(),
                  g_cons=None, g_cons_args=()):
         """
-        :param x: tuple, vector of vertex coordinates
-        :param field: function, a scalar field f: R^n --> R associated with
-                      the geometry
-        :param nn: list, optional, list of nearest neighbours
-        :param index: int, optional, index of the vertex
-        :param field_args: tuple, additional arguments to be passed to field
-        :param g_cons: function, constraints on the vertex
-        :param g_cons_args: tuple, additional arguments to be passed to g_cons
+        Parameters
+        ----------
+        x : tuple,
+            vector of vertex coordinates
+        field : callable, optional
+            a scalar field f: R^n --> R associated with the geometry
+        nn : list, optional
+            list of nearest neighbours
+        index : int, optional
+            index of the vertex
+        field_args : tuple, optional
+            additional arguments to be passed to field
+        g_cons : callable, optional
+            constraints on the vertex
+        g_cons_args : tuple, optional
+            additional arguments to be passed to g_cons
 
         """
         super().__init__(x, nn=nn, index=index)
 
         # Note Vertex is only initiated once for all x so only
         # evaluated once
-        #self.feasible = None
+        # self.feasible = None
 
         # self.f is externally defined by the cache to allow parallel
         # processing
-        #self.f = None  # None type that will break arithmetic operations unless
-                       # defined
+        # None type that will break arithmetic operations unless defined
+        # self.f = None
 
         self.check_min = True
         self.check_max = True
 
-
     def connect(self, v):
-        """
-        Connects self to another vertex object v.
+        """Connects self to another vertex object v.
 
         Parameters
         ----------
         v : VertexBase or VertexScalarField object
         """
         if v is not self and v not in self.nn:
             self.nn.add(v)
@@ -135,85 +138,119 @@
             # Flags for checking homology properties:
             self.check_min = True
             self.check_max = True
             v.check_min = True
             v.check_max = True
 
     def minimiser(self):
-        """Check whether this vertex is strictly less than all its neighbours"""
+        """Check whether this vertex is strictly less than all its
+           neighbours"""
         if self.check_min:
             self._min = all(self.f < v.f for v in self.nn)
             self.check_min = False
 
         return self._min
 
     def maximiser(self):
-        """Check whether this vertex is strictly greater than all its
-        neighbours"""
+        """
+        Check whether this vertex is strictly greater than all its
+        neighbours.
+        """
         if self.check_max:
             self._max = all(self.f > v.f for v in self.nn)
             self.check_max = False
 
         return self._max
 
+
 class VertexVectorField(VertexBase):
-    """Add homology properties of a scalar field f: R^n --> R^m associated with
-    the geometry built from the VertexBase class"""
+    """
+    Add homology properties of a scalar field f: R^n --> R^m associated with
+    the geometry built from the VertexBase class.
+    """
 
     def __init__(self, x, sfield=None, vfield=None, field_args=(),
                  vfield_args=(), g_cons=None,
                  g_cons_args=(), nn=None, index=None):
-        super(VertexVectorField, self).__init__(x, nn=nn, index=index)
+        super().__init__(x, nn=nn, index=index)
 
         raise NotImplementedError("This class is still a work in progress")
 
-"""
-Cache objects
-"""
-class VertexCacheBase(object):
-    """
-    Base class for a vertex cache for a simplicial complex.
-    """
+
+class VertexCacheBase:
+    """Base class for a vertex cache for a simplicial complex."""
     def __init__(self):
 
-        self.cache = collections.OrderedDict()  #TODO: Perhaps unneeded?
+        self.cache = collections.OrderedDict()
         self.nfev = 0  # Feasible points
-        self.index = -1  #TODO: Is this needed?
-
-        #TODO: Define a getitem method based on if indexing is on or not so
-        # that we do not have to do an if check every call (does the python
-        # compiler make this irrelevant or not?) and in addition whether or not
-        # we have defined a field function.
+        self.index = -1
 
     def __iter__(self):
         for v in self.cache:
             yield self.cache[v]
         return
 
     def size(self):
-        """
-        Returns the size of the vertex cache
-
-        :return:
-        """
+        """Returns the size of the vertex cache."""
         return self.index + 1
 
     def print_out(self):
         headlen = len(f"Vertex cache of size: {len(self.cache)}:")
         print('=' * headlen)
         print(f"Vertex cache of size: {len(self.cache)}:")
         print('=' * headlen)
         for v in self.cache:
             self.cache[v].print_out()
 
 
-#TODO: Make a non-linear constraint cache with no scalar field
+class VertexCube(VertexBase):
+    """Vertex class to be used for a pure simplicial complex with no associated
+    differential geometry (single level domain that exists in R^n)"""
+    def __init__(self, x, nn=None, index=None):
+        super().__init__(x, nn=nn, index=index)
+
+    def connect(self, v):
+        if v is not self and v not in self.nn:
+            self.nn.add(v)
+            v.nn.add(self)
+
+    def disconnect(self, v):
+        if v in self.nn:
+            self.nn.remove(v)
+            v.nn.remove(self)
+
+
+class VertexCacheIndex(VertexCacheBase):
+    def __init__(self):
+        """
+        Class for a vertex cache for a simplicial complex without an associated
+        field. Useful only for building and visualising a domain complex.
+
+        Parameters
+        ----------
+        """
+        super().__init__()
+        self.Vertex = VertexCube
+
+    def __getitem__(self, x, nn=None):
+        try:
+            return self.cache[x]
+        except KeyError:
+            self.index += 1
+            xval = self.Vertex(x, index=self.index)
+            # logging.info("New generated vertex at x = {}".format(x))
+            # NOTE: Surprisingly high performance increase if logging
+            # is commented out
+            self.cache[x] = xval
+            return self.cache[x]
+
+
 class VertexCacheField(VertexCacheBase):
     def __init__(self, field=None, field_args=(), g_cons=None, g_cons_args=(),
-                 workers=None):
+                 workers=1):
         """
         Class for a vertex cache for a simplicial complex with an associated
         field.
 
         Parameters
         ----------
         field : callable
@@ -228,56 +265,55 @@
             Any additional fixed parameters needed to completely specify the
             constraint functions
         workers : int  optional
             Uses `multiprocessing.Pool <multiprocessing>`) to compute the field
              functions in parrallel.
 
         """
-        #TODO: add possible h_cons tolerance check
         super().__init__()
         self.index = -1
         self.Vertex = VertexScalarField
         self.field = field
         self.field_args = field_args
-        self.wfield = FieldWraper(field, field_args)  # if workers is not None
+        self.wfield = FieldWraper(field, field_args)  # if workers is not 1
 
         self.g_cons = g_cons
         self.g_cons_args = g_cons_args
         self.wgcons = ConstraintWraper(g_cons, g_cons_args)
         self.gpool = set()  # A set of tuples to process for feasibility
 
         # Field processing objects
         self.fpool = set()  # A set of tuples to process for scalar function
         self.sfc_lock = False  # True if self.fpool is non-Empty
 
-        if workers == None:
+        if workers == 1:
             self.process_gpool = self.proc_gpool
-            if g_cons == None:
+            if g_cons is None:
                 self.process_fpool = self.proc_fpool_nog
             else:
                 self.process_fpool = self.proc_fpool_g
         else:
             self.workers = workers
-            self.pool = mp.Pool(processes=workers)  #TODO: Move this pool to
-                                                    # the complex object
+            self._mapwrapper = MapWrapper(workers)
+            self.pool = self._mapwrapper.pool
             self.process_gpool = self.pproc_gpool
-            if g_cons == None:
+            if g_cons is None:
                 self.process_fpool = self.pproc_fpool_nog
             else:
                 self.process_fpool = self.pproc_fpool_g
 
-
-    def __getitem__(self, x, nn=None): #TODO: Test to add optional nn argument?
+    def __getitem__(self, x, nn=None):
         try:
             return self.cache[x]
         except KeyError:
             self.index += 1
             xval = self.Vertex(x, field=self.field, nn=nn, index=self.index,
                                field_args=self.field_args,
-                               g_cons=self.g_cons, g_cons_args=self.g_cons_args)
+                               g_cons=self.g_cons,
+                               g_cons_args=self.g_cons_args)
 
             self.cache[x] = xval  # Define in cache
             self.gpool.add(xval)  # Add to pool for processing feasibility
             self.fpool.add(xval)  # Add to pool for processing field values
             return self.cache[x]
 
     def __getstate__(self):
@@ -296,80 +332,66 @@
         for g, args in zip(self.g_cons, self.g_cons_args):
             if g(v.x_a, *args) < 0.0:
                 v.f = np.inf
                 v.feasible = False
                 break
 
     def compute_sfield(self, v):
-        """
-        Compute the scalar field values of a vertex object `v`.
+        """Compute the scalar field values of a vertex object `v`.
 
         Parameters
         ----------
         v : VertexBase or VertexScalarField object
         """
         try:
             v.f = self.field(v.x_a, *self.field_args)
             self.nfev += 1
-        except:
+        except AttributeError:
             v.f = np.inf
-            #logging.warning(f"Field function not found at x = {self.x_a}")
+            # logging.warning(f"Field function not found at x = {self.x_a}")
         if np.isnan(v.f):
             v.f = np.inf
 
     def proc_gpool(self):
-        """
-        Process all constraints.
-        """
+        """Process all constraints."""
         if self.g_cons is not None:
             for v in self.gpool:
                 self.feasibility_check(v)
         # Clean the pool
         self.gpool = set()
 
     def pproc_gpool(self):
-        """
-        Process all constraints in parallel.
-        """
+        """Process all constraints in parallel."""
         gpool_l = []
         for v in self.gpool:
             gpool_l.append(v.x_a)
 
         G = self.pool.map(self.wgcons.gcons, gpool_l)
         for v, g in zip(self.gpool, G):
             v.feasible = g  # set vertex object attribute v.feasible = g (bool)
 
     def proc_fpool_g(self):
-        """
-        Process all field functions with constraints supplied.
-        """
-        # TODO: do try check if v.f exists
+        """Process all field functions with constraints supplied."""
         for v in self.fpool:
             if v.feasible:
                 self.compute_sfield(v)
         # Clean the pool
         self.fpool = set()
 
     def proc_fpool_nog(self):
-        """
-        Process all field functions with no constraints supplied.
-        """
-        # TODO: do try check if v.f exists
+        """Process all field functions with no constraints supplied."""
         for v in self.fpool:
             self.compute_sfield(v)
         # Clean the pool
         self.fpool = set()
 
-    #TODO: Make static method to possibly improve pickling speed
     def pproc_fpool_g(self):
         """
         Process all field functions with constraints supplied in parallel.
         """
-        #TODO: Ensure that .f is not already computed? (it shouldn't be addable
-        #      to the self.fpool if it is).
         self.wfield.func
         fpool_l = []
         for v in self.fpool:
             if v.feasible:
                 fpool_l.append(v.x_a)
             else:
                 v.f = np.inf
@@ -381,64 +403,56 @@
         # Clean the pool
         self.fpool = set()
 
     def pproc_fpool_nog(self):
         """
         Process all field functions with no constraints supplied in parallel.
         """
-        #TODO: Ensure that .f is not already computed? (it shouldn't be addable
-        #      to the self.fpool if it is).
         self.wfield.func
         fpool_l = []
         for v in self.fpool:
             fpool_l.append(v.x_a)
         F = self.pool.map(self.wfield.func, fpool_l)
         for va, f in zip(fpool_l, F):
             vt = tuple(va)
             self[vt].f = f  # set vertex object attribute v.f = f
             self.nfev += 1
         # Clean the pool
         self.fpool = set()
 
     def proc_minimisers(self):
-        """
-        Check for minimisers
-        """
+        """Check for minimisers."""
         for v in self:
             v.minimiser()
             v.maximiser()
 
 
-class ConstraintWraper(object):
-    """
-    Object to wrap constraints to pass to `multiprocessing.Pool`.
-    """
+class ConstraintWraper:
+    """Object to wrap constraints to pass to `multiprocessing.Pool`."""
     def __init__(self, g_cons, g_cons_args):
         self.g_cons = g_cons
         self.g_cons_args = g_cons_args
 
     def gcons(self, v_x_a):
         vfeasible = True
         for g, args in zip(self.g_cons, self.g_cons_args):
-            if g(v_x_a, *args) < 0.0:  #TODO: Add exception handling?
+            if g(v_x_a, *args) < 0.0:
                 vfeasible = False
                 break
         return vfeasible
 
-class FieldWraper(object):
-    """
-    Object to wrap field to pass to `multiprocessing.Pool`.
-    """
+
+class FieldWraper:
+    """Object to wrap field to pass to `multiprocessing.Pool`."""
     def __init__(self, field, field_args):
         self.field = field
         self.field_args = field_args
 
     def func(self, v_x_a):
         try:
             v_f = self.field(v_x_a, *self.field_args)
-        except:  #TODO: except only various floating issues
-            # logging.warning(f"Field function not found at x = {self.x_a}")
+        except Exception:
             v_f = np.inf
         if np.isnan(v_f):
             v_f = np.inf
 
         return v_f
```

### Comparing `shgo-0.5.1/shgo/_shgo_lib/sobol_seq.py` & `shgo-1.0.0/shgo/_shgo_lib/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `shgo-0.5.1/shgo/_shgo_lib/sobol_vec.gz` & `shgo-1.0.0/shgo/_shgo_lib/sobol_vec.gz`

 * *Files identical despite different names*

### Comparing `shgo-0.5.1/shgo/_shgo_lib/triangulation.py` & `shgo-1.0.0/shgo/_shgo_lib/triangulation.py`

 * *Files identical despite different names*

### Comparing `shgo-0.5.1/shgo/tests/test__shgo.py` & `shgo-1.0.0/shgo/tests/test__shgo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import logging
-import numpy as np
+import numpy
+import time
+from numpy.testing import assert_allclose
 import pytest
 from pytest import raises as assert_raises, warns
-from nose.tools import nottest
-from shgo import shgo
-from shgo._shgo import SHGO
+from scipy.optimize import (Bounds, minimize_scalar, minimize, rosen,
+                            rosen_der, rosen_hess)
 
-class StructTestFunction(object):
+from .._shgo import shgo, SHGO
+
+
+class StructTestFunction:
     def __init__(self, bounds, expected_x, expected_fun=None,
                  expected_xl=None, expected_funl=None):
         self.bounds = bounds
         self.expected_x = expected_x
         self.expected_fun = expected_fun
         self.expected_xl = expected_xl
         self.expected_funl = expected_funl
@@ -33,67 +37,69 @@
 
 
 class StructTest1(StructTestFunction):
     def f(self, x):
         return x[0] ** 2 + x[1] ** 2
 
     def g(x):
-        return -(np.sum(x, axis=0) - 6.0)
+        return -(numpy.sum(x, axis=0) - 6.0)
 
     cons = wrap_constraints(g)
 
 
 test1_1 = StructTest1(bounds=[(-1, 6), (-1, 6)],
                       expected_x=[0, 0])
 test1_2 = StructTest1(bounds=[(0, 1), (0, 1)],
                       expected_x=[0, 0])
 test1_3 = StructTest1(bounds=[(None, None), (None, None)],
                       expected_x=[0, 0])
 
+
 class StructTest2(StructTestFunction):
     """
     Scalar function with several minima to test all minimiser retrievals
     """
 
     def f(self, x):
-        return (x - 30) * np.sin(x)
+        return (x - 30) * numpy.sin(x)
 
     def g(x):
-        return 58 - np.sum(x, axis=0)
+        return 58 - numpy.sum(x, axis=0)
 
     cons = wrap_constraints(g)
 
 
 test2_1 = StructTest2(bounds=[(0, 60)],
                       expected_x=[1.53567906],
                       expected_fun=-28.44677132,
-                      # Important: test that funl return is in the correct order
-                      expected_xl=np.array([[1.53567906],
+                      # Important: test that funl return is in the correct
+                      # order
+                      expected_xl=numpy.array([[1.53567906],
                                                [55.01782167],
                                                [7.80894889],
                                                [48.74797493],
                                                [14.07445705],
                                                [42.4913859],
                                                [20.31743841],
                                                [36.28607535],
                                                [26.43039605],
                                                [30.76371366]]),
 
-                      expected_funl=np.array([-28.44677132, -24.99785984,
+                      expected_funl=numpy.array([-28.44677132, -24.99785984,
                                                  -22.16855376, -18.72136195,
                                                  -15.89423937, -12.45154942,
                                                  -9.63133158, -6.20801301,
                                                  -3.43727232, -0.46353338])
                       )
 
 test2_2 = StructTest2(bounds=[(0, 4.5)],
                       expected_x=[1.53567906],
                       expected_fun=[-28.44677132],
-                      expected_xl=np.array([[1.53567906]]),
-                      expected_funl=np.array([-28.44677132])
+                      expected_xl=numpy.array([[1.53567906]]),
+                      expected_funl=numpy.array([-28.44677132])
                       )
 
 
 class StructTest3(StructTestFunction):
     """
     Hock and Schittkowski 18 problem (HS18). Hoch and Schittkowski (1981)
     http://www.ai7.uni-bayreuth.de/test_problem_coll.pdf
@@ -170,33 +176,35 @@
                       expected_fun=680.6300573
                       )
 
 
 class StructTest5(StructTestFunction):
     def f(self, x):
         return (-(x[1] + 47.0)
-                * np.sin(np.sqrt(abs(x[0] / 2.0 + (x[1] + 47.0))))
-                - x[0] * np.sin(np.sqrt(abs(x[0] - (x[1] + 47.0))))
+                * numpy.sin(numpy.sqrt(abs(x[0] / 2.0 + (x[1] + 47.0))))
+                - x[0] * numpy.sin(numpy.sqrt(abs(x[0] - (x[1] + 47.0))))
                 )
 
     g = None
     cons = wrap_constraints(g)
 
 
 test5_1 = StructTest5(bounds=[(-512, 512), (-512, 512)],
                       expected_fun=[-959.64066272085051],
                       expected_x=[512., 404.23180542])
 
 
 class StructTestLJ(StructTestFunction):
     """
-    LennardJones objective function. Used to test symmetry constraints settings.
+    LennardJones objective function. Used to test symmetry constraints
+    settings.
     """
 
     def f(self, x, *args):
+        print(f'x = {x}')
         self.N = args[0]
         k = int(self.N / 3)
         s = 0.0
 
         for i in range(k - 1):
             for j in range(i + 1, k):
                 a = 3 * i
@@ -217,41 +225,38 @@
 
 N = 6
 boundsLJ = list(zip([-4.0] * 6, [4.0] * 6))
 
 testLJ = StructTestLJ(bounds=boundsLJ,
                       expected_fun=[-1.0],
                       expected_x=None,
-                      #expected_x=[-2.71247337e-08,
+                      # expected_x=[-2.71247337e-08,
                       #            -2.71247337e-08,
-                      ##            -2.50000222e+00,
+                      #            -2.50000222e+00,
                       #            -2.71247337e-08,
                       #            -2.71247337e-08,
                       #            -1.50000222e+00]
                       )
 
 
 class StructTestS(StructTestFunction):
-    #def f(self, x):
-    #    print(f'np.sum(x)**2 = {np.sum(x)**2}')
-    #    return np.sum(x)**2
-
     def f(self, x):
         return ((x[0] - 0.5) ** 2 + (x[1] - 0.5) ** 2
-                + (x[2] - 0.5) ** 2  + (x[3] - 0.5) ** 2 )
-    
+                + (x[2] - 0.5) ** 2 + (x[3] - 0.5) ** 2)
+
     g = None
     cons = wrap_constraints(g)
 
 
 test_s = StructTestS(bounds=[(0, 2.0), ] * 4,
                      expected_fun=0.0,
-                     expected_x=np.ones(4) - 0.5
+                     expected_x=numpy.ones(4) - 0.5
                      )
 
+
 class StructTestTable(StructTestFunction):
     def f(self, x):
         if x[0] == 3.0 and x[1] == 3.0:
             return 50
         else:
             return 100
 
@@ -289,51 +294,51 @@
 
 
 test_infeasible = StructTestInfeasible(bounds=[(2, 50), (-1, 1)],
                                        expected_fun=None,
                                        expected_x=None
                                        )
 
-@nottest
+
+@pytest.mark.skip("Not a test")
 def run_test(test, args=(), test_atol=1e-5, n=100, iters=None,
              callback=None, minimizer_kwargs=None, options=None,
-             sampling_method='sobol', workers=None):
+             sampling_method='sobol', workers=1):
     res = shgo(test.f, test.bounds, args=args, constraints=test.cons,
                n=n, iters=iters, callback=callback,
                minimizer_kwargs=minimizer_kwargs, options=options,
                sampling_method=sampling_method, workers=workers)
 
-    logging.info(res)
-
+    print(f'res = {res}')
+    logging.info(f'res = {res}')
     if test.expected_x is not None:
-        np.testing.assert_allclose(res.x, test.expected_x,
+        numpy.testing.assert_allclose(res.x, test.expected_x,
                                       rtol=test_atol,
                                       atol=test_atol)
 
     # (Optional tests)
     if test.expected_fun is not None:
-        np.testing.assert_allclose(res.fun,
+        numpy.testing.assert_allclose(res.fun,
                                       test.expected_fun,
                                       atol=test_atol)
 
     if test.expected_xl is not None:
-        np.testing.assert_allclose(res.xl,
+        numpy.testing.assert_allclose(res.xl,
                                       test.expected_xl,
                                       atol=test_atol)
 
     if test.expected_funl is not None:
-        np.testing.assert_allclose(res.funl,
+        numpy.testing.assert_allclose(res.funl,
                                       test.expected_funl,
                                       atol=test_atol)
-    logging.info(f'res = {res}')
     return
 
 
 # Base test functions:
-class TestShgoSobolTestFunctions(object):
+class TestShgoSobolTestFunctions:
     """
     Global optimisation tests with Sobol sampling:
     """
 
     # Sobol algorithm
     def test_f1_1_sobol(self):
         """Multivariate test function 1:
@@ -364,36 +369,34 @@
     def test_f3_sobol(self):
         """NLP: Hock and Schittkowski problem 18"""
         run_test(test3_1)
 
     @pytest.mark.slow
     def test_f4_sobol(self):
         """NLP: (High dimensional) Hock and Schittkowski 11 problem (HS11)"""
-        # run_test(test4_1, n=500)
-        # run_test(test4_1, n=800)
         options = {'infty_constraints': False}
-        #run_test(test4_1, n=990, options=options)
-        run_test(test4_1, n=990*2, options=options)
+        # run_test(test4_1, n=990, options=options)
+        run_test(test4_1, n=990 * 2, options=options)
 
     def test_f5_1_sobol(self):
         """NLP: Eggholder, multimodal"""
-        #run_test(test5_1, n=30)
+        # run_test(test5_1, n=30)
         run_test(test5_1, n=60)
 
     def test_f5_2_sobol(self):
         """NLP: Eggholder, multimodal"""
         # run_test(test5_1, n=60, iters=5)
         run_test(test5_1, n=60, iters=5)
 
         # def test_t911(self):
         #    """1D tabletop function"""
         #    run_test(test11_1)
 
 
-class TestShgoSimplicialTestFunctions(object):
+class TestShgoSimplicialTestFunctions:
     """
     Global optimisation tests with Simplicial sampling:
     """
 
     def test_f1_1_simplicial(self):
         """Multivariate test function 1:
         x[0]**2 + x[1]**2 with bounds=[(-1, 6), (-1, 6)]"""
@@ -409,15 +412,15 @@
         with bounds=[(None, None),(None, None)]"""
         run_test(test1_3, n=5, sampling_method='simplicial')
 
     def test_f2_1_simplicial(self):
         """Univariate test function on
         f(x) = (x - 30) * sin(x) with bounds=[(0, 60)]"""
         options = {'minimize_every_iter': False}
-        run_test(test2_1, iters=7, options=options,
+        run_test(test2_1, n=200, iters=7, options=options,
                  sampling_method='simplicial')
 
     def test_f2_2_simplicial(self):
         """Univariate test function on
         f(x) = (x - 30) * sin(x) bounds=[(0, 4.5)]"""
         run_test(test2_2, n=1, sampling_method='simplicial')
 
@@ -426,111 +429,140 @@
         run_test(test3_1, n=1, sampling_method='simplicial')
 
     @pytest.mark.slow
     def test_f4_simplicial(self):
         """NLP: (High dimensional) Hock and Schittkowski 11 problem (HS11)"""
         run_test(test4_1, n=1, sampling_method='simplicial')
 
+    def test_lj_symmetry_old(self):
+        """LJ: Symmetry-constrained test function"""
+        options = {'symmetry': True,
+                   'disp': True}
+        args = (6,)  # Number of atoms
+        run_test(testLJ, args=args, n=300,
+                 options=options, iters=1,
+                 sampling_method='simplicial')
+
     def test_f5_1_lj_symmetry(self):
         """LJ: Symmetry constrained test function"""
-        options = {'symmetry': [0, ]*6,
+        options = {'symmetry': [0, ] * 6,
                    'disp': True}
         args = (6,)  # No. of atoms
 
-        run_test(testLJ, args=args, n=100,
-                 options=options, iters=3,
+        run_test(testLJ, args=args, n=300,
+                 options=options, iters=1,
                  sampling_method='simplicial')
 
-        #run_test(testLJ, args=args, n=None,
-        #         options=options, iters=3,
-        #         sampling_method='simplicial')
-
-        #run_test(testLJ, args=args, n=None,
-        #         options=options, iters=4,
-        #         sampling_method='simplicial')
-
     def test_f5_2_cons_symmetry(self):
         """Symmetry constrained test function"""
         options = {'symmetry': [0, 0],
                    'disp': True}
 
-        #dim = len(options['symmetry'])
-        #test_s = StructTestS(bounds=[(0, 2.0),]*dim,
-        #                     expected_fun=np.zeros(dim),
-        #                      expected_x=np.zeros(dim))
-
-        run_test(test1_1, n=100,
-                 options=options, iters=2,
+        run_test(test1_1, n=200,
+                 options=options, iters=1,
                  sampling_method='simplicial')
 
     def test_f5_3_cons_symmetry(self):
         """Assymmetrically constrained test function"""
         options = {'symmetry': [0, 0, 0, 3],
                    'disp': True}
 
-        run_test(test_s, #n=10000,
+        run_test(test_s, n=10000,
                  options=options,
-                 #iters=2,
-                 iters=3,
+                 iters=1,
                  sampling_method='simplicial')
 
+    @pytest.mark.skip("Not a test")
+    def test_f0_min_variance(self):
+        """Return a minimum on a perfectly symmetric problem, based on
+            gh10429"""
+        avg = 0.5  # Given average value of x
+        cons = {'type': 'eq', 'fun': lambda x: numpy.mean(x) - avg}
+
+        # Minimize the variance of x under the given constraint
+        res = shgo(numpy.var, bounds=6 * [(0, 1)], constraints=cons)
+        assert res.success
+        assert_allclose(res.fun, 0, atol=1e-15)
+        assert_allclose(res.x, 0.5)
+
+    @pytest.mark.skip("Not a test")
+    def test_f0_min_variance_1D(self):
+        """Return a minimum on a perfectly symmetric 1D problem, based on
+            gh10538"""
+
+        def fun(x):
+            return x * (x - 1.0) * (x - 0.5)
+
+        bounds = [(0, 1)]
+        res = shgo(fun, bounds=bounds)
+        ref = minimize_scalar(fun, bounds=bounds[0])
+        assert res.success
+        assert_allclose(res.fun, ref.fun)
+        assert_allclose(res.x, ref.x, rtol=1e-6)
+
 # Argument test functions
-class TestShgoArguments(object):
+class TestShgoArguments:
     def test_1_1_simpl_iter(self):
         """Iterative simplicial sampling on TestFunction 1 (multivariate)"""
         run_test(test1_2, n=None, iters=2, sampling_method='simplicial')
 
     def test_1_2_simpl_iter(self):
         """Iterative simplicial on TestFunction 2 (univariate)"""
         options = {'minimize_every_iter': False}
-        #run_test(test2_1, n=None, iters=7, options=options,
-        #         sampling_method='simplicial')
         run_test(test2_1, n=None, iters=9, options=options,
                  sampling_method='simplicial')
-        #run_test(test2_1, n=None, iters=12, options=options,
-        #         sampling_method='simplicial')
 
     def test_2_1_sobol_iter(self):
         """Iterative Sobol sampling on TestFunction 1 (multivariate)"""
         run_test(test1_2, n=None, iters=1, sampling_method='sobol')
 
     def test_2_2_sobol_iter(self):
         """Iterative Sobol sampling on TestFunction 2 (univariate)"""
         res = shgo(test2_1.f, test2_1.bounds, constraints=test2_1.cons,
                    n=None, iters=1, sampling_method='sobol')
 
-        np.testing.assert_allclose(res.x, test2_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test2_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
-        np.testing.assert_allclose(res.fun, test2_1.expected_fun, atol=1e-5)
+        numpy.testing.assert_allclose(res.fun, test2_1.expected_fun, atol=1e-5)
 
     def test_3_1_disp_simplicial(self):
-        """Iterative sampling on TestFunction 1 and 2  (multi and univariate)"""
+        """Iterative sampling on TestFunction 1 and 2  (multi and univariate)
+        """
 
         def callback_func(x):
             print("Local minimization callback test")
 
         for test in [test1_1, test2_1]:
-            res = shgo(test.f, test.bounds, iters=1,
-                       sampling_method='simplicial',
-                       callback=callback_func, options={'disp': True})
-            res = shgo(test.f, test.bounds, n=1, sampling_method='simplicial',
-                       callback=callback_func, options={'disp': True})
+            shgo(test.f, test.bounds, iters=1,
+                 sampling_method='simplicial',
+                 callback=callback_func, options={'disp': True})
+            shgo(test.f, test.bounds, n=1, sampling_method='simplicial',
+                 callback=callback_func, options={'disp': True})
 
     def test_3_2_disp_sobol(self):
         """Iterative sampling on TestFunction 1 and 2 (multi and univariate)"""
 
         def callback_func(x):
             print("Local minimization callback test")
 
         for test in [test1_1, test2_1]:
-            res = shgo(test.f, test.bounds, iters=1, sampling_method='sobol',
-                       callback=callback_func, options={'disp': True})
+            shgo(test.f, test.bounds, iters=1, sampling_method='sobol',
+                 callback=callback_func, options={'disp': True})
 
-            res = shgo(test.f, test.bounds, n=1, sampling_method='simplicial',
-                       callback=callback_func, options={'disp': True})
+            shgo(test.f, test.bounds, n=1, sampling_method='simplicial',
+                 callback=callback_func, options={'disp': True})
+
+    def test_args_gh14589(self):
+        """Using `args` used to cause `shgo` to fail; see #14589, #15986,
+        #16506"""
+        res = shgo(func=lambda x, y, z: x * z + y, bounds=[(0, 3)], args=(1, 2)
+                   )
+        ref = shgo(func=lambda x: 2 * x + 1, bounds=[(0, 3)])
+        assert_allclose(res.fun, ref.fun)
+        assert_allclose(res.x, ref.x)
 
     @pytest.mark.slow
     def test_4_1_known_f_min(self):
         """Test known function minima stopping criteria"""
         # Specify known function value
         options = {'f_min': test4_1.expected_fun,
                    'f_tol': 1e-6,
@@ -548,161 +580,155 @@
             # Specify number of local iterations to perform
             'minimize_every_iter': True,
             'local_iter': 1}
 
         run_test(test4_1, n=None, test_atol=1e-5, options=options,
                  sampling_method='simplicial')
 
-    #@pytest.mark.slow
-    #@pytest.mark.skip(reason="no way of currently testing this")
-    @nottest
-    def test_4_3_known_f_min(self):
-        """Test Global mode limiting local evaluations"""
-        options = {  # Specify known function value
-            'f_min': test4_1.expected_fun,
-            'f_tol': 1e-6,
-            # Specify number of local iterations to perform+
-            'minimize_every_iter': True,
-            'local_iter': 1,
-            'infty_constraints': False}
-
-        run_test(test4_1, n=300000,
-                 test_atol=1e-5, options=options,
-                 sampling_method='sobol')
-
-    #@nottest
     def test_4_4_known_f_min(self):
         """Test Global mode limiting local evaluations for 1D funcs"""
         options = {  # Specify known function value
             'f_min': test2_1.expected_fun,
             'f_tol': 1e-6,
             # Specify number of local iterations to perform+
             'minimize_every_iter': True,
             'local_iter': 1,
             'infty_constraints': False}
 
         res = shgo(test2_1.f, test2_1.bounds, constraints=test2_1.cons,
                    n=None, iters=None, options=options,
                    sampling_method='sobol')
-        np.testing.assert_allclose(res.x, test2_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test2_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
 
     def test_5_1_simplicial_argless(self):
         """Test Default simplicial sampling settings on TestFunction 1"""
         res = shgo(test1_1.f, test1_1.bounds, constraints=test1_1.cons)
-        np.testing.assert_allclose(res.x, test1_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test1_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
 
     def test_5_2_sobol_argless(self):
         """Test Default sobol sampling settings on TestFunction 1"""
         res = shgo(test1_1.f, test1_1.bounds, constraints=test1_1.cons,
                    sampling_method='sobol')
-        np.testing.assert_allclose(res.x, test1_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test1_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
 
     def test_6_1_simplicial_max_iter(self):
         """Test that maximum iteration option works on TestFunction 3"""
         options = {'max_iter': 2}
         res = shgo(test3_1.f, test3_1.bounds, constraints=test3_1.cons,
                    options=options, sampling_method='simplicial')
-        np.testing.assert_allclose(res.x, test3_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test3_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
-        np.testing.assert_allclose(res.fun, test3_1.expected_fun, atol=1e-5)
+        numpy.testing.assert_allclose(res.fun, test3_1.expected_fun, atol=1e-5)
 
     def test_6_2_simplicial_min_iter(self):
         """Test that maximum iteration option works on TestFunction 3"""
         options = {'min_iter': 2}
         res = shgo(test3_1.f, test3_1.bounds, constraints=test3_1.cons,
                    options=options, sampling_method='simplicial')
-        np.testing.assert_allclose(res.x, test3_1.expected_x, rtol=1e-5,
+        numpy.testing.assert_allclose(res.x, test3_1.expected_x, rtol=1e-5,
                                       atol=1e-5)
-        np.testing.assert_allclose(res.fun, test3_1.expected_fun, atol=1e-5)
+        numpy.testing.assert_allclose(res.fun, test3_1.expected_fun, atol=1e-5)
 
     def test_7_1_minkwargs(self):
         """Test the minimizer_kwargs arguments for solvers with constraints"""
         # Test solvers
         for solver in ['COBYLA', 'SLSQP']:
             # Note that passing global constraints to SLSQP is tested in other
             # unittests which run test4_1 normally
             minimizer_kwargs = {'method': solver,
                                 'constraints': test3_1.cons}
             run_test(test3_1, n=100, test_atol=1e-3,
-                     minimizer_kwargs=minimizer_kwargs, sampling_method='sobol')
+                     minimizer_kwargs=minimizer_kwargs,
+                     sampling_method='sobol')
 
     def test_7_2_minkwargs(self):
         """Test the minimizer_kwargs default inits"""
         minimizer_kwargs = {'ftol': 1e-5}
         options = {'disp': True}  # For coverage purposes
-        SHGOc = SHGO(test3_1.f, test3_1.bounds, constraints=test3_1.cons[0],
-                     minimizer_kwargs=minimizer_kwargs, options=options)
+        SHGO(test3_1.f, test3_1.bounds, constraints=test3_1.cons[0],
+             minimizer_kwargs=minimizer_kwargs, options=options)
 
     def test_7_3_minkwargs(self):
         """Test minimizer_kwargs arguments for solvers without constraints"""
         for solver in ['Nelder-Mead', 'Powell', 'CG', 'BFGS', 'Newton-CG',
                        'L-BFGS-B', 'TNC', 'dogleg', 'trust-ncg', 'trust-exact',
                        'trust-krylov']:
             def jac(x):
-                return np.array([2 * x[0], 2 * x[1]]).T
+                return numpy.array([2 * x[0], 2 * x[1]]).T
 
             def hess(x):
-                return np.array([[2, 0], [0, 2]])
+                return numpy.array([[2, 0], [0, 2]])
 
             minimizer_kwargs = {'method': solver,
                                 'jac': jac,
                                 'hess': hess}
-            logging.info("Solver = {}".format(solver))
+            logging.info(f"Solver = {solver}")
             logging.info("=" * 100)
             run_test(test1_1, n=100, test_atol=1e-3,
-                     minimizer_kwargs=minimizer_kwargs, sampling_method='sobol')
+                     minimizer_kwargs=minimizer_kwargs,
+                     sampling_method='sobol')
 
     def test_8_homology_group_diff(self):
         options = {'minhgrd': 1,
                    'minimize_every_iter': True}
 
         run_test(test1_1, n=None, iters=None, options=options,
                  sampling_method='simplicial')
 
     def test_9_cons_g(self):
         """Test single function constraint passing"""
-        SHGOc = SHGO(test3_1.f, test3_1.bounds, constraints=test3_1.cons[0])
+        SHGO(test3_1.f, test3_1.bounds, constraints=test3_1.cons[0])
 
     def test_10_finite_time(self):
         """Test single function constraint passing"""
         options = {'maxtime': 1e-15}
-        res = shgo(test1_1.f, test1_1.bounds, n=1, iters=None,
-                   options=options, sampling_method='sobol')
+
+        def f(x):
+            time.sleep(1e-14)
+            return 0.0
+
+        res = shgo(f, test1_1.bounds, iters=5, options=options)
+        # Assert that only 1 rather than 5 requested iterations ran:
+        assert res.nit == 1
 
     def test_11_f_min_0(self):
         """Test to cover the case where f_lowest == 0"""
         options = {'f_min': 0.0,
                    'disp': True}
         res = shgo(test1_2.f, test1_2.bounds, n=10, iters=None,
                    options=options, sampling_method='sobol')
-        np.testing.assert_equal(0, res.x[0])
-        np.testing.assert_equal(0, res.x[1])
+        numpy.testing.assert_equal(0, res.x[0])
+        numpy.testing.assert_equal(0, res.x[1])
 
-    @nottest
+    # @nottest
+    @pytest.mark.skip(reason="no way of currently testing this")
     def test_12_sobol_inf_cons(self):
         """Test to cover the case where f_lowest == 0"""
-        #TODO: This test doesn't cover anything new, it is unknown what the
+        # TODO: This test doesn't cover anything new, it is unknown what the
         # original test was intended for as it was never complete. Delete or
         # replace in the future.
         options = {'maxtime': 1e-15,
                    'f_min': 0.0}
         res = shgo(test1_2.f, test1_2.bounds, n=1, iters=None,
                    options=options, sampling_method='sobol')
-        np.testing.assert_equal(0.0, res.fun)
+        numpy.testing.assert_equal(0.0, res.fun)
 
     def test_13_high_sobol(self):
         """Test init of high-dimensional sobol sequences"""
+
         def f(x):
             return 0
+
         bounds = [(None, None), ] * 41
         SHGOc = SHGO(f, bounds, sampling_method='sobol')
-        SHGOc.sobol_points(2, 50)
+        # SHGOc.sobol_points(2, 50)
+        SHGOc.sampling_function(2, 50)
 
     def test_14_local_iter(self):
         """Test limited local iterations for a pseudo-global mode"""
         options = {'local_iter': 4}
         run_test(test5_1, n=60, options=options)
 
     def test_15_min_every_iter(self):
@@ -716,113 +742,215 @@
         options = {'disp': True}
         minimizer_kwargs = {'method': 'nelder-mead'}
         run_test(test1_2, sampling_method='simplicial',
                  options=options, minimizer_kwargs=minimizer_kwargs)
 
     def test_17_custom_sampling(self):
         """Test the functionality to add custom sampling methods to shgo"""
+
         def sample(n, d):
-            return np.random.uniform(size=(n,d))
-        
+            return numpy.random.uniform(size=(n, d))
+
         run_test(test1_1, n=30, sampling_method=sample)
 
-    def test_18_parallelization(self):
+    def test_18_bounds_class(self):
+        # test that new and old bounds yield same result
+        def f(x):
+            return numpy.square(x).sum()
+
+        lb = [-6., 1., -5.]
+        ub = [-1., 3., 5.]
+        bounds_old = list(zip(lb, ub))
+        bounds_new = Bounds(lb, ub)
+
+        res_old_bounds = shgo(f, bounds_old)
+        res_new_bounds = shgo(f, bounds_new)
+
+        assert res_new_bounds.nfev == res_old_bounds.nfev
+        assert res_new_bounds.message == res_old_bounds.message
+        assert res_new_bounds.success == res_old_bounds.success
+        x_opt = numpy.array([-1., 1., 0.])
+        numpy.testing.assert_allclose(res_new_bounds.x, x_opt)
+        numpy.testing.assert_allclose(res_new_bounds.x,
+                                      res_old_bounds.x)
+
+    def test_19_parallelization(self):
         """Test the functionality to add custom sampling methods to shgo"""
 
         run_test(test1_1, n=30, workers=1)  # Constrained
         run_test(test_s, n=30, workers=1)  # Unconstrained
 
-    def test_19_constrained_args(self):
+    def test_20_constrained_args(self):
         """Test that constraints can be passed to arguments"""
+
         def eggholder(x):
             return (-(x[1] + 47.0)
-                    * np.sin(np.sqrt(abs(x[0] / 2.0 + (x[1] + 47.0))))
-                    - x[0] * np.sin(np.sqrt(abs(x[0] - (x[1] + 47.0))))
+                    * numpy.sin(numpy.sqrt(abs(x[0] / 2.0 + (x[1] + 47.0))))
+                    - x[0] * numpy.sin(numpy.sqrt(abs(x[0] - (x[1] + 47.0))))
                     )
 
         def f(x):  # (cattle-feed)
             return 24.55 * x[0] + 26.75 * x[1] + 39 * x[2] + 40.50 * x[3]
 
         bounds = [(0, 1.0), ] * 4
-        
+
         def g1_modified(x, i):
             return i * 2.3 * x[0] + i * 5.6 * x[1] + 11.1 * x[2] + 1.3 * x[
                 3] - 5  # >=0
 
         def g2(x):
             return (12 * x[0] + 11.9 * x[1] + 41.8 * x[2] + 52.1 * x[3] - 21
-                    - 1.645 * np.sqrt(0.28 * x[0] ** 2 + 0.19 * x[1] ** 2
-                                      + 20.5 * x[2] ** 2 + 0.62 * x[3] ** 2)
+                    - 1.645 * numpy.sqrt(0.28 * x[0] ** 2 + 0.19 * x[1] ** 2
+                                         + 20.5 * x[2] ** 2 + 0.62 * x[3] ** 2)
                     )  # >=0
 
         def h1(x):
             return x[0] + x[1] + x[2] + x[3] - 1  # == 0
 
-
         cons = ({'type': 'ineq', 'fun': g1_modified, "args": (0,)},
                 {'type': 'ineq', 'fun': g2},
                 {'type': 'eq', 'fun': h1})
 
-        res_modConstr = shgo(f, bounds, iters=3, constraints=cons)
+        shgo(f, bounds, n=300, iters=1, constraints=cons)
         # using constrain with arguments AND sampling method sobol
-        res_modConstr_sobol = shgo(f, bounds, iters=3, constraints=cons,
-                                   sampling_method='sobol')
+        shgo(f, bounds, n=300, iters=1, constraints=cons,
+             sampling_method='sobol')
 
-    def test_20_jac_true(self):
+    def test_21_1_jac_true(self):
         """Test that shgo can handle objective functions that return the
-        gradient alongside the objective value"""
+        gradient alongside the objective value. Fixes gh-13547"""
+        # previous
         def func(x):
-            return np.sum(np.power(x, 2)), 2 * x
+            return numpy.sum(numpy.power(x, 2)), 2 * x
 
         shgo(
             func,
             bounds=[[-1, 1], [1, 2]],
             n=100, iters=5,
             sampling_method="sobol",
             minimizer_kwargs={'method': 'SLSQP', 'jac': True}
         )
 
-        
+        # new
+        def func(x):
+            return numpy.sum(x ** 2), 2 * x
+
+        bounds = [[-1, 1], [1, 2], [-1, 1], [1, 2], [0, 3]]
+
+        res = shgo(func, bounds=bounds, sampling_method="sobol",
+                   minimizer_kwargs={'method': 'SLSQP', 'jac': True})
+        ref = minimize(func, x0=[1, 1, 1, 1, 1], bounds=bounds,
+                       jac=True)
+        assert res.success
+        assert_allclose(res.fun, ref.fun)
+        assert_allclose(res.x, ref.x, atol=1e-15)
+
+    @pytest.mark.parametrize('derivative', ['jac', 'hess', 'hessp'])
+    def test_21_2_derivative_options(self, derivative):
+        """shgo used to raise an error when passing `options` with 'jac'
+        # see gh-12963. check that this is resolved
+        """
+
+        def objective(x):
+            return 3 * x[0] * x[0] + 2 * x[0] + 5
+
+        def gradient(x):
+            return 6 * x[0] + 2
+
+        def hess(x):
+            return 6
+
+        def hessp(x, p):
+            return 6 * p
+
+        derivative_funcs = {'jac': gradient, 'hess': hess, 'hessp': hessp}
+        options = {derivative: derivative_funcs[derivative]}
+        minimizer_kwargs = {'method': 'trust-constr'}
+
+        bounds = [(-100, 100)]
+        res = shgo(objective, bounds, minimizer_kwargs=minimizer_kwargs,
+                   options=options)
+        ref = minimize(objective, x0=[0], bounds=bounds, **minimizer_kwargs,
+                       **options)
+
+        assert res.success
+        numpy.testing.assert_allclose(res.fun, ref.fun)
+        numpy.testing.assert_allclose(res.x, ref.x)
+
+    def test_21_3_hess_options_rosen(self):
+        """Ensure the Hessian gets passed correctly to the local minimizer
+        routine. Previous report gh-14533.
+        """
+        bounds = [(0, 1.6), (0, 1.6), (0, 1.4), (0, 1.4), (0, 1.4)]
+        options = {'jac': rosen_der, 'hess': rosen_hess}
+        minimizer_kwargs = {'method': 'Newton-CG'}
+        res = shgo(rosen, bounds, minimizer_kwargs=minimizer_kwargs,
+                   options=options)
+        ref = minimize(rosen, numpy.zeros(5), method='Newton-CG',
+                       **options)
+        assert res.success
+        assert_allclose(res.fun, ref.fun)
+        assert_allclose(res.x, ref.x, atol=1e-15)
+
+    def test_21_arg_tuple_sobol(self):
+        """shgo used to raise an error when passing `args` with Sobol sampling
+        # see gh-12114. check that this is resolved"""
+
+        def fun(x, k):
+            return x[0] ** k
+
+        constraints = ({'type': 'ineq', 'fun': lambda x: x[0] - 1})
+
+        bounds = [(0, 10)]
+        res = shgo(fun, bounds, args=(1,), constraints=constraints,
+                   sampling_method='sobol')
+        ref = minimize(fun, numpy.zeros(1), bounds=bounds, args=(1,),
+                       constraints=constraints)
+        assert res.success
+        assert_allclose(res.fun, ref.fun)
+        assert_allclose(res.x, ref.x)
+
+
 # Failure test functions
-class TestShgoFailures(object):
+class TestShgoFailures:
     def test_1_maxiter(self):
         """Test failure on insufficient iterations"""
         options = {'maxiter': 2}
         res = shgo(test4_1.f, test4_1.bounds, n=2, iters=None,
                    options=options, sampling_method='sobol')
 
-        np.testing.assert_equal(False, res.success)
-        #np.testing.assert_equal(4, res.nfev)
-        np.testing.assert_equal(4, res.tnev)
+        numpy.testing.assert_equal(False, res.success)
+        # numpy.testing.assert_equal(4, res.nfev)
+        numpy.testing.assert_equal(4, res.tnev)
 
     def test_2_sampling(self):
         """Rejection of unknown sampling method"""
         assert_raises(ValueError, shgo, test1_1.f, test1_1.bounds,
                       sampling_method='not_Sobol')
 
     def test_3_1_no_min_pool_sobol(self):
         """Check that the routine stops when no minimiser is found
            after maximum specified function evaluations"""
         options = {'maxfev': 10,
-                   #'maxev': 10,
+                   # 'maxev': 10,
                    'disp': True}
         res = shgo(test_table.f, test_table.bounds, n=3, options=options,
                    sampling_method='sobol')
-        np.testing.assert_equal(False, res.success)
-        # np.testing.assert_equal(9, res.nfev)
-        np.testing.assert_equal(12, res.nfev)
+        numpy.testing.assert_equal(False, res.success)
+        # numpy.testing.assert_equal(9, res.nfev)
+        numpy.testing.assert_equal(12, res.nfev)
 
     def test_3_2_no_min_pool_simplicial(self):
         """Check that the routine stops when no minimiser is found
            after maximum specified sampling evaluations"""
         options = {'maxev': 10,
                    'disp': True}
         res = shgo(test_table.f, test_table.bounds, n=3, options=options,
                    sampling_method='simplicial')
-        np.testing.assert_equal(False, res.success)
+        numpy.testing.assert_equal(False, res.success)
 
     def test_4_1_bound_err(self):
         """Specified bounds ub > lb"""
         bounds = [(6, 3), (3, 5)]
         assert_raises(ValueError, shgo, test1_1.f, bounds)
 
     def test_4_2_bound_err(self):
@@ -836,40 +964,40 @@
         options = {'maxev': 100,
                    'disp': True}
 
         res = shgo(test_infeasible.f, test_infeasible.bounds,
                    constraints=test_infeasible.cons, n=100, options=options,
                    sampling_method='sobol')
 
-        np.testing.assert_equal(False, res.success)
+        numpy.testing.assert_equal(False, res.success)
 
     def test_5_1_2_infeasible_sobol(self):
         """Ensures the algorithm terminates on infeasible problems
            after maxev is exceeded. Do not use infty constraints option"""
         options = {'maxev': 100,
                    'disp': True,
                    'infty_constraints': False}
 
         res = shgo(test_infeasible.f, test_infeasible.bounds,
                    constraints=test_infeasible.cons, n=100, options=options,
                    sampling_method='sobol')
 
-        np.testing.assert_equal(False, res.success)
+        numpy.testing.assert_equal(False, res.success)
 
     def test_5_2_infeasible_simplicial(self):
         """Ensures the algorithm terminates on infeasible problems
            after maxev is exceeded."""
         options = {'maxev': 1000,
                    'disp': False}
 
         res = shgo(test_infeasible.f, test_infeasible.bounds,
                    constraints=test_infeasible.cons, n=100, options=options,
                    sampling_method='simplicial')
 
-        np.testing.assert_equal(False, res.success)
+        numpy.testing.assert_equal(False, res.success)
 
     def test_6_1_lower_known_f_min(self):
         """Test Global mode limiting local evaluations with f* too high"""
         options = {  # Specify known function value
             'f_min': test2_1.expected_fun + 2.0,
             'f_tol': 1e-6,
             # Specify number of local iterations to perform+
@@ -881,7 +1009,46 @@
                   'n': None,
                   'iters': None,
                   'options': options,
                   'sampling_method': 'sobol'
                   }
         warns(UserWarning, shgo, *args, **kwargs)
 
+    def test(self):
+        from scipy.optimize import rosen, shgo
+        bounds = [(0, 2), (0, 2), (0, 2), (0, 2), (0, 2)]
+
+        def fun(x):
+            fun.nfev += 1
+            return rosen(x)
+
+        fun.nfev = 0
+
+        result = shgo(fun, bounds)
+        print(result.x, result.fun, fun.nfev)  # 50
+
+
+# Returns
+class TestShgoReturns:
+    def test_1_nfev_simplicial(self):
+        bounds = [(0, 2), (0, 2), (0, 2), (0, 2), (0, 2)]
+
+        def fun(x):
+            fun.nfev += 1
+            return rosen(x)
+
+        fun.nfev = 0
+
+        result = shgo(fun, bounds)
+        numpy.testing.assert_equal(fun.nfev, result.nfev)
+
+    def test_1_nfev_sobol(self):
+        bounds = [(0, 2), (0, 2), (0, 2), (0, 2), (0, 2)]
+
+        def fun(x):
+            fun.nfev += 1
+            return rosen(x)
+
+        fun.nfev = 0
+
+        result = shgo(fun, bounds, sampling_method='sobol')
+        numpy.testing.assert_equal(fun.nfev, result.nfev)
```

### Comparing `shgo-0.5.1/shgo.egg-info/PKG-INFO` & `shgo-1.0.0/shgo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 Metadata-Version: 2.1
 Name: shgo
-Version: 0.5.1
+Version: 1.0.0
 Summary: Simplicial homology global optimisation
 Home-page: https://github.com/stefan-endres/shgo
 Author: Stefan Endres, Carl Sandrock
 Author-email: stefan.c.endres@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/Stefan-Endres/shgo.svg?branch=master
-            :target: https://travis-ci.org/Stefan-Endres/shgo
-        .. image:: https://coveralls.io/repos/github/Stefan-Endres/shgo/badge.png?branch=master
-            :target: https://coveralls.io/github/Stefan-Endres/shgo?branch=master
-        
-        Repository: https://github.com/Stefan-Endres/shgo
-        
-        Description
-        -----------
-        
-        Finds the global minimum of a function using simplicial homology global
-        optimisation (shgo_). Appropriate for solving general purpose NLP and blackbox
-        optimisation problems to global optimality (low dimensional problems).
-        The general form of an optimisation problem is given by:
-        
-        .. _shgo: https://stefan-endres.github.io/shgo/
-        
-        ::
-        
-            minimize f(x) subject to
-        
-            g_i(x) >= 0,  i = 1,...,m
-            h_j(x)  = 0,  j = 1,...,p
-        
-        where x is a vector of one or more variables. ``f(x)`` is the objective
-        function ``R^n -> R``, ``g_i(x)`` are the inequality constraints.
-        ``h_j(x)`` are the equality constrains.
-        
-        
-        Installation
-        ------------
-        Stable:
-        
-        .. code::
-        
-            $ pip install shgo
-            
-        Latest:
-        
-        .. code::
-        
-            $ git clone https://github.com/Stefan-Endres/shgo
-            $ cd shgo
-            $ python setup.py install
-            $ python setup.py test
-        
-        Documentation
-        -------------
-        The project website https://stefan-endres.github.io/shgo/ contains more detailed examples, notes and performance profiles.
-        
-        Quick example
-        -------------
-        
-        Consider the problem of minimizing the Rosenbrock function. This function is implemented in ``rosen`` in ``scipy.optimize``
-        
-        .. code:: python
-        
-            >>> from scipy.optimize import rosen
-            >>> from shgo import shgo
-            >>> bounds = [(0,2), (0, 2), (0, 2), (0, 2), (0, 2)]
-            >>> result = shgo(rosen, bounds)
-            >>> result.x, result.fun
-            (array([ 1.,  1.,  1.,  1.,  1.]), 2.9203923741900809e-18)
-        
-        Note that bounds determine the dimensionality of the objective function and is therefore a required input, however you can specify empty bounds using ``None`` or objects like numpy.inf which will be converted to large float numbers.
-        
-        
 Keywords: optimization
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/Stefan-Endres/shgo.svg?branch=master
+    :target: https://travis-ci.org/Stefan-Endres/shgo
+.. image:: https://coveralls.io/repos/github/Stefan-Endres/shgo/badge.png?branch=master
+    :target: https://coveralls.io/github/Stefan-Endres/shgo?branch=master
+
+Repository: https://github.com/Stefan-Endres/shgo
+
+Description
+-----------
+
+Finds the global minimum of a function using simplicial homology global
+optimisation (shgo_). Appropriate for solving general purpose NLP and blackbox
+optimisation problems to global optimality (low dimensional problems).
+The general form of an optimisation problem is given by:
+
+.. _shgo: https://stefan-endres.github.io/shgo/
+
+::
+
+    minimize f(x) subject to
+
+    g_i(x) >= 0,  i = 1,...,m
+    h_j(x)  = 0,  j = 1,...,p
+
+where x is a vector of one or more variables. ``f(x)`` is the objective
+function ``R^n -> R``, ``g_i(x)`` are the inequality constraints.
+``h_j(x)`` are the equality constrains.
+
+
+Installation
+------------
+Stable:
+
+.. code::
+
+    $ pip install shgo
+    
+Latest:
+
+.. code::
+
+    $ git clone https://github.com/Stefan-Endres/shgo
+    $ cd shgo
+    $ python setup.py install
+    $ python setup.py test
+
+Documentation
+-------------
+The project website https://stefan-endres.github.io/shgo/ contains more detailed examples, notes and performance profiles.
+
+Quick example
+-------------
+
+Consider the problem of minimizing the Rosenbrock function. This function is implemented in ``rosen`` in ``scipy.optimize``
+
+.. code:: python
+
+    >>> from scipy.optimize import rosen
+    >>> from shgo import shgo
+    >>> bounds = [(0,2), (0, 2), (0, 2), (0, 2), (0, 2)]
+    >>> result = shgo(rosen, bounds)
+    >>> result.x, result.fun
+    (array([ 1.,  1.,  1.,  1.,  1.]), 2.9203923741900809e-18)
+
+Note that bounds determine the dimensionality of the objective function and is therefore a required input, however you can specify empty bounds using ``None`` or objects like numpy.inf which will be converted to large float numbers.
+
```

