# Comparing `tmp/pybefit-0.1.0.tar.gz` & `tmp/pybefit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybefit-0.1.0.tar", last modified: Mon Jan  9 11:29:52 2023, max compression
+gzip compressed data, was "pybefit-0.1.2.tar", last modified: Fri Apr 21 16:37:23 2023, max compression
```

## Comparing `pybefit-0.1.0.tar` & `pybefit-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/
--rw-r--r--   0 dima      (1000) dima      (1000)     1114 2019-07-29 10:22:58.000000 pybefit-0.1.0/LICENSE.md
--rw-r--r--   0 dima      (1000) dima      (1000)      464 2023-01-09 11:29:52.711789 pybefit-0.1.0/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-09 11:17:54.000000 pybefit-0.1.0/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-01-09 11:29:52.711789 pybefit-0.1.0/setup.cfg
--rw-r--r--   0 dima      (1000) dima      (1000)     1388 2023-01-09 11:28:04.000000 pybefit-0.1.0/setup.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.708456 pybefit-0.1.0/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.708456 pybefit-0.1.0/src/pybefit/
--rw-r--r--   0 dima      (1000) dima      (1000)       22 2023-01-09 11:28:51.000000 pybefit-0.1.0/src/pybefit/__init__.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/src/pybefit/agents/
--rwxr-xr-x   0 dima      (1000) dima      (1000)      208 2023-01-09 11:22:22.000000 pybefit-0.1.0/src/pybefit/agents/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     1414 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/agent.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/src/pybefit/agents/jax/
--rw-r--r--   0 dima      (1000) dima      (1000)     6438 2022-06-06 10:00:49.000000 pybefit-0.1.0/src/pybefit/agents/jax/hsmm_ai.py
--rw-r--r--   0 dima      (1000) dima      (1000)      337 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/jax/utils.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/src/pybefit/agents/torch/
--rwxr-xr-x   0 dima      (1000) dima      (1000)    13080 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/torch/active_inference.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    21781 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/torch/bayesian.py
--rw-r--r--   0 dima      (1000) dima      (1000)    22614 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/agents/torch/dynamic_programming.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1191 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/torch/random.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     5247 2022-02-24 12:07:49.000000 pybefit-0.1.0/src/pybefit/agents/torch/rl.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/src/pybefit/inference/
--rwxr-xr-x   0 dima      (1000) dima      (1000)      144 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/inference/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2022-01-10 13:25:33.000000 pybefit-0.1.0/src/pybefit/inference/flat.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/inference/hierarchical.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/inference/infer.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6139 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/inference/mixed.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2022-01-10 13:25:33.000000 pybefit-0.1.0/src/pybefit/inference/nonparametric.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6507 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/inference/regression.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     2916 2022-01-10 13:25:33.000000 pybefit-0.1.0/src/pybefit/simulate.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.711789 pybefit-0.1.0/src/pybefit/tasks/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       59 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/tasks/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     4136 2022-01-10 13:25:33.000000 pybefit-0.1.0/src/pybefit/tasks/bandits.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     2650 2022-01-10 13:25:33.000000 pybefit-0.1.0/src/pybefit/tasks/rev_learning.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3716 2022-08-29 15:32:10.000000 pybefit-0.1.0/src/pybefit/tasks/sat.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-01-09 11:29:52.708456 pybefit-0.1.0/src/pybefit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      464 2023-01-09 11:29:52.000000 pybefit-0.1.0/src/pybefit.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)      939 2023-01-09 11:29:52.000000 pybefit-0.1.0/src/pybefit.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-01-09 11:29:52.000000 pybefit-0.1.0/src/pybefit.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       76 2023-01-09 11:29:52.000000 pybefit-0.1.0/src/pybefit.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-01-09 11:29:52.000000 pybefit-0.1.0/src/pybefit.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/
+-rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.2/LICENSE.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      460 2023-04-21 16:37:23.046908 pybefit-0.1.2/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.2/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-04-21 16:37:23.046908 pybefit-0.1.2/setup.cfg
+-rw-r--r--   0 dima      (1000) dima      (1000)     1375 2023-04-21 16:37:13.000000 pybefit-0.1.2/setup.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.043575 pybefit-0.1.2/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.043575 pybefit-0.1.2/src/pybefit/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.2/src/pybefit/__init__.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)       19 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     1414 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/base.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/jax/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/jax/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/agents/jax/hsmm_ai.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/agents/jax/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/torch/
+-rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/active_inference.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/bayesian.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/dynamic_programming.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/random.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/rl.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/inference/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    10154 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/methods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/models.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5429 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/posteriors.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5904 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/priors.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/regression.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/simulate.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/tasks/
+-rwxr--r--   0 dima      (1000) dima      (1000)       59 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     4136 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/bandits.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     2650 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/rev_learning.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3716 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/sat.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)      460 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)      974 2023-04-21 16:37:23.000000 pybefit-0.1.2/src/pybefit.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/top_level.txt
```

### Comparing `pybefit-0.1.0/LICENSE.md` & `pybefit-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/README.md` & `pybefit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/setup.py` & `pybefit-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,37 +22,38 @@
  'optax',
  'torch',
  'pyro-ppl',
  'pandas',
  'pycm',
  'seaborn',
  'matplotlib',
