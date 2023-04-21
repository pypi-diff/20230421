# Comparing `tmp/chebyfit-2022.9.29.tar.gz` & `tmp/chebyfit-2023.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chebyfit-2022.9.29.tar", last modified: Thu Sep 29 16:37:32 2022, max compression
+gzip compressed data, was "chebyfit-2023.4.22.tar", last modified: Fri Apr 21 18:35:34 2023, max compression
```

## Comparing `chebyfit-2022.9.29.tar` & `chebyfit-2023.4.22.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-09-29 16:37:32.197660 chebyfit-2022.9.29/
--rw-rw-rw-   0        0        0     1559 2022-09-29 16:37:30.000000 chebyfit-2022.9.29/LICENSE
--rw-rw-rw-   0        0        0      130 2018-08-29 19:01:21.000000 chebyfit-2022.9.29/MANIFEST.in
--rw-rw-rw-   0        0        0     3636 2022-09-29 16:37:32.197660 chebyfit-2022.9.29/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2022-09-29 16:37:30.000000 chebyfit-2022.9.29/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-29 16:37:32.188660 chebyfit-2022.9.29/chebyfit/
--rw-rw-rw-   0        0        0      104 2020-01-01 02:43:28.000000 chebyfit-2022.9.29/chebyfit/__init__.py
--rw-rw-rw-   0        0        0    51841 2022-09-29 16:37:18.000000 chebyfit-2022.9.29/chebyfit/chebyfit.c
--rw-rw-rw-   0        0        0     9833 2022-09-29 16:33:39.000000 chebyfit-2022.9.29/chebyfit/chebyfit.py
-drwxrwxrwx   0        0        0        0 2022-09-29 16:37:32.196660 chebyfit-2022.9.29/chebyfit.egg-info/
--rw-rw-rw-   0        0        0     3636 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-29 16:37:31.000000 chebyfit-2022.9.29/chebyfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-29 16:37:32.198659 chebyfit-2022.9.29/setup.cfg
--rw-rw-rw-   0        0        0     3016 2022-09-26 22:21:31.000000 chebyfit-2022.9.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:35:34.810300 chebyfit-2023.4.22/
+drwxrwxrwx   0        0        0        0 2023-04-21 18:35:34.775746 chebyfit-2023.4.22/.github/
+drwxrwxrwx   0        0        0        0 2023-04-21 18:35:34.792072 chebyfit-2023.4.22/.github/workflows/
+-rw-rw-rw-   0        0        0      903 2023-04-21 18:29:13.000000 chebyfit-2023.4.22/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1559 2023-04-21 18:35:31.000000 chebyfit-2023.4.22/LICENSE
+-rw-rw-rw-   0        0        0      395 2023-04-21 17:00:03.000000 chebyfit-2023.4.22/MANIFEST.in
+-rw-rw-rw-   0        0        0     3986 2023-04-21 18:35:34.810300 chebyfit-2023.4.22/PKG-INFO
+-rw-rw-rw-   0        0        0     3051 2023-04-21 18:35:31.000000 chebyfit-2023.4.22/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 18:35:34.795640 chebyfit-2023.4.22/chebyfit/
+-rw-rw-rw-   0        0        0      104 2020-01-01 02:43:28.000000 chebyfit-2023.4.22/chebyfit/__init__.py
+-rw-rw-rw-   0        0        0    51841 2023-04-21 16:45:21.000000 chebyfit-2023.4.22/chebyfit/chebyfit.c
+-rw-rw-rw-   0        0        0    10123 2023-04-21 16:48:36.000000 chebyfit-2023.4.22/chebyfit/chebyfit.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:35:34.805279 chebyfit-2023.4.22/chebyfit.egg-info/
+-rw-rw-rw-   0        0        0     3986 2023-04-21 18:35:33.000000 chebyfit-2023.4.22/chebyfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-04-21 18:35:34.000000 chebyfit-2023.4.22/chebyfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:35:33.000000 chebyfit-2023.4.22/chebyfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 18:35:33.000000 chebyfit-2023.4.22/chebyfit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-21 18:35:33.000000 chebyfit-2023.4.22/chebyfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:35:33.000000 chebyfit-2023.4.22/chebyfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:35:34.810300 chebyfit-2023.4.22/setup.cfg
+-rw-rw-rw-   0        0        0     2941 2023-04-21 16:44:48.000000 chebyfit-2023.4.22/setup.py
```

### Comparing `chebyfit-2022.9.29/LICENSE` & `chebyfit-2023.4.22/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2008-2022, Christoph Gohlke
+Copyright (c) 2008-2023, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `chebyfit-2022.9.29/PKG-INFO` & `chebyfit-2023.4.22/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chebyfit
-Version: 2022.9.29
+Version: 2023.4.22
 Summary: Fit exponential and harmonic functions using Chebyshev polynomials
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/chebyfit/issues
 Project-URL: Source Code, https://github.com/cgohlke/chebyfit
@@ -12,47 +12,63 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 
 Fit exponential and harmonic functions using Chebyshev polynomials
 ==================================================================
 
 Chebyfit is a Python library that implements the algorithms described in:
 
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.29
+:Version: 2023.4.22
+
+Quickstart
+----------
+
+Install the chebyfit package and all dependencies from the
+`Python Package Index <https://pypi.org/project/chebyfit/>`_::
+
+    python -m pip install -U chebyfit
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/chebyfit>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.4.22
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.29
 
 - Add type hints.
 - Convert to Google style docstrings.
 
 2022.8.26
