# Comparing `tmp/ndindex-1.6.tar.gz` & `tmp/ndindex-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndindex-1.6.tar", last modified: Mon Jan 24 22:20:22 2022, max compression
+gzip compressed data, was "ndindex-1.7.tar", last modified: Fri Apr 21 01:09:29 2023, max compression
```

## Comparing `ndindex-1.6.tar` & `ndindex-1.7.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-01-24 22:20:22.558313 ndindex-1.6/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1071 2021-07-08 20:18:13.000000 ndindex-1.6/LICENSE
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       66 2021-07-08 20:18:13.000000 ndindex-1.6/MANIFEST.in
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3406 2022-01-24 22:20:22.558445 ndindex-1.6/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2929 2021-08-20 07:52:51.000000 ndindex-1.6/README.md
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-01-24 22:20:22.599307 ndindex-1.6/ndindex/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      706 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     7773 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/_crt.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      495 2022-01-24 22:20:22.599445 ndindex-1.6/ndindex/_version.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     5468 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/array.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     7499 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/booleanarray.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    15019 2022-01-24 20:27:26.000000 ndindex-1.6/ndindex/chunking.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2832 2022-01-18 00:15:38.000000 ndindex-1.6/ndindex/ellipsis.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     4861 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/integer.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     6663 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/integerarray.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    32208 2022-01-24 20:27:26.000000 ndindex-1.6/ndindex/ndindex.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2579 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/newaxis.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    21774 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/slice.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2842 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/subindex_helpers.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-01-24 22:20:22.557679 ndindex-1.6/ndindex/tests/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3082 2021-07-08 20:18:13.000000 ndindex-1.6/ndindex/tests/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2910 2022-01-17 23:22:39.000000 ndindex-1.6/ndindex/tests/doctest.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    11349 2022-01-17 23:22:39.000000 ndindex-1.6/ndindex/tests/helpers.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1053 2021-07-08 20:18:13.000000 ndindex-1.6/ndindex/tests/test_array.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     4085 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/tests/test_as_subindex.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3786 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/tests/test_booleanarray.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3227 2021-07-08 20:18:13.000000 ndindex-1.6/ndindex/tests/test_broadcast_arrays.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     9067 2022-01-18 01:08:25.000000 ndindex-1.6/ndindex/tests/test_chunking.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1196 2022-01-24 21:58:01.000000 ndindex-1.6/ndindex/tests/test_crt.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2223 2021-07-08 20:18:13.000000 ndindex-1.6/ndindex/tests/test_ellipsis.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2957 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/tests/test_expand.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     6481 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/tests/test_integer.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3888 2021-08-20 07:52:51.000000 ndindex-1.6/ndindex/tests/test_integerarray.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    10786 2022-01-24 20:52:58.000000 ndindex-1.6/ndindex/tests/test_ndindex.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2235 2021-07-08 20:18:13.000000 ndindex-1.6/ndindex/tests/test_newaxis.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1676 2022-01-17 23:22:39.000000 ndindex-1.6/ndindex/tests/test_newshape.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     6076 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/tests/test_no_dependencies.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    15689 2021-11-01 22:06:07.000000 ndindex-1.6/ndindex/tests/test_slice.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     7841 2021-08-20 07:52:58.000000 ndindex-1.6/ndindex/tests/test_tuple.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    30943 2022-01-19 00:18:23.000000 ndindex-1.6/ndindex/tuple.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-01-24 22:20:22.544088 ndindex-1.6/ndindex.egg-info/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3406 2022-01-24 22:20:22.000000 ndindex-1.6/ndindex.egg-info/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1075 2022-01-24 22:20:22.000000 ndindex-1.6/ndindex.egg-info/SOURCES.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2022-01-24 22:20:22.000000 ndindex-1.6/ndindex.egg-info/dependency_links.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       16 2022-01-24 22:20:22.000000 ndindex-1.6/ndindex.egg-info/requires.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)        8 2022-01-24 22:20:22.000000 ndindex-1.6/ndindex.egg-info/top_level.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      192 2022-01-24 22:20:22.558951 ndindex-1.6/setup.cfg
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2055 2022-01-24 20:27:27.000000 ndindex-1.6/setup.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    68612 2021-07-08 20:18:13.000000 ndindex-1.6/versioneer.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-21 01:09:29.072527 ndindex-1.7/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1071 2023-01-31 17:19:42.000000 ndindex-1.7/LICENSE
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      129 2023-04-20 21:49:02.000000 ndindex-1.7/MANIFEST.in
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3386 2023-04-21 01:09:29.072968 ndindex-1.7/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2929 2023-01-31 17:19:42.000000 ndindex-1.7/README.md
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2111 2023-04-20 21:49:02.000000 ndindex-1.7/conftest.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-21 01:09:29.075242 ndindex-1.7/ndindex/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      781 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     7773 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/_crt.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      495 2023-04-21 01:09:29.076628 ndindex-1.7/ndindex/_version.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     6126 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/array.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     7543 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/booleanarray.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    15042 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/chunking.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2937 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/ellipsis.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     5205 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/integer.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     6739 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/integerarray.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    22650 2023-04-20 21:59:31.000000 ndindex-1.7/ndindex/ndindex.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2684 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/newaxis.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    18538 2023-04-20 21:50:17.000000 ndindex-1.7/ndindex/shapetools.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    22034 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/slice.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2842 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/subindex_helpers.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-21 01:09:29.071874 ndindex-1.7/ndindex/tests/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3082 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2910 2023-04-20 00:30:54.000000 ndindex-1.7/ndindex/tests/doctest.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    14549 2023-04-20 22:42:19.000000 ndindex-1.7/ndindex/tests/helpers.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1053 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_array.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     4127 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tests/test_as_subindex.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3786 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_booleanarray.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3269 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tests/test_broadcast_arrays.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     9067 2023-04-20 21:20:01.000000 ndindex-1.7/ndindex/tests/test_chunking.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1196 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_crt.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2223 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_ellipsis.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2957 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_expand.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     6481 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_integer.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3888 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_integerarray.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1382 2023-04-20 22:37:12.000000 ndindex-1.7/ndindex/tests/test_isvalid.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     4062 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tests/test_ndindex.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2235 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_newaxis.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1676 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_newshape.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     6076 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_no_dependencies.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    21922 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tests/test_shapetools.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    15692 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tests/test_slice.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     7841 2023-03-31 08:32:03.000000 ndindex-1.7/ndindex/tests/test_tuple.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    30801 2023-04-20 21:49:02.000000 ndindex-1.7/ndindex/tuple.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-21 01:09:29.056161 ndindex-1.7/ndindex.egg-info/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3386 2023-04-21 01:09:28.000000 ndindex-1.7/ndindex.egg-info/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1183 2023-04-21 01:09:28.000000 ndindex-1.7/ndindex.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2023-04-21 01:09:28.000000 ndindex-1.7/ndindex.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       16 2023-04-21 01:09:28.000000 ndindex-1.7/ndindex.egg-info/requires.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)        8 2023-04-21 01:09:28.000000 ndindex-1.7/ndindex.egg-info/top_level.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      105 2023-04-20 22:37:29.000000 ndindex-1.7/pytest.ini
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      192 2023-04-21 01:09:29.074495 ndindex-1.7/setup.cfg
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2055 2023-01-31 17:19:42.000000 ndindex-1.7/setup.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    68612 2023-01-31 17:19:42.000000 ndindex-1.7/versioneer.py
```

### Comparing `ndindex-1.6/LICENSE` & `ndindex-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/PKG-INFO` & `ndindex-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: ndindex
-Version: 1.6
+Version: 1.7
 Summary: A Python library for manipulating indices of ndarrays.
 Home-page: https://quansight-labs.github.io/ndindex/
 Author: Quansight Labs
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: arrays
 License-File: LICENSE
@@ -103,9 +102,7 @@
 
 <p align="center">
 <a href="https://labs.quansight.org/"><img src="https://labs.quansight.org/images/QuansightLabs_logo_V2.png" alt="https://labs.quansight.org/"
 width="200"></a>
 <a href="https://www.deshaw.com"><img src="https://www.deshaw.com/assets/logos/blue_logo_417x125.png" alt="https://www.deshaw.com"
 width="200"></a>
 </p>
-
-
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: ndindex Version: 1.6 Summary: A Python library for
+Metadata-Version: 2.1 Name: ndindex Version: 1.7 Summary: A Python library for
 manipulating indices of ndarrays. Home-page: https://quansight-labs.github.io/