- 'arviz']
+ 'arviz',
+ 'jupyterthemes',
+ 'jupyter-black']
 
 classifiers = \
 [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10'
 ]
 
 setup_kwargs = {
     'name': 'pybefit',
-    'version': '0.1.0',
+    'version': '0.1.2',
     'description': 'Probabilistic inference for models of behaviour',
     'long_description': 'PyBefit is a Python library for Bayesian analysis of behavioral data. It is based on Pyro/Numpyro a probabilistic programing language, PyTorch, and Jax machine learning libraries.',
-    'author': 'Dimitrije Markovic',
+    'author': 'Dimitrije Marković',
     'author_email': 'dimitrije.markovic@tu-dresden.de',
     'url': 'https://github.com/dimarkov/pybefit',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.11',
+    'python_requires': '>=3.10',
 }
 
 setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybefit-0.1.0/src/pybefit/agents/agent.py` & `pybefit-0.1.2/src/pybefit/agents/base.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit/agents/jax/hsmm_ai.py` & `pybefit-0.1.2/src/pybefit/agents/jax/hsmm_ai.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit/agents/torch/active_inference.py` & `pybefit-0.1.2/src/pybefit/agents/torch/active_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 This module contains active inference agents for various experimental tasks. 
 
 @author: Dimitrije Markovic
 """
 
 import torch
-from torch import zeros, ones, tensor, eye
+from torch import zeros, ones, eye
 
 from torch.distributions import Categorical
 
 from numpy import nan_to_num
 
 from itertools import product
 
-from ..agent import Discrete
+from ..base import Discrete
 
 __all__ = [
         'AIBandits',
 ]
 
 def ntn(x):
     return torch.from_numpy(nan_to_num(x))
```

### Comparing `pybefit-0.1.0/src/pybefit/agents/torch/bayesian.py` & `pybefit-0.1.2/src/pybefit/agents/torch/bayesian.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import warnings
 import torch
 from torch import zeros, ones
 from opt_einsum import contract
 
 from torch.distributions import Categorical
 
-from ..agent import Discrete
+from ..base import Discrete
 
 softplus = torch.nn.functional.softplus
 
 __all__ = [
         'HGFSocInf',
         'SGFSocInf',
         'ExplicitHMM',
```

### Comparing `pybefit-0.1.0/src/pybefit/agents/torch/dynamic_programming.py` & `pybefit-0.1.2/src/pybefit/agents/torch/dynamic_programming.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from torch.distributions import Categorical, Bernoulli
 
 from numpy import nan, ravel_multi_index
 
 from itertools import product
 
-from ..agent import Discrete
+from ..base import Discrete
 
 __all__ = [
         'BIBanditsFlat',
         'BIBanditsDeep',
         'VISAT'
 ]
```

### Comparing `pybefit-0.1.0/src/pybefit/agents/torch/random.py` & `pybefit-0.1.2/src/pybefit/agents/torch/random.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: Dimitrije Markovic
 """
 
 from torch import ones, zeros, arange
 from torch.distributions import Categorical
 
-from ..agent import Discrete
+from ..base import Discrete
 
 __all__ = [
         'Random'
 ]
 
 class Random(Discrete):
     """Agent with discrete number of actions.
```

### Comparing `pybefit-0.1.0/src/pybefit/agents/torch/rl.py` & `pybefit-0.1.2/src/pybefit/agents/torch/rl.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 @author: Dimitrije Markovic
 """
 
 import torch
 from torch import ones, zeros, zeros_like, arange
 from torch.distributions import Categorical
 
-from ..agent import Discrete
+from ..base import Discrete
 
 __all__ = [
         'RLSocInf',
         'RLTempRevLearn'
 ]
 
 softplus = torch.nn.Softplus()
 
 class RLSocInf(Discrete):
