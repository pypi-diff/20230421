# Comparing `tmp/mFractal-0.0.1a1.tar.gz` & `tmp/mFractal-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mFractal-0.0.1a1.tar", last modified: Tue Mar  9 00:23:06 2021, max compression
+gzip compressed data, was "mFractal-0.0.1a2.tar", last modified: Fri Apr 21 21:26:56 2023, max compression
```

## Comparing `mFractal-0.0.1a1.tar` & `mFractal-0.0.1a2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 00:23:06.467751 mFractal-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (116)     3346 2021-03-09 00:23:06.467751 mFractal-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2560 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 00:23:06.463751 mFractal-0.0.1a1/mFractal/
--rw-r--r--   0 runner    (1001) docker     (116)       40 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/mFractal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4158 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/mFractal/chj.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 00:23:06.463751 mFractal-0.0.1a1/mFractal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3346 2021-03-09 00:23:06.000000 mFractal-0.0.1a1/mFractal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      219 2021-03-09 00:23:06.000000 mFractal-0.0.1a1/mFractal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-09 00:23:06.000000 mFractal-0.0.1a1/mFractal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2021-03-09 00:23:06.000000 mFractal-0.0.1a1/mFractal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-09 00:23:06.467751 mFractal-0.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      677 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 00:23:06.463751 mFractal-0.0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1245 2021-03-09 00:22:57.000000 mFractal-0.0.1a1/tests/test_chj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/mFractal/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/mFractal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/mFractal/chj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/mFractal/sigmoid_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/mFractal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-21 21:26:56.000000 mFractal-0.0.1a2/mFractal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 21:26:56.000000 mFractal-0.0.1a2/mFractal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:26:56.000000 mFractal-0.0.1a2/mFractal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 21:26:56.000000 mFractal-0.0.1a2/mFractal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:26:56.365151 mFractal-0.0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-21 21:26:46.000000 mFractal-0.0.1a2/tests/test_chj.py
```

### Comparing `mFractal-0.0.1a1/PKG-INFO` & `mFractal-0.0.1a2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-Metadata-Version: 2.1
-Name: mFractal
-Version: 0.0.1a1
-Summary: UNKNOWN
-Home-page: https://github.com/lucasfr/mFractal
-Author: Lucas G. S. França, Yujiang Wang, José G V Miranda
-Author-email: lucas.franca@kcl.ac.uk
-License: UNKNOWN
-Description: # mFractal
-        
-        [![pytest](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml/badge.svg)](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml)
-        [![codecov](https://codecov.io/gh/lucasfr/mFractal/branch/main/graph/badge.svg?token=EB7Z9AWZVN)](https://codecov.io/gh/lucasfr/mFractal)
-        ![GitHub](https://img.shields.io/github/license/lucasfr/mFractal)
-        ![PyVers](https://img.shields.io/badge/Python-v3.6_|_v3.7_|_v3.8_|_v3.9-blue)
-        
-        This is a development version of a module for multifractal analyses in Python. It already includes a version of the Chhabra-Jensen method.
-        
-        :warning: Please, use the following article for references of the Chhabra-Jensen function:
-        
-        França, L.G.S., Miranda, J.G.V., Leite, M., Sharma, N.K., Walker, M.C., Lemieux, L. and Wang, Y., 2018. [Fractal and Multifractal Properties of Electrographic Recordings of Human Brain Activity: Towards its Use as a Signal Feature for Machine Learning in Clinical Applications](https://www.frontiersin.org/articles/10.3389/fphys.2018.01767/). Frontiers in Physiology, 9, p.1767. DOI: 10.3389/fphys.2018.01767
-        
-        The code was developed based on the method described in:
-        
-        Chhabra, A. & Jensen, R., 1989. [Direct determination of the f(α) singularity spectrum](http://link.aps.org/doi/10.1103/PhysRevA.40.5284). Physical Review Letters, 62(12), pp.1327–1330.
-        
-        ## LICENSE
-        
-        This software is licensed under an MIT License.
-        
-        Copyright (c) 2021 [Lucas G S França](https://www.lfranca.uk/), [Yujiang Wang](http://xaphire.de/), José G V Miranda.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# mFractal
+
+[![pytest](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml/badge.svg)](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml)
+[![codecov](https://codecov.io/gh/lucasfr/mFractal/branch/main/graph/badge.svg?token=EB7Z9AWZVN)](https://codecov.io/gh/lucasfr/mFractal)
+![GitHub](https://img.shields.io/github/license/lucasfr/mFractal)
+![PyPI](https://img.shields.io/pypi/v/mFractal?color=purple)
+![PyVers](https://img.shields.io/badge/Python-v3.6_|_v3.7_|_v3.8_|_v3.9-blue)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4589625.svg)](https://doi.org/10.5281/zenodo.4589625)
+
+This is a development version of a module for multifractal analyses in Python. It already includes a version of the Chhabra-Jensen method.
+
+:warning: Please, use the following article for references of the Chhabra-Jensen function:
+
+França, L.G.S., Miranda, J.G.V., Leite, M., Sharma, N.K., Walker, M.C., Lemieux, L. and Wang, Y., 2018. [Fractal and Multifractal Properties of Electrographic Recordings of Human Brain Activity: Towards its Use as a Signal Feature for Machine Learning in Clinical Applications](https://www.frontiersin.org/articles/10.3389/fphys.2018.01767/). Frontiers in Physiology, 9, p.1767. DOI: 10.3389/fphys.2018.01767
+
+The code was developed based on the method described in:
+
+Chhabra, A. & Jensen, R., 1989. [Direct determination of the f(α) singularity spectrum](http://link.aps.org/doi/10.1103/PhysRevA.40.5284). Physical Review Letters, 62(12), pp.1327–1330.
+
+If you have any questions or suggestions, please [open an issue in the relevant tab](https://github.com/CoDe-Neuro/dynfc/issues). 
+
+Please do not hesitate to suggest improvements to this module.
+
+## Installation
+
+The easiest way to install mFractal is via pip (PyPI) with the command below.
+
+```
+pip install mFractal
+```
+
+If you would like to specify a version use the following command to install version *0.0.1a1*, for example.
+
+```
+pip install mFractal==0.0.1a1
+```
+
+Alternatively one can clone this repository and add it to a project. For that use the following command.
+
+```
+git clone https://github.com/lucasfr/mFractal/
+```
+
+## LICENSE
+
+This software is licensed under an MIT License.
+
+Copyright (c) 2021 [Lucas G S França](https://www.lfranca.uk/), [Yujiang Wang](http://xaphire.de/), José G V Miranda.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mFractal-0.0.1a1/README.md` & `mFractal-0.0.1a2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,63 @@
+Metadata-Version: 2.1
+Name: mFractal
+Version: 0.0.1a2
+Home-page: https://github.com/lucasfr/mFractal
+Author: Lucas G. S. França, Yujiang Wang, José G V Miranda
+Author-email: lucas.franca@northumbria.ac.uk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mFractal
 
 [![pytest](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml/badge.svg)](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/lucasfr/mFractal/branch/main/graph/badge.svg?token=EB7Z9AWZVN)](https://codecov.io/gh/lucasfr/mFractal)
 ![GitHub](https://img.shields.io/github/license/lucasfr/mFractal)
+![PyPI](https://img.shields.io/pypi/v/mFractal?color=purple)
 ![PyVers](https://img.shields.io/badge/Python-v3.6_|_v3.7_|_v3.8_|_v3.9-blue)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4589625.svg)](https://doi.org/10.5281/zenodo.4589625)
 
 This is a development version of a module for multifractal analyses in Python. It already includes a version of the Chhabra-Jensen method.
 
 :warning: Please, use the following article for references of the Chhabra-Jensen function:
 
 França, L.G.S., Miranda, J.G.V., Leite, M., Sharma, N.K., Walker, M.C., Lemieux, L. and Wang, Y., 2018. [Fractal and Multifractal Properties of Electrographic Recordings of Human Brain Activity: Towards its Use as a Signal Feature for Machine Learning in Clinical Applications](https://www.frontiersin.org/articles/10.3389/fphys.2018.01767/). Frontiers in Physiology, 9, p.1767. DOI: 10.3389/fphys.2018.01767
 
 The code was developed based on the method described in:
 
 Chhabra, A. & Jensen, R., 1989. [Direct determination of the f(α) singularity spectrum](http://link.aps.org/doi/10.1103/PhysRevA.40.5284). Physical Review Letters, 62(12), pp.1327–1330.
 
+If you have any questions or suggestions, please [open an issue in the relevant tab](https://github.com/CoDe-Neuro/dynfc/issues). 
+
+Please do not hesitate to suggest improvements to this module.
+
+## Installation
+
+The easiest way to install mFractal is via pip (PyPI) with the command below.
+
+```
+pip install mFractal
+```
+
+If you would like to specify a version use the following command to install version *0.0.1a1*, for example.
+
+```
+pip install mFractal==0.0.1a1
+```
+
+Alternatively one can clone this repository and add it to a project. For that use the following command.
+
+```
+git clone https://github.com/lucasfr/mFractal/
+```
+
 ## LICENSE
 
 This software is licensed under an MIT License.
 
 Copyright (c) 2021 [Lucas G S França](https://www.lfranca.uk/), [Yujiang Wang](http://xaphire.de/), José G V Miranda.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,8 +72,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `mFractal-0.0.1a1/mFractal/chj.py` & `mFractal-0.0.1a2/mFractal/chj.py`

 * *Files identical despite different names*

### Comparing `mFractal-0.0.1a1/mFractal.egg-info/PKG-INFO` & `mFractal-0.0.1a2/mFractal.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,79 @@
 Metadata-Version: 2.1
 Name: mFractal
-Version: 0.0.1a1
-Summary: UNKNOWN
+Version: 0.0.1a2
 Home-page: https://github.com/lucasfr/mFractal
 Author: Lucas G. S. França, Yujiang Wang, José G V Miranda
-Author-email: lucas.franca@kcl.ac.uk
-License: UNKNOWN
-Description: # mFractal
-        
-        [![pytest](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml/badge.svg)](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml)
-        [![codecov](https://codecov.io/gh/lucasfr/mFractal/branch/main/graph/badge.svg?token=EB7Z9AWZVN)](https://codecov.io/gh/lucasfr/mFractal)
-        ![GitHub](https://img.shields.io/github/license/lucasfr/mFractal)
-        ![PyVers](https://img.shields.io/badge/Python-v3.6_|_v3.7_|_v3.8_|_v3.9-blue)
-        
-        This is a development version of a module for multifractal analyses in Python. It already includes a version of the Chhabra-Jensen method.
-        
-        :warning: Please, use the following article for references of the Chhabra-Jensen function:
-        
-        França, L.G.S., Miranda, J.G.V., Leite, M., Sharma, N.K., Walker, M.C., Lemieux, L. and Wang, Y., 2018. [Fractal and Multifractal Properties of Electrographic Recordings of Human Brain Activity: Towards its Use as a Signal Feature for Machine Learning in Clinical Applications](https://www.frontiersin.org/articles/10.3389/fphys.2018.01767/). Frontiers in Physiology, 9, p.1767. DOI: 10.3389/fphys.2018.01767
-        
-        The code was developed based on the method described in:
-        
-        Chhabra, A. & Jensen, R., 1989. [Direct determination of the f(α) singularity spectrum](http://link.aps.org/doi/10.1103/PhysRevA.40.5284). Physical Review Letters, 62(12), pp.1327–1330.
-        
-        ## LICENSE
-        
-        This software is licensed under an MIT License.
-        
-        Copyright (c) 2021 [Lucas G S França](https://www.lfranca.uk/), [Yujiang Wang](http://xaphire.de/), José G V Miranda.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Platform: UNKNOWN
+Author-email: lucas.franca@northumbria.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mFractal
+
+[![pytest](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml/badge.svg)](https://github.com/lucasfr/mFractal/actions/workflows/python-package.yml)
+[![codecov](https://codecov.io/gh/lucasfr/mFractal/branch/main/graph/badge.svg?token=EB7Z9AWZVN)](https://codecov.io/gh/lucasfr/mFractal)
+![GitHub](https://img.shields.io/github/license/lucasfr/mFractal)
+![PyPI](https://img.shields.io/pypi/v/mFractal?color=purple)
+![PyVers](https://img.shields.io/badge/Python-v3.6_|_v3.7_|_v3.8_|_v3.9-blue)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4589625.svg)](https://doi.org/10.5281/zenodo.4589625)
+
+This is a development version of a module for multifractal analyses in Python. It already includes a version of the Chhabra-Jensen method.
+
+:warning: Please, use the following article for references of the Chhabra-Jensen function:
+
+França, L.G.S., Miranda, J.G.V., Leite, M., Sharma, N.K., Walker, M.C., Lemieux, L. and Wang, Y., 2018. [Fractal and Multifractal Properties of Electrographic Recordings of Human Brain Activity: Towards its Use as a Signal Feature for Machine Learning in Clinical Applications](https://www.frontiersin.org/articles/10.3389/fphys.2018.01767/). Frontiers in Physiology, 9, p.1767. DOI: 10.3389/fphys.2018.01767
+
+The code was developed based on the method described in:
+
+Chhabra, A. & Jensen, R., 1989. [Direct determination of the f(α) singularity spectrum](http://link.aps.org/doi/10.1103/PhysRevA.40.5284). Physical Review Letters, 62(12), pp.1327–1330.
+
+If you have any questions or suggestions, please [open an issue in the relevant tab](https://github.com/CoDe-Neuro/dynfc/issues). 
+
+Please do not hesitate to suggest improvements to this module.
+
+## Installation
+
+The easiest way to install mFractal is via pip (PyPI) with the command below.
+
+```
+pip install mFractal
+```
+
+If you would like to specify a version use the following command to install version *0.0.1a1*, for example.
+
+```
+pip install mFractal==0.0.1a1
+```
+
+Alternatively one can clone this repository and add it to a project. For that use the following command.
+
+```
+git clone https://github.com/lucasfr/mFractal/
+```
+
+## LICENSE
+
+This software is licensed under an MIT License.
+
+Copyright (c) 2021 [Lucas G S França](https://www.lfranca.uk/), [Yujiang Wang](http://xaphire.de/), José G V Miranda.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mFractal-0.0.1a1/setup.py` & `mFractal-0.0.1a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mFractal", 
-    version="0.0.1-a1",
+    version="0.0.1-a2",
     author="Lucas G. S. França, Yujiang Wang, José G V Miranda",
-    author_email="lucas.franca@kcl.ac.uk",
+    author_email="lucas.franca@northumbria.ac.uk",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lucasfr/mFractal",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

### Comparing `mFractal-0.0.1a1/tests/test_chj.py` & `mFractal-0.0.1a2/tests/test_chj.py`

 * *Files identical despite different names*

