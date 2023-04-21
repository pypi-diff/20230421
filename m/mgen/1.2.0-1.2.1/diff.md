# Comparing `tmp/mgen-1.2.0.tar.gz` & `tmp/mgen-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mgen-1.2.0.tar", last modified: Tue Apr 17 17:19:26 2018, max compression
+gzip compressed data, was "mgen-1.2.1.tar", last modified: Fri Apr 21 20:26:04 2023, max compression
```

## Comparing `mgen-1.2.0.tar` & `mgen-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-17 17:19:26.000000 mgen-1.2.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-17 17:19:26.000000 mgen-1.2.0/docs/
--rw-r--r--   0 travis    (2000) travis    (2000)      601 2018-04-17 17:16:09.000000 mgen-1.2.0/docs/Makefile
--rw-r--r--   0 travis    (2000) travis    (2000)     5481 2018-04-17 17:16:09.000000 mgen-1.2.0/docs/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3109 2018-04-17 17:16:09.000000 mgen-1.2.0/docs/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      772 2018-04-17 17:16:09.000000 mgen-1.2.0/docs/make.bat
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen/
--rw-r--r--   0 travis    (2000) travis    (2000)      566 2018-04-17 17:16:09.000000 mgen-1.2.0/mgen/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      526 2018-04-17 17:16:09.000000 mgen-1.2.0/mgen/rotation_matrix_2d.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7713 2018-04-17 17:16:09.000000 mgen-1.2.0/mgen/rotation_matrix_3d.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3973 2018-04-17 17:16:09.000000 mgen-1.2.0/mgen/rotation_matrix_nd.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4264 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      485 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-17 17:16:20.000000 mgen-1.2.0/mgen.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       46 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/pbr.json
--rw-r--r--   0 travis    (2000) travis    (2000)       10 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        5 2018-04-17 17:19:26.000000 mgen-1.2.0/mgen.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-17 17:19:26.000000 mgen-1.2.0/tests/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-04-17 17:16:09.000000 mgen-1.2.0/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8364 2018-04-17 17:16:09.000000 mgen-1.2.0/tests/test_rotations.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1646 2018-04-17 17:16:09.000000 mgen-1.2.0/.travis.yml
--rw-r--r--   0 travis    (2000) travis    (2000)      111 2018-04-17 17:19:26.000000 mgen-1.2.0/AUTHORS
--rw-r--r--   0 travis    (2000) travis    (2000)      699 2018-04-17 17:19:26.000000 mgen-1.2.0/ChangeLog
--rw-r--r--   0 travis    (2000) travis    (2000)     1504 2018-04-17 17:16:09.000000 mgen-1.2.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)     3301 2018-04-17 17:16:09.000000 mgen-1.2.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       71 2018-04-17 17:16:09.000000 mgen-1.2.0/readthedocs.yml
--rw-r--r--   0 travis    (2000) travis    (2000)        9 2018-04-17 17:16:09.000000 mgen-1.2.0/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      324 2018-04-17 17:19:26.000000 mgen-1.2.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      100 2018-04-17 17:16:09.000000 mgen-1.2.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4264 2018-04-17 17:19:26.000000 mgen-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.084766 mgen-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 20:25:49.000000 mgen-1.2.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-21 20:25:49.000000 mgen-1.2.1/.github/workflows/deploy_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-21 20:25:49.000000 mgen-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 20:26:04.000000 mgen-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 20:26:04.000000 mgen-1.2.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-21 20:25:49.000000 mgen-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-21 20:26:04.088766 mgen-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-21 20:25:49.000000 mgen-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 20:25:49.000000 mgen-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-21 20:25:49.000000 mgen-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 20:25:49.000000 mgen-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-21 20:25:49.000000 mgen-1.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/mgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 20:25:49.000000 mgen-1.2.1/mgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-21 20:25:49.000000 mgen-1.2.1/mgen/rotation_matrix_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-21 20:25:49.000000 mgen-1.2.1/mgen/rotation_matrix_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-21 20:25:49.000000 mgen-1.2.1/mgen/rotation_matrix_nd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/mgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 20:26:04.000000 mgen-1.2.1/mgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 20:25:49.000000 mgen-1.2.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 20:25:49.000000 mgen-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-21 20:26:04.088766 mgen-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 20:25:49.000000 mgen-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:26:04.088766 mgen-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:25:49.000000 mgen-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-21 20:25:49.000000 mgen-1.2.1/tests/test_rotations.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mgen-1.2.0/docs/Makefile` & `mgen-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/docs/conf.py` & `mgen-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/docs/index.rst` & `mgen-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/docs/make.bat` & `mgen-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/mgen/__init__.py` & `mgen-1.2.1/mgen/__init__.py`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/mgen/rotation_matrix_2d.py` & `mgen-1.2.1/mgen/rotation_matrix_2d.py`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/mgen/rotation_matrix_3d.py` & `mgen-1.2.1/mgen/rotation_matrix_3d.py`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/mgen/rotation_matrix_nd.py` & `mgen-1.2.1/mgen/rotation_matrix_nd.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     :param abs_tolerance: The absolute tolerance to use when checking if vectors have length 0 or are parallel.
     :type abs_tolerance: float
 
     :returns: the rotation matrix
     :rtype: an nxn :any:`numpy.ndarray`
     '''
 
-    vector1 = np.asarray(vector1, dtype=np.float)
-    vector2 = np.asarray(vector2, dtype=np.float)
+    vector1 = np.asarray(vector1, dtype=float)
+    vector2 = np.asarray(vector2, dtype=float)
 
     vector1_length = np.linalg.norm(vector1)
     if math.isclose(vector1_length, 0., abs_tol=abs_tolerance):
         raise ValueError(
             'Given vector1 must have norm greater than zero within given numerical tolerance: {:.0e}'.format(abs_tolerance))
 
     vector2_length = np.linalg.norm(vector2)
```