-    """Reiforcement learning agent (using Rescorla-Wagner learning rule) for 
+    """Reinforcement learning agent (using Rescorla-Wagner learning rule) for 
     the Social Influence task.
     """
 
     def __init__(self, runs=1, blocks=1, trials=1):
 
         na = 2  # number of actions
         ns = 2  # number of states
```

### Comparing `pybefit-0.1.0/src/pybefit/inference/infer.py` & `pybefit-0.1.2/src/pybefit/inference/methods.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,356 @@
 """This module contains the class that defines the interaction between
 different modules that govern agent's behavior.
 """
+import pyro
+import pyro.infer as pinfer
 
-from tqdm import tqdm
-import pandas as pd
+import numpyro.infer as ninfer
+
+import jax.random as jr
+
+import optax
 import numpy as np
+import pandas as pd
 
-import torch
-from torch import zeros, ones
+from numpyro.optim import optax_to_numpyro
+
+from multipledispatch import dispatch
+
+from tqdm.auto import trange
+
+from pyro import clear_param_store, get_param_store
 
-from pyro import param, clear_param_store, get_param_store
-from pyro.infer import SVI, Trace_ELBO, TraceEnum_ELBO
-from pyro.infer.enum import get_importance_trace
-from pyro.infer.predictive import Predictive
 from pyro.optim import Adam
 
+from .models import NumpyroModel, NumpyroGuide, PyroModel, PyroGuide
+
+adabelief = lambda *args, **kwargs: optax.adabelief(*args, eps=1e-8, eps_root=1e-8, **kwargs)
+
 __all__ = [
-    'Inferrer'
+    'run_svi',
+    'run_nuts',
+    'format_posterior_samples'
 ]
 
-class Inferrer(object):
+default_dict_pyro_svi = dict(
+    enumerate=False,            
+    iter_steps=10000,
+    optim_kwargs={'lr': 1e-3},
+    elbo_kwargs=dict(
+        num_particles=10,
+        vectorize_particles=True
+    ),
+    svi_kwargs=dict(
+        progress_bar=True,
+        stable_update=True
+    ),
+    sample_kwargs=dict(
+        num_samples=100
+    )
+)
+
+# Pyro/Pytorch based models
+@dispatch(PyroModel, PyroGuide, dict, opts=dict)
+def run_svi(model,
+            guide,
+            data,
+            *,
+            opts=default_dict_pyro_svi
+        ):
+    """Perform SVI over free model parameters.
+    """
+
+    clear_param_store()
+
+    if opts['enumerate']:
+        elbo = pinfer.TraceEnum_ELBO(**opts['elbo_kwargs'])
+    else:
+        elbo = pinfer.Trace_ELBO(**opts['elbo_kwargs'])
+    
+    svi = pinfer.SVI(
+        model=model,
+        guide=guide,
+        optim=Adam(opts['optim_kwargs']),
+        loss=elbo
+    )
+
+    loss = []
+    pbar = trange(opts['iter_steps'], position=0)
+    for _ in pbar:
+        loss.append(svi.step(data))
+        pbar.set_description("Mean ELBO %6.2f" % np.mean(loss[-20:]))
+        if np.isnan(loss[-1]):
+            break
+            print('loss returned NAN value')
+
+    param_store = get_param_store()
+    params = {}
+    for name in param_store.get_all_param_names():
+        params[name] = pyro.param(name)
+
+    results = {
+        'loss': loss,
+        'params': params
+    }
+
+    pred = pinfer.Predictive(model, guide=guide, **opts['sample_kwargs'])
+    samples = pred(data)
+
+    return samples, svi, results
+
+
+@dispatch(PyroModel, opts=dict)
+def run_nuts(
+    model,
+    *,
+    opts=dict(
+        num_samples=1000,            
+        num_warmup=100,
+        sampler_kwargs={'kernel': {}, 'mcmc': {}}
+    )
+):
+    """Perform SVI over free model parameters.
+    """
+
+    clear_param_store()
+
+    kernel = pinfer.NUTS(model, **opts['sampler_kwargs']['kernel'])
+    mcmc = pinfer.MCMC(
+        kernel, 
+        opts['num_samples'], 
+        warmup_steps=opts['num_warmup'],
+        **opts['sampler_kwargs']['mcmc']
+    )
+
+    mcmc.run()
+    samples = mcmc.get_samples()
+
+    return samples, mcmc
+
+
+default_dict_numpyro_svi = dict(
+    seed=0,
+    enumerate=False,            
+    iter_steps=10000,
+    optim=None,
+    optim_kwargs={'learning_rate': 1e-3},
+    elbo_kwargs=dict(
+        num_particles=10,
+        max_plate_nesting=1,
+    ),
+    svi_kwargs=dict(
+        progress_bar=True,
+        stable_update=True
+    ),
+    sample_kwargs=dict(
+        num_samples=100
+    )
+)
+
+# Numpyro/Jax based models
+@dispatch(NumpyroModel, NumpyroGuide, dict, opts=dict)
+def run_svi(model,
+            guide,
+            data,
+            *,
+            opts=default_dict_numpyro_svi
+        ):
+    """Estimate posterior over free model parameters using stochastic variational inference.
+    """
+    rng_key = jr.PRNGKey(opts['seed'])
+
+    if opts['enumerate']:
+        elbo = ninfer.TraceEnum_ELBO(**opts['elbo_kwargs'])
+    else:
+        elbo = ninfer.TraceGraph_ELBO(num_particles=opts['elbo_kwargs']['num_particles'])
+    
+    if opts['optim'] is None:
+        optim = optax_to_numpyro(adabelief(**opts['optim_kwargs']))
+    else:
+        optim = optim
+    
+    svi = ninfer.SVI(model, guide, optim, elbo)
+    rng_key, _rng_key = jr.split(rng_key)
+    results = svi.run(
+        _rng_key,
+        opts['iter_steps'],
+        progress_bar=opts['svi_kwargs']['progress_bar'],
+        stable_update=opts['svi_kwargs']['stable_update'],
+        init_state = opts['svi_kwargs'].pop('init_state', None),
+        data=data
+    )
+
+    rng_key, _rng_key = jr.split(rng_key)
+    pred = ninfer.Predictive(model, guide=guide, params=results.params, **opts['sample_kwargs'])
+    samples = pred(_rng_key, data=data)
+
+    return samples, svi, results
+
+default_dict_numpyro_nuts = dict(
+    seed=0,
+    num_samples=1000,            
+    num_warmup=100,
+    sampler_kwargs={
+        'kernel': {}, 
+        'mcmc': dict(progress_bar=True)
+    }
+)
+
+@dispatch(NumpyroModel, dict, opts=dict)
+def run_nuts(
+    model,
+    data,
+    *,
+    opts=default_dict_numpyro_nuts
+):
+    """Estimate posterior over free model parameters using No-U-Turn sampler.
+    """
+    rng_key = jr.PRNGKey(opts['seed'])
+
+    kernel = ninfer.NUTS(model, **opts['sampler_kwargs']['kernel'])
+    mcmc = ninfer.MCMC(
+        kernel,
+        num_warmup=opts['num_warmup'],
+        num_samples=opts['num_samples'], 
+        **opts['sampler_kwargs']['mcmc']
+    )
+
+    rng_key, _rng_key = jr.split(rng_key)
+    mcmc.run(_rng_key, data=data)
+    samples = mcmc.get_samples()
+
+    return samples, mcmc
+
+def format_posterior_samples(labels, samples, transform, *args, **kwargs):
+    """Format samples into DataFrames based on agent transform
+    """
+
+    num_samples, num_agents, num_params = samples['z'].shape
+    assert num_params == len(labels)
+
+    subject_id = np.arange(1,  num_agents + 1)[None].repeat(num_samples, axis=0).reshape(-1)
+
+    agent = transform(samples['z'], *args, **kwargs)
+
+    pars = []
+    for lab in labels:
+        pars.append(np.array(getattr(agent, lab).reshape(-1)))
+        
+    pars_df = pd.DataFrame(data=np.stack(pars, -1), columns=labels)
+    pars_df['subject'] = subject_id
+
+    trans_pars_df = pd.DataFrame(data=samples['z'].reshape(-1, num_params), columns=labels)
+    trans_pars_df['subject'] = subject_id
+
+    return trans_pars_df, pars_df
+
+
+#     def sample_posterior_marginal(self, n_samples=100):
+#         '''Draw posterior samples over descrete variables in the model'''
+#         if self.enumerate:
+#             elbo = TraceEnum_ELBO()
+#             post_discrete_samples = {}
+
+#             pbar = tqdm(range(n_samples), position=0)
+
+#             for n in pbar:
+#                 pbar.set_description("Sample posterior discrete marginal")
+#                 # get marginal posterior over planning depths
+#                 post_sample = elbo.compute_marginals(self.model, self.guide)
+#                 for name in post_sample.keys():
+#                     post_discrete_samples.setdefault(name, [])
+#                     post_discrete_samples[name].append(post_sample[name].probs.detach().clone())
+
+#             for name in post_discrete_samples.keys():
+#                 post_discrete_samples[name] = torch.stack(post_discrete_samples[name]).numpy()
+
+#             return post_discrete_samples
+#         else:
+#             print("No enumerate variables in the model")
+#             return -1
+
+#     def _get_quantiles(self, quantiles):
+#         """
+#         Returns posterior quantiles each latent variable. Example::
+
+#             print(agent.get_quantiles([0.05, 0.5, 0.95]))
+
+#         :param quantiles: A list of requested quantiles between 0 and 1.
+#         :type quantiles: torch.tensor or list
+#         :return: A dict mapping sample site name to a list of quantile values.
+#         :rtype: dict
+#         """
+
+#         raise NotImplementedError
+
+#     def formated_results(self, par_names, labels=None):
+#         """Returns median, 5th and 95th percentile for each parameter and subject.
+#         """
+#         nsub = self.runs
+#         npar = self.npar
+
+#         if labels is None:
+#             labels = par_names
+
+#         quantiles = self._get_quantiles([.05, .5, .95])
+
+#         locs = quantiles['locs'].transpose(dim0=0, dim1=-1).transpose(dim0=1, dim1=-1)
+
+#         if self.fixed_values:
+#             x = zeros(3, nsub, npar)
+#             x[..., self.locs['fixed']] = self.values
+#             x[..., self.locs['free']] = locs.detach()
+#         else:
+#             x = locs.detach()
+
+#         self.agent.set_parameters(x, set_variables=False)
+
+#         par_values = {}
+#         for name in par_names:
+#             values = getattr(self.agent, name)
+#             if values.dim() < 3:
+#                 values = values.unsqueeze(dim=-1)
+#             par_values[name] = values
+
+#         count = {}
+#         percentiles = {}
+#         for name in par_names:
+#             count.setdefault(name, 0)
+#             for lbl in labels:
+#                 if lbl.startswith(name):
+#                     percentiles[lbl] = par_values[name][..., count[name]].numpy().reshape(-1)
+#                     count[name] += 1
+
+#         df_percentiles = pd.DataFrame(percentiles)
+
+#         subjects = torch.arange(1, nsub+1).repeat(3, 1).reshape(-1)
+#         df_percentiles['subjects'] = subjects.numpy()
+
+#         from numpy import tile, array
+#         variables = tile(array(['5th', 'median', '95th']), [nsub, 1]).T.reshape(-1)
+#         df_percentiles['variables'] = variables
+
+#         return df_percentiles.melt(id_vars=['subjects', 'variables'], var_name='parameter')
+
+import torch
+
+def get_log_evidence_per_subject(svi, num_agents, *args, num_particles=100, max_plate_nesting=1, **kwargs):
+    """Return subject specific log model evidence"""
 
