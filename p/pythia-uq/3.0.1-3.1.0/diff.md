# Comparing `tmp/pythia-uq-3.0.1.tar.gz` & `tmp/pythia-uq-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythia-uq-3.0.1.tar", last modified: Thu Feb 16 09:41:14 2023, max compression
+gzip compressed data, was "pythia-uq-3.1.0.tar", last modified: Fri Apr 21 12:19:24 2023, max compression
```

## Comparing `pythia-uq-3.0.1.tar` & `pythia-uq-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/
--rw-rw-r--   0 nando     (1000) nando     (1000)    35076 2022-08-31 13:49:08.000000 pythia-uq-3.0.1/LICENSE.txt
--rw-rw-r--   0 nando     (1000) nando     (1000)     4218 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/PKG-INFO
--rw-rw-r--   0 nando     (1000) nando     (1000)     3789 2023-02-16 09:37:19.000000 pythia-uq-3.0.1/README.md
--rw-rw-r--   0 nando     (1000) nando     (1000)      136 2023-02-16 09:37:19.000000 pythia-uq-3.0.1/pyproject.toml
-drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/pythia/
--rw-rw-r--   0 nando     (1000) nando     (1000)      275 2023-02-16 08:37:12.000000 pythia-uq-3.0.1/pythia/__init__.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     9776 2022-12-09 14:34:41.000000 pythia-uq-3.0.1/pythia/basis.py
--rw-rw-r--   0 nando     (1000) nando     (1000)    12254 2023-01-31 17:36:13.000000 pythia-uq-3.0.1/pythia/chaos.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     7968 2022-12-09 13:19:49.000000 pythia-uq-3.0.1/pythia/index.py
--rw-rw-r--   0 nando     (1000) nando     (1000)    12392 2022-12-09 14:34:41.000000 pythia-uq-3.0.1/pythia/misc.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     2196 2022-12-10 11:15:06.000000 pythia-uq-3.0.1/pythia/parameter.py
--rw-rw-r--   0 nando     (1000) nando     (1000)    50002 2022-12-09 14:34:41.000000 pythia-uq-3.0.1/pythia/sampler.py
-drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/pythia_uq.egg-info/
--rw-rw-r--   0 nando     (1000) nando     (1000)     4218 2023-02-16 09:41:14.000000 pythia-uq-3.0.1/pythia_uq.egg-info/PKG-INFO
--rw-rw-r--   0 nando     (1000) nando     (1000)      454 2023-02-16 09:41:14.000000 pythia-uq-3.0.1/pythia_uq.egg-info/SOURCES.txt
--rw-rw-r--   0 nando     (1000) nando     (1000)        1 2023-02-16 09:41:14.000000 pythia-uq-3.0.1/pythia_uq.egg-info/dependency_links.txt
--rw-rw-r--   0 nando     (1000) nando     (1000)       72 2023-02-16 09:41:14.000000 pythia-uq-3.0.1/pythia_uq.egg-info/requires.txt
--rw-rw-r--   0 nando     (1000) nando     (1000)        7 2023-02-16 09:41:14.000000 pythia-uq-3.0.1/pythia_uq.egg-info/top_level.txt
--rw-rw-r--   0 nando     (1000) nando     (1000)       38 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/setup.cfg
--rw-rw-r--   0 nando     (1000) nando     (1000)      806 2023-02-16 09:37:19.000000 pythia-uq-3.0.1/setup.py
-drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-02-16 09:41:14.486368 pythia-uq-3.0.1/tests/
--rw-rw-r--   0 nando     (1000) nando     (1000)    11961 2022-10-11 08:22:32.000000 pythia-uq-3.0.1/tests/test_basis.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     4852 2022-12-09 13:19:49.000000 pythia-uq-3.0.1/tests/test_chaos.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     3233 2022-11-17 18:59:34.000000 pythia-uq-3.0.1/tests/test_index.py
--rw-rw-r--   0 nando     (1000) nando     (1000)    10620 2022-08-31 13:49:09.000000 pythia-uq-3.0.1/tests/test_misc.py
--rw-rw-r--   0 nando     (1000) nando     (1000)     2142 2022-12-10 11:15:06.000000 pythia-uq-3.0.1/tests/test_parameter.py
--rw-rw-r--   0 nando     (1000) nando     (1000)    20056 2022-11-18 09:56:43.000000 pythia-uq-3.0.1/tests/test_sampler.py
+drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/
+-rw-rw-r--   0 nando     (1000) nando     (1000)    18808 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/LICENSE.Hippocratic-3.0-ECO-MEDIA-MIL.md
+-rw-rw-r--   0 nando     (1000) nando     (1000)     7642 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/LICENSE.LGPL-3.0.md
+-rw-rw-r--   0 nando     (1000) nando     (1000)       51 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/LICENSE.md
+-rw-rw-r--   0 nando     (1000) nando     (1000)     4562 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/PKG-INFO
+-rw-rw-r--   0 nando     (1000) nando     (1000)     4045 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/README.md
+-rw-rw-r--   0 nando     (1000) nando     (1000)      136 2023-02-16 09:37:19.000000 pythia-uq-3.1.0/pyproject.toml
+drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/pythia/
+-rw-rw-r--   0 nando     (1000) nando     (1000)      275 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/__init__.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     9853 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/basis.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)    12331 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/chaos.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     8046 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/index.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)    11941 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/misc.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     2272 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/parameter.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)    50078 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/pythia/sampler.py
+drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/pythia_uq.egg-info/
+-rw-rw-r--   0 nando     (1000) nando     (1000)     4562 2023-04-21 12:19:24.000000 pythia-uq-3.1.0/pythia_uq.egg-info/PKG-INFO
+-rw-rw-r--   0 nando     (1000) nando     (1000)      514 2023-04-21 12:19:24.000000 pythia-uq-3.1.0/pythia_uq.egg-info/SOURCES.txt
+-rw-rw-r--   0 nando     (1000) nando     (1000)        1 2023-04-21 12:19:24.000000 pythia-uq-3.1.0/pythia_uq.egg-info/dependency_links.txt
+-rw-rw-r--   0 nando     (1000) nando     (1000)       72 2023-04-21 12:19:24.000000 pythia-uq-3.1.0/pythia_uq.egg-info/requires.txt
+-rw-rw-r--   0 nando     (1000) nando     (1000)        7 2023-04-21 12:19:24.000000 pythia-uq-3.1.0/pythia_uq.egg-info/top_level.txt
+-rw-rw-r--   0 nando     (1000) nando     (1000)       38 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/setup.cfg
+-rw-rw-r--   0 nando     (1000) nando     (1000)      806 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/setup.py
+drwxrwxr-x   0 nando     (1000) nando     (1000)        0 2023-04-21 12:19:24.471034 pythia-uq-3.1.0/tests/
+-rw-rw-r--   0 nando     (1000) nando     (1000)    11961 2022-10-11 08:22:32.000000 pythia-uq-3.1.0/tests/test_basis.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     4852 2022-12-09 13:19:49.000000 pythia-uq-3.1.0/tests/test_chaos.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     3233 2022-11-17 18:59:34.000000 pythia-uq-3.1.0/tests/test_index.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)    10085 2023-04-21 12:11:22.000000 pythia-uq-3.1.0/tests/test_misc.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)     2142 2022-12-10 11:15:06.000000 pythia-uq-3.1.0/tests/test_parameter.py
+-rw-rw-r--   0 nando     (1000) nando     (1000)    20056 2022-11-18 09:56:43.000000 pythia-uq-3.1.0/tests/test_sampler.py
```

### Comparing `pythia-uq-3.0.1/PKG-INFO` & `pythia-uq-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: pythia-uq
-Version: 3.0.1
-Summary: Toolbox for non-intrusive functional approximation of data via (sparse) general polynomial chaos.
-Home-page: https://gitlab1.ptb.de/pythia/pythia
-Author: Nando Farchmin
-Author-email: nando.farchmin@ptb.de
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ![PyThia Logo Full](logo/logo_full_transparent.png)
 
 # PyThia Uncertainty Quantification Toolbox
 
 The PyThia UQ toolbox uses polynomial chaos surrogates to efficiently generate a surrogate of any (parametric) forward problem.
 The surrogate is fast to evaluate, allows analytical differentiation and has a built-in global sensitivity analysis via Sobol indices.
 Assembling the surrogate is done non-intrusive by least-squares regression, hence only training pairs of parameter realizations and evaluations of the forward problem are required to construct the surrogate.
 No need to compute any nasty interfaces for lagacy code.
 
