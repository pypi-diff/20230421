# Comparing `tmp/bacteria-0.0.2.tar.gz` & `tmp/bacteria-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.2.tar", last modified: Fri Apr 21 11:07:54 2023, max compression
+gzip compressed data, was "bacteria-0.0.3.tar", last modified: Fri Apr 21 11:17:49 2023, max compression
```

## Comparing `bacteria-0.0.2.tar` & `bacteria-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.931000 bacteria-0.0.2/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:07:54.821000 bacteria-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.345000 bacteria-0.0.2/bacteria/
--rw-rw-rw-   0        0        0      646 2023-04-21 10:41:12.000000 bacteria-0.0.2/bacteria/__init__.py
--rw-rw-rw-   0        0        0   163931 2023-04-21 10:50:06.000000 bacteria-0.0.2/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.791000 bacteria-0.0.2/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:07:54.892000 bacteria-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-04-21 11:07:48.000000 bacteria-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.940000 bacteria-0.0.3/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:17:49.870000 bacteria-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.497000 bacteria-0.0.3/bacteria/
+-rw-rw-rw-   0        0        0      681 2023-04-21 11:17:27.000000 bacteria-0.0.3/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   163931 2023-04-21 10:50:06.000000 bacteria-0.0.3/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 11:16:40.000000 bacteria-0.0.3/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.793000 bacteria-0.0.3/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-21 11:17:49.000000 bacteria-0.0.3/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:17:49.908000 bacteria-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 11:17:38.000000 bacteria-0.0.3/setup.py
```

### Comparing `bacteria-0.0.2/PKG-INFO` & `bacteria-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.2
+Version: 0.0.3
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.2/bacteria/__init__.py` & `bacteria-0.0.3/bacteria/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import sys
 import time
 import shutil
 import graphviz
 import scipy.io
-import matlab.engine
+# import matlab.engine
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from IPython import display
 from scipy.stats import sem
 from natsort import natsorted # pip install natsort
 from bacteria.functions import *
+from bacteria.pipeline import *
 from datetime import date,timedelta
 from matplotlib.lines import Line2D
 from sklearn import preprocessing as pre
 from sklearn.linear_model import LinearRegression
 from scipy.signal import savgol_filter, argrelextrema
 from anytree import Node, RenderTree, PostOrderIter # pip install anytree
```

### Comparing `bacteria-0.0.2/bacteria/functions.py` & `bacteria-0.0.3/bacteria/functions.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.2/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.3/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.2
+Version: 0.0.3
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.2/setup.py` & `bacteria-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.2',      
+    version = '0.0.3',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