-    def __init__(self, agent, stimulus, responses, mask=None, fixed_params=None, enumerate=False):
+    model = svi.model
+    guide = svi.guide
 
-        self.agent = agent  # agent used for computing response probabilities
-        self.stimulus = stimulus  # stimulus and action outcomes presented to each participant
-        self.responses = responses  # measured behavioral data accross all subjects
-        self.nb, self.nt, self.runs = self.responses.shape
-
-        # set a mask for excluding certain responses (e.g. NaN resonses) from
-        # the computations of the log-model evidence and the posterior beliefs over
-        # parameter values
-        if mask is not None:
-            self.notnans = mask
-        else:
-            self.notnans = ones(self.nb, self.nt, self.runs, dtype=torch.bool)
-
-        if fixed_params is not None:
-            n_fixed = len(fixed_params['labels'])
-            self.npar = agent.npar - n_fixed
-
-            self.locs = {}
-            self.locs['fixed'] = fixed_params['labels']
-            self.locs['free'] = list(set(range(agent.npar)) - set(fixed_params['labels']))
-            self.values = fixed_params['values']
-            self.fixed_values = True
-        else:
-            self.npar = agent.npar
-            self.fixed_values = False
-
-        self.enumerate = enumerate
-
-    def model(self):
-        """
-        Full generative model of behavior.
-        """
-        raise NotImplementedError
-
-    def guide(self):
-        """Approximate posterior over model parameters.
-        """
-        raise NotImplementedError
-
-    def infer_posterior(self,
-                        iter_steps=10000,
-                        num_particles=100,
-                        optim_kwargs={'lr': .01}):
-        """Perform SVI over free model parameters.
-        """
-
-        clear_param_store()
-
-        model = self.model
-        guide = self.guide
-        if self.enumerate:
-            elbo = TraceEnum_ELBO(num_particles=num_particles, vectorize_particles=True)
-        else:
-            elbo = Trace_ELBO(num_particles=num_particles, vectorize_particles=True)
-        svi = SVI(model=model,
-                  guide=guide,
-                  optim=Adam(optim_kwargs),
-                  loss=elbo)
-
-        loss = []
-        pbar = tqdm(range(iter_steps), position=0)
-        for step in pbar:
-            loss.append(svi.step())
-            pbar.set_description("Mean ELBO %6.2f" % np.mean(loss[-20:]))
-            if np.isnan(loss[-1]):
-                break
-
-        param_store = get_param_store()
-        parameters = {}
-        for name in param_store.get_all_param_names():
-            parameters[name] = param(name)
-
-        self.parameters = parameters
-        self.loss = loss
-        self.elbo = elbo
-
-    def sample_posterior(self, labels, num_samples=1000):
-        """Generate samples from posterior distribution.
-        """
-        nsub = self.runs
-        npar = self.npar
-        assert npar == len(labels)
-
-        sites = ['sigma', 'mu', 'locs']
-        predict = Predictive(self.model, guide=self.guide, num_samples=num_samples, return_sites=sites, parallel=True)
-        samples = predict()
-
-        subject_id = torch.arange(1, nsub+1).repeat(num_samples, 1).reshape(-1)
-        trans_pars_df = pd.DataFrame(data=samples['locs'].detach().reshape(-1, npar).numpy(), columns=labels)
-        trans_pars_df['subject'] = subject_id.numpy()
-
-        locs = samples['locs'].detach()
-        if self.fixed_values:
-            x = zeros(locs.shape[:-1] + (self.agent.npar,))
-            x[..., self.locs['fixed']] = self.values
-            x[..., self.locs['free']] = locs
-        else:
-            x = locs
-
-        self.agent.set_parameters(x)
-        pars = []
-        for lab in labels:
-            pars.append(getattr(self.agent, lab[2:-1]).reshape(-1).numpy())
-        pars_df = pd.DataFrame(data=np.stack(pars, -1), columns=labels)
-        pars_df['subject'] = subject_id.numpy()
-
-        mu = np.take(samples['mu'].detach().numpy(), 0, axis=-2)
-        sigma = np.take(samples['sigma'].detach().numpy(), 0, axis=-2)
-
-        mu_df = pd.DataFrame(data=mu, columns=labels)
-        sigma_df = pd.DataFrame(data=sigma, columns=labels)
-
-        return (trans_pars_df, pars_df, mu_df, sigma_df)
-
-
-    def sample_posterior_marginal(self, n_samples=100):
-        '''Draw posterior samples over descrete variables in the model'''
-        if self.enumerate:
-            elbo = TraceEnum_ELBO()
-            post_discrete_samples = {}
-
-            pbar = tqdm(range(n_samples), position=0)
-
-            for n in pbar:
-                pbar.set_description("Sample posterior discrete marginal")
-                # get marginal posterior over planning depths
-                post_sample = elbo.compute_marginals(self.model, self.guide)
-                for name in post_sample.keys():
-                    post_discrete_samples.setdefault(name, [])
-                    post_discrete_samples[name].append(post_sample[name].probs.detach().clone())
-
-            for name in post_discrete_samples.keys():
-                post_discrete_samples[name] = torch.stack(post_discrete_samples[name]).numpy()
-
-            return post_discrete_samples
-        else:
-            print("No enumerate variables in the model")
-            return -1
-
-    def _get_quantiles(self, quantiles):
-        """
-        Returns posterior quantiles each latent variable. Example::
-
-            print(agent.get_quantiles([0.05, 0.5, 0.95]))
-
-        :param quantiles: A list of requested quantiles between 0 and 1.
-        :type quantiles: torch.tensor or list
-        :return: A dict mapping sample site name to a list of quantile values.
-        :rtype: dict
-        """
-
-        raise NotImplementedError
-
-    def formated_results(self, par_names, labels=None):
-        """Returns median, 5th and 95th percentile for each parameter and subject.
-        """
-        nsub = self.runs
-        npar = self.npar
-
-        if labels is None:
-            labels = par_names
-
-        quantiles = self._get_quantiles([.05, .5, .95])
-
-        locs = quantiles['locs'].transpose(dim0=0, dim1=-1).transpose(dim0=1, dim1=-1)
-
-        if self.fixed_values:
-            x = zeros(3, nsub, npar)
-            x[..., self.locs['fixed']] = self.values
-            x[..., self.locs['free']] = locs.detach()
-        else:
-            x = locs.detach()
-
-        self.agent.set_parameters(x, set_variables=False)
-
-        par_values = {}
-        for name in par_names:
-            values = getattr(self.agent, name)
-            if values.dim() < 3:
-                values = values.unsqueeze(dim=-1)
-            par_values[name] = values
-
-        count = {}
-        percentiles = {}
-        for name in par_names:
-            count.setdefault(name, 0)
-            for lbl in labels:
-                if lbl.startswith(name):
-                    percentiles[lbl] = par_values[name][..., count[name]].numpy().reshape(-1)
-                    count[name] += 1
-
-        df_percentiles = pd.DataFrame(percentiles)
-
-        subjects = torch.arange(1, nsub+1).repeat(3, 1).reshape(-1)
-        df_percentiles['subjects'] = subjects.numpy()
-
-        from numpy import tile, array
-        variables = tile(array(['5th', 'median', '95th']), [nsub, 1]).T.reshape(-1)
-        df_percentiles['variables'] = variables
-
-        return df_percentiles.melt(id_vars=['subjects', 'variables'], var_name='parameter')
-
-    def get_log_evidence_per_subject(self, *args, num_particles=100, max_plate_nesting=1, **kwargs):
-        """Return subject specific log model evidence"""
-
-        model = self.model
-        guide = self.guide
-
-        elbo = zeros(self.runs)
-        for i in range(num_particles):
-            model_trace, guide_trace = get_importance_trace('flat', max_plate_nesting, model, guide, args, kwargs)
-            for site in model_trace.nodes.values():
-                if site['name'].startswith('obs'):
-                    elbo += site['log_prob'].detach()
-                elif site['name'] == 'locs':
-                    elbo += site['log_prob'].detach()
-
-            for site in guide_trace.nodes.values():
-                if site['name'] == 'locs':
-                    elbo -= site['log_prob'].detach()
+    elbo = torch.zeros(num_agents)
+    for i in range(num_particles):
+        model_trace, guide_trace = pyro.infer.enum.get_importance_trace('flat', max_plate_nesting, model, guide, args, kwargs)
+        for site in model_trace.nodes.values():
+            if site['name'].startswith('obs'):
+                elbo += site['log_prob'].detach()
+            elif site['name'] == 'locs':
+                elbo += site['log_prob'].detach()
+
+        for site in guide_trace.nodes.values():
+            if site['name'] == 'locs':
+                elbo -= site['log_prob'].detach()
 