### Comparing `mgen-1.2.0/mgen.egg-info/PKG-INFO` & `mgen-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,105 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mgen
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package to generate rotation matrices
 Home-page: https://github.com/NOhs/mgen
 Author: NOhs
-Author-email: UNKNOWN
 License: BSD
-Description: |test| |coverage| |documentation| |pypi| |license| |codacy|
-        
-        .. |test| image:: https://travis-ci.org/NOhs/mgen.svg?branch=master
-            :target: https://travis-ci.org/NOhs/mgen
-        .. |coverage| image:: https://coveralls.io/repos/github/NOhs/mgen/badge.svg
-            :target: https://coveralls.io/github/NOhs/mgen
-        .. |documentation| image:: https://readthedocs.org/projects/mgen/badge/?version=latest
-            :target: http://mgen.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        .. |pypi| image:: https://badge.fury.io/py/mgen.svg
-            :target: https://badge.fury.io/py/mgen
-        
-        .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-            :target: https://opensource.org/licenses/BSD-3-Clause
-            
-        .. |codacy| image:: https://api.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936    
-            :target: https://www.codacy.com/app/NOhs/mgen?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/mgen&amp;utm_campaign=Badge_Grade
-        
-        MGen: Convenient matrix generation functions
-        ============================================
-        
-        Python and its most popular packages do not offer out-of-the-box convenient
-        functions to generate rotation matrices. While there are other projects
-        that offer rotation and vector classes, or offer rotations via the use of quaternions,
-        if you simply want a rotation matrix, for example if other packages require them
-        as an input, or you do not wish to change your current data structure to use
-        special rotation classes, the common suggestion is to implement them yourself
-        (see for example this discussion on SE:
-        https://stackoverflow.com/questions/6802577/rotation-of-3d-vector). However,
-        everybody implementing their own version of the same thing can hardly be seen as
-        ideal.
-        
-        Therefore, this package provides simple functions to generate rotation matrices
-        in 2d for a given angle or in 3d for a given axis and angle, or for three given
-        angles (proper Euler angles or Tait-Bryan angles).
-        
-        Additionally, n-dimensional rotations can be generated using an angle and two
-        orthogonal vectors that span the plane of rotation.
-        
-        Trivial example usage
-        ----------------------
-        
-        Below you see examples of how to use mgen to generate rotation matrices. For further
-        documentation please have a look here: https://mgen.readthedocs.io
-        
-        .. code:: python
-        
-            import numpy as np
-            np.set_printoptions(suppress=True)
-        
-            from mgen import rotation_around_axis
-            from mgen import rotation_from_angles
-            from mgen import rotation_around_x
-            from mgen import rotation_from_angle_and_plane
-            from mgen import rotation_from_angle
-            from mgen import random_matrix
-        
-            # 2D example
-            matrix = rotation_from_angle(np.pi/2)
-            matrix.dot([1, 0])
-            # array([0., 1.])
-        
-            #3D examples
-            matrix = rotation_from_angles([np.pi/2, 0, 0], 'XYX')
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            matrix = rotation_around_axis([1, 0, 0], np.pi/2)
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            matrix = rotation_around_x(np.pi/2)
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            # n-dimensional example
-            matrix = rotation_from_angle_and_plane(np.pi/2, (0, 1, 0, 0), (0, 0, 1, 0))
-            matrix.dot([0, 1, 0, 0])
-            # array([0., 0., 1., 0.])
-        
-            # n-dimensional random matrix O(n), e.g. n=27
-            matrix = random_matrix(27)
-        
-        
-Keywords: matrix,rotations,Euler angles
-Platform: UNKNOWN
+Keywords: matrix, rotations, Euler angles
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+|test| |coverage| |documentation| |pypi| |python_vers| |license| |codacy|
+
+.. |test| image:: https://github.com/NOhs/mgen/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/NOhs/mgen/actions/workflows/test.yml
+
+.. |coverage| image:: https://codecov.io/github/NOhs/mgen/branch/master/graph/badge.svg?token=FC0NS4nchO
+    :target: https://codecov.io/github/NOhs/mgen
+
+.. |documentation| image:: https://readthedocs.org/projects/mgen/badge/?version=latest
+    :target: http://mgen.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |pypi| image:: https://badge.fury.io/py/mgen.svg
+    :target: https://badge.fury.io/py/mgen
+
+.. |python_vers| image:: https://img.shields.io/pypi/pyversions/mgen
+    :alt: PyPI - Python Version
+
+.. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+    :target: https://opensource.org/licenses/BSD-3-Clause
+
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936
+    :target: https://app.codacy.com/gh/NOhs/mgen/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+
+MGen: Convenient matrix generation functions
+============================================
+
+Python and its most popular packages do not offer out-of-the-box convenient
+functions to generate rotation matrices. While there are other projects
+that offer rotation and vector classes, or offer rotations via the use of quaternions,
+if you simply want a rotation matrix, for example if other packages require them
+as an input, or you do not wish to change your current data structure to use
+special rotation classes, the common suggestion is to implement them yourself
+(see for example this discussion on SE:
+https://stackoverflow.com/questions/6802577/rotation-of-3d-vector). However,
+everybody implementing their own version of the same thing can hardly be seen as
+ideal.
+
+Therefore, this package provides simple functions to generate rotation matrices
+in 2d for a given angle or in 3d for a given axis and angle, or for three given
+angles (proper Euler angles or Tait-Bryan angles).
+
+Additionally, n-dimensional rotations can be generated using an angle and two
+orthogonal vectors that span the plane of rotation.
+
+Trivial example usage
+----------------------
+
+Below you see examples of how to use mgen to generate rotation matrices. For further
+documentation please have a look here: https://mgen.readthedocs.io
+
+.. code:: python
+
+    import numpy as np
+    np.set_printoptions(suppress=True)
+
+    from mgen import rotation_around_axis
+    from mgen import rotation_from_angles
+    from mgen import rotation_around_x
+    from mgen import rotation_from_angle_and_plane
+    from mgen import rotation_from_angle
+    from mgen import random_matrix
+
+    # 2D example
+    matrix = rotation_from_angle(np.pi/2)
+    matrix.dot([1, 0])
+    # array([0., 1.])
+
+    #3D examples
+    matrix = rotation_from_angles([np.pi/2, 0, 0], 'XYX')
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    matrix = rotation_around_axis([1, 0, 0], np.pi/2)
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    matrix = rotation_around_x(np.pi/2)
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    # n-dimensional example
+    matrix = rotation_from_angle_and_plane(np.pi/2, (0, 1, 0, 0), (0, 0, 1, 0))
+    matrix.dot([0, 1, 0, 0])
+    # array([0., 0., 1., 0.])
+
+    # n-dimensional random matrix O(n), e.g. n=27
+    matrix = random_matrix(27)
+
```

### Comparing `mgen-1.2.0/tests/test_rotations.py` & `mgen-1.2.1/tests/test_rotations.py`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/ChangeLog` & `mgen-1.2.1/ChangeLog`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.2.1
+-----
+
+* Fix deployment GitHub Actions scripts (#14)
+* Update CI/CD and fix deprecated numpy usage (#13)
+
 1.2.0
 -----
 
 * nd rotations now accept non-orthogonal vectors (#10)
 * Added codacy badge to readme
 
 1.1.1
```

### Comparing `mgen-1.2.0/LICENSE` & `mgen-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mgen-1.2.0/README.rst` & `mgen-1.2.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-|test| |coverage| |documentation| |pypi| |license| |codacy|
+|test| |coverage| |documentation| |pypi| |python_vers| |license| |codacy|
+
+.. |test| image:: https://github.com/NOhs/mgen/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/NOhs/mgen/actions/workflows/test.yml
+
+.. |coverage| image:: https://codecov.io/github/NOhs/mgen/branch/master/graph/badge.svg?token=FC0NS4nchO
+    :target: https://codecov.io/github/NOhs/mgen
 
-.. |test| image:: https://travis-ci.org/NOhs/mgen.svg?branch=master
-    :target: https://travis-ci.org/NOhs/mgen
-.. |coverage| image:: https://coveralls.io/repos/github/NOhs/mgen/badge.svg
-    :target: https://coveralls.io/github/NOhs/mgen
 .. |documentation| image:: https://readthedocs.org/projects/mgen/badge/?version=latest
     :target: http://mgen.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
+
 .. |pypi| image:: https://badge.fury.io/py/mgen.svg
     :target: https://badge.fury.io/py/mgen
 
+.. |python_vers| image:: https://img.shields.io/pypi/pyversions/mgen
+    :alt: PyPI - Python Version
+
 .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
     :target: https://opensource.org/licenses/BSD-3-Clause
-    
-.. |codacy| image:: https://api.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936    
-    :target: https://www.codacy.com/app/NOhs/mgen?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/mgen&amp;utm_campaign=Badge_Grade
+
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936
+    :target: https://app.codacy.com/gh/NOhs/mgen/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
 
 MGen: Convenient matrix generation functions
 ============================================
 
 Python and its most popular packages do not offer out-of-the-box convenient
 functions to generate rotation matrices. While there are other projects
 that offer rotation and vector classes, or offer rotations via the use of quaternions,
```

### Comparing `mgen-1.2.0/PKG-INFO` & `mgen-1.2.1/mgen.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,105 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mgen
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package to generate rotation matrices
 Home-page: https://github.com/NOhs/mgen
 Author: NOhs
-Author-email: UNKNOWN
 License: BSD
-Description: |test| |coverage| |documentation| |pypi| |license| |codacy|
-        
-        .. |test| image:: https://travis-ci.org/NOhs/mgen.svg?branch=master
-            :target: https://travis-ci.org/NOhs/mgen
-        .. |coverage| image:: https://coveralls.io/repos/github/NOhs/mgen/badge.svg
-            :target: https://coveralls.io/github/NOhs/mgen
-        .. |documentation| image:: https://readthedocs.org/projects/mgen/badge/?version=latest
-            :target: http://mgen.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        .. |pypi| image:: https://badge.fury.io/py/mgen.svg
-            :target: https://badge.fury.io/py/mgen
-        
-        .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-            :target: https://opensource.org/licenses/BSD-3-Clause
-            
-        .. |codacy| image:: https://api.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936    
-            :target: https://www.codacy.com/app/NOhs/mgen?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/mgen&amp;utm_campaign=Badge_Grade
-        
-        MGen: Convenient matrix generation functions
-        ============================================
-        
-        Python and its most popular packages do not offer out-of-the-box convenient
-        functions to generate rotation matrices. While there are other projects
-        that offer rotation and vector classes, or offer rotations via the use of quaternions,
-        if you simply want a rotation matrix, for example if other packages require them
-        as an input, or you do not wish to change your current data structure to use
-        special rotation classes, the common suggestion is to implement them yourself
-        (see for example this discussion on SE:
-        https://stackoverflow.com/questions/6802577/rotation-of-3d-vector). However,
-        everybody implementing their own version of the same thing can hardly be seen as
-        ideal.
-        
-        Therefore, this package provides simple functions to generate rotation matrices
-        in 2d for a given angle or in 3d for a given axis and angle, or for three given
-        angles (proper Euler angles or Tait-Bryan angles).
-        
-        Additionally, n-dimensional rotations can be generated using an angle and two
-        orthogonal vectors that span the plane of rotation.
-        
-        Trivial example usage
-        ----------------------
-        
-        Below you see examples of how to use mgen to generate rotation matrices. For further
-        documentation please have a look here: https://mgen.readthedocs.io
-        
-        .. code:: python
-        
-            import numpy as np
-            np.set_printoptions(suppress=True)
-        
-            from mgen import rotation_around_axis
-            from mgen import rotation_from_angles
-            from mgen import rotation_around_x
-            from mgen import rotation_from_angle_and_plane
-            from mgen import rotation_from_angle
-            from mgen import random_matrix
-        
-            # 2D example
-            matrix = rotation_from_angle(np.pi/2)
-            matrix.dot([1, 0])
-            # array([0., 1.])
-        
-            #3D examples
-            matrix = rotation_from_angles([np.pi/2, 0, 0], 'XYX')
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            matrix = rotation_around_axis([1, 0, 0], np.pi/2)
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            matrix = rotation_around_x(np.pi/2)
-            matrix.dot([0, 1, 0])
-            # array([0., 0., 1.])
-        
-            # n-dimensional example
-            matrix = rotation_from_angle_and_plane(np.pi/2, (0, 1, 0, 0), (0, 0, 1, 0))
-            matrix.dot([0, 1, 0, 0])
-            # array([0., 0., 1., 0.])
-        
-            # n-dimensional random matrix O(n), e.g. n=27
-            matrix = random_matrix(27)
-        
-        
-Keywords: matrix,rotations,Euler angles
-Platform: UNKNOWN
+Keywords: matrix, rotations, Euler angles
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+|test| |coverage| |documentation| |pypi| |python_vers| |license| |codacy|
+
+.. |test| image:: https://github.com/NOhs/mgen/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/NOhs/mgen/actions/workflows/test.yml
+
+.. |coverage| image:: https://codecov.io/github/NOhs/mgen/branch/master/graph/badge.svg?token=FC0NS4nchO
+    :target: https://codecov.io/github/NOhs/mgen
+
+.. |documentation| image:: https://readthedocs.org/projects/mgen/badge/?version=latest
+    :target: http://mgen.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |pypi| image:: https://badge.fury.io/py/mgen.svg
+    :target: https://badge.fury.io/py/mgen
+
+.. |python_vers| image:: https://img.shields.io/pypi/pyversions/mgen
+    :alt: PyPI - Python Version
+
+.. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+    :target: https://opensource.org/licenses/BSD-3-Clause
+
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/ab622cde22a24af4b9bcb62a49002936
+    :target: https://app.codacy.com/gh/NOhs/mgen/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+
+MGen: Convenient matrix generation functions
+============================================
+
+Python and its most popular packages do not offer out-of-the-box convenient
+functions to generate rotation matrices. While there are other projects
+that offer rotation and vector classes, or offer rotations via the use of quaternions,
+if you simply want a rotation matrix, for example if other packages require them
+as an input, or you do not wish to change your current data structure to use
+special rotation classes, the common suggestion is to implement them yourself
+(see for example this discussion on SE:
+https://stackoverflow.com/questions/6802577/rotation-of-3d-vector). However,
+everybody implementing their own version of the same thing can hardly be seen as
+ideal.
+
+Therefore, this package provides simple functions to generate rotation matrices
+in 2d for a given angle or in 3d for a given axis and angle, or for three given
+angles (proper Euler angles or Tait-Bryan angles).
+
+Additionally, n-dimensional rotations can be generated using an angle and two
+orthogonal vectors that span the plane of rotation.
+
+Trivial example usage
+----------------------
+
+Below you see examples of how to use mgen to generate rotation matrices. For further
+documentation please have a look here: https://mgen.readthedocs.io
+
+.. code:: python
+
+    import numpy as np
+    np.set_printoptions(suppress=True)
+
+    from mgen import rotation_around_axis
+    from mgen import rotation_from_angles
+    from mgen import rotation_around_x
+    from mgen import rotation_from_angle_and_plane
+    from mgen import rotation_from_angle
+    from mgen import random_matrix
+
+    # 2D example
+    matrix = rotation_from_angle(np.pi/2)
+    matrix.dot([1, 0])
+    # array([0., 1.])
+
+    #3D examples
+    matrix = rotation_from_angles([np.pi/2, 0, 0], 'XYX')
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    matrix = rotation_around_axis([1, 0, 0], np.pi/2)
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    matrix = rotation_around_x(np.pi/2)
+    matrix.dot([0, 1, 0])
+    # array([0., 0., 1.])
+
+    # n-dimensional example
+    matrix = rotation_from_angle_and_plane(np.pi/2, (0, 1, 0, 0), (0, 0, 1, 0))
+    matrix.dot([0, 1, 0, 0])
+    # array([0., 0., 1., 0.])
+
+    # n-dimensional random matrix O(n), e.g. n=27
+    matrix = random_matrix(27)
+
```

