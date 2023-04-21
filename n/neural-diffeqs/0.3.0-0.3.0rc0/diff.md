# Comparing `tmp/neural-diffeqs-0.3.0.tar.gz` & `tmp/neural-diffeqs-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-diffeqs-0.3.0.tar", last modified: Fri Apr 21 20:02:18 2023, max compression
+gzip compressed data, was "neural-diffeqs-0.3.0rc0.tar", last modified: Thu Apr 13 21:24:41 2023, max compression
```

## Comparing `neural-diffeqs-0.3.0.tar` & `neural-diffeqs-0.3.0rc0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:02:18.371047 neural-diffeqs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-21 20:02:18.371047 neural-diffeqs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:02:18.367047 neural-diffeqs-0.3.0/neural_diffeqs/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_latent_potential_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_latent_potential_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_potential_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/_potential_sde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:02:18.371047 neural-diffeqs-0.3.0/neural_diffeqs/core/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_base_latent_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_base_latent_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_diffeq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/neural_diffeqs/core/_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:02:18.367047 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-21 20:02:18.000000 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 20:02:18.000000 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:02:18.000000 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 20:02:18.000000 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 20:02:18.000000 neural-diffeqs-0.3.0/neural_diffeqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:02:18.371047 neural-diffeqs-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-21 20:02:08.000000 neural-diffeqs-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_diffeq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/setup.py
```

### Comparing `neural-diffeqs-0.3.0/LICENSE` & `neural-diffeqs-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/README.md` & `neural-diffeqs-0.3.0rc0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: neural-diffeqs
+Version: 0.3.0rc0
+Summary: Neural differential equations made easy.
+Author: Michael E. Vinyard
+Author-email: mvinyard@broadinstitute.org
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ![neural-diffeqs](/assets/neural-diffeqs.logo.svg)
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/neural_diffeqs.svg)](https://pypi.python.org/pypi/pydk/)
 [![PyPI version](https://badge.fury.io/py/neural_diffeqs.svg)](https://badge.fury.io/py/pydk)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A PyTorch-based library for the instantiation of neural differential equations.
@@ -20,21 +35,9 @@
 ```
 
 ## To-do and/or potential directions:
 * Integration of neural controlled differential equations ([neural CDEs](https://github.com/patrick-kidger/torchcde)).
 * Build SDE-GANs
 * Neural PDEs
 
-## References
-The library builds upon the foundational research and developments in the field. We acknowledge and express our gratitude to the authors of the following key works that have shaped our understanding of neural differential equations and their applications:
-Patrick Kidger, James Foster, Xuechen Li, Harald Oberhauser, Terry Lyons
-
-[[1](https://arxiv.org/abs/2102.03657)] Kidger, P., Foster, J., Li, X., Oberhauser, H., Lyons, T., (**2021**). Neural SDEs as Infinite-Dimensional GANs. *ICML*.
-
-[[2](https://arxiv.org/abs/1806.07366)] Chen, R. T. Q., Rubanova, Y., Bettencourt, J., & Duvenaud, D. K. (**2018**). Neural Ordinary Differential Equations. *Adv Neural Inf Process Sys*.
-
-[[3](https://arxiv.org/abs/1904.01681)] Dupont, E., Doucet, A., & Teh, Y. W. (**2019**). Augmented Neural ODEs. *Adv Neural Inf Process Sys*.
-
-[[4](https://arxiv.org/abs/2202.02435)] Kidger, P. (**2022**) On Neural Differential Equations. arXiv:2202.02435
-
 ---
 **Questions or suggestions**? Open an [issue](https://github.com/mvinyard/neural-diffeqs/issues/new) or send an email to [Michael Vinyard](mailto:mvinyard.ai@gmail.com).
```

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/__init__.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """__init__.py module"""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
-__version__ = "0.3.0"
+__version__ = "0.3.0rc"
 
 
 # -- import subpackages: -------------------------------------------------------
 from . import core
 
 
 # -- import modules: -----------------------------------------------------------
```

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_latent_potential_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_latent_potential_sde.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_neural_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_neural_sde.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_potential_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/_potential_sde.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_base_latent_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_base_latent_sde.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_diffeq.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_diffeq.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_base_neural_sde.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_diffeq_config.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_diffeq_config.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs/core/_potential.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_potential.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/neural_diffeqs.egg-info/SOURCES.txt` & `neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0/setup.py` & `neural-diffeqs-0.3.0rc0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="neural-diffeqs",
-    version="0.3.0",
-    python_requires=">3.9.0",
+    version="0.3.0rc0",
+    python_requires=">3.7.0",
     author="Michael E. Vinyard",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Neural differential equations made easy.",
     packages=setuptools.find_packages(),
@@ -20,13 +20,13 @@
         "numpy==1.22.4",
         "torch>=2.0.0",
         "torch-nets>=0.0.4",
         "torchsde>=0.2.5",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.7",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