-        return elbo/num_particles
+    return elbo/num_particles
```

### Comparing `pybefit-0.1.0/src/pybefit/inference/mixed.py` & `pybefit-0.1.2/src/pybefit/inference/regression.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,176 @@
-"""This module contains the hierarchical parametric model with 
-descrete variables.
-"""
-
-import torch
-from torch import zeros, ones
-from torch.distributions import biject_to
-
-import pyro.distributions as dist
-from pyro.distributions import constraints
-from pyro import sample, param, poutine, deterministic, plate, markov
-from pyro.distributions.util import sum_rightmost
-from pyro.ops.indexing import Vindex
-from pyro.infer.reparam import LocScaleReparam
-
-from .infer import Inferrer
-
-__all__ = [
-    'NormalGammaDiscreteDepth'
-]
-
-
-class NormalGammaDiscreteDepth(Inferrer):
-    def __init__(self,
-                 agent,
-                 stimulus,
-                 responses,
-                 mask):
-
-        super(NormalGammaDiscreteDepth, self).__init__(
-            agent, 
-            stimulus, 
-            responses, 
-            mask=mask, 
-            fixed_params=None,
-            enumerate=True)
-
-        self.agent = agent
-        self.mask = mask
-        self.N = mask.sum(dim=0)
-
-        self.subs = torch.arange(0, self.runs, 1, dtype=torch.long) # helper variable for indexing
-
-        self.depth_transition = zeros(2, 3, 2, 3)
-        self.depth_transition[0, :, 0] = torch.tensor([1., 0., 0.])
-        self.depth_transition[0, :, 1] = torch.tensor([.5, .5, 0.])
-        self.depth_transition[1] = torch.tensor([1., 0., 0.])
-
-        self.states = stimulus['states']
-        self.configs = stimulus['configs']
-        self.conditions = stimulus['conditions']
-
-    def model(self):
-        agent = self.agent
-        np = agent.npar  # number of parameters
-
-        nblk = self.nb  # number of mini-blocks
-        nsub = self.runs  # number of subjects
-
-        # define prior uncertanty over model parameters and subjects
-        a = param('a', ones(np), constraint=constraints.softplus_positive)
-        lam = param('lam', ones(np), constraint=constraints.softplus_positive)
-        var_tau = sample('var_tau', dist.Gamma(a, 1).to_event(1))
-
-        sig = deterministic('sigma', torch.sqrt(lam/(a*var_tau)))
-
-        # each model parameter has a hyperprior defining group level mean
-        m = param('m', zeros(np))
-        s = param('s', ones(np), constraint=constraints.softplus_positive)
-        with poutine.reparam(config={"mu": LocScaleReparam()}):
-            mu = sample("mu", dist.Normal(m, s*sig).to_event(1))
-
-        ac12 = param("alphas12", ones(2, 2), constraint=constraints.softplus_positive)
-        ac34 = param("alphas34", ones(2, 3), constraint=constraints.softplus_positive)
-
-        with plate('subjects', nsub):
-            with poutine.reparam(config={"locs": LocScaleReparam()}):
-                locs = sample("locs", dist.Normal(mu, sig).to_event(1))
+import jax.numpy as jnp
+import jax.random as random
+import numpyro.distributions as dist
+
+
+from jax import lax, vmap
+from jax.nn import logsumexp
+from numpyro.distributions import constraints
+from numpyro import handlers, sample, deterministic, plate
+from numpyro.infer import MCMC, NUTS, Predictive, init_to_feasible, log_likelihood
+from numpyro.infer.reparam import TransformReparam
+from numpyro.distributions.transforms import Transform, AffineTransform, ComposeTransform
+
+#TODO: Make the regression work for both Pyro and Numpyro backends
+
+class QRTransform(Transform):
+    domain = constraints.real_vector
+    codomain = constraints.real_vector
+
+    def __init__(self, R, R_inv):
+        self.R = R
+        self.R_inv = R_inv
+
+    def __call__(self, x):
+        return jnp.squeeze(
+            jnp.matmul(self.R, x[..., jnp.newaxis]), axis=-1
+        )
+
+    def _inverse(self, y):
+        return jnp.squeeze(
+            jnp.matmul(self.R_inv, y[..., jnp.newaxis]), axis=-1
+        )
+
+    def log_abs_det_jacobian(self, x, y, intermediates=None):
+        return jnp.broadcast_to(
+            jnp.log(jnp.diagonal(self.R, axis1=-2, axis2=-1)).sum(-1),
+            jnp.shape(x)[:-1],
+        )
+
+    def forward_shape(self, shape):
+        if len(shape) < 1:
+            raise ValueError("Too few dimensions on input")
+        return lax.broadcast_shapes(shape, self.R.shape[:-1])
+
+    def inverse_shape(self, shape):
+        if len(shape) < 1:
+            raise ValueError("Too few dimensions on input")
+        return lax.broadcast_shapes(shape, self.R.shape[:-1])
+
+class BayesRegression(object):
+    def __init__(self, rng_key, X, tau=1., p0=None, fixed_lam=False, with_qr=True, reg_type='linear'):
+        self.batch, self.N, self.D = X.shape
+        self.X = X
+        self.rng_key = rng_key
+        self.tau = tau
+        self.fixed_lam = fixed_lam
+        self.with_qr = with_qr
+        self.p0 = p0
+        self.type = reg_type # type of the rergression problem
+        
+        if self.with_qr:
+            # use QR decomposition
+            self.Q, self.R = vmap(jnp.linalg.qr)(X)
+            self.R_inv = vmap(jnp.linalg.inv)(self.R)
+        
+    def model(self, obs=None):
+
+        if self.batch > 1:
+            a = sample('a', dist.InverseGamma(1/2, 1/2))
+            b = sample('b', dist.InverseGamma(1/2, 1/2))
+
+            s = sample('s', dist.Exponential(jnp.ones(self.D)).to_event(1))
+            m = sample('m', dist.Normal(jnp.zeros(self.D), 1.).to_event(1))
+
+            if self.p0 is None:
+                rho = sample('rho', dist.Beta(1., 1.))
+                p0 = deterministic('p0', 1 + (self.D - 1) * rho)
+            else:
+                p0 = self.p0
+        else:
+            a = 2.
+            b = 2.
+            m = 0.
+            s = 1.
+
+            if self.p0 is None:
+                p0 = self.D
+            else:
+                p0 = self.p0
+        
+        gb = deterministic('group_beta', m * s)
+                
+        with plate('batch', self.batch):
+            sigma_sqr = sample('var_sigma^2', dist.InverseGamma(a, 1.))
+            sigma = deterministic('sigma', jnp.sqrt(b * sigma_sqr))
             
