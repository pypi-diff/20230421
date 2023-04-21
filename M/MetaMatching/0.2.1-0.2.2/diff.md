# Comparing `tmp/MetaMatching-0.2.1.tar.gz` & `tmp/MetaMatching-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaMatching-0.2.1.tar", last modified: Fri Apr 21 11:46:36 2023, max compression
+gzip compressed data, was "MetaMatching-0.2.2.tar", last modified: Fri Apr 21 12:26:09 2023, max compression
```

## Comparing `MetaMatching-0.2.1.tar` & `MetaMatching-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 11:46:36.160341 MetaMatching-0.2.1/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)     1068 2023-04-21 07:13:05.000000 MetaMatching-0.2.1/LICENSE.txt
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 11:46:36.160341 MetaMatching-0.2.1/MetaMatching/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       69 2023-04-21 11:41:56.000000 MetaMatching-0.2.1/MetaMatching/__init__.py
--rw-rw-r--   0 leqi      (1000) leqi      (1000)     6773 2023-04-21 11:41:44.000000 MetaMatching-0.2.1/MetaMatching/model.py
--rw-rw-r--   0 leqi      (1000) leqi      (1000)    12243 2023-04-21 11:41:35.000000 MetaMatching-0.2.1/MetaMatching/utils.py
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 11:46:36.160341 MetaMatching-0.2.1/MetaMatching.egg-info/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/PKG-INFO
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      314 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/SOURCES.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/dependency_links.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/not-zip-safe
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       84 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/requires.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       13 2023-04-21 11:46:36.000000 MetaMatching-0.2.1/MetaMatching.egg-info/top_level.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 11:46:36.160341 MetaMatching-0.2.1/PKG-INFO
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      115 2023-04-21 07:11:30.000000 MetaMatching-0.2.1/README.rst
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       38 2023-04-21 11:46:36.160341 MetaMatching-0.2.1/setup.cfg
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      699 2023-04-21 11:42:57.000000 MetaMatching-0.2.1/setup.py
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:26:09.569721 MetaMatching-0.2.2/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)     1068 2023-04-21 07:13:05.000000 MetaMatching-0.2.2/LICENSE.txt
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:26:09.569721 MetaMatching-0.2.2/MetaMatching/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       69 2023-04-21 11:41:56.000000 MetaMatching-0.2.2/MetaMatching/__init__.py
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)     6736 2023-04-21 12:24:11.000000 MetaMatching-0.2.2/MetaMatching/model.py
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)    12243 2023-04-21 11:41:35.000000 MetaMatching-0.2.2/MetaMatching/utils.py
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:26:09.569721 MetaMatching-0.2.2/MetaMatching.egg-info/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/PKG-INFO
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      314 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/SOURCES.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/dependency_links.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/not-zip-safe
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       84 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/requires.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       13 2023-04-21 12:26:09.000000 MetaMatching-0.2.2/MetaMatching.egg-info/top_level.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 12:26:09.569721 MetaMatching-0.2.2/PKG-INFO
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      115 2023-04-21 07:11:30.000000 MetaMatching-0.2.2/README.rst
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       38 2023-04-21 12:26:09.569721 MetaMatching-0.2.2/setup.cfg
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      699 2023-04-21 12:25:12.000000 MetaMatching-0.2.2/setup.py
```

### Comparing `MetaMatching-0.2.1/LICENSE.txt` & `MetaMatching-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MetaMatching-0.2.1/MetaMatching/model.py` & `MetaMatching-0.2.2/MetaMatching/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sparse_nn.package.MetaMatching.utils import *
+from utils import *
 import torch.nn as nn
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 import torch.utils.data as Data
 from sklearn.model_selection import train_test_split
 import random
@@ -35,16 +35,14 @@
         self.layer2 = layer2
         
     def forward(self,input):
         out = self.layer1(input)
         out = self.layer2(out)
         return out
     
-    
-
 
 # Define the function for train the model 
 def sparse_nn(expression, target, partition, feature_meta, sparsify_coefficient=0.3, threshold_layer_size=100, 
               num_hidden_layer_neuron_list=[20], drop_out=0.3, random_seed=10, batch_size=32, lr=0.001, weight_decay=0,
               num_epoch=100):
 
     # set the partition to be self-connected
```

### Comparing `MetaMatching-0.2.1/MetaMatching/utils.py` & `MetaMatching-0.2.2/MetaMatching/utils.py`

 * *Files identical despite different names*

### Comparing `MetaMatching-0.2.1/setup.py` & `MetaMatching-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author : Leqi Tian
 # @File : setup.py
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 setup(
     name='MetaMatching',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data',  
     packages=find_packages(),
     author='Leqi Tian',
```