-ndindex/ Author: Quansight Labs License: MIT Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: arrays License-File:
-LICENSE # ndindex ![ndindex logo](docs/_static/ndindex_logo_white_bg.svg) A
-Python library for manipulating indices of ndarrays. The documentation for
-ndindex can be found at https://quansight-labs.github.io/ndindex/ ndindex is a
-library that allows representing and manipulating objects that can be valid
-indices to numpy arrays, i.e., slices, integers, ellipses, None, integer and
-boolean arrays, and tuples thereof. The goals of the library are - Provide a
-uniform API to manipulate these objects. Unlike the standard index objects
-themselves like `slice`, `int`, and `tuple`, which do not share any methods in
-common related to being indices, ndindex classes can all be manipulated
-uniformly. For example, `idx.args` always gives the arguments used to construct
-`idx`. - Give 100% correct semantics as defined by numpy's ndarray. This means
-that ndindex will not make a transformation on an index object unless it is
-correct for all possible input array shapes. The only exception to this rule is
-that ndindex assumes that any given index will not raise IndexError (for
-instance, from an out of bounds integer index or from too few dimensions). For
-those operations where the array shape is known, there is a `reduce()` method
-to reduce an index to a simpler index that is equivalent for the given shape. -
-Enable useful transformation and manipulation functions on index objects. ##
-Examples **Canonicalize a slice (over a given shape, or independent of array
-shape)** ```py >>> from ndindex import * >>> Slice(-2, 10, 3).reduce() Slice(-
-2, 10, 2) >>> Slice(-2, 10, 3).reduce(5) Slice(3, 4, 1) ``` **Compute the
-maximum length of a sliced axis** ```py >>> import numpy as np >>> len(Slice(2,
-10, 3)) 3 >>> len(np.arange(10)[2:10:3]) 3 ``` **Compute the shape of an array
-of shape `(10, 20)` indexed by `[0, 0:10]`** ```py >>> Tuple(0, slice(0,
-10)).newshape((10, 20)) (10,) >>> np.ones((10, 20))[0, 0:10].shape (10,) ```
-**Check if an indexed array would be empty** ```py >>> Tuple(0, ..., Slice(10,
-20)).isempty((3, 4, 5)) True >>> np.ones((3, 4, 5))[0,...,10:20] array([],
-shape=(4, 0), dtype=float64) ``` See the [documentation](https://quansight-
-labs.github.io/ndindex/) for full details on what ndindex can do. ## License
-[MIT License](LICENSE) ## Acknowledgments ndindex development is supported by
-[Quansight Labs](https://labs.quansight.org/) and is sponsored in part by [the
-D. E. Shaw group](https://www.deshaw.com/). The D. E. Shaw group collaborates
-with Quansight on numerous open source projects, including Numba, Dask and
-Project Jupyter.
+ndindex/ Author: Quansight Labs License: MIT Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Type: text/markdown Provides-Extra: arrays License-File: LICENSE # ndindex !
+[ndindex logo](docs/_static/ndindex_logo_white_bg.svg) A Python library for
+manipulating indices of ndarrays. The documentation for ndindex can be found at
+https://quansight-labs.github.io/ndindex/ ndindex is a library that allows
+representing and manipulating objects that can be valid indices to numpy
+arrays, i.e., slices, integers, ellipses, None, integer and boolean arrays, and
+tuples thereof. The goals of the library are - Provide a uniform API to
+manipulate these objects. Unlike the standard index objects themselves like
+`slice`, `int`, and `tuple`, which do not share any methods in common related
+to being indices, ndindex classes can all be manipulated uniformly. For
+example, `idx.args` always gives the arguments used to construct `idx`. - Give
+100% correct semantics as defined by numpy's ndarray. This means that ndindex
+will not make a transformation on an index object unless it is correct for all
+possible input array shapes. The only exception to this rule is that ndindex
+assumes that any given index will not raise IndexError (for instance, from an
+out of bounds integer index or from too few dimensions). For those operations
+where the array shape is known, there is a `reduce()` method to reduce an index
+to a simpler index that is equivalent for the given shape. - Enable useful
+transformation and manipulation functions on index objects. ## Examples
+**Canonicalize a slice (over a given shape, or independent of array shape)**
+```py >>> from ndindex import * >>> Slice(-2, 10, 3).reduce() Slice(-2, 10, 2)
+>>> Slice(-2, 10, 3).reduce(5) Slice(3, 4, 1) ``` **Compute the maximum length
+of a sliced axis** ```py >>> import numpy as np >>> len(Slice(2, 10, 3)) 3 >>>
+len(np.arange(10)[2:10:3]) 3 ``` **Compute the shape of an array of shape `(10,
+20)` indexed by `[0, 0:10]`** ```py >>> Tuple(0, slice(0, 10)).newshape((10,
+20)) (10,) >>> np.ones((10, 20))[0, 0:10].shape (10,) ``` **Check if an indexed
+array would be empty** ```py >>> Tuple(0, ..., Slice(10, 20)).isempty((3, 4,
+5)) True >>> np.ones((3, 4, 5))[0,...,10:20] array([], shape=(4, 0),
+dtype=float64) ``` See the [documentation](https://quansight-labs.github.io/
+ndindex/) for full details on what ndindex can do. ## License [MIT License]
+(LICENSE) ## Acknowledgments ndindex development is supported by [Quansight
+Labs](https://labs.quansight.org/) and is sponsored in part by [the D. E. Shaw
+group](https://www.deshaw.com/). The D. E. Shaw group collaborates with
+Quansight on numerous open source projects, including Numba, Dask and Project
+Jupyter.
             [https://labs.quansight.org/] [https://www.deshaw.com]
```

### Comparing `ndindex-1.6/README.md` & `ndindex-1.7/README.md`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/__init__.py` & `ndindex-1.7/ndindex/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 __all__ = []
 
-from .ndindex import ndindex, iter_indices, AxisError, BroadcastError
+from .ndindex import ndindex
 
-__all__ += ['ndindex', 'iter_indices', 'AxisError', 'BroadcastError']
+__all__ += ['ndindex']
+
+from .shapetools import broadcast_shapes, iter_indices, AxisError, BroadcastError
+
+__all__ += ['broadcast_shapes', 'iter_indices', 'AxisError', 'BroadcastError']
 
 from .slice import Slice
 
 __all__ += ['Slice']
 
 from .integer import Integer
```

### Comparing `ndindex-1.6/ndindex/_crt.py` & `ndindex-1.7/ndindex/_crt.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/array.py` & `ndindex-1.7/ndindex/array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 
-from .ndindex import NDIndex, asshape
+from .ndindex import NDIndex
+from .shapetools import asshape
 
 class ArrayIndex(NDIndex):
     """
     Superclass for array indices
 
     This class should not be instantiated directly. Rather, use one of its
     subclasses, :class:`~.IntegerArray` or :class:`~.BooleanArray`.
@@ -15,15 +16,15 @@
     __slots__ = ()
 
     # Subclasses should redefine this
     dtype = None
 
     def _typecheck(self, idx, shape=None, _copy=True):
         try:
-            from numpy import ndarray, asarray, integer, bool_, empty, intp
+            from numpy import ndarray, asarray, integer, bool_, empty, intp, VisibleDeprecationWarning
         except ImportError: # pragma: no cover
             raise ImportError("NumPy must be installed to create array indices")
 
         if self.dtype is None:
             raise TypeError("Do not instantiate the superclass ArrayIndex directly")
 
         if shape is not None:
@@ -33,15 +34,18 @@
             if 0 not in shape:
                 raise ValueError("The shape argument must be an empty shape")
             idx = empty(shape, dtype=self.dtype)
 
         if isinstance(idx, (list, ndarray, bool, integer, int, bool_)):
             # Ignore deprecation warnings for things like [1, []]. These will be
             # filtered out anyway since they produce object arrays.
-            with warnings.catch_warnings(record=True):
+            with warnings.catch_warnings():
+                warnings.filterwarnings('ignore',
+                                        category=VisibleDeprecationWarning,
+                                        message='Creating an ndarray from ragged nested sequences')
                 a = asarray(idx)
                 if a is idx and _copy:
                     a = a.copy()
                 if isinstance(idx, list) and 0 in a.shape:
                     if not _copy:
                         raise ValueError("_copy=False is not allowed with list input")
                     a = a.astype(self.dtype)
@@ -155,7 +159,18 @@
         return (self.__class__.__name__
                 + "("
                 + array2string(self.array).replace('\n', '')
                 + ")")
 
     def __hash__(self):
         return hash(self.array.tobytes())
+
+    def isvalid(self, shape, _axis=0):
+        shape = asshape(shape)
+        try:
+            # The logic is in _raise_indexerror because the error message uses
+            # the additional information that is computed when checking if the
+            # array is valid.
+            self._raise_indexerror(shape, _axis)
+        except IndexError:
+            return False
+        return True
```

### Comparing `ndindex-1.6/ndindex/booleanarray.py` & `ndindex-1.7/ndindex/booleanarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .array import ArrayIndex
-from .ndindex import asshape
+from .shapetools import asshape
 
 class BooleanArray(ArrayIndex):
     """
     Represents a boolean array index (also known as a mask).
 
     If `idx` is an n-dimensional boolean array with shape `s = (s1, ..., sn)`
     and `a` is an array of shape `s = (s1, ..., sn, ..., sm)`, `a[idx]`
@@ -98,14 +98,23 @@
         >>> from ndindex import BooleanArray
         >>> BooleanArray([True, False, True]).count_nonzero
         2
         """
         from numpy import count_nonzero
         return count_nonzero(self.array)
 
+    def _raise_indexerror(self, shape, axis=0):
+        if len(shape) < self.ndim + axis:
+            raise IndexError(f"too many indices for array: array is {len(shape)}-dimensional, but {self.ndim + axis} were indexed")
+
+        for i in range(axis, axis+self.ndim):
+            if self.shape[i-axis] != 0 and shape[i] != self.shape[i-axis]:
+
+                raise IndexError(f"boolean index did not match indexed array along dimension {i}; dimension is {shape[i]} but corresponding boolean dimension is {self.shape[i-axis]}")
+
     def reduce(self, shape=None, axis=0):
         """
         Reduce a `BooleanArray` index on an array of shape `shape`.
 
         The result will either be `IndexError` if the index is invalid for the
         given shape, or a `BooleanArray` index. Presently, no simplifications
         are done for BooleanArray: if `reduce()` does not produce an
@@ -133,30 +142,22 @@
 
         """
         if shape is None:
             return self
 
         shape = asshape(shape)
 
-        if len(shape) < self.ndim + axis:
-            raise IndexError(f"too many indices for array: array is {len(shape)}-dimensional, but {self.ndim + axis} were indexed")
-
-        for i in range(axis, axis+self.ndim):
-            if self.shape[i-axis] != 0 and shape[i] != self.shape[i-axis]:
-
-                raise IndexError(f"boolean index did not match indexed array along dimension {i}; dimension is {shape[i]} but corresponding boolean dimension is {self.shape[i-axis]}")
-
+        self._raise_indexerror(shape, axis)
         return self
 
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
-        # reduce will raise IndexError if it should be raised
-        self.reduce(shape)
+        self._raise_indexerror(shape)
         return (self.count_nonzero,) + shape[self.ndim:]
 
     def isempty(self, shape=None):
         if shape is not None:
             return 0 in self.newshape(shape)
 
         return self.count_nonzero == 0
```

### Comparing `ndindex-1.6/ndindex/chunking.py` & `ndindex-1.7/ndindex/chunking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections.abc import Sequence
 from itertools import product
 
-from .ndindex import ImmutableObject, operator_index, asshape, ndindex
+from .ndindex import ImmutableObject, operator_index, ndindex
 from .tuple import Tuple
 from .slice import Slice
 from .integer import Integer
 from .integerarray import IntegerArray
 from .newaxis import Newaxis
+from .shapetools import asshape
 from .subindex_helpers import ceiling
 from ._crt import prod
 
 class ChunkSize(ImmutableObject, Sequence):
     """
     Represents a chunk size tuple.
```

### Comparing `ndindex-1.6/ndindex/ellipsis.py` & `ndindex-1.7/ndindex/ellipsis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .ndindex import NDIndex, asshape
+from .ndindex import NDIndex
 from .tuple import Tuple
+from .shapetools import asshape
 
 class ellipsis(NDIndex):
     """
     Represents an ellipsis index, i.e., `...` (or `Ellipsis`).
 
     Ellipsis indices by themselves return the full array. Inside of a tuple
     index, an ellipsis skips 0 or more axes of the array so that everything
@@ -73,14 +74,18 @@
             shape = asshape(shape)
         return Tuple()
 
     @property
     def raw(self):
         return ...
 
+    def isvalid(self, shape):
+        shape = asshape(shape)
+        return True
+
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
         return shape
 
     def as_subindex(self, index):
```

### Comparing `ndindex-1.6/ndindex/integer.py` & `ndindex-1.7/ndindex/integer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .ndindex import NDIndex, asshape, operator_index
+from .ndindex import NDIndex, operator_index
+from .shapetools import asshape
 
 class Integer(NDIndex):
     """
     Represents an integer index on an axis of an nd-array.
 
     Any object that implements `__index__` can be used as an integer index.
 
@@ -44,14 +45,27 @@
         Returns the number of elements indexed by `self`
 
         Since `self` is an integer index, this always returns 1. Note that
         integer indices always remove an axis.
         """
         return 1
 
+    def isvalid(self, shape, _axis=0):
+        # The docstring for this method is on the NDIndex base class
+        shape = asshape(shape)
+        if not shape:
+            return False
+        size = shape[_axis]
+        return -size <= self.raw < size
+
+    def _raise_indexerror(self, shape, axis=0):
+        if not self.isvalid(shape, axis):
+            size = shape[axis]
+            raise IndexError(f"index {self.raw} is out of bounds for axis {axis} with size {size}")
+
     def reduce(self, shape=None, axis=0):
         """
         Reduce an Integer index on an array of shape `shape`.
 
         The result will either be `IndexError` if the index is invalid for the
         given shape, or an Integer index where the value is nonnegative.
 
@@ -76,29 +90,27 @@
         .BooleanArray.reduce
 
         """
         if shape is None:
             return self
 
         shape = asshape(shape, axis=axis)
-        size = shape[axis]
-        if self.raw >= size or -size > self.raw < 0:
-            raise IndexError(f"index {self.raw} is out of bounds for axis {axis} with size {size}")
+        self._raise_indexerror(shape, axis)
 
         if self.raw < 0:
+            size = shape[axis]
             return self.__class__(size + self.raw)
 
         return self
 
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
-        # reduce will raise IndexError if it should be raised
-        self.reduce(shape)
+        self._raise_indexerror(shape)
         return shape[1:]
 
     def as_subindex(self, index):
         index = ndindex(index)
 
         if isinstance(index, Tuple):
             return Tuple(self).as_subindex(index)
```

### Comparing `ndindex-1.6/ndindex/integerarray.py` & `ndindex-1.7/ndindex/integerarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .array import ArrayIndex
-from .ndindex import asshape
+from .shapetools import asshape
 from .subindex_helpers import subindex_slice
 
 class IntegerArray(ArrayIndex):
     """
     Represents an integer array index.
 
     If `idx` is an n-dimensional integer array with shape `s = (s1, ..., sn)`
@@ -47,14 +47,20 @@
         """
         The dtype of `IntegerArray` is `np.intp`, which is typically either
         `np.int32` or `np.int64` depending on the platform.
         """
         from numpy import intp
         return intp
 
+    def _raise_indexerror(self, shape, axis=0):
+        size = shape[axis]
+        out_of_bounds = (self.array >= size) | ((-size > self.array) & (self.array < 0))
+        if out_of_bounds.any():
+            raise IndexError(f"index {self.array[out_of_bounds].flat[0]} is out of bounds for axis {axis} with size {size}")
+
     def reduce(self, shape=None, axis=0):
         """
         Reduce an `IntegerArray` index on an array of shape `shape`.
 
         The result will either be `IndexError` if the index is invalid for the
         given shape, an `IntegerArray` index where the values are all
         nonnegative, or, if `self` is a scalar array index (`self.shape ==
@@ -85,29 +91,26 @@
             return Integer(self.array).reduce(shape, axis=axis)
 
         if shape is None:
             return self
 
         shape = asshape(shape, axis=axis)
 
+        self._raise_indexerror(shape, axis)
+
         size = shape[axis]
         new_array = self.array.copy()
-        out_of_bounds = (new_array >= size) | ((-size > new_array) & (new_array < 0))
-        if out_of_bounds.any():
-            raise IndexError(f"index {new_array[out_of_bounds].flat[0]} is out of bounds for axis {axis} with size {size}")
-
         new_array[new_array < 0] += size
         return IntegerArray(new_array)
 
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
-        # reduce will raise IndexError if it should be raised
-        self.reduce(shape)
+        self._raise_indexerror(shape)
         return self.shape + shape[1:]
 
     def isempty(self, shape=None):
         if shape is not None:
             return 0 in self.newshape(shape)
 
         return 0 in self.shape
```

### Comparing `ndindex-1.6/ndindex/ndindex.py` & `ndindex-1.7/ndindex/ndindex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import sys
 import inspect
-import itertools
-import numbers
 import operator
-import functools
 
 newaxis = None
 
 def ndindex(obj):
     """
     Convert an object into an ndindex type
 
@@ -293,14 +290,54 @@
         .IntegerArray.reduce
         .BooleanArray.reduce
 
         """
         # XXX: Should the default be raise NotImplementedError or return self?
         raise NotImplementedError
 
+    def isvalid(self, shape):
+        """
+        Check whether a given index is valid on an array of a given shape.
+
+        Returns `True` if an array of shape `shape` can be indexed by `self`
+        and `False` if it would raise `IndexError`.
+
+        >>> from ndindex import ndindex
+        >>> ndindex(3).isvalid((4,))
+        True
+        >>> ndindex(3).isvalid((2,))
+        False
+
+        Note that some indices can never be valid and will raise a
+        `IndexError` or `TypeError` if you attempt to construct them.
+
+        >>> ndindex((..., 0, ...))
+        Traceback (most recent call last):
+          ...
+        IndexError: an index can only have a single ellipsis ('...')
+        >>> ndindex(slice(True))
+        Traceback (most recent call last):
+          ...
+        TypeError: 'bool' object cannot be interpreted as an integer
+
+        See Also
+        ========
+        .NDIndex.newshape
+
+        """
+        # Every class except for Tuple has a more direct efficient
+        # implementation. The logic for checking if a Tuple index is valid is
+        # basically the same as the logic in reduce/expand, so there's no
+        # point in duplicating it.
+        try:
+            self.reduce(shape)
+            return True
+        except IndexError:
+            return False
+
     def expand(self, shape):
         r"""
         Expand a Tuple index on an array of shape `shape`
 
         An expanded index is as explicit as possible. Unlike :meth:`reduce
         <ndindex.ndindex.NDIndex.reduce>`, which tries to simplify an index
         and remove redundancies, `expand()` typically makes an index larger.
@@ -373,30 +410,34 @@
     def newshape(self, shape):
         """
         Returns the shape of `a[idx.raw]`, assuming `a` has shape `shape`.
 
         `shape` should be a tuple of ints, or an int, which is equivalent to a
         1-D shape.
 
-        Raises `IndexError` if `self` would be out of shape for an array of
-        shape `shape`.
+        Raises `IndexError` if `self` would be invalid for an array of shape
+        `shape`.
 
         >>> from ndindex import Slice, Integer, Tuple
         >>> shape = (6, 7, 8)
         >>> Integer(1).newshape(shape)
         (7, 8)
         >>> Integer(10).newshape(shape)
         Traceback (most recent call last):
         ...
         IndexError: index 10 is out of bounds for axis 0 with size 6
         >>> Slice(2, 5).newshape(shape)
         (3, 7, 8)
         >>> Tuple(0, ..., Slice(1, 3)).newshape(shape)
         (7, 2)
 
+        See Also
+        ========
+        .NDIndex.isvalid
+
         """
         raise NotImplementedError
 
     def as_subindex(self, index):
         """
         `i.as_subindex(j)` produces an index `k` such that `a[j][k]` gives all of
         the elements of `a[j]` that are also in `a[i]`.
@@ -553,315 +594,14 @@
         ========
 
         expand
 
         """
         return self
 
-
-# TODO: Use this in other places in the code that check broadcast compatibility.
-class BroadcastError(ValueError):
-    """
-    Exception raised by :func:`iter_indices()` when the input shapes are not
-    broadcast compatible.
-
-    This is used instead of the NumPy exception of the same name so that
-    `iter_indices` does not need to depend on NumPy.
-    """
-
-class AxisError(ValueError, IndexError):
-    """
-    Exception raised by :func:`iter_indices()` when the `skip_axes` argument
-    is out of bounds.
-
-    This is used instead of the NumPy exception of the same name so that
-    `iter_indices` does not need to depend on NumPy.
-
-    """
-    __slots__ = ("axis", "ndim")
-
-    def __init__(self, axis, ndim):
-        self.axis = axis
-        self.ndim = ndim
-
-    def __str__(self):
-        return f"axis {self.axis} is out of bounds for array of dimension {self.ndim}"
-
-def broadcast_shapes(*shapes):
-    """
-    Broadcast the input shapes `shapes` to a single shape.
-
-    This is the same as :py:func:`np.broadcast_shapes()
-    <numpy.broadcast_shapes>`. It is included as a separate helper function
-    because `np.broadcast_shapes()` is on available in NumPy 1.20 or newer, and
-    so that ndindex functions that use this function can do without requiring
-    NumPy to be installed.
-
-    """
-
-    def _broadcast_shapes(shape1, shape2):
-        """Broadcasts `shape1` and `shape2`"""
-        N1 = len(shape1)
-        N2 = len(shape2)
-        N = max(N1, N2)
-        shape = [None for _ in range(N)]
-        i = N - 1
-        while i >= 0:
-            n1 = N1 - N + i
-            if N1 - N + i >= 0:
-                d1 = shape1[n1]
-            else:
-                d1 = 1
-            n2 = N2 - N + i
-            if N2 - N + i >= 0:
-                d2 = shape2[n2]
-            else:
-                d2 = 1
-
-            if d1 == 1:
-                shape[i] = d2
-            elif d2 == 1:
-                shape[i] = d1
-            elif d1 == d2:
-                shape[i] = d1
-            else:
-                # TODO: Build an error message that matches NumPy
-                raise BroadcastError("shape mismatch: objects cannot be broadcast to a single shape.")
-
-            i = i - 1
-
-        return tuple(shape)
-
-    return functools.reduce(_broadcast_shapes, shapes, ())
-
-def iter_indices(*shapes, skip_axes=(), _debug=False):
-    """
-    Iterate indices for every element of an arrays of shape `shapes`.
-
-    Each shape in `shapes` should be a shape tuple, which are broadcast
-    compatible. Each iteration step will produce a tuple of indices, one for
-    each shape, which would correspond to the same elements if the arrays of
-    the given shapes were first broadcast together.
-
-    This is a generalization of the NumPy :py:class:`np.ndindex()
-    <numpy.ndindex>` function (which otherwise has no relation).
-    `np.ndindex()` only iterates indices for a single shape, whereas
-    `iter_indices()` supports generating indices for multiple broadcast
-    compatible shapes at once. This is equivalent to first broadcasting the
-    arrays then generating indices for the single broadcasted shape.
-
-    Additionally, this function supports the ability to skip axes of the
-    shapes using `skip_axes`. These axes will be fully sliced in each index.
-    The remaining axes will be indexed one element at a time with integer
-    indices.
-
-    `skip_axes` should be a tuple of axes to skip. It can use negative
-    integers, e.g., `skip_axes=(-1,)` will skip the last axis. The order of
-    the axes in `skip_axes` does not matter, but it should not contain
-    duplicate axes. The axes in `skip_axes` refer to the final broadcasted
-    shape of `shapes`. For example, `iter_indices((3,), (1, 2, 3),
-    skip_axes=(0,))` will skip the first axis, and only applies to the second
-    shape, since the first shape corresponds to axis `2` of the final
-    broadcasted shape `(1, 2, 3)`
-
-    For example, suppose `a` is an array with shape `(3, 2, 4, 4)`, which we
-    wish to think of as a `(3, 2)` stack of 4 x 4 matrices. We can generate an
-    iterator for each matrix in the "stack" with `iter_indices((3, 2, 4, 4),
-    skip_axes=(-1, -2))`:
-
-    >>> from ndindex import iter_indices
-    >>> for idx in iter_indices((3, 2, 4, 4), skip_axes=(-1, -2)):
-    ...     print(idx)
-    (Tuple(0, 0, slice(None, None, None), slice(None, None, None)),)
-    (Tuple(0, 1, slice(None, None, None), slice(None, None, None)),)
-    (Tuple(1, 0, slice(None, None, None), slice(None, None, None)),)
-    (Tuple(1, 1, slice(None, None, None), slice(None, None, None)),)
-    (Tuple(2, 0, slice(None, None, None), slice(None, None, None)),)
-    (Tuple(2, 1, slice(None, None, None), slice(None, None, None)),)
-
-    Note that the iterates of `iter_indices` are always a tuple, even if only
-    a single shape is provided (one could instead use `for idx, in
-    iter_indices(...)` above).
-
-    As another example, say `a` is shape `(1, 3)` and `b` is shape `(2, 1)`,
-    and we want to generate indices for every value of the broadcasted
-    operation `a + b`. We can do this by using `a[idx1.raw] + b[idx2.raw]` for every
-    `idx1` and `idx2` as below:
-
-    >>> import numpy as np
-    >>> a = np.arange(3).reshape((1, 3))
-    >>> b = np.arange(100, 111, 10).reshape((2, 1))
-    >>> a
-    array([[0, 1, 2]])
-    >>> b
-    array([[100],
-           [110]])
-    >>> for idx1, idx2 in iter_indices((1, 3), (2, 1)): # doctest: +SKIP37
-    ...     print(f"{idx1 = }; {idx2 = }; {(a[idx1.raw], b[idx2.raw]) = }")
-    idx1 = Tuple(0, 0); idx2 = Tuple(0, 0); (a[idx1.raw], b[idx2.raw]) = (0, 100)
-    idx1 = Tuple(0, 1); idx2 = Tuple(0, 0); (a[idx1.raw], b[idx2.raw]) = (1, 100)
-    idx1 = Tuple(0, 2); idx2 = Tuple(0, 0); (a[idx1.raw], b[idx2.raw]) = (2, 100)
-    idx1 = Tuple(0, 0); idx2 = Tuple(1, 0); (a[idx1.raw], b[idx2.raw]) = (0, 110)
-    idx1 = Tuple(0, 1); idx2 = Tuple(1, 0); (a[idx1.raw], b[idx2.raw]) = (1, 110)
-    idx1 = Tuple(0, 2); idx2 = Tuple(1, 0); (a[idx1.raw], b[idx2.raw]) = (2, 110)
-    >>> a + b
-    array([[100, 101, 102],
-           [110, 111, 112]])
-
-    To include an index into the final broadcasted array, you can simply
-    include the final broadcasted shape as one of the shapes (the NumPy
-    function :func:`np.broadcast_shapes() <numpy:numpy.broadcast_shapes>` is
-    useful here).
-
-    >>> np.broadcast_shapes((1, 3), (2, 1))
-    (2, 3)
-    >>> for idx1, idx2, broadcasted_idx in iter_indices((1, 3), (2, 1), (2, 3)):
-    ...     print(broadcasted_idx)
-    Tuple(0, 0)
-    Tuple(0, 1)
-    Tuple(0, 2)
-    Tuple(1, 0)
-    Tuple(1, 1)
-    Tuple(1, 2)
-
-    """
-    if not shapes:
-        yield ()
-        return
-
-    shapes = [asshape(shape) for shape in shapes]
-    ndim = len(max(shapes, key=len))
-
-    if isinstance(skip_axes, int):
-        skip_axes = (skip_axes,)
-    _skip_axes = []
-    for a in skip_axes:
-        try:
-            a = ndindex(a).reduce(ndim).args[0]
-        except IndexError:
-            raise AxisError(a, ndim)
-        if a in _skip_axes:
-            raise ValueError("skip_axes should not contain duplicate axes")
-        _skip_axes.append(a)
-
-    _shapes = [(1,)*(ndim - len(shape)) + shape for shape in shapes]
-    iters = [[] for i in range(len(shapes))]
-    broadcasted_shape = broadcast_shapes(*shapes)
-
-    for i in range(-1, -ndim-1, -1):
-        for it, shape, _shape in zip(iters, shapes, _shapes):
-            if -i > len(shape):
-                for j in range(len(it)):
-                    if broadcasted_shape[i] not in [0, 1]:
-                        it[j] = ncycles(it[j], broadcasted_shape[i])
-                    break
-            elif ndim + i in _skip_axes:
-                it.insert(0, [slice(None)])
-            else:
-                if broadcasted_shape[i] != 1 and shape[i] == 1:
-                    it.insert(0, ncycles(range(shape[i]), broadcasted_shape[i]))
-                else:
-                    it.insert(0, range(shape[i]))
-
-    if _debug: # pragma: no cover
-        print(iters)
-        # Use this instead when we drop Python 3.7 support
-        # print(f"{iters = }")
-    for idxes in itertools.zip_longest(*[itertools.product(*i) for i in
-                                         iters], fillvalue=()):
-        yield tuple(ndindex(idx) for idx in idxes)
-
-class ncycles:
-    """
-    Iterate `iterable` repeated `n` times.
-
-    This is based on a recipe from the `Python itertools docs
-    <https://docs.python.org/3/library/itertools.html#itertools-recipes>`_,
-    but improved to give a repr, and to denest when it can. This makes
-    debugging :func:`~.iter_indices` easier.
-
-    >>> from ndindex.ndindex import ncycles
-    >>> ncycles(range(3), 2)
-    ncycles(range(0, 3), 2)
-    >>> list(_)
-    [0, 1, 2, 0, 1, 2]
-    >>> ncycles(ncycles(range(3), 3), 2)
-    ncycles(range(0, 3), 6)
-
-    """
-    def __new__(cls, iterable, n):
-        if n == 1:
-            return iterable
-        return object.__new__(cls)
-
-    def __init__(self, iterable, n):
-        if isinstance(iterable, ncycles):
-            self.iterable = iterable.iterable
-            self.n = iterable.n*n
-        else:
-            self.iterable = iterable
-            self.n = n
-
-    def __repr__(self):
-        return f"ncycles({self.iterable!r}, {self.n!r})"
-
-    def __iter__(self):
-        return itertools.chain.from_iterable(itertools.repeat(tuple(self.iterable), self.n))
-
-def asshape(shape, axis=None):
-    """
-    Cast `shape` as a valid NumPy shape.
-
-    The input can be an integer `n`, which is equivalent to `(n,)`, or a tuple
-    of integers.
-
-    If the `axis` argument is provided, an `IndexError` is raised if it is out
-    of bounds for the shape.
-
-    The resulting shape is always a tuple of nonnegative integers.
-
-    All ndindex functions that take a shape input should use::
-
-        shape = asshape(shape)
-
-    or::
-
-        shape = asshape(shape, axis=axis)
-
-    """
-    from .integer import Integer
-    from .tuple import Tuple
-    if isinstance(shape, (Tuple, Integer)):
-        raise TypeError("ndindex types are not meant to be used as a shape - "
-                        "did you mean to use the built-in tuple type?")
-
-    if isinstance(shape, numbers.Number):
-        shape = (operator_index(shape),)
-
-    try:
-        l = len(shape)
-    except TypeError:
-        raise TypeError("expected sequence object with len >= 0 or a single integer")
-
-    newshape = []
-    # numpy uses __getitem__ rather than __iter__ to index into shape, so we
-    # match that
-    for i in range(l):
-        # Raise TypeError if invalid
-        newshape.append(operator_index(shape[i]))
-
-        if shape[i] < 0:
-            raise ValueError("unknown (negative) dimensions are not supported")
-
-    if axis is not None:
-        if len(newshape) <= axis:
-            raise IndexError(f"too many indices for array: array is {len(shape)}-dimensional, but {axis + 1} were indexed")
-
-    return tuple(newshape)
-
 def operator_index(idx):
     """
     Convert `idx` into an integer index using `__index__()` or raise
     `TypeError`.
 
     This is the same as `operator.index()` except it disallows boolean types.
```

### Comparing `ndindex-1.6/ndindex/newaxis.py` & `ndindex-1.7/ndindex/newaxis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .ndindex import NDIndex, asshape
+from .ndindex import NDIndex
+from .shapetools import asshape
 
 class Newaxis(NDIndex):
     """
     Represents a `np.newaxis` (i.e., `None`) index.
 
     `Newaxis` adds a shape 1 dimension to the array. If a `Newaxis` is inside
     of a tuple index, it adds a shape 1 dimension at that location in the
@@ -65,14 +66,18 @@
         .BooleanArray.reduce
 
         """
         if shape is not None:
             shape = asshape(shape)
         return self
 
+    def isvalid(self, shape):
+        shape = asshape(shape)
+        return True
+
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
         # reduce will raise IndexError if it should be raised
         self.reduce(shape)
```

### Comparing `ndindex-1.6/ndindex/slice.py` & `ndindex-1.7/ndindex/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .ndindex import NDIndex, asshape, operator_index
+from .ndindex import NDIndex, operator_index
 from .subindex_helpers import subindex_slice
+from .shapetools import asshape
 
 class default:
     """
     A default keyword argument value.
 
     Used as the default value for keyword arguments where `None` is also a
     meaningful value but not the default.
@@ -24,16 +25,16 @@
     `Slice(a, b)` is the same as the syntax `a:b` in an index and `Slice(a, b,
     c)` is the same as `a:b:c`. An argument being `None` is equivalent to the
     syntax where the item is omitted, for example, `Slice(None, None, k)` is
     the same as the syntax `::k`.
 
     `Slice.args` always has three arguments, and does not make any distinction
     between, for instance, `Slice(x, y)` and `Slice(x, y, None)`. This is
-    because Python itself does not make the distinction between x:y and x:y:
-    syntactically.
+    because Python itself does not make the distinction between `x:y` and
+    `x:y:` syntactically.
 
     See :ref:`slices-docs` for a description of the semantic meaning of slices
     on arrays.
 
     Slice has attributes `start`, `stop`, and `step` to access the
     corresponding attributes.
 
@@ -466,14 +467,21 @@
             if stop < 0 and start % step != 0:
                 # At this point, negative stop is only necessary to index the
                 # first element. If that element isn't actually indexed, we
                 # prefer a nonnegative stop. Otherwise, stop will be -size - 1.
                 stop = start % -step - 1
         return self.__class__(start, stop, step)
 
+    def isvalid(self, shape):
+        # The docstring for this method is on the NDIndex base class
+        shape = asshape(shape)
+
+        # All slices are valid as long as there is at least one dimension
+        return bool(shape)
+
     def newshape(self, shape):
         # The docstring for this method is on the NDIndex base class
         shape = asshape(shape)
 
         idx = self.reduce(shape)
 
         # len() won't raise an error after reducing with a shape
```

### Comparing `ndindex-1.6/ndindex/subindex_helpers.py` & `ndindex-1.7/ndindex/subindex_helpers.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/__init__.py` & `ndindex-1.7/ndindex/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/doctest.py` & `ndindex-1.7/ndindex/tests/doctest.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/helpers.py` & `ndindex-1.7/ndindex/tests/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import sys
 from itertools import chain
-from functools import reduce
-from operator import mul
+import warnings
+from functools import wraps
 
 from numpy import intp, bool_, array, broadcast_shapes
 import numpy.testing
 
 from pytest import fail
 
 from hypothesis import assume, note
 from hypothesis.strategies import (integers, none, one_of, lists, just,
                                    builds, shared, composite, sampled_from,
                                    booleans)
 from hypothesis.extra.numpy import (arrays, mutually_broadcastable_shapes as
                                     mbs, BroadcastableShapes)
 
 from ..ndindex import ndindex
+from ..shapetools import remove_indices, unremove_indices
+from .._crt import prod
 
 # Hypothesis strategies for generating indices. Note that some of these
 # strategies are nominally already defined in hypothesis, but we redefine them
 # here because the hypothesis definitions are too restrictive. For example,
 # hypothesis's slices strategy does not generate slices with negative indices.
 # Similarly, hypothesis.extra.numpy.basic_indices only generates tuples.
 
-# np.prod has overflow and math.prod is Python 3.8+ only
-def prod(seq):
-    return reduce(mul, seq, 1)
-
 nonnegative_ints = integers(0, 10)
 negative_ints = integers(-10, -1)
 ints = lambda: one_of(nonnegative_ints, negative_ints)
 
 def slices(start=one_of(none(), ints()), stop=one_of(none(), ints()),
            step=one_of(none(), ints())):
     return builds(slice, start, stop, step)
@@ -46,146 +44,225 @@
 MAX_ARRAY_SIZE = 100000
 SHORT_MAX_ARRAY_SIZE = 1000
 shapes = tuples(integers(0, 10)).filter(
              # numpy gives errors with empty arrays with large shapes.
              # See https://github.com/numpy/numpy/issues/15753
              lambda shape: prod([i for i in shape if i]) < MAX_ARRAY_SIZE)
 
-_short_shapes = tuples(integers(0, 10)).filter(
+_short_shapes = lambda n: tuples(integers(0, 10), min_size=n).filter(
              # numpy gives errors with empty arrays with large shapes.
              # See https://github.com/numpy/numpy/issues/15753
              lambda shape: prod([i for i in shape if i]) < SHORT_MAX_ARRAY_SIZE)
 
+# short_shapes should be used in place of shapes in any test function that
+# uses ndindices, boolean_arrays, or tuples
+short_shapes = shared(_short_shapes(0))
+
+_integer_arrays = arrays(intp, short_shapes)
+integer_scalars = arrays(intp, ()).map(lambda x: x[()])
+integer_arrays = one_of(integer_scalars, _integer_arrays.flatmap(lambda x: one_of(just(x), just(x.tolist()))))
+
+# We need to make sure shapes for boolean arrays are generated in a way that
+# makes them related to the test array shape. Otherwise, it will be very
+# difficult for the boolean array index to match along the test array, which
+# means we won't test any behavior other than IndexError.
+
+@composite
+def subsequences(draw, sequence):
+    seq = draw(sequence)
+    start = draw(integers(0, max(0, len(seq)-1)))
+    stop = draw(integers(start, len(seq)))
+    return seq[start:stop]
+
+_boolean_arrays = arrays(bool_, one_of(subsequences(short_shapes), short_shapes))
+boolean_scalars = arrays(bool_, ()).map(lambda x: x[()])
+boolean_arrays = one_of(boolean_scalars, _boolean_arrays.flatmap(lambda x: one_of(just(x), just(x.tolist()))))
+
+def _doesnt_raise(idx):
+    try:
+        ndindex(idx)
+    except (IndexError, ValueError, NotImplementedError):
+        return False
+    return True
+
+Tuples = tuples(one_of(ellipses(), ints(), slices(), newaxes(),
+                       integer_arrays, boolean_arrays)).filter(_doesnt_raise)
+
+ndindices = one_of(
+    ints(),
+    slices(),
+    ellipses(),
+    newaxes(),
+    Tuples,
+    integer_arrays,
+    boolean_arrays,
+).filter(_doesnt_raise)
+
 # Note: We could use something like this:
 
 # mutually_broadcastable_shapes = shared(integers(1, 32).flatmap(lambda i: mbs(num_shapes=i).filter(
 #     lambda broadcastable_shapes: prod([i for i in broadcastable_shapes.result_shape if i]) < MAX_ARRAY_SIZE)))
 
-
 @composite
-def _mutually_broadcastable_shapes(draw):
+def _mutually_broadcastable_shapes(draw, *, shapes=short_shapes, min_shapes=0, max_shapes=32, min_side=0):
     # mutually_broadcastable_shapes() with the default inputs doesn't generate
     # very interesting examples (see
     # https://github.com/HypothesisWorks/hypothesis/issues/3170). It's very
     # difficult to get it to do so by tweaking the max_* parameters, because
     # making them too big leads to generating too large shapes and filtering
     # too much. So instead, we trick it into generating more interesting
     # examples by telling it to create shapes that broadcast against some base
     # shape.
 
     # Unfortunately, this, along with the filtering below, has a downside that
     # it tends to generate a result shape of () more often than you might
     # like. But it generates enough "real" interesting shapes that both of
     # these workarounds are worth doing (plus I don't know if any other better
     # way of handling the situation).
-    base_shape = draw(short_shapes)
+    base_shape = draw(shapes)
 
     input_shapes, result_shape = draw(
         mbs(
-            num_shapes=32,
+            num_shapes=max_shapes,
             base_shape=base_shape,
-            min_side=0,
+            min_side=min_side,
         ))
 
     # The hypothesis mutually_broadcastable_shapes doesn't allow num_shapes to
     # be a strategy. It's tempting to do something like num_shapes =
-    # draw(integers(1, 32)), but this shrinks poorly. See
+    # draw(integers(min_shapes, max_shapes)), but this shrinks poorly. See
     # https://github.com/HypothesisWorks/hypothesis/issues/3151. So instead of
-    # using a strategy to draw the number of shapes, we just generate 32
+    # using a strategy to draw the number of shapes, we just generate max_shapes
     # shapes and pick a subset of them.
-    final_input_shapes = draw(lists(sampled_from(input_shapes), min_size=0, max_size=32,
-                        unique_by=id,))
+    final_input_shapes = draw(lists(sampled_from(input_shapes),
+                                    min_size=min_shapes, max_size=max_shapes))
 
 
     # Note: result_shape is input_shapes broadcasted with base_shape, but
     # base_shape itself is not part of input_shapes. We "really" want our base
     # shape to be (). We are only using it here to trick
     # mutually_broadcastable_shapes into giving more interesting examples.
     final_result_shape = broadcast_shapes(*final_input_shapes)
 
     # The broadcast compatible shapes can be bigger than the base shape. This
     # is already somewhat limited by the mutually_broadcastable_shapes
     # defaults, and pretty unlikely, but we filter again here just to be safe.
     if not prod([i for i in final_result_shape if i]) < SHORT_MAX_ARRAY_SIZE: # pragma: no cover
-        note(f"Filtering {result_shape}")
+        note(f"Filtering the shape {result_shape} (too many elements)")
         assume(False)
 
     return BroadcastableShapes(final_input_shapes, final_result_shape)
 
 mutually_broadcastable_shapes = shared(_mutually_broadcastable_shapes())
 
 @composite
-def skip_axes(draw):
+def _skip_axes_st(draw,
+                  mutually_broadcastable_shapes=mutually_broadcastable_shapes,
+                  num_skip_axes=None):
     shapes, result_shape = draw(mutually_broadcastable_shapes)
-    n = len(result_shape)
-    axes = draw(one_of(none(),
-                      lists(integers(-n, max(0, n-1)), max_size=n)))
-    if isinstance(axes, list):
-        axes = tuple(axes)
-        # Sometimes return an integer
-        if len(axes) == 1 and draw(booleans()): # pragma: no cover
-            return axes[0]
+    if result_shape == ():
+        assume(num_skip_axes is None)
+        return ()
+    negative = draw(booleans(), label='skip_axes < 0')
+    N = len(min(shapes, key=len))
+    if num_skip_axes is not None:
+        min_size = max_size = num_skip_axes
+        assume(N >= num_skip_axes)
+    else:
+        min_size = 0
+        max_size = None
+    if N == 0:
+        return ()
+    if negative:
+        axes = draw(lists(integers(-N, -1), min_size=min_size, max_size=max_size, unique=True))
+    else:
+        axes = draw(lists(integers(0, N-1), min_size=min_size, max_size=max_size, unique=True))
+    axes = tuple(axes)
+    # Sometimes return an integer
+    if num_skip_axes is None and len(axes) == 1 and draw(booleans(), label='skip_axes integer'): # pragma: no cover
+        return axes[0]
     return axes
 
-# We need to make sure shapes for boolean arrays are generated in a way that
-# makes them related to the test array shape. Otherwise, it will be very
-# difficult for the boolean array index to match along the test array, which
-# means we won't test any behavior other than IndexError.
-
-# short_shapes should be used in place of shapes in any test function that
-# uses ndindices, boolean_arrays, or tuples
-short_shapes = shared(_short_shapes)
-
-_integer_arrays = arrays(intp, short_shapes)
-integer_scalars = arrays(intp, ()).map(lambda x: x[()])
-integer_arrays = one_of(integer_scalars, _integer_arrays.flatmap(lambda x: one_of(just(x), just(x.tolist()))))
+skip_axes_st = shared(_skip_axes_st())
 
 @composite
-def subsequences(draw, sequence):
-    seq = draw(sequence)
-    start = draw(integers(0, max(0, len(seq)-1)))
-    stop = draw(integers(start, len(seq)))
-    return seq[start:stop]
-
-_boolean_arrays = arrays(bool_, one_of(subsequences(short_shapes), short_shapes))
-boolean_scalars = arrays(bool_, ()).map(lambda x: x[()])
-boolean_arrays = one_of(boolean_scalars, _boolean_arrays.flatmap(lambda x: one_of(just(x), just(x.tolist()))))
-
-def _doesnt_raise(idx):
-    try:
-        ndindex(idx)
-    except (IndexError, ValueError, NotImplementedError):
-        return False
-    return True
+def mutually_broadcastable_shapes_with_skipped_axes(draw, skip_axes_st=skip_axes_st, mutually_broadcastable_shapes=mutually_broadcastable_shapes,
+skip_axes_values=integers(0)):
+    """
+    mutually_broadcastable_shapes except skip_axes() axes might not be
+    broadcastable
 
-Tuples = tuples(one_of(ellipses(), ints(), slices(), newaxes(),
-                       integer_arrays, boolean_arrays)).filter(_doesnt_raise)
+    The result_shape will be None in the position of skip_axes.
+    """
+    skip_axes_ = draw(skip_axes_st)
+    shapes, result_shape = draw(mutually_broadcastable_shapes)
+    if isinstance(skip_axes_, int):
+        skip_axes_ = (skip_axes_,)
 
-ndindices = one_of(
-    ints(),
-    slices(),
-    ellipses(),
-    newaxes(),
-    Tuples,
-    integer_arrays,
-    boolean_arrays,
-).filter(_doesnt_raise)
+    # Randomize the shape values in the skipped axes
+    shapes_ = []
+    for shape in shapes:
+        _shape = list(unremove_indices(shape, skip_axes_))
+        # sanity check
+        assert remove_indices(_shape, skip_axes_) == shape, (_shape, skip_axes_, shape)
+
+        # Replace None values with random values
+        for j in range(len(_shape)):
+            if _shape[j] is None:
+                _shape[j] = draw(skip_axes_values)
+        shapes_.append(tuple(_shape))
+
+    result_shape_ = unremove_indices(result_shape, skip_axes_)
+    # sanity check
+    assert remove_indices(result_shape_, skip_axes_) == result_shape
+
+    for shape in shapes_:
+        if prod([i for i in shape if i]) >= SHORT_MAX_ARRAY_SIZE:
+            note(f"Filtering the shape {shape} (too many elements)")
+            assume(False)
+    return BroadcastableShapes(shapes_, result_shape_)
+
+two_mutually_broadcastable_shapes_1 = shared(_mutually_broadcastable_shapes(
+    shapes=_short_shapes(1),
+    min_shapes=2,
+    max_shapes=2,
+    min_side=1))
+one_skip_axes = shared(_skip_axes_st(
+    mutually_broadcastable_shapes=two_mutually_broadcastable_shapes_1,
+    num_skip_axes=1))
+two_mutually_broadcastable_shapes_2 = shared(_mutually_broadcastable_shapes(
+    shapes=_short_shapes(2),
+    min_shapes=2,
+    max_shapes=2,
+    min_side=2))
+two_skip_axes = shared(_skip_axes_st(
+    mutually_broadcastable_shapes=two_mutually_broadcastable_shapes_2,
+    num_skip_axes=2))
 
 def assert_equal(actual, desired, err_msg='', verbose=True):
     """
     Same as numpy.testing.assert_equal except it also requires the shapes and
     dtypes to be equal.
 
     """
     numpy.testing.assert_equal(actual, desired, err_msg=err_msg,
                                verbose=verbose)
     assert actual.shape == desired.shape, err_msg or f"{actual.shape} != {desired.shape}"
     assert actual.dtype == desired.dtype, err_msg or f"{actual.dtype} != {desired.dtype}"
 
-def check_same(a, idx, raw_func=lambda a, idx: a[idx],
+def warnings_are_errors(f):
+    @wraps(f)
+    def inner(*args, **kwargs):
+        with warnings.catch_warnings():
+            warnings.simplefilter("error")
+            return f(*args, **kwargs)
+    return inner
+
+@warnings_are_errors
+def check_same(a, idx, *, raw_func=lambda a, idx: a[idx],
                ndindex_func=lambda a, index: a[index.raw],
                same_exception=True, assert_equal=assert_equal):
     """
     Check that a raw index idx produces the same result on an array a before
     and after being transformed by ndindex.
 
     Tests that raw_func(a, idx) == ndindex_func(a, ndindex(idx)) or that they
@@ -211,16 +288,19 @@
         # deprecation warning. We want to test against the post-deprecation
         # behavior.
         e_inner = None
         try:
             try:
                 a_raw = raw_func(a, idx)
             except Warning as w:
-                if ("Using a non-tuple sequence for multidimensional indexing is deprecated" in w.args[0]):
-                    idx = array(idx)
+                # In NumPy < 1.23, this is a FutureWarning. In 1.23 the
+                # deprecation was removed and lists are always interpreted as
+                # array indices.
+                if ("Using a non-tuple sequence for multidimensional indexing is deprecated" in w.args[0]): # pragma: no cover
+                    idx = array(idx, dtype=intp)
                     a_raw = raw_func(a, idx)
                 elif "Out of bound index found. This was previously ignored when the indexing result contained no elements. In the future the index error will be raised. This error occurs either due to an empty slice, or if an array has zero elements even before indexing." in w.args[0]:
                     same_exception = False
                     raise IndexError
                 else: # pragma: no cover
                     fail(f"Unexpected warning raised: {w}")
         except Exception:
```

### Comparing `ndindex-1.6/ndindex/tests/test_array.py` & `ndindex-1.7/ndindex/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_as_subindex.py` & `ndindex-1.7/ndindex/tests/test_as_subindex.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from hypothesis import given, assume, example
 from hypothesis.strategies import integers, one_of
 
 from ..ndindex import ndindex
 from ..integerarray import IntegerArray
 from ..tuple import Tuple
-from .helpers import ndindices, short_shapes, assert_equal
+from .helpers import ndindices, short_shapes, assert_equal, warnings_are_errors
 
 @example((slice(0, 8), slice(0, 9), slice(0, 10)),
          ([2, 5, 6, 7], slice(1, 9, 1), slice(5, 10, 1)),
          (20, 20, 20))
 @example((), (None, array([], dtype=intp)), 0)
 @example((), array([], dtype=bool), 0)
 @example((), IntegerArray(0), 1)
@@ -46,14 +46,15 @@
 @example([0], slice(0, 0), 1)
 @example(0, slice(0, 1), 1)
 @example([0], slice(0, 1), 1)
 @example(slice(0, 5), 2, 10)
 @example(0, (slice(None, 0, None), Ellipsis), 1)
 @example(0, (slice(1, 2),), 1)
 @given(ndindices, ndindices, one_of(integers(0, 100), short_shapes))
+@warnings_are_errors
 def test_as_subindex_hypothesis(idx1, idx2, shape):
     if isinstance(shape, int):
         a = arange(shape)
     else:
         a = arange(prod(shape)).reshape(shape)
 
     try:
```

### Comparing `ndindex-1.6/ndindex/tests/test_booleanarray.py` & `ndindex-1.7/ndindex/tests/test_booleanarray.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_broadcast_arrays.py` & `ndindex-1.7/ndindex/tests/test_broadcast_arrays.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 
 from ..ndindex import ndindex
 from ..array import ArrayIndex
 from ..booleanarray import BooleanArray
 from ..integerarray import IntegerArray
 from ..integer import Integer
 from ..tuple import Tuple
-from .helpers import ndindices, check_same, short_shapes
+from .helpers import ndindices, check_same, short_shapes, warnings_are_errors
 
 @example((..., False, False), 1)
 @example((True, False), 1)
 @example((True, True), 1)
 @example(array([False]), 0)
 @example((slice(None, -1, None), array([[1]])), (1, 1))
 @example((1, False), 0)
 @example(True, 1)
 @example(False, 1)
 @example([[True, False], [False, False]], (2, 2, 3))
 @given(ndindices, one_of(short_shapes, integers(0, 10)))
+@warnings_are_errors
 def test_broadcast_arrays_hypothesis(idx, shape):
     if isinstance(shape, int):
         a = arange(shape)
     else:
         a = arange(prod(shape)).reshape(shape)
 
     index = ndindex(idx)
```

### Comparing `ndindex-1.6/ndindex/tests/test_chunking.py` & `ndindex-1.7/ndindex/tests/test_chunking.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_crt.py` & `ndindex-1.7/ndindex/tests/test_crt.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_ellipsis.py` & `ndindex-1.7/ndindex/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_expand.py` & `ndindex-1.7/ndindex/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_integer.py` & `ndindex-1.7/ndindex/tests/test_integer.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_integerarray.py` & `ndindex-1.7/ndindex/tests/test_integerarray.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_newaxis.py` & `ndindex-1.7/ndindex/tests/test_newaxis.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_newshape.py` & `ndindex-1.7/ndindex/tests/test_newshape.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_no_dependencies.py` & `ndindex-1.7/ndindex/tests/test_no_dependencies.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tests/test_slice.py` & `ndindex-1.7/ndindex/tests/test_slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from hypothesis import given, assume, example
 from hypothesis.strategies import integers, one_of
 
 from ..slice import Slice
 from ..integer import Integer
 from ..ellipsis import ellipsis
-from ..ndindex import asshape
+from ..shapetools import asshape
 from .helpers import check_same, slices, prod, shapes, iterslice, assert_equal
 
 def test_slice_args():
     # Test the behavior when not all three arguments are given
     # TODO: Incorporate this into the normal slice tests
     raises(TypeError, lambda: slice())
     raises(TypeError, lambda: Slice())
```

### Comparing `ndindex-1.6/ndindex/tests/test_tuple.py` & `ndindex-1.7/ndindex/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/ndindex/tuple.py` & `ndindex-1.7/ndindex/tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 
-from .ndindex import NDIndex, ndindex, asshape
+from .ndindex import NDIndex, ndindex
 from .subindex_helpers import subindex_slice
+from .shapetools import asshape, broadcast_shapes, BroadcastError
 
 class Tuple(NDIndex):
     """
     Represents a tuple of single-axis indices.
 
     Valid single axis indices are
 
@@ -88,23 +89,20 @@
 
         if newargs.count(...) > 1:
             raise IndexError("an index can only have a single ellipsis ('...')")
         if len(arrays) > 0:
             if has_boolean_scalar:
                 raise NotImplementedError("Tuples mixing boolean scalars (True or False) with arrays are not yet supported.")
 
-            from numpy import broadcast
             try:
-                broadcast(*[i for i in arrays])
-            except ValueError as e:
-                assert str(e).startswith("shape mismatch: objects cannot be broadcast to a single shape"), e.args
-                # TODO: Newer versions of NumPy include where the mismatch is
-                # in the error message in a more informative way than this
-                # (but we can't use it directly because it talks about the
-                # "arg"s to broadcast()).
+                broadcast_shapes(*[i.shape for i in arrays])
+            except BroadcastError:
+                # This matches the NumPy error message. The BroadcastError has
+                # a better error message, but it will be shown in the chained
+                # traceback.
                 raise IndexError("shape mismatch: indexing arrays could not be broadcast together with shapes %s" % ' '.join([str(i.shape) for i in arrays]))
 
         return tuple(newargs)
 
     def __eq__(self, other):
         if isinstance(other, tuple):
             return self.args == other
@@ -288,17 +286,17 @@
                 continue
             elif isinstance(i, IntegerArray):
                 arrays.append(i.raw)
             elif isinstance(i, BooleanArray):
                 # TODO: Avoid explicitly calling nonzero
                 arrays.extend(i.raw.nonzero())
         if arrays:
-            from numpy import broadcast, broadcast_to
+            from numpy import broadcast_to
 
-            broadcast_shape = broadcast(*arrays).shape
+            broadcast_shape = broadcast_shapes(*[a.shape for a in arrays])
         else:
             broadcast_shape = ()
 
         # If the broadcast shape is empty, out of bounds indices in
         # non-empty arrays are ignored, e.g., ([], [10]) would broadcast to
         # ([], []), so the bounds for 10 are not checked. Thus, we must do
         # this before calling reduce() on the arguments. This rule, however,
@@ -424,17 +422,17 @@
             elif isinstance(s, BooleanArray):
                 nz = s.raw.nonzero()
                 arrays.extend(nz)
                 boolean_nonzero[s] = nz
         if not arrays:
             return self
 
-        from numpy import array, broadcast, broadcast_to, intp
+        from numpy import array, broadcast_to, intp
 
-        broadcast_shape = broadcast(*arrays).shape
+        broadcast_shape = broadcast_shapes(*[a.shape for a in arrays])
 
         newargs = []
         for s in args:
             if isinstance(s, BooleanArray):
                 if not _is_boolean_scalar(s):
                     newargs.extend([IntegerArray(broadcast_to(i, broadcast_shape))
                                     for i in boolean_nonzero[s]])
@@ -483,17 +481,17 @@
             elif isinstance(i, IntegerArray):
                 arrays.append(i.raw)
             elif isinstance(i, BooleanArray):
                 # TODO: Avoid calling nonzero twice
                 arrays.extend(i.raw.nonzero())
 
         if arrays:
-            from numpy import broadcast, broadcast_to, array, intp
+            from numpy import broadcast_to, array, intp
 
-            broadcast_shape = broadcast(*arrays).shape
+            broadcast_shape = broadcast_shapes(*[a.shape for a in arrays])
             # If the broadcast shape is empty, out of bounds indices in
             # non-empty arrays are ignored, e.g., ([], [10]) would broadcast to
             # ([], []), so the bounds for 10 are not checked. Thus, we must do
             # this before calling reduce() on the arguments. This rule, however,
             # is *not* followed for scalar integer indices.
 
             for i in range(len(args)):
```

### Comparing `ndindex-1.6/ndindex.egg-info/PKG-INFO` & `ndindex-1.7/ndindex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: ndindex
-Version: 1.6
+Version: 1.7
 Summary: A Python library for manipulating indices of ndarrays.
 Home-page: https://quansight-labs.github.io/ndindex/
 Author: Quansight Labs
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: arrays
 License-File: LICENSE
@@ -103,9 +102,7 @@
 
 <p align="center">
 <a href="https://labs.quansight.org/"><img src="https://labs.quansight.org/images/QuansightLabs_logo_V2.png" alt="https://labs.quansight.org/"
 width="200"></a>
 <a href="https://www.deshaw.com"><img src="https://www.deshaw.com/assets/logos/blue_logo_417x125.png" alt="https://www.deshaw.com"
 width="200"></a>
 </p>
-
-
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: ndindex Version: 1.6 Summary: A Python library for
+Metadata-Version: 2.1 Name: ndindex Version: 1.7 Summary: A Python library for
 manipulating indices of ndarrays. Home-page: https://quansight-labs.github.io/
-ndindex/ Author: Quansight Labs License: MIT Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: arrays License-File:
-LICENSE # ndindex ![ndindex logo](docs/_static/ndindex_logo_white_bg.svg) A
-Python library for manipulating indices of ndarrays. The documentation for
-ndindex can be found at https://quansight-labs.github.io/ndindex/ ndindex is a
-library that allows representing and manipulating objects that can be valid
-indices to numpy arrays, i.e., slices, integers, ellipses, None, integer and
-boolean arrays, and tuples thereof. The goals of the library are - Provide a
-uniform API to manipulate these objects. Unlike the standard index objects
-themselves like `slice`, `int`, and `tuple`, which do not share any methods in
-common related to being indices, ndindex classes can all be manipulated
-uniformly. For example, `idx.args` always gives the arguments used to construct
-`idx`. - Give 100% correct semantics as defined by numpy's ndarray. This means
-that ndindex will not make a transformation on an index object unless it is
-correct for all possible input array shapes. The only exception to this rule is
-that ndindex assumes that any given index will not raise IndexError (for
-instance, from an out of bounds integer index or from too few dimensions). For
-those operations where the array shape is known, there is a `reduce()` method
-to reduce an index to a simpler index that is equivalent for the given shape. -
-Enable useful transformation and manipulation functions on index objects. ##
-Examples **Canonicalize a slice (over a given shape, or independent of array
-shape)** ```py >>> from ndindex import * >>> Slice(-2, 10, 3).reduce() Slice(-
-2, 10, 2) >>> Slice(-2, 10, 3).reduce(5) Slice(3, 4, 1) ``` **Compute the
-maximum length of a sliced axis** ```py >>> import numpy as np >>> len(Slice(2,
-10, 3)) 3 >>> len(np.arange(10)[2:10:3]) 3 ``` **Compute the shape of an array
-of shape `(10, 20)` indexed by `[0, 0:10]`** ```py >>> Tuple(0, slice(0,
-10)).newshape((10, 20)) (10,) >>> np.ones((10, 20))[0, 0:10].shape (10,) ```
-**Check if an indexed array would be empty** ```py >>> Tuple(0, ..., Slice(10,
-20)).isempty((3, 4, 5)) True >>> np.ones((3, 4, 5))[0,...,10:20] array([],
-shape=(4, 0), dtype=float64) ``` See the [documentation](https://quansight-
-labs.github.io/ndindex/) for full details on what ndindex can do. ## License
-[MIT License](LICENSE) ## Acknowledgments ndindex development is supported by
-[Quansight Labs](https://labs.quansight.org/) and is sponsored in part by [the
-D. E. Shaw group](https://www.deshaw.com/). The D. E. Shaw group collaborates
-with Quansight on numerous open source projects, including Numba, Dask and
-Project Jupyter.
+ndindex/ Author: Quansight Labs License: MIT Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Type: text/markdown Provides-Extra: arrays License-File: LICENSE # ndindex !
+[ndindex logo](docs/_static/ndindex_logo_white_bg.svg) A Python library for
+manipulating indices of ndarrays. The documentation for ndindex can be found at
+https://quansight-labs.github.io/ndindex/ ndindex is a library that allows
+representing and manipulating objects that can be valid indices to numpy
+arrays, i.e., slices, integers, ellipses, None, integer and boolean arrays, and
+tuples thereof. The goals of the library are - Provide a uniform API to
+manipulate these objects. Unlike the standard index objects themselves like
+`slice`, `int`, and `tuple`, which do not share any methods in common related
+to being indices, ndindex classes can all be manipulated uniformly. For
+example, `idx.args` always gives the arguments used to construct `idx`. - Give
+100% correct semantics as defined by numpy's ndarray. This means that ndindex
+will not make a transformation on an index object unless it is correct for all
+possible input array shapes. The only exception to this rule is that ndindex
+assumes that any given index will not raise IndexError (for instance, from an
+out of bounds integer index or from too few dimensions). For those operations
+where the array shape is known, there is a `reduce()` method to reduce an index
+to a simpler index that is equivalent for the given shape. - Enable useful
+transformation and manipulation functions on index objects. ## Examples
+**Canonicalize a slice (over a given shape, or independent of array shape)**
+```py >>> from ndindex import * >>> Slice(-2, 10, 3).reduce() Slice(-2, 10, 2)
+>>> Slice(-2, 10, 3).reduce(5) Slice(3, 4, 1) ``` **Compute the maximum length
+of a sliced axis** ```py >>> import numpy as np >>> len(Slice(2, 10, 3)) 3 >>>
+len(np.arange(10)[2:10:3]) 3 ``` **Compute the shape of an array of shape `(10,
+20)` indexed by `[0, 0:10]`** ```py >>> Tuple(0, slice(0, 10)).newshape((10,
+20)) (10,) >>> np.ones((10, 20))[0, 0:10].shape (10,) ``` **Check if an indexed
+array would be empty** ```py >>> Tuple(0, ..., Slice(10, 20)).isempty((3, 4,
+5)) True >>> np.ones((3, 4, 5))[0,...,10:20] array([], shape=(4, 0),
+dtype=float64) ``` See the [documentation](https://quansight-labs.github.io/
+ndindex/) for full details on what ndindex can do. ## License [MIT License]
+(LICENSE) ## Acknowledgments ndindex development is supported by [Quansight
+Labs](https://labs.quansight.org/) and is sponsored in part by [the D. E. Shaw
+group](https://www.deshaw.com/). The D. E. Shaw group collaborates with
+Quansight on numerous open source projects, including Numba, Dask and Project
+Jupyter.
             [https://labs.quansight.org/] [https://www.deshaw.com]
```

### Comparing `ndindex-1.6/ndindex.egg-info/SOURCES.txt` & `ndindex-1.7/ndindex.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
+conftest.py
+pytest.ini
 setup.cfg
 setup.py
 versioneer.py
 ndindex/__init__.py
 ndindex/_crt.py
 ndindex/_version.py
 ndindex/array.py
 ndindex/booleanarray.py
 ndindex/chunking.py
 ndindex/ellipsis.py
 ndindex/integer.py
 ndindex/integerarray.py
 ndindex/ndindex.py
 ndindex/newaxis.py
+ndindex/shapetools.py
 ndindex/slice.py
 ndindex/subindex_helpers.py
 ndindex/tuple.py
 ndindex.egg-info/PKG-INFO
 ndindex.egg-info/SOURCES.txt
 ndindex.egg-info/dependency_links.txt
 ndindex.egg-info/requires.txt
@@ -32,13 +35,15 @@
 ndindex/tests/test_broadcast_arrays.py
 ndindex/tests/test_chunking.py
 ndindex/tests/test_crt.py
 ndindex/tests/test_ellipsis.py
 ndindex/tests/test_expand.py
 ndindex/tests/test_integer.py
 ndindex/tests/test_integerarray.py
+ndindex/tests/test_isvalid.py
 ndindex/tests/test_ndindex.py
 ndindex/tests/test_newaxis.py
 ndindex/tests/test_newshape.py
 ndindex/tests/test_no_dependencies.py
+ndindex/tests/test_shapetools.py
 ndindex/tests/test_slice.py
 ndindex/tests/test_tuple.py
```

### Comparing `ndindex-1.6/setup.py` & `ndindex-1.7/setup.py`

 * *Files identical despite different names*

### Comparing `ndindex-1.6/versioneer.py` & `ndindex-1.7/versioneer.py`

 * *Files identical despite different names*