-            # define priors over planning depth
-            probs_c12 = sample("probs_cond_12", dist.Dirichlet(ac12).to_event(1))
-            probs_c34 = sample("probs_cond_34", dist.Dirichlet(ac34).to_event(1))
-
-        agent.set_parameters(locs)
-
-        tmp = torch.nn.functional.pad(probs_c12, (0, 1), value=0.)
-        priors = torch.concat([tmp, probs_c34], -2)
-
-        for b in markov(range(nblk)):
-            conditions = self.conditions[..., b]
-            states = self.states[:, b]
-            responses = self.responses[b]
-            max_trials = conditions[-1] - 2
-            noise = conditions[-2]
-
-            tm = self.depth_transition[:, :, max_trials]
-            for t in markov(range(3)):
-
-                if t == 0:
-                    res = None
-                    probs = priors[..., self.subs, 2*max_trials + noise, :]
-                else:
-                    res = responses[t-1]
-                    probs = tm[t-1, -1]
-
-                agent.update_beliefs(b, t, states[:, t], conditions, res)
-                agent.plan_actions(b, t)
-
-                valid = self.mask[:, b, t]
-                N = self.N[b, t]
-                res = responses[t, valid]
-
-                logits = agent.logits[-1][..., valid, :]
-                probs = probs[..., valid, :]
-
-                if t == 2:
-                    agent.update_beliefs(b, t + 1, states[:, t + 1], conditions, responses[t])
-
-                if N > 0:
-                    with plate('responses_{}_{}'.format(b, t), N):
-                        d = sample('d_{}_{}'.format(b, t),
-                                   dist.Categorical(probs),
-                                   infer={"enumerate": "parallel"})
-
-                        sample('obs_{}_{}'.format(b, t),
-                               dist.Bernoulli(logits=Vindex(logits)[..., d]),
-                               obs=res)
-
-    def guide(self):
-        npar = self.agent.npar  # number of parameters
-        nsub = self.runs  # number of subjects
-
-        m_hyp = param('m_hyp', zeros(2*npar))
-        st_hyp = param('scale_tril_hyp',
-                       torch.eye(2*npar),
-                       constraint=constraints.lower_cholesky)
-        hyp = sample('hyp', dist.MultivariateNormal(m_hyp, scale_tril=st_hyp),
-                     infer={'is_auxiliary': True})
-
-        unc_mu = hyp[..., :npar]
-        unc_tau = hyp[..., npar:]
-
-        trns_tau = biject_to(constraints.softplus_positive)
-
-        c_tau = trns_tau(unc_tau)
-
-        ld_tau = trns_tau.inv.log_abs_det_jacobian(c_tau, unc_tau)
-        ld_tau = sum_rightmost(ld_tau, ld_tau.dim() - c_tau.dim() + 1)
-
-        sample("mu_decentered", dist.Delta(unc_mu, event_dim=1))
-        sample("var_tau", dist.Delta(c_tau, log_density=ld_tau, event_dim=1))
-
-        m_locs = param('m_locs', zeros(nsub, npar))
-        st_locs = param('s_locs', torch.eye(npar).repeat(nsub, 1, 1),
-                        constraint=constraints.lower_cholesky)
-
-        alpha_12 = param('guide_alpha12', ones(nsub, 2, 2), constraint=constraints.softplus_positive)
-        alpha_34 = param('guide_alpha34', ones(nsub, 2, 3), constraint=constraints.softplus_positive)
-
-        with plate('subjects', nsub):
-            sample("locs_decentered", dist.MultivariateNormal(m_locs, scale_tril=st_locs))
-            sample("probs_cond_12", dist.Dirichlet(alpha_12).to_event(1))
-            sample("probs_cond_34", dist.Dirichlet(alpha_34).to_event(1))
+            tau0 = self.tau * p0 * sigma / ((self.D + 1 - p0) * jnp.sqrt(self.N))
+            var_tau = sample('var_tau', dist.HalfCauchy(1.))
+            tau = deterministic('tau', tau0 * var_tau)
+
+            if self.fixed_lam:
+                lam = deterministic('lam', jnp.ones(self.D))
+            else:
+                lam = sample('lam', dist.HalfCauchy(1.).expand([self.D]).to_event(1))
+
+            if self.with_qr:
+                rt = QRTransform(self.R, self.R_inv)
+                aff = AffineTransform(gb, jnp.expand_dims(tau, -1) * lam)
+                ct = ComposeTransform([aff, rt])
+                with handlers.reparam(config={"theta": TransformReparam()}):
+                    theta = sample(
+                        'theta', 
+                        dist.TransformedDistribution(dist.Normal(0., 1.).expand([self.D]).to_event(1), ct)
+                    )
+
+                deterministic('beta', rt.inv(theta))
+                tmp = jnp.squeeze(jnp.matmul(self.Q, theta[..., jnp.newaxis]), axis=-1)
+
+            else:
+                aff = AffineTransform(0., jnp.expand_dims(tau, -1) * lam)
+                with handlers.reparam(config={"beta": TransformReparam()}):
+                    beta = sample(
+                        'beta', 
+                        dist.TransformedDistribution(dist.Normal(0., 1.).expand([self.D]).to_event(1), aff)
+                    )
+                tmp = jnp.squeeze(jnp.matmul(self.X, beta[..., jnp.newaxis]), axis=-1)
+
+            alpha = sample('alpha', dist.Normal(0., 10.))
+            mu = deterministic('mu', jnp.expand_dims(alpha, -1) + tmp)
+            
+            with plate('data', self.N):
+                if self.type == 'linear':
+                    sample('obs', dist.Normal(mu.T, sigma), obs=obs)
+                elif self.type == 'logistic':
+                    sample('obs', dist.Bernoulli(logits=mu.T), obs=obs)
+                elif self.type == 'possion':
+                    sample('obs', dist.Poisson(jnp.exp(mu.T)), obs=obs)
+    
+    def fit(self, data, num_samples=1000, warmup_steps=1000, num_chains=1, summary=True, progress_bar=True):
+        self.rng_key, _rng_key = random.split(self.rng_key)
+
+        nuts_kernel = NUTS(self.model, init_strategy=init_to_feasible)
+        mcmc = MCMC(nuts_kernel, 
+                    num_warmup=warmup_steps, 
+                    num_samples=num_samples, 
+                    num_chains=num_chains,
+                    chain_method='vectorized',
+                    progress_bar=progress_bar)
+        mcmc.run(_rng_key, obs=data)
+
+        if summary:
+            mcmc.print_summary()
+
+        samples = mcmc.get_samples(group_by_chain=False)
+        self.mcmc = mcmc
+        self.samples = samples
+
+        return samples
+
+    def predictions(self, rng_key, num_samples=1):
+        predictive = Predictive(self.model, self.samples, num_samples=num_samples)
+
+        return predictive.get_samples(rng_key)['obs']
+
+    def waic(self, data):
+        '''Widely applicable information criterion: 
+        Watanabe, Sumio. "A widely applicable Bayesian information criterion." Journal of Machine Learning Research 14.27 (2013): 867-897.
+        '''
+        log_lk = log_likelihood(self.model, self.samples, obs=data)['obs']
+        
+        S = log_lk.shape[0]
+
+        T = logsumexp(log_lk, 0) - jnp.log(S)
+        V = jnp.square(log_lk).mean(0) - jnp.square(log_lk.mean(0))
+
+        return - T.mean(0) + V.mean(0)
```

### Comparing `pybefit-0.1.0/src/pybefit/simulate.py` & `pybefit-0.1.2/src/pybefit/simulate.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit/tasks/bandits.py` & `pybefit-0.1.2/src/pybefit/tasks/bandits.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit/tasks/rev_learning.py` & `pybefit-0.1.2/src/pybefit/tasks/rev_learning.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit/tasks/sat.py` & `pybefit-0.1.2/src/pybefit/tasks/sat.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.0/src/pybefit.egg-info/SOURCES.txt` & `pybefit-0.1.2/src/pybefit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 src/pybefit/simulate.py
 src/pybefit.egg-info/PKG-INFO
 src/pybefit.egg-info/SOURCES.txt
 src/pybefit.egg-info/dependency_links.txt
 src/pybefit.egg-info/requires.txt
 src/pybefit.egg-info/top_level.txt
 src/pybefit/agents/__init__.py
-src/pybefit/agents/agent.py
+src/pybefit/agents/base.py
+src/pybefit/agents/jax/__init__.py
 src/pybefit/agents/jax/hsmm_ai.py
 src/pybefit/agents/jax/utils.py
+src/pybefit/agents/torch/__init__.py
 src/pybefit/agents/torch/active_inference.py
 src/pybefit/agents/torch/bayesian.py
 src/pybefit/agents/torch/dynamic_programming.py
 src/pybefit/agents/torch/random.py
 src/pybefit/agents/torch/rl.py
 src/pybefit/inference/__init__.py
-src/pybefit/inference/flat.py
-src/pybefit/inference/hierarchical.py
-src/pybefit/inference/infer.py
-src/pybefit/inference/mixed.py
-src/pybefit/inference/nonparametric.py
+src/pybefit/inference/methods.py
+src/pybefit/inference/models.py
+src/pybefit/inference/posteriors.py
+src/pybefit/inference/priors.py
 src/pybefit/inference/regression.py
 src/pybefit/tasks/__init__.py
 src/pybefit/tasks/bandits.py
 src/pybefit/tasks/rev_learning.py
 src/pybefit/tasks/sat.py
```

