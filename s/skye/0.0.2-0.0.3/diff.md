# Comparing `tmp/skye-0.0.2.tar.gz` & `tmp/skye-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skye-0.0.2.tar", last modified: Thu Apr 20 06:46:09 2023, max compression
+gzip compressed data, was "skye-0.0.3.tar", last modified: Fri Apr 21 01:18:50 2023, max compression
```

## Comparing `skye-0.0.2.tar` & `skye-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.317968 skye-0.0.2/
--rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.2/LICENSE
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-20 06:46:09.317641 skye-0.0.2/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.2/README.md
--rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-20 06:46:09.318059 skye-0.0.2/setup.cfg
--rw-r--r--   0 iosefa     (501) staff       (20)      756 2023-04-20 06:44:05.000000 skye-0.0.2/setup.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.316039 skye-0.0.2/skye/
--rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.2/skye/__init__.py
--rw-r--r--   0 iosefa     (501) staff       (20)     9442 2023-04-20 06:22:51.000000 skye-0.0.2/skye/core.py
--rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.2/skye/utils.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.317310 skye-0.0.2/skye.egg-info/
--rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      182 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/SOURCES.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/dependency_links.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/top_level.txt
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.290155 skye-0.0.3/
+-rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.3/LICENSE
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:18:50.289884 skye-0.0.3/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.3/README.md
+-rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-21 01:18:50.290239 skye-0.0.3/setup.cfg
+-rw-r--r--   0 iosefa     (501) staff       (20)     1036 2023-04-21 01:16:21.000000 skye-0.0.3/setup.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.287733 skye-0.0.3/skye/
+-rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.3/skye/__init__.py
+-rw-r--r--   0 iosefa     (501) staff       (20)     9463 2023-04-21 01:17:17.000000 skye-0.0.3/skye/core.py
+-rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.3/skye/utils.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-21 01:18:50.289532 skye-0.0.3/skye.egg-info/
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      209 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/SOURCES.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/dependency_links.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)      152 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/requires.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-21 01:18:50.000000 skye-0.0.3/skye.egg-info/top_level.txt
```

### Comparing `skye-0.0.2/LICENSE` & `skye-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skye-0.0.2/PKG-INFO` & `skye-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.2
+Version: 0.0.3
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skye-0.0.2/skye/core.py` & `skye-0.0.3/skye/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import random
 import logging
 import warnings
-
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
+import scipy
+
 from IPython.core.display_functions import clear_output
 from tqdm.auto import tqdm
 from math import atan, pi, sqrt
-
-import pandas as pd
-import scipy
 from PIL import Image
 from skimage import io
 from skimage.segmentation import quickshift
 from skimage.segmentation import mark_boundaries
 from skimage.util import img_as_float
 from sklearn.ensemble import RandomForestClassifier
 
@@ -225,16 +224,16 @@
             ax.imshow(mask)
             plt.axis("off")
 
             ax.imshow(mark_boundaries(img, mask))
             plt.axis([x_min, x_max, y_min, y_max])
             plt.show()
 
-            klass = input("Enter class or type 'end' to end.")
-            if klass == 'end':
+            klass = input("Enter class or type 'I give up!' to end.")
+            if klass.lower() == 'i give up!':
                 break
             self.training_classes.loc[len(self.training_classes)] = [klass] + list(
                 self.objects_df.loc[self.objects_df['segment_id'] == i].values[0]
             )[1:]
             if notebook:
                 clear_output(wait=True)
```

### Comparing `skye-0.0.2/skye/utils.py` & `skye-0.0.3/skye/utils.py`

 * *Files identical despite different names*

### Comparing `skye-0.0.2/skye.egg-info/PKG-INFO` & `skye-0.0.3/skye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.2
+Version: 0.0.3
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