```

### Comparing `chebyfit-2022.9.29/README.rst` & `chebyfit-2023.4.22/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,45 @@
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.29
+:Version: 2023.4.22
+
+Quickstart
+----------
+
+Install the chebyfit package and all dependencies from the
+`Python Package Index <https://pypi.org/project/chebyfit/>`_::
+
+    python -m pip install -U chebyfit
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/chebyfit>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.4.22
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.29
 
 - Add type hints.
 - Convert to Google style docstrings.
 
 2022.8.26
```

### Comparing `chebyfit-2022.9.29/chebyfit/chebyfit.c` & `chebyfit-2023.4.22/chebyfit/chebyfit.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /* chebyfit.c */
 
 /*
-Copyright (c) 2008-2022, Christoph Gohlke
+Copyright (c) 2008-2023, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -40,15 +40,15 @@
 and tests.\n\
 \n\
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_\n\
 :License: BSD 3-Clause\n\
 :Version: 2022.9.29\n\
 "
 
-#define _VERSION_ "2022.9.29"
+#define _VERSION_ "2023.4.22"
 
 #define WIN32_LEAN_AND_MEAN
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 #include "math.h"
 #include "float.h"
```

### Comparing `chebyfit-2022.9.29/chebyfit/chebyfit.py` & `chebyfit-2023.4.22/chebyfit/chebyfit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # chebyfit.py
 
-# Copyright (c) 2008-2022, Christoph Gohlke
+# Copyright (c) 2008-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -36,28 +36,45 @@
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.29
+:Version: 2023.4.22
+
+Quickstart
+----------
+
+Install the chebyfit package and all dependencies from the
+`Python Package Index <https://pypi.org/project/chebyfit/>`_::
+
+    python -m pip install -U chebyfit
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/chebyfit>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.4.22
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.29
 
 - Add type hints.
 - Convert to Google style docstrings.
 
 2022.8.26
 
@@ -129,15 +146,15 @@
 >>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
 True
 
 """
 
 from __future__ import annotations
 
-__version__ = '2022.9.29'
+__version__ = '2023.4.22'
 
 __all__ = [
     'fit_exponentials',
     'fit_harmonic_decay',
     'chebyshev_forward',
     'chebyshev_invers',
     'chebyshev_norm',
@@ -152,19 +169,15 @@
 except ImportError:
     import _chebyfit  # type: ignore
 
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    try:
-        from numpy.typing import ArrayLike
-    except ImportError:
-        # numpy < 1.20
-        from numpy import ndarray as ArrayLike
+    from numpy.typing import ArrayLike
 
 MAXEXPS = 8
 MAXCOEF = 64
 DEFCOEF = 32
 
 
 def fit_exponentials(
```

### Comparing `chebyfit-2022.9.29/chebyfit.egg-info/PKG-INFO` & `chebyfit-2023.4.22/chebyfit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chebyfit
-Version: 2022.9.29
+Version: 2023.4.22
 Summary: Fit exponential and harmonic functions using Chebyshev polynomials
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/chebyfit/issues
 Project-URL: Source Code, https://github.com/cgohlke/chebyfit
@@ -12,47 +12,63 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 
 Fit exponential and harmonic functions using Chebyshev polynomials
 ==================================================================
 
 Chebyfit is a Python library that implements the algorithms described in:
 
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.29
+:Version: 2023.4.22
+
+Quickstart
+----------
+
+Install the chebyfit package and all dependencies from the
+`Python Package Index <https://pypi.org/project/chebyfit/>`_::
+
+    python -m pip install -U chebyfit
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/chebyfit>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.4.22
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.29
 
 - Add type hints.
 - Convert to Google style docstrings.
 
 2022.8.26
```

### Comparing `chebyfit-2022.9.29/setup.py` & `chebyfit-2023.4.22/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code)
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
-    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}[__version__|from]',
+    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
 
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
@@ -74,30 +74,29 @@
     author_email='cgohlke@cgohlke.com',
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/chebyfit/issues',
         'Source Code': 'https://github.com/cgohlke/chebyfit',
         # 'Documentation': 'https://',
     },
-    python_requires='>=3.8',
-    install_requires=['numpy>=1.19.2'],
-    setup_requires=['setuptools>=18.0', 'numpy>=1.19.2'],
+    python_requires='>=3.9',
+    install_requires=['numpy'],
+    setup_requires=['setuptools', 'numpy'],
     cmdclass={'build_ext': build_ext},
     packages=['chebyfit'],
     ext_modules=[Extension('chebyfit._chebyfit', ['chebyfit/chebyfit.c'])],
     package_data={'chebyfit': ['examples/*.py']},
     zip_safe=False,
     platforms=['any'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: C',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

