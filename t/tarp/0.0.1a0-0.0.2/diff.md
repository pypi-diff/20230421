# Comparing `tmp/tarp-0.0.1a0.tar.gz` & `tmp/tarp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarp-0.0.1a0.tar", last modified: Thu Feb 23 16:14:08 2023, max compression
+gzip compressed data, was "tarp-0.0.2.tar", last modified: Fri Apr 21 14:44:16 2023, max compression
```

## Comparing `tarp-0.0.1a0.tar` & `tarp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-02-23 16:14:08.365068 tarp-0.0.1a0/
--rw-r--r--   0 amcoogan   (501) staff       (20)     1086 2023-02-22 14:16:43.000000 tarp-0.0.1a0/LICENSE
--rw-r--r--   0 amcoogan   (501) staff       (20)     3925 2023-02-23 16:14:08.364934 tarp-0.0.1a0/PKG-INFO
--rw-r--r--   0 amcoogan   (501) staff       (20)     1979 2023-02-23 16:03:38.000000 tarp-0.0.1a0/README.md
--rw-r--r--   0 amcoogan   (501) staff       (20)     1075 2023-02-23 16:02:53.000000 tarp-0.0.1a0/pyproject.toml
--rw-r--r--   0 amcoogan   (501) staff       (20)       38 2023-02-23 16:14:08.365102 tarp-0.0.1a0/setup.cfg
--rw-r--r--   0 amcoogan   (501) staff       (20)       38 2023-02-22 13:56:24.000000 tarp-0.0.1a0/setup.py
-drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-02-23 16:14:08.363224 tarp-0.0.1a0/src/
-drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-02-23 16:14:08.364113 tarp-0.0.1a0/src/tarp/
--rw-r--r--   0 amcoogan   (501) staff       (20)       19 2023-02-22 14:26:00.000000 tarp-0.0.1a0/src/tarp/__init__.py
--rw-r--r--   0 amcoogan   (501) staff       (20)      396 2023-02-22 14:30:09.000000 tarp-0.0.1a0/src/tarp/drp.py
-drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-02-23 16:14:08.364679 tarp-0.0.1a0/src/tarp.egg-info/
--rw-r--r--   0 amcoogan   (501) staff       (20)     3925 2023-02-23 16:14:08.000000 tarp-0.0.1a0/src/tarp.egg-info/PKG-INFO
--rw-r--r--   0 amcoogan   (501) staff       (20)      255 2023-02-23 16:14:08.000000 tarp-0.0.1a0/src/tarp.egg-info/SOURCES.txt
--rw-r--r--   0 amcoogan   (501) staff       (20)        1 2023-02-23 16:14:08.000000 tarp-0.0.1a0/src/tarp.egg-info/dependency_links.txt
--rw-r--r--   0 amcoogan   (501) staff       (20)      119 2023-02-23 16:14:08.000000 tarp-0.0.1a0/src/tarp.egg-info/requires.txt
--rw-r--r--   0 amcoogan   (501) staff       (20)        5 2023-02-23 16:14:08.000000 tarp-0.0.1a0/src/tarp.egg-info/top_level.txt
-drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-02-23 16:14:08.364786 tarp-0.0.1a0/tests/
--rw-r--r--   0 amcoogan   (501) staff       (20)      133 2023-02-23 16:02:23.000000 tarp-0.0.1a0/tests/test_drp.py
+drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-04-21 14:44:16.928155 tarp-0.0.2/
+-rw-r--r--   0 amcoogan   (501) staff       (20)     1086 2023-02-22 14:16:43.000000 tarp-0.0.2/LICENSE
+-rw-r--r--   0 amcoogan   (501) staff       (20)     3759 2023-04-21 14:44:16.927996 tarp-0.0.2/PKG-INFO
+-rw-r--r--   0 amcoogan   (501) staff       (20)     1815 2023-02-27 18:37:17.000000 tarp-0.0.2/README.md
+-rw-r--r--   0 amcoogan   (501) staff       (20)     1028 2023-04-21 14:39:09.000000 tarp-0.0.2/pyproject.toml
+-rw-r--r--   0 amcoogan   (501) staff       (20)       38 2023-04-21 14:44:16.928197 tarp-0.0.2/setup.cfg
+-rw-r--r--   0 amcoogan   (501) staff       (20)       38 2023-02-22 13:56:24.000000 tarp-0.0.2/setup.py
+drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-04-21 14:44:16.925785 tarp-0.0.2/src/
+drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-04-21 14:44:16.926880 tarp-0.0.2/src/tarp/
+-rw-r--r--   0 amcoogan   (501) staff       (20)       19 2023-02-22 14:26:00.000000 tarp-0.0.2/src/tarp/__init__.py
+-rw-r--r--   0 amcoogan   (501) staff       (20)     3394 2023-02-27 18:45:10.000000 tarp-0.0.2/src/tarp/drp.py
+drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-04-21 14:44:16.927546 tarp-0.0.2/src/tarp.egg-info/
+-rw-r--r--   0 amcoogan   (501) staff       (20)     3759 2023-04-21 14:44:16.000000 tarp-0.0.2/src/tarp.egg-info/PKG-INFO
+-rw-r--r--   0 amcoogan   (501) staff       (20)      255 2023-04-21 14:44:16.000000 tarp-0.0.2/src/tarp.egg-info/SOURCES.txt
+-rw-r--r--   0 amcoogan   (501) staff       (20)        1 2023-04-21 14:44:16.000000 tarp-0.0.2/src/tarp.egg-info/dependency_links.txt
+-rw-r--r--   0 amcoogan   (501) staff       (20)      102 2023-04-21 14:44:16.000000 tarp-0.0.2/src/tarp.egg-info/requires.txt
+-rw-r--r--   0 amcoogan   (501) staff       (20)        5 2023-04-21 14:44:16.000000 tarp-0.0.2/src/tarp.egg-info/top_level.txt
+drwxr-xr-x   0 amcoogan   (501) staff       (20)        0 2023-04-21 14:44:16.927684 tarp-0.0.2/tests/
+-rw-r--r--   0 amcoogan   (501) staff       (20)      612 2023-02-27 18:42:23.000000 tarp-0.0.2/tests/test_drp.py
```

### Comparing `tarp-0.0.1a0/LICENSE` & `tarp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarp-0.0.1a0/PKG-INFO` & `tarp-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarp
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Statistical coverage testing in python.
 Author-email: Adam Coogan <dr.adam.coogan@gmail.com>, Pablo Lemos <plemos91@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Adam Coogan & Pablo Lemos]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,37 +36,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # tarp
 
 [![Documentation Status](https://readthedocs.org/projects/tarp/badge/?version=latest)](https://tarp.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://pypi.org/project/caustic/)
+[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://badge.fury.io/py/tarp)
 [![Tests](https://github.com/Ciela-Institute/tarp/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/Ciela-Institute/tarp/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/Ciela-Institute/tarp)](https://app.codecov.io/gh/Ciela-Institute/tarp)
 
 `tarp` is a small python package for performing statistical coverage tests to assess
-the quality of posterior estimators. `tarp` is framework-agnostic: it works with
-posterior estimators and samplers written in numpy, pytorch, jax.
+the quality of posterior estimators.
+<!-- `tarp` is framework-agnostic: it works with posterior estimators and samplers written in numpy, pytorch, jax. -->
 
 `tarp` currently implements the distance to random point (DRP) test introduced
 in [Lemos, Coogan et al 2023](https://arxiv.org/abs/2302.03026), which relies on
 posterior samples.
 
 <!-- An upcoming release will implement the highest posterior density region test (HPDR; see [Hermans, Delaunoy et al 2022](https://arxiv.org/abs/2110.06581) or [Cole et al 2022](https://arxiv.org/abs/2111.08030)), which requires a posterior density estimator. -->
 
 ## Installation
 
-Soon you'll be able to install from PyPI with `pip install tarp`. For now,
-```
-git clone git@github.com:Ciela-Institute/tarp.git
-cd tarp
-pip install .
-```
-will install the `tarp` package.
+`pip install tarp`
 
 ## Contributing
 
 Please reach out to us if you're interested in contributing!
 
 To start, follow the installation instructions, replacing the last line with
 ```bash
```

### Comparing `tarp-0.0.1a0/README.md` & `tarp-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # tarp
 
 [![Documentation Status](https://readthedocs.org/projects/tarp/badge/?version=latest)](https://tarp.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://pypi.org/project/caustic/)
+[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://badge.fury.io/py/tarp)
 [![Tests](https://github.com/Ciela-Institute/tarp/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/Ciela-Institute/tarp/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/Ciela-Institute/tarp)](https://app.codecov.io/gh/Ciela-Institute/tarp)
 
 `tarp` is a small python package for performing statistical coverage tests to assess
-the quality of posterior estimators. `tarp` is framework-agnostic: it works with
-posterior estimators and samplers written in numpy, pytorch, jax.
+the quality of posterior estimators.
+<!-- `tarp` is framework-agnostic: it works with posterior estimators and samplers written in numpy, pytorch, jax. -->
 
 `tarp` currently implements the distance to random point (DRP) test introduced
 in [Lemos, Coogan et al 2023](https://arxiv.org/abs/2302.03026), which relies on
 posterior samples.
 
 <!-- An upcoming release will implement the highest posterior density region test (HPDR; see [Hermans, Delaunoy et al 2022](https://arxiv.org/abs/2110.06581) or [Cole et al 2022](https://arxiv.org/abs/2111.08030)), which requires a posterior density estimator. -->
 
 ## Installation
 
-Soon you'll be able to install from PyPI with `pip install tarp`. For now,
-```
-git clone git@github.com:Ciela-Institute/tarp.git
-cd tarp
-pip install .
-```
-will install the `tarp` package.
+`pip install tarp`
 
 ## Contributing
 
 Please reach out to us if you're interested in contributing!
 
 To start, follow the installation instructions, replacing the last line with
 ```bash
```

### Comparing `tarp-0.0.1a0/pyproject.toml` & `tarp-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [project]
 name = "tarp"
-version = "0.0.1a0"
+version = "0.0.2"
 authors = [
     {name = "Adam Coogan", email = "dr.adam.coogan@gmail.com"},
     {name = "Pablo Lemos", email = "plemos91@gmail.com"},
 ]
 description = "Statistical coverage testing in python."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["bayesian", "coverage", "posterior", "statistics"]
-dependencies = [
-    "jax",
-    "jaxlib",
-    "numpy",
-    "torch",
-]
+dependencies = ["numpy"]
 
 [project.optional-dependencies]
 dev = [
     "build",
     "furo",
     "myst-parser",
     "pip",
```

### Comparing `tarp-0.0.1a0/src/tarp.egg-info/PKG-INFO` & `tarp-0.0.2/src/tarp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarp
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Statistical coverage testing in python.
 Author-email: Adam Coogan <dr.adam.coogan@gmail.com>, Pablo Lemos <plemos91@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Adam Coogan & Pablo Lemos]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,37 +36,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # tarp
 
 [![Documentation Status](https://readthedocs.org/projects/tarp/badge/?version=latest)](https://tarp.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://pypi.org/project/caustic/)
+[![PyPI version](https://badge.fury.io/py/tarp.svg)](https://badge.fury.io/py/tarp)
 [![Tests](https://github.com/Ciela-Institute/tarp/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/Ciela-Institute/tarp/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/Ciela-Institute/tarp)](https://app.codecov.io/gh/Ciela-Institute/tarp)
 
 `tarp` is a small python package for performing statistical coverage tests to assess
-the quality of posterior estimators. `tarp` is framework-agnostic: it works with
-posterior estimators and samplers written in numpy, pytorch, jax.
+the quality of posterior estimators.
+<!-- `tarp` is framework-agnostic: it works with posterior estimators and samplers written in numpy, pytorch, jax. -->
 
 `tarp` currently implements the distance to random point (DRP) test introduced
 in [Lemos, Coogan et al 2023](https://arxiv.org/abs/2302.03026), which relies on
 posterior samples.
 
 <!-- An upcoming release will implement the highest posterior density region test (HPDR; see [Hermans, Delaunoy et al 2022](https://arxiv.org/abs/2110.06581) or [Cole et al 2022](https://arxiv.org/abs/2111.08030)), which requires a posterior density estimator. -->
 
 ## Installation
 
-Soon you'll be able to install from PyPI with `pip install tarp`. For now,
-```
-git clone git@github.com:Ciela-Institute/tarp.git
-cd tarp
-pip install .
-```
-will install the `tarp` package.
+`pip install tarp`
 
 ## Contributing
 
 Please reach out to us if you're interested in contributing!
 
 To start, follow the installation instructions, replacing the last line with
 ```bash
```