-
 ## Why the Name?
 
 Pythia was the title of the high priestess of the temple of Apollo in Delphi.
 Hence you could say she used her prophetic abilities to quantify which was uncertain.
 Moreover, the package is written in python, so...
 
 ## Installation
@@ -48,36 +35,43 @@
 
 There is no official related article to cite PyThia yet.
 If you make use of PyThia in a publication, please use the meta data from the `CITATION.cff` file or cite it with a BibTeX entry similar to this:
 ```bibtex
 @software{pythia,
     author = {Farchmin, Nando and Heidenreich, Sebastian},
     title = {PyThia UQ Toolbox},
-    version = {3.0.1},
-    url = {https://pythia-uq.readthedocs.io/en/v3.0.1/},
+    version = {3.1.0},
+    url = {https://pythia-uq.readthedocs.io/en/v3.1.0/},
     year = {2022},
     month = {12}
 }
 ```
 
 ## Want to contribute?
 
 Check out the [contribution guidelines](CONTRIBUTING.md) on how to create issues or file bug reports and feature requests.
 Or ever better start developping the PyThia project yourself after reading the [development guidelines](DEVELOPERS.md).
 
+## License
+This work is dual-licensed under GNU Lesser General Public License v3.0 or later and Hippocratic License 3.0 or later.
+You can choose between one of them if you use this work.
+
+`SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL`
+
+## Funding
+
+The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
+The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
+
 ## References
 
 Here we list the papers that describe concepts implemented in **PyThia** for the interested user.
 In principle **PyThia** uses a (sparse) polynomial chaos expansion to construct a surrogate of any function via least-squares regression.
 We first applied the **PyThia** software package to analyse the sensitivities of a scatterometry experiment [^pythia-scat-A] using global sensitivity analysis via Sobol indices [^sobol-indices].
 We also solved the inverse problem for the same experiment [^pythia-scat-B] via Bayesian inversion.
 To use a minimal but still sufficient amount of random samples for the regression, we integrated weighted least-squares sampling [^wls-sampling] into **PyThia**.
 
 [^pythia-scat-A]: [An efficient approach to global sensitivity analysis and parameter estimation for line gratings](https://arxiv.org/abs/1910.14435)
 [^pythia-scat-B]: [Efficient Bayesian inversion for shape reconstruction of lithography masks](https://arxiv.org/abs/2005.05164)
 [^sobol-indices]: [Global sensitivity analysis using polynomial chaos expansions](https://www.sciencedirect.com/science/article/abs/pii/S0951832007001329)
 [^wls-sampling]: [Optimal weighted least-squares methods](https://arxiv.org/abs/1608.00512)
 
-## Who paid for this?
-
-The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
-The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
```

### Comparing `pythia-uq-3.0.1/README.md` & `pythia-uq-3.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+Metadata-Version: 2.1
+Name: pythia-uq
+Version: 3.1.0
+Summary: Toolbox for non-intrusive functional approximation of data via (sparse) general polynomial chaos.
+Home-page: https://gitlab1.ptb.de/pythia/pythia
+Author: Nando Farchmin
+Author-email: nando.farchmin@ptb.de
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.Hippocratic-3.0-ECO-MEDIA-MIL.md
+License-File: LICENSE.LGPL-3.0.md
+License-File: LICENSE.md
+
 ![PyThia Logo Full](logo/logo_full_transparent.png)
 
 # PyThia Uncertainty Quantification Toolbox
 
 The PyThia UQ toolbox uses polynomial chaos surrogates to efficiently generate a surrogate of any (parametric) forward problem.
 The surrogate is fast to evaluate, allows analytical differentiation and has a built-in global sensitivity analysis via Sobol indices.
 Assembling the surrogate is done non-intrusive by least-squares regression, hence only training pairs of parameter realizations and evaluations of the forward problem are required to construct the surrogate.
 No need to compute any nasty interfaces for lagacy code.
 
-
 ## Why the Name?
 
 Pythia was the title of the high priestess of the temple of Apollo in Delphi.
 Hence you could say she used her prophetic abilities to quantify which was uncertain.
 Moreover, the package is written in python, so...
 
 ## Installation
@@ -36,36 +49,43 @@
 
 There is no official related article to cite PyThia yet.
 If you make use of PyThia in a publication, please use the meta data from the `CITATION.cff` file or cite it with a BibTeX entry similar to this:
 ```bibtex
 @software{pythia,
     author = {Farchmin, Nando and Heidenreich, Sebastian},
     title = {PyThia UQ Toolbox},
-    version = {3.0.1},
-    url = {https://pythia-uq.readthedocs.io/en/v3.0.1/},
+    version = {3.1.0},
+    url = {https://pythia-uq.readthedocs.io/en/v3.1.0/},
     year = {2022},
     month = {12}
 }
 ```
 
 ## Want to contribute?
 
 Check out the [contribution guidelines](CONTRIBUTING.md) on how to create issues or file bug reports and feature requests.
 Or ever better start developping the PyThia project yourself after reading the [development guidelines](DEVELOPERS.md).
 
+## License
+This work is dual-licensed under GNU Lesser General Public License v3.0 or later and Hippocratic License 3.0 or later.
+You can choose between one of them if you use this work.
+
+`SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL`
+
+## Funding
+
+The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
+The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
+
 ## References
 
 Here we list the papers that describe concepts implemented in **PyThia** for the interested user.
 In principle **PyThia** uses a (sparse) polynomial chaos expansion to construct a surrogate of any function via least-squares regression.
 We first applied the **PyThia** software package to analyse the sensitivities of a scatterometry experiment [^pythia-scat-A] using global sensitivity analysis via Sobol indices [^sobol-indices].
 We also solved the inverse problem for the same experiment [^pythia-scat-B] via Bayesian inversion.
 To use a minimal but still sufficient amount of random samples for the regression, we integrated weighted least-squares sampling [^wls-sampling] into **PyThia**.
 
 [^pythia-scat-A]: [An efficient approach to global sensitivity analysis and parameter estimation for line gratings](https://arxiv.org/abs/1910.14435)
 [^pythia-scat-B]: [Efficient Bayesian inversion for shape reconstruction of lithography masks](https://arxiv.org/abs/2005.05164)
 [^sobol-indices]: [Global sensitivity analysis using polynomial chaos expansions](https://www.sciencedirect.com/science/article/abs/pii/S0951832007001329)
 [^wls-sampling]: [Optimal weighted least-squares methods](https://arxiv.org/abs/1608.00512)
 
-## Who paid for this?
-
-The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
-The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
```

### Comparing `pythia-uq-3.0.1/pythia/basis.py` & `pythia-uq-3.1.0/pythia/basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 the domain and distribution (and other degrees of freedom) of the parameter(s).
 
 Currently supported are the following distribution types:
     - uniform
     - normal
     - Gamma
     - Beta
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
 """
 from typing import List, Tuple, Optional, Callable, Union
 import numpy as np
 import scipy.integrate
 import scipy.special
 import pythia as pt
```

### Comparing `pythia-uq-3.0.1/pythia/chaos.py` & `pythia-uq-3.1.0/pythia/chaos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ Sample-based computation of polynomial chaos expansion.
 
 This module provides a class to compute the polynomial chaos approximation of
 an unknown function given via input/output training data pairs via linear
 least-squares regression.
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
 """
 from typing import List, Tuple, Optional, Union
 import psutil
 import warnings
 import numpy as np
 import pythia as pt
```

### Comparing `pythia-uq-3.0.1/pythia/index.py` & `pythia-uq-3.1.0/pythia/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Create, manipulate and store information about multiindices."""
+"""Create, manipulate and store information about multiindices.
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
+"""
 from typing import List, Tuple, Union, Optional
 import itertools
 import numpy as np
 import pythia as pt
 
 
 class IndexSet:
```

### Comparing `pythia-uq-3.0.1/pythia/misc.py` & `pythia-uq-3.1.0/pythia/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,18 @@
-"""Miscellaneous functions to support PyThia core functionality."""
+"""Miscellaneous functions to support PyThia core functionality.
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
+"""
 import os
 import datetime
 import shutil
 import numpy as np
 from typing import List, Tuple, Sequence, Iterator, Optional, Union, Dict
 
 
-def distributionDict() -> Dict:
-    """Set aliases for distribution descriptions.
-
-    .. deprecated:: 2.0.0
-        `distributionDict` will be removed in PyThia 3.0.0.
-
-    Returns
-    -------
-    :
-        Dictionary with aliases for distribution descriptions.
-    """
-    distDict = {}
-    distDict['uniform'] = ['uniform', 'Uniform', 'U']
-    distDict['normal'] = ['normal', 'gauss', 'Gauss', 'gaussian', 'N']
-    distDict['gamma'] = ['gamma', 'Gamma', 'G']
-    distDict['beta'] = ['beta', 'Beta', 'B']
-    return distDict
-
-
 def shiftCoord(x: Union[float, np.ndarray],
                T: Union[np.ndarray, List],
                I: Union[np.ndarray, List]
                ) -> np.ndarray:
     """Shift `x` in interval `T` to interval `I`.
 
     Use an affine transformation to shift points :math:`x` from the interval
```

### Comparing `pythia-uq-3.0.1/pythia/parameter.py` & `pythia-uq-3.1.0/pythia/parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-""" PyThia classes containing Parameter information. """
+"""PyThia classes containing Parameter information.
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
+"""
 from typing import List, Tuple, Optional, Union
 from dataclasses import dataclass
 import numpy as np
 
 
 @dataclass
 class Parameter:
```

### Comparing `pythia-uq-3.0.1/pythia/sampler.py` & `pythia-uq-3.1.0/pythia/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-""" Sampler classes for generating in random samples and PDF evaluations. """
+"""Sampler classes for generating in random samples and PDF evaluations.
+
+SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL
+"""
 from typing import List, Tuple, Union, Callable, Optional
 from abc import ABC, abstractmethod, abstractproperty
 import warnings
 import numpy as np
 import scipy.stats
 from scipy.integrate import quad
 from scipy.special import gamma
```

### Comparing `pythia-uq-3.0.1/pythia_uq.egg-info/PKG-INFO` & `pythia-uq-3.1.0/pythia_uq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pythia-uq
-Version: 3.0.1
+Version: 3.1.0
 Summary: Toolbox for non-intrusive functional approximation of data via (sparse) general polynomial chaos.
 Home-page: https://gitlab1.ptb.de/pythia/pythia
 Author: Nando Farchmin
 Author-email: nando.farchmin@ptb.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE.Hippocratic-3.0-ECO-MEDIA-MIL.md
+License-File: LICENSE.LGPL-3.0.md
+License-File: LICENSE.md
 
 ![PyThia Logo Full](logo/logo_full_transparent.png)
 
 # PyThia Uncertainty Quantification Toolbox
 
 The PyThia UQ toolbox uses polynomial chaos surrogates to efficiently generate a surrogate of any (parametric) forward problem.
 The surrogate is fast to evaluate, allows analytical differentiation and has a built-in global sensitivity analysis via Sobol indices.
 Assembling the surrogate is done non-intrusive by least-squares regression, hence only training pairs of parameter realizations and evaluations of the forward problem are required to construct the surrogate.
 No need to compute any nasty interfaces for lagacy code.
 
-
 ## Why the Name?
 
 Pythia was the title of the high priestess of the temple of Apollo in Delphi.
 Hence you could say she used her prophetic abilities to quantify which was uncertain.
 Moreover, the package is written in python, so...
 
 ## Installation
@@ -48,36 +49,43 @@
 
 There is no official related article to cite PyThia yet.
 If you make use of PyThia in a publication, please use the meta data from the `CITATION.cff` file or cite it with a BibTeX entry similar to this:
 ```bibtex
 @software{pythia,
     author = {Farchmin, Nando and Heidenreich, Sebastian},
     title = {PyThia UQ Toolbox},
-    version = {3.0.1},
-    url = {https://pythia-uq.readthedocs.io/en/v3.0.1/},
+    version = {3.1.0},
+    url = {https://pythia-uq.readthedocs.io/en/v3.1.0/},
     year = {2022},
     month = {12}
 }
 ```
 
 ## Want to contribute?
 
 Check out the [contribution guidelines](CONTRIBUTING.md) on how to create issues or file bug reports and feature requests.
 Or ever better start developping the PyThia project yourself after reading the [development guidelines](DEVELOPERS.md).
 
+## License
+This work is dual-licensed under GNU Lesser General Public License v3.0 or later and Hippocratic License 3.0 or later.
+You can choose between one of them if you use this work.
+
+`SPDX-License-Identifier: LGPL-3.0-or-later OR Hippocratic-3.0-ECO-MEDIA-MIL`
+
+## Funding
+
+The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
+The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
+
 ## References
 
 Here we list the papers that describe concepts implemented in **PyThia** for the interested user.
 In principle **PyThia** uses a (sparse) polynomial chaos expansion to construct a surrogate of any function via least-squares regression.
 We first applied the **PyThia** software package to analyse the sensitivities of a scatterometry experiment [^pythia-scat-A] using global sensitivity analysis via Sobol indices [^sobol-indices].
 We also solved the inverse problem for the same experiment [^pythia-scat-B] via Bayesian inversion.
 To use a minimal but still sufficient amount of random samples for the regression, we integrated weighted least-squares sampling [^wls-sampling] into **PyThia**.
 
 [^pythia-scat-A]: [An efficient approach to global sensitivity analysis and parameter estimation for line gratings](https://arxiv.org/abs/1910.14435)
 [^pythia-scat-B]: [Efficient Bayesian inversion for shape reconstruction of lithography masks](https://arxiv.org/abs/2005.05164)
 [^sobol-indices]: [Global sensitivity analysis using polynomial chaos expansions](https://www.sciencedirect.com/science/article/abs/pii/S0951832007001329)
 [^wls-sampling]: [Optimal weighted least-squares methods](https://arxiv.org/abs/1608.00512)
 
-## Who paid for this?
-
-The development of PyThia UQ Toolbox vers. 1 and 2 has been funded by the German Central Innovation Program (ZIM) No. ZF4014017RR7.
-The development of PyThia UQ Toolbox vers. 3 has been funded by the EMPIR project 20IND04-ATMOC.
```

### Comparing `pythia-uq-3.0.1/setup.py` & `pythia-uq-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythia-uq",
-    version="3.0.1",
+    version="3.1.0",
     author="Nando Farchmin",
     author_email="nando.farchmin@ptb.de",
     description=("Toolbox for non-intrusive functional approximation of data "
                  + "via (sparse) general polynomial chaos."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab1.ptb.de/pythia/pythia",
```

### Comparing `pythia-uq-3.0.1/tests/test_basis.py` & `pythia-uq-3.1.0/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `pythia-uq-3.0.1/tests/test_chaos.py` & `pythia-uq-3.1.0/tests/test_chaos.py`

 * *Files identical despite different names*

### Comparing `pythia-uq-3.0.1/tests/test_index.py` & `pythia-uq-3.1.0/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pythia-uq-3.0.1/tests/test_misc.py` & `pythia-uq-3.1.0/tests/test_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 """ Test pythia.misc module. """
 import pytest
 import numpy as np
 import pythia.misc as misc
 
 
-def test_distributionDict() -> None:
-    """Test distribution dictionary mappings.
-    """
-    dist_dict = misc.distributionDict()
-    assert all(dist in ['uniform', 'Uniform', 'U']
-               for dist in dist_dict["uniform"])
-    assert all(dist in ['normal', 'gauss', 'Gauss', 'gaussian', 'N']
-               for dist in dist_dict["normal"])
-    assert all(dist in ['gamma', 'Gamma', 'G']
-               for dist in dist_dict["gamma"])
-    assert all(dist in ['beta', 'Beta', 'B']
-               for dist in dist_dict["beta"])
-
-
 def test_shiftCoord() -> None:
     """Test affine transformation from one interval to another."""
 
     # normal usecase float input
     assert misc.shiftCoord(0, [-1, 1], [0, 1]) == 0.5
 
     # normal usecase array input
```

### Comparing `pythia-uq-3.0.1/tests/test_parameter.py` & `pythia-uq-3.1.0/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pythia-uq-3.0.1/tests/test_sampler.py` & `pythia-uq-3.1.0/tests/test_sampler.py`

 * *Files identical despite different names*

