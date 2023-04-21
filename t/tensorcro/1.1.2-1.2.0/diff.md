# Comparing `tmp/tensorcro-1.1.2.tar.gz` & `tmp/tensorcro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcro-1.1.2.tar", last modified: Thu Apr 20 20:39:31 2023, max compression
+gzip compressed data, was "tensorcro-1.2.0.tar", last modified: Fri Apr 21 10:33:49 2023, max compression
```

## Comparing `tensorcro-1.1.2.tar` & `tensorcro-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.393387 tensorcro-1.1.2/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       43 2023-04-20 20:15:01.000000 tensorcro-1.1.2/MANIFEST.in
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     4964 2023-04-20 20:39:31.393387 tensorcro-1.1.2/PKG-INFO
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     4045 2023-04-20 20:37:28.000000 tensorcro-1.1.2/README.md
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       97 2023-03-13 09:28:19.000000 tensorcro-1.1.2/pyproject.toml
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       74 2023-04-20 20:39:31.393387 tensorcro-1.1.2/setup.cfg
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2197 2023-04-20 20:36:47.000000 tensorcro-1.1.2/setup.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.389387 tensorcro-1.1.2/src/
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.389387 tensorcro-1.1.2/src/tensorcro/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      883 2023-04-20 17:46:24.000000 tensorcro-1.1.2/src/tensorcro/__init__.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      693 2023-04-18 22:50:13.000000 tensorcro-1.1.2/src/tensorcro/__special__.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.389387 tensorcro-1.1.2/src/tensorcro/replay/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      599 2023-04-19 16:21:28.000000 tensorcro-1.1.2/src/tensorcro/replay/__init__.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     6591 2023-04-20 16:47:26.000000 tensorcro-1.1.2/src/tensorcro/replay/watch_replay.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)    17389 2023-04-20 19:52:44.000000 tensorcro-1.1.2/src/tensorcro/slcro.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.389387 tensorcro-1.1.2/src/tensorcro/substrates/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      821 2023-04-20 15:27:11.000000 tensorcro-1.1.2/src/tensorcro/substrates/__init__.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.393387 tensorcro-1.1.2/src/tensorcro/substrates/algorithms/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      694 2023-04-20 14:47:19.000000 tensorcro-1.1.2/src/tensorcro/substrates/algorithms/__init__.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1575 2023-04-20 18:31:39.000000 tensorcro-1.1.2/src/tensorcro/substrates/algorithms/differential_search.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1827 2023-04-20 18:42:15.000000 tensorcro-1.1.2/src/tensorcro/substrates/algorithms/harmony_search.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1427 2023-04-20 18:40:44.000000 tensorcro-1.1.2/src/tensorcro/substrates/algorithms/random_search.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.393387 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      808 2023-04-19 14:45:24.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/__init__.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1521 2023-04-20 18:31:02.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/blxalpha_crossover.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1445 2023-04-20 18:31:02.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/gaussian_crossover.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1430 2023-04-19 14:12:20.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/masked_crossover.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1606 2023-04-20 18:31:02.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/multipoint_crossover.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1230 2023-04-19 14:12:20.000000 tensorcro-1.1.2/src/tensorcro/substrates/crossovers/uniform_crossover.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1591 2023-04-20 15:19:13.000000 tensorcro-1.1.2/src/tensorcro/substrates/mutation.py
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1474 2023-04-20 15:19:13.000000 tensorcro-1.1.2/src/tensorcro/substrates/substrate.py
-drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-20 20:39:31.389387 tensorcro-1.1.2/src/tensorcro.egg-info/
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     4964 2023-04-20 20:39:31.000000 tensorcro-1.1.2/src/tensorcro.egg-info/PKG-INFO
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1096 2023-04-20 20:39:31.000000 tensorcro-1.1.2/src/tensorcro.egg-info/SOURCES.txt
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)        1 2023-04-20 20:39:31.000000 tensorcro-1.1.2/src/tensorcro.egg-info/dependency_links.txt
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       87 2023-04-20 20:39:31.000000 tensorcro-1.1.2/src/tensorcro.egg-info/requires.txt
--rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       10 2023-04-20 20:39:31.000000 tensorcro-1.1.2/src/tensorcro.egg-info/top_level.txt
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.293500 tensorcro-1.2.0/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       43 2023-04-20 20:15:01.000000 tensorcro-1.2.0/MANIFEST.in
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     5412 2023-04-21 10:33:49.293500 tensorcro-1.2.0/PKG-INFO
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     4493 2023-04-21 10:18:12.000000 tensorcro-1.2.0/README.md
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       97 2023-03-13 09:28:19.000000 tensorcro-1.2.0/pyproject.toml
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       74 2023-04-21 10:33:49.293500 tensorcro-1.2.0/setup.cfg
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2197 2023-04-21 10:20:58.000000 tensorcro-1.2.0/setup.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.289500 tensorcro-1.2.0/src/
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.289500 tensorcro-1.2.0/src/tensorcro/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      883 2023-04-20 17:46:24.000000 tensorcro-1.2.0/src/tensorcro/__init__.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      693 2023-04-18 22:50:13.000000 tensorcro-1.2.0/src/tensorcro/__special__.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.289500 tensorcro-1.2.0/src/tensorcro/replay/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      599 2023-04-19 16:21:28.000000 tensorcro-1.2.0/src/tensorcro/replay/__init__.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     6593 2023-04-21 09:24:47.000000 tensorcro-1.2.0/src/tensorcro/replay/watch_replay.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)    17730 2023-04-21 09:24:47.000000 tensorcro-1.2.0/src/tensorcro/slcro.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.289500 tensorcro-1.2.0/src/tensorcro/substrates/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      835 2023-04-21 09:04:38.000000 tensorcro-1.2.0/src/tensorcro/substrates/__init__.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.293500 tensorcro-1.2.0/src/tensorcro/substrates/algorithms/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      694 2023-04-20 14:47:19.000000 tensorcro-1.2.0/src/tensorcro/substrates/algorithms/__init__.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2345 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/algorithms/differential_search.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2729 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/algorithms/harmony_search.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1834 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/algorithms/random_search.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.293500 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)      808 2023-04-19 14:45:24.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/__init__.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1999 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/blxalpha_crossover.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1836 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/gaussian_crossover.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1786 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/masked_crossover.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2122 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/multipoint_crossover.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1629 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/crossovers/uniform_crossover.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     2109 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/mutation.py
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1792 2023-04-21 10:04:43.000000 tensorcro-1.2.0/src/tensorcro/substrates/substrate.py
+drwxrwxr-x   0 sugar137  (1000) sugar137  (1000)        0 2023-04-21 10:33:49.289500 tensorcro-1.2.0/src/tensorcro.egg-info/
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     5412 2023-04-21 10:33:49.000000 tensorcro-1.2.0/src/tensorcro.egg-info/PKG-INFO
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)     1096 2023-04-21 10:33:49.000000 tensorcro-1.2.0/src/tensorcro.egg-info/SOURCES.txt
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)        1 2023-04-21 10:33:49.000000 tensorcro-1.2.0/src/tensorcro.egg-info/dependency_links.txt
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       87 2023-04-21 10:33:49.000000 tensorcro-1.2.0/src/tensorcro.egg-info/requires.txt
+-rw-rw-r--   0 sugar137  (1000) sugar137  (1000)       10 2023-04-21 10:33:49.000000 tensorcro-1.2.0/src/tensorcro.egg-info/top_level.txt
```

### Comparing `tensorcro-1.1.2/PKG-INFO` & `tensorcro-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcro
-Version: 1.1.2
+Version: 1.2.0
 Summary: TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.
 Home-page: https://github.com/iTzAlver/tensorcro.git
 Author: Palomo-Alonso, Alberto
 Author-email: a.palomo@edu.uah
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/iTzAlver/tensorcro/blob/main/
 Project-URL: Bug Reports, https://github.com/iTzAlver/tensorcro/issues
 Project-URL: Source Code, https://github.com/iTzAlver/tensorcro.git
@@ -21,29 +21,31 @@
 # TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.
 
 <p align="center">
     <img src="https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png" width="400px">
 </p>
 
 <p align="center">
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/LICENSE">
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/LICENSE">
         <img src="https://img.shields.io/github/license/iTzAlver/basenet_api?color=purple&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/test">
-        <img src="https://img.shields.io/badge/Code coverage-100-green?color=green&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/requirements.txt">
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/test">
+        <img src="https://img.shields.io/badge/coverage-100%25-green?color=green&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/build/requirements.txt">
         <img src="https://img.shields.io/badge/requirements-python3.8-red?color=blue&style=plastic" /></a>
-    <a href="">
-        <img src="https://img.shields.io/badge/doc-unavailable-green?color=red&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/multimedia/notebooks">
+        <img src="https://img.shields.io/badge/doc-notebook-green?color=orange&style=plastic" /></a>
     <a href="">
         <img src="https://img.shields.io/badge/release-1.2.0-white?color=white&style=plastic" /></a>
 </p>
 
 <p align="center">
     <a href="https://www.tensorflow.org/">
         <img src="https://img.shields.io/badge/dependencies-tensorflow-red?color=orange&style=for-the-badge" /></a>
+    <a href="https://developer.nvidia.com/cuda-downloads">
+        <img src="https://img.shields.io/badge/dependencies-CUDA-red?color=green&style=for-the-badge" /></a>
 </p>
 
 # Table of contents
 
 1. [About](#about)
 2. [What's new?](#whats-new)
 3. [Install](#install)
@@ -76,16 +78,18 @@
 masked and multipoint.
 5. Algorithms: The framework allows to implement algorithms as substrate layers such as Differential Evolution,
 Harmony Search and Random Search.
 6. Watch Replay: The algorithm also allows to watch the replay of the solutions found in the training process, with
 an interactive GUI.
 7. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
-### 1.1.2
+### 1.2.0
 1. Progress bar: The framework now also includes a progress bar to monitor the training process.
+2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
 ## Install
 
 To install it you must install the dependencies. Then, you can install the package with the following command
 using PIP:
 
 ```bash
@@ -94,24 +98,25 @@
 
 Or you can clone the repository and install it with the following commands
 using Git:
 
 ```bash
 git clone https://github.com.iTzAlver/TensorCRO.git
 cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl
+pip install ./tensorcro-1.2.0-py3-none-any.whl
 ```
 
 ### Requirements
 
 * Python 3.6 or higher
 * Tensorflow 2.0 or higher
 * Numpy 1.18.1 or higher
 * Matplotlib 3.1.3 or higher
 * Pandas 1.0.1 or higher
+* CUDA for GPU support (optional but strongly recommended)
 
 # Usage:
 
 We have a JuPyter Notebook with an example of use of the algorithm. You can find it in the folder `/multimedia/notebooks` 
 of the repository.
 
 # Cite:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensorcro Version: 1.1.2 Summary: TensorCRO: A
+Metadata-Version: 2.1 Name: tensorcro Version: 1.2.0 Summary: TensorCRO: A
 Tensorflow-based implementation of the Coral Reef Optimization algorithm. Home-
 page: https://github.com/iTzAlver/tensorcro.git Author: Palomo-Alonso, Alberto
 Author-email: a.palomo@edu.uah Project-URL: Documentation, https://
 htmlpreview.github.io/?https://github.com/iTzAlver/tensorcro/blob/main/
 Project-URL: Bug Reports, https://github.com/iTzAlver/tensorcro/issues Project-
 URL: Source Code, https://github.com/iTzAlver/tensorcro.git Keywords:
 deeplearning,ml,api,optimization,heuristic Classifier: Development Status :: 5
@@ -10,21 +10,22 @@
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev # TensorCRO: A Tensorflow-based implementation of the Coral Reef
 Optimization algorithm.
     [https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png]
                [https://img.shields.io/github/license/iTzAlver/
-  basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/Code
- coverage-100-green?color=green&style=plastic] [https://img.shields.io/badge/
+basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/coverage-
+    100%25-green?color=green&style=plastic] [https://img.shields.io/badge/
  requirements-python3.8-red?color=blue&style=plastic] [https://img.shields.io/
- badge/doc-unavailable-green?color=red&style=plastic] [https://img.shields.io/
+ badge/doc-notebook-green?color=orange&style=plastic] [https://img.shields.io/
              badge/release-1.2.0-white?color=white&style=plastic]
             [https://img.shields.io/badge/dependencies-tensorflow-
-                     red?color=orange&style=for-the-badge]
+     red?color=orange&style=for-the-badge] [https://img.shields.io/badge/
+            dependencies-CUDA-red?color=green&style=for-the-badge]
 # Table of contents 1. [About](#about) 2. [What's new?](#whats-new) 3.
 [Install](#install) 4. [Usage](#usage) ## About ## ```biblitex Implementation
 author: A.Palomo-Alonso (alberto.palomo@uah.es) Original Algorithm author:
 S.Salcedo-Sanz (sancho.salcedo@uah.es) Universidad de AlcalÃ¡ (Madrid - Spain).
 Escuela PolitÃ©cnica Superior Signal Processing and Communications Department
 (TDSC) ``` This is a Tensorflow-based implementation of the Coral Reef
 Optimization algorithm. The algorithm is implemented as a Tensorflow graph,
@@ -39,22 +40,25 @@
 conventional implementations. 4. Substrate crossovers: The framework allows to
 implement crossover operators as blxalpha, gaussian, uniform, masked and
 multipoint. 5. Algorithms: The framework allows to implement algorithms as
 substrate layers such as Differential Evolution, Harmony Search and Random
 Search. 6. Watch Replay: The algorithm also allows to watch the replay of the
 solutions found in the training process, with an interactive GUI. 7. Jupyter
 Notebook: The framework includes a Jupyter Notebook with example of use for the
-Max-Ones-From-Zeros problem. ### 1.1.2 1. Progress bar: The framework now also
-includes a progress bar to monitor the training process. ## Install To install
-it you must install the dependencies. Then, you can install the package with
-the following command using PIP: ```bash pip install tensorcro ``` Or you can
-clone the repository and install it with the following commands using Git:
-```bash git clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl ``` ### Requirements * Python
-3.6 or higher * Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib
-3.1.3 or higher * Pandas 1.0.1 or higher # Usage: We have a JuPyter Notebook
-with an example of use of the algorithm. You can find it in the folder `/
-multimedia/notebooks` of the repository. # Cite: If you use this code, please
-cite the following paper: ```bibtex @inproceedings{palomo2022tensorcro, title=
-{TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization
-algorithm}, author={Palomo-Alonso, A and Salcedo-Sanz, S}, journal={arXiv
-preprint arXiv:X.Y}, year={2022} } ```
+Max-Ones-From-Zeros problem. ### 1.2.0 1. Progress bar: The framework now also
+includes a progress bar to monitor the training process. 2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of
+use for the Max-Ones-From-Zeros problem. ## Install To install it you must
+install the dependencies. Then, you can install the package with the following
+command using PIP: ```bash pip install tensorcro ``` Or you can clone the
+repository and install it with the following commands using Git: ```bash git
+clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/ pip install
+./tensorcro-1.2.0-py3-none-any.whl ``` ### Requirements * Python 3.6 or higher
+* Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib 3.1.3 or
+higher * Pandas 1.0.1 or higher * CUDA for GPU support (optional but strongly
+recommended) # Usage: We have a JuPyter Notebook with an example of use of the
+algorithm. You can find it in the folder `/multimedia/notebooks` of the
+repository. # Cite: If you use this code, please cite the following paper:
+```bibtex @inproceedings{palomo2022tensorcro, title={TensorCRO: A Tensorflow-
+based implementation of the Coral Reef Optimization algorithm}, author={Palomo-
+Alonso, A and Salcedo-Sanz, S}, journal={arXiv preprint arXiv:X.Y}, year={2022}
+} ```
```

### Comparing `tensorcro-1.1.2/README.md` & `tensorcro-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.
 
 <p align="center">
     <img src="https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png" width="400px">
 </p>
 
 <p align="center">
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/LICENSE">
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/LICENSE">
         <img src="https://img.shields.io/github/license/iTzAlver/basenet_api?color=purple&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/test">
-        <img src="https://img.shields.io/badge/Code coverage-100-green?color=green&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/requirements.txt">
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/test">
+        <img src="https://img.shields.io/badge/coverage-100%25-green?color=green&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/build/requirements.txt">
         <img src="https://img.shields.io/badge/requirements-python3.8-red?color=blue&style=plastic" /></a>
-    <a href="">
-        <img src="https://img.shields.io/badge/doc-unavailable-green?color=red&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/multimedia/notebooks">
+        <img src="https://img.shields.io/badge/doc-notebook-green?color=orange&style=plastic" /></a>
     <a href="">
         <img src="https://img.shields.io/badge/release-1.2.0-white?color=white&style=plastic" /></a>
 </p>
 
 <p align="center">
     <a href="https://www.tensorflow.org/">
         <img src="https://img.shields.io/badge/dependencies-tensorflow-red?color=orange&style=for-the-badge" /></a>
+    <a href="https://developer.nvidia.com/cuda-downloads">
+        <img src="https://img.shields.io/badge/dependencies-CUDA-red?color=green&style=for-the-badge" /></a>
 </p>
 
 # Table of contents
 
 1. [About](#about)
 2. [What's new?](#whats-new)
 3. [Install](#install)
@@ -56,16 +58,18 @@
 masked and multipoint.
 5. Algorithms: The framework allows to implement algorithms as substrate layers such as Differential Evolution,
 Harmony Search and Random Search.
 6. Watch Replay: The algorithm also allows to watch the replay of the solutions found in the training process, with
 an interactive GUI.
 7. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
-### 1.1.2
+### 1.2.0
 1. Progress bar: The framework now also includes a progress bar to monitor the training process.
+2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
 ## Install
 
 To install it you must install the dependencies. Then, you can install the package with the following command
 using PIP:
 
 ```bash
@@ -74,24 +78,25 @@
 
 Or you can clone the repository and install it with the following commands
 using Git:
 
 ```bash
 git clone https://github.com.iTzAlver/TensorCRO.git
 cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl
+pip install ./tensorcro-1.2.0-py3-none-any.whl
 ```
 
 ### Requirements
 
 * Python 3.6 or higher
 * Tensorflow 2.0 or higher
 * Numpy 1.18.1 or higher
 * Matplotlib 3.1.3 or higher
 * Pandas 1.0.1 or higher
+* CUDA for GPU support (optional but strongly recommended)
 
 # Usage:
 
 We have a JuPyter Notebook with an example of use of the algorithm. You can find it in the folder `/multimedia/notebooks` 
 of the repository.
 
 # Cite:
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
 # TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization
 algorithm.
     [https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png]
                [https://img.shields.io/github/license/iTzAlver/
-  basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/Code
- coverage-100-green?color=green&style=plastic] [https://img.shields.io/badge/
+basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/coverage-
+    100%25-green?color=green&style=plastic] [https://img.shields.io/badge/
  requirements-python3.8-red?color=blue&style=plastic] [https://img.shields.io/
- badge/doc-unavailable-green?color=red&style=plastic] [https://img.shields.io/
+ badge/doc-notebook-green?color=orange&style=plastic] [https://img.shields.io/
              badge/release-1.2.0-white?color=white&style=plastic]
             [https://img.shields.io/badge/dependencies-tensorflow-
-                     red?color=orange&style=for-the-badge]
+     red?color=orange&style=for-the-badge] [https://img.shields.io/badge/
+            dependencies-CUDA-red?color=green&style=for-the-badge]
 # Table of contents 1. [About](#about) 2. [What's new?](#whats-new) 3.
 [Install](#install) 4. [Usage](#usage) ## About ## ```biblitex Implementation
 author: A.Palomo-Alonso (alberto.palomo@uah.es) Original Algorithm author:
 S.Salcedo-Sanz (sancho.salcedo@uah.es) Universidad de AlcalÃ¡ (Madrid - Spain).
 Escuela PolitÃ©cnica Superior Signal Processing and Communications Department
 (TDSC) ``` This is a Tensorflow-based implementation of the Coral Reef
 Optimization algorithm. The algorithm is implemented as a Tensorflow graph,
@@ -27,22 +28,25 @@
 conventional implementations. 4. Substrate crossovers: The framework allows to
 implement crossover operators as blxalpha, gaussian, uniform, masked and
 multipoint. 5. Algorithms: The framework allows to implement algorithms as
 substrate layers such as Differential Evolution, Harmony Search and Random
 Search. 6. Watch Replay: The algorithm also allows to watch the replay of the
 solutions found in the training process, with an interactive GUI. 7. Jupyter
 Notebook: The framework includes a Jupyter Notebook with example of use for the
-Max-Ones-From-Zeros problem. ### 1.1.2 1. Progress bar: The framework now also
-includes a progress bar to monitor the training process. ## Install To install
-it you must install the dependencies. Then, you can install the package with
-the following command using PIP: ```bash pip install tensorcro ``` Or you can
-clone the repository and install it with the following commands using Git:
-```bash git clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl ``` ### Requirements * Python
-3.6 or higher * Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib
-3.1.3 or higher * Pandas 1.0.1 or higher # Usage: We have a JuPyter Notebook
-with an example of use of the algorithm. You can find it in the folder `/
-multimedia/notebooks` of the repository. # Cite: If you use this code, please
-cite the following paper: ```bibtex @inproceedings{palomo2022tensorcro, title=
-{TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization
-algorithm}, author={Palomo-Alonso, A and Salcedo-Sanz, S}, journal={arXiv
-preprint arXiv:X.Y}, year={2022} } ```
+Max-Ones-From-Zeros problem. ### 1.2.0 1. Progress bar: The framework now also
+includes a progress bar to monitor the training process. 2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of
+use for the Max-Ones-From-Zeros problem. ## Install To install it you must
+install the dependencies. Then, you can install the package with the following
+command using PIP: ```bash pip install tensorcro ``` Or you can clone the
+repository and install it with the following commands using Git: ```bash git
+clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/ pip install
+./tensorcro-1.2.0-py3-none-any.whl ``` ### Requirements * Python 3.6 or higher
+* Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib 3.1.3 or
+higher * Pandas 1.0.1 or higher * CUDA for GPU support (optional but strongly
+recommended) # Usage: We have a JuPyter Notebook with an example of use of the
+algorithm. You can find it in the folder `/multimedia/notebooks` of the
+repository. # Cite: If you use this code, please cite the following paper:
+```bibtex @inproceedings{palomo2022tensorcro, title={TensorCRO: A Tensorflow-
+based implementation of the Coral Reef Optimization algorithm}, author={Palomo-
+Alonso, A and Salcedo-Sanz, S}, journal={arXiv preprint arXiv:X.Y}, year={2022}
+} ```
```

### Comparing `tensorcro-1.1.2/setup.py` & `tensorcro-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'matplotlib>=3.7.1',
     'pandas>=2.0.0',
 ]
 
 
 setuptools.setup(
     name='tensorcro',
-    version='1.1.2',
+    version='1.2.0',
     author='Palomo-Alonso, Alberto',
     author_email='a.palomo@edu.uah',
     description='TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.',
     keywords='deeplearning, ml, api, optimization, heuristic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/iTzAlver/tensorcro.git',
```

### Comparing `tensorcro-1.1.2/src/tensorcro/__init__.py` & `tensorcro-1.2.0/src/tensorcro/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcro-1.1.2/src/tensorcro/__special__.py` & `tensorcro-1.2.0/src/tensorcro/__special__.py`

 * *Files identical despite different names*

### Comparing `tensorcro-1.1.2/src/tensorcro/replay/__init__.py` & `tensorcro-1.2.0/src/tensorcro/replay/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcro-1.1.2/src/tensorcro/replay/watch_replay.py` & `tensorcro-1.2.0/src/tensorcro/replay/watch_replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.list_fitness()
 
     def render(self):
         reef = self.fitness[self.index]
         names = self.names['names']
         shards = self.names['shards']
         self.label.destroy()
-        self.label = tk.Label(self.master, text=f"Epoch {shards * self.index + 1} / {shards * len(self.fitness)}",
+        self.label = tk.Label(self.master, text=f"Epoch {shards * (self.index + 1)} / {shards * len(self.fitness)}",
                               font=("Arial", 20))
         self.label.place(x=240, y=10)
         padding = reef.shape[1] // len(names)
         fig = plt.figure(figsize=(6, 6))
         ax = fig.add_subplot(111, projection='3d')
         __one_line_colors = np.array([[np.array(cm.tab10(int(_ // padding)))] for _ in range(reef.shape[1])])
         kol = np.reshape(np.tile(__one_line_colors, [reef.shape[0], 1]), (reef.shape[0], reef.shape[1], 4))
```

### Comparing `tensorcro-1.1.2/src/tensorcro/slcro.py` & `tensorcro-1.2.0/src/tensorcro/slcro.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,17 @@
         self._substrate_functions = subs
         if self._reef_shape[1] % len(subs) != 0:
             raise ValueError('TensorCRO: The reef columns are not divisible by the number of selected substrates.')
         else:
             self._substrate_segmentation = tf.constant(self._reef_shape[1] // len(subs), dtype=tf.int32)
             self._number_of_reefs = tf.constant(len(subs), dtype=tf.int32)
         # Save utils:
-        self.n_fit = 0
-        if os.path.exists(__replay_path__):
-            shutil.rmtree(__replay_path__)
-        os.mkdir(__replay_path__)
         self.shards = None
         self.seed = None
+        self.n_fit = None
 
     def fit(self, fitness_function: tf.function, individual_directives: tf.Tensor, max_iter: int = 100,
             device: str = '/GPU:0', seed: int = None, init=None, shards=None) \
             -> tf.Tensor:
         """
         This function is the main loop of the algorithm. It will run the algorithm until the maximum number of
         iterations is reached or the fitness function returns a value that is considered optimal.
@@ -90,33 +87,43 @@
         :param max_iter: maximum number of iterations.
         :param device: device to use for the calculations.
         :param seed: seed for the random number generator.
         :param init: initial population and fitness to use as a tuple.
         :param shards: number of shards to use for the computation.
         :return: the best solution found.
         """
+        # Formatting directives:
+        if not isinstance(individual_directives, tf.Tensor):
+            individual_directives = tf.convert_to_tensor(individual_directives, dtype=tf.float32)
+        # Clearing save buffer:
+        if os.path.exists(__replay_path__):
+            shutil.rmtree(__replay_path__)
+        os.mkdir(__replay_path__)
+        # Set up the seed:
         if seed is None:
             seed = tf.random.uniform((1,), minval=0, maxval=2147483647, dtype=tf.int32)
         self.seed = int(seed)
         tf.random.set_seed(self.seed)
+        # Set up shards and initial population:
+        if shards is None:
+            shards = max_iter
+        self.shards = shards
+        rf = init
+        self.n_fit = 0
+        # Using the selected device:
         with tf.device(device):
-            if shards is None:
-                shards = max_iter
-            self.shards = shards
-            rf = init
             for _ in range(max_iter // shards):
                 rf = self._fit(fitness_function, individual_directives, shards, rf)
                 reef, fitness = rf
                 self.__save_replay(reef, fitness)
             sorted_reef = tf.gather(tf.reshape(reef, (-1, tf.shape(individual_directives)[-1])),
                                     tf.argsort(tf.reshape(fitness, (-1,)), direction='DESCENDING'))
             return sorted_reef
 
-    @tf.function
-    def _fit(self, fitness_function: tf.function, individual_directives, max_iter: int = 20, init=None) \
+    def _fit(self, fitness_function: tf.function, individual_directives, max_iter: int = 100, init=None) \
             -> tuple[tf.Tensor, tf.Tensor]:
         # Precompute some useful parameters:
         __number_of_parameters = tf.shape(individual_directives)[-1]  # Number of parameters for each coral.
         __parameter_diff = tf.subtract(individual_directives[1], individual_directives[0])  # Max - Min.
         __number_of_reefs = self._number_of_reefs
         __number_of_columns = self._substrate_segmentation
         __reef_shape = tf.convert_to_tensor((__number_of_reefs, self._reef_shape[0],  # Reefs-Rows-Columns-Params.
@@ -273,15 +280,15 @@
         if os.path.exists(path):
             shutil.rmtree(path)
         shutil.copytree(__replay_path__, path)
 
     @staticmethod
     def watch_replay(path: str = __replay_path__, lock: bool = False, mp: bool = True):
         """
-        This function is used to watch a replay.
+        This function is used to watch a replay in the GUI.
         :param path: A string with the path to the replay.
         :param lock: A boolean that indicates if the function should wait for the replay to finish.
         :param mp: A boolean that indicates if the function should run in a separate process.
         :return: A multiprocessing.Process object.
         """
         if mp:
             p = multiprocessing.Process(target=watch_replay, args=(path,))
```

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/__init__.py` & `tensorcro-1.2.0/src/tensorcro/substrates/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 #                                                           #
 #   This file was created by: Alberto Palomo Alonso         #
 # Universidad de Alcalá - Escuela Politécnica Superior      #
 #                                                           #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 from .crossovers import UniformCrossover, GaussianCrossover, MaskedCrossover, MultipointCrossover, BLXAlphaCrossover
 from .algorithms import HarmonySearch, RandomSearch, DifferentialSearch
-from .substrate import ComposedSubstrate
+from .substrate import ComposedSubstrate, CROSubstrate
 from .mutation import Mutation
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 #                        END OF FILE                        #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
```

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/algorithms/__init__.py` & `tensorcro-1.2.0/src/tensorcro/substrates/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/crossovers/__init__.py` & `tensorcro-1.2.0/src/tensorcro/substrates/crossovers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/crossovers/blxalpha_crossover.py` & `tensorcro-1.2.0/src/tensorcro/substrates/crossovers/blxalpha_crossover.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 from ..substrate import CROSubstrate
 
 
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 #                        MAIN CLASS                         #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 class BLXAlphaCrossover(CROSubstrate):
-    def __init__(self, directives, scale: float = 0.1):
+    def __init__(self, directives: tf.Tensor, scale: float = 0.1):
+        """
+        The BLXAlphaCrossover method implements the BLX-Alpha crossover method. This method is a
+        generalization of the BLX crossover method, which is a generalization of the SBX crossover
+        method. The BLX-Alpha crossover method is a linear combination of the parents, with a
+        random alpha value between 0 and 1.
+        :param directives: Specifications of the parameters.
+        :param scale: Scale of the alpha value.
+        """
         self.mins = directives[0] * scale
         self.maxs = directives[1] * scale
 
     def _call(self, individuals: tf.Tensor):
         # Split the individuals in two groups
         noi = tf.shape(individuals)[0] // 2
         fathers = individuals[0:noi]
```

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/crossovers/gaussian_crossover.py` & `tensorcro-1.2.0/src/tensorcro/substrates/crossovers/gaussian_crossover.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 #                        MAIN CLASS                         #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 class GaussianCrossover(CROSubstrate):
     def __init__(self, mean: float = 0.75, stddev: float = 0.25):
+        """
+        The GaussianCrossover method implements a gaussian crossover. It is a selector between two parents,
+        where the probability of selecting a parent is given by a gaussian distribution. If the mean is 0.5 it is
+        equivalent to a uniform crossover.
+        :param mean: Mean of the gaussian.
+        :param stddev: Standard deviation of the gaussian.
+        """
         self.mean = tf.constant(mean)
         self.stddev = tf.constant(stddev)
 
     def _call(self, individuals: tf.Tensor):
         noi = tf.shape(individuals)[0] // 2
         fathers = individuals[0:noi]
         mothers = individuals[noi:noi * 2]
```

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/crossovers/multipoint_crossover.py` & `tensorcro-1.2.0/src/tensorcro/substrates/crossovers/multipoint_crossover.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 #                        MAIN CLASS                         #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 class MultipointCrossover(CROSubstrate):
     def __init__(self, points: list[int]):
+        """
+        The MultipointCrossover class implements a multipoint crossover. The points is a list of indices where
+        the points between the parents are swapped. The mask is applied to each parent, so the offspring will be
+        composed of the points of the first parent in the positions indicated by the mask, and the points of the
+        second parent in the positions not indicated by the mask.
+        :param points: List of indices where the points between the parents are swapped.
+        """
         self.points = tf.convert_to_tensor(points)
 
     def _call(self, individuals: tf.Tensor):
         # Split the individuals in two groups
         noi = tf.shape(individuals)[0] // 2
         fathers = individuals[0:noi]
         mothers = individuals[noi:noi * 2]
```

### Comparing `tensorcro-1.1.2/src/tensorcro/substrates/mutation.py` & `tensorcro-1.2.0/src/tensorcro/substrates/mutation.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,24 +7,34 @@
 import tensorflow as tf
 from .substrate import CROSubstrate
 FUNC = {
     'uniform': tf.random.uniform,
     'gaussian': tf.random.normal,
     'truncated_normal': tf.random.truncated_normal,
     'poisson': tf.random.poisson,
-    'shuffle': tf.random.shuffle,
     'gamma': tf.random.gamma
 }
 
 
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 #                        MAIN CLASS                         #
 # - x - x - x - x - x - x - x - x - x - x - x - x - x - x - #
 class Mutation(CROSubstrate):
-    def __init__(self, mutation_type, **kwargs):
+    def __init__(self, mutation_type: str, **kwargs):
+        """
+        Mutation class. It is a CROSubstrate that applies a mutation to the individuals. The supported mutation types
+        are:
+            - uniform (uniform): tf.random.uniform
+            - gaussian (normal): tf.random.normal
+            - truncated_normal (truncated normal): tf.random.truncated_normal
+            - poisson (poisson): tf.random.poisson
+            - gamma (gamma): tf.random.gamma
+        :param mutation_type: Mutation type as a string.
+        :param kwargs: Arguments for the mutation function.
+        """
         if mutation_type not in FUNC:
             raise ValueError(f"TensorCRO:Mutation: Mutation type {mutation_type} not supported."
                              f"\nSupported types: {list(FUNC.keys())}")
         self.func = FUNC[mutation_type]
         self.arguments = kwargs
 
     def _call(self, individuals: tf.Tensor) -> tf.Tensor:
```

### Comparing `tensorcro-1.1.2/src/tensorcro.egg-info/PKG-INFO` & `tensorcro-1.2.0/src/tensorcro.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcro
-Version: 1.1.2
+Version: 1.2.0
 Summary: TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.
 Home-page: https://github.com/iTzAlver/tensorcro.git
 Author: Palomo-Alonso, Alberto
 Author-email: a.palomo@edu.uah
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/iTzAlver/tensorcro/blob/main/
 Project-URL: Bug Reports, https://github.com/iTzAlver/tensorcro/issues
 Project-URL: Source Code, https://github.com/iTzAlver/tensorcro.git
@@ -21,29 +21,31 @@
 # TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization algorithm.
 
 <p align="center">
     <img src="https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png" width="400px">
 </p>
 
 <p align="center">
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/LICENSE">
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/LICENSE">
         <img src="https://img.shields.io/github/license/iTzAlver/basenet_api?color=purple&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/test">
-        <img src="https://img.shields.io/badge/Code coverage-100-green?color=green&style=plastic" /></a>
-    <a href="https://github.com/iTzAlver/tensorcro/blob/main/requirements.txt">
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/test">
+        <img src="https://img.shields.io/badge/coverage-100%25-green?color=green&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/blob/master/build/requirements.txt">
         <img src="https://img.shields.io/badge/requirements-python3.8-red?color=blue&style=plastic" /></a>
-    <a href="">
-        <img src="https://img.shields.io/badge/doc-unavailable-green?color=red&style=plastic" /></a>
+    <a href="https://github.com/iTzAlver/TensorCRO/tree/master/multimedia/notebooks">
+        <img src="https://img.shields.io/badge/doc-notebook-green?color=orange&style=plastic" /></a>
     <a href="">
         <img src="https://img.shields.io/badge/release-1.2.0-white?color=white&style=plastic" /></a>
 </p>
 
 <p align="center">
     <a href="https://www.tensorflow.org/">
         <img src="https://img.shields.io/badge/dependencies-tensorflow-red?color=orange&style=for-the-badge" /></a>
+    <a href="https://developer.nvidia.com/cuda-downloads">
+        <img src="https://img.shields.io/badge/dependencies-CUDA-red?color=green&style=for-the-badge" /></a>
 </p>
 
 # Table of contents
 
 1. [About](#about)
 2. [What's new?](#whats-new)
 3. [Install](#install)
@@ -76,16 +78,18 @@
 masked and multipoint.
 5. Algorithms: The framework allows to implement algorithms as substrate layers such as Differential Evolution,
 Harmony Search and Random Search.
 6. Watch Replay: The algorithm also allows to watch the replay of the solutions found in the training process, with
 an interactive GUI.
 7. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
-### 1.1.2
+### 1.2.0
 1. Progress bar: The framework now also includes a progress bar to monitor the training process.
+2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of use for the Max-Ones-From-Zeros problem.
 
 ## Install
 
 To install it you must install the dependencies. Then, you can install the package with the following command
 using PIP:
 
 ```bash
@@ -94,24 +98,25 @@
 
 Or you can clone the repository and install it with the following commands
 using Git:
 
 ```bash
 git clone https://github.com.iTzAlver/TensorCRO.git
 cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl
+pip install ./tensorcro-1.2.0-py3-none-any.whl
 ```
 
 ### Requirements
 
 * Python 3.6 or higher
 * Tensorflow 2.0 or higher
 * Numpy 1.18.1 or higher
 * Matplotlib 3.1.3 or higher
 * Pandas 1.0.1 or higher
+* CUDA for GPU support (optional but strongly recommended)
 
 # Usage:
 
 We have a JuPyter Notebook with an example of use of the algorithm. You can find it in the folder `/multimedia/notebooks` 
 of the repository.
 
 # Cite:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensorcro Version: 1.1.2 Summary: TensorCRO: A
+Metadata-Version: 2.1 Name: tensorcro Version: 1.2.0 Summary: TensorCRO: A
 Tensorflow-based implementation of the Coral Reef Optimization algorithm. Home-
 page: https://github.com/iTzAlver/tensorcro.git Author: Palomo-Alonso, Alberto
 Author-email: a.palomo@edu.uah Project-URL: Documentation, https://
 htmlpreview.github.io/?https://github.com/iTzAlver/tensorcro/blob/main/
 Project-URL: Bug Reports, https://github.com/iTzAlver/tensorcro/issues Project-
 URL: Source Code, https://github.com/iTzAlver/tensorcro.git Keywords:
 deeplearning,ml,api,optimization,heuristic Classifier: Development Status :: 5
@@ -10,21 +10,22 @@
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev # TensorCRO: A Tensorflow-based implementation of the Coral Reef
 Optimization algorithm.
     [https://github.com/iTzAlver/TensorCRO/blob/master/multimedia/logo.png]
                [https://img.shields.io/github/license/iTzAlver/
-  basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/Code
- coverage-100-green?color=green&style=plastic] [https://img.shields.io/badge/
+basenet_api?color=purple&style=plastic] [https://img.shields.io/badge/coverage-
+    100%25-green?color=green&style=plastic] [https://img.shields.io/badge/
  requirements-python3.8-red?color=blue&style=plastic] [https://img.shields.io/
- badge/doc-unavailable-green?color=red&style=plastic] [https://img.shields.io/
+ badge/doc-notebook-green?color=orange&style=plastic] [https://img.shields.io/
              badge/release-1.2.0-white?color=white&style=plastic]
             [https://img.shields.io/badge/dependencies-tensorflow-
-                     red?color=orange&style=for-the-badge]
+     red?color=orange&style=for-the-badge] [https://img.shields.io/badge/
+            dependencies-CUDA-red?color=green&style=for-the-badge]
 # Table of contents 1. [About](#about) 2. [What's new?](#whats-new) 3.
 [Install](#install) 4. [Usage](#usage) ## About ## ```biblitex Implementation
 author: A.Palomo-Alonso (alberto.palomo@uah.es) Original Algorithm author:
 S.Salcedo-Sanz (sancho.salcedo@uah.es) Universidad de AlcalÃ¡ (Madrid - Spain).
 Escuela PolitÃ©cnica Superior Signal Processing and Communications Department
 (TDSC) ``` This is a Tensorflow-based implementation of the Coral Reef
 Optimization algorithm. The algorithm is implemented as a Tensorflow graph,
@@ -39,22 +40,25 @@
 conventional implementations. 4. Substrate crossovers: The framework allows to
 implement crossover operators as blxalpha, gaussian, uniform, masked and
 multipoint. 5. Algorithms: The framework allows to implement algorithms as
 substrate layers such as Differential Evolution, Harmony Search and Random
 Search. 6. Watch Replay: The algorithm also allows to watch the replay of the
 solutions found in the training process, with an interactive GUI. 7. Jupyter
 Notebook: The framework includes a Jupyter Notebook with example of use for the
-Max-Ones-From-Zeros problem. ### 1.1.2 1. Progress bar: The framework now also
-includes a progress bar to monitor the training process. ## Install To install
-it you must install the dependencies. Then, you can install the package with
-the following command using PIP: ```bash pip install tensorcro ``` Or you can
-clone the repository and install it with the following commands using Git:
-```bash git clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/
-pip install ./tensorcro-1.0.0-py3-none-any.whl ``` ### Requirements * Python
-3.6 or higher * Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib
-3.1.3 or higher * Pandas 1.0.1 or higher # Usage: We have a JuPyter Notebook
-with an example of use of the algorithm. You can find it in the folder `/
-multimedia/notebooks` of the repository. # Cite: If you use this code, please
-cite the following paper: ```bibtex @inproceedings{palomo2022tensorcro, title=
-{TensorCRO: A Tensorflow-based implementation of the Coral Reef Optimization
-algorithm}, author={Palomo-Alonso, A and Salcedo-Sanz, S}, journal={arXiv
-preprint arXiv:X.Y}, year={2022} } ```
+Max-Ones-From-Zeros problem. ### 1.2.0 1. Progress bar: The framework now also
+includes a progress bar to monitor the training process. 2. Minor bug fixing.
+3. Jupyter Notebook: The framework includes a Jupyter Notebook with example of
+use for the Max-Ones-From-Zeros problem. ## Install To install it you must
+install the dependencies. Then, you can install the package with the following
+command using PIP: ```bash pip install tensorcro ``` Or you can clone the
+repository and install it with the following commands using Git: ```bash git
+clone https://github.com.iTzAlver/TensorCRO.git cd TensorCRO/dist/ pip install
+./tensorcro-1.2.0-py3-none-any.whl ``` ### Requirements * Python 3.6 or higher
+* Tensorflow 2.0 or higher * Numpy 1.18.1 or higher * Matplotlib 3.1.3 or
+higher * Pandas 1.0.1 or higher * CUDA for GPU support (optional but strongly
+recommended) # Usage: We have a JuPyter Notebook with an example of use of the
+algorithm. You can find it in the folder `/multimedia/notebooks` of the
+repository. # Cite: If you use this code, please cite the following paper:
+```bibtex @inproceedings{palomo2022tensorcro, title={TensorCRO: A Tensorflow-
+based implementation of the Coral Reef Optimization algorithm}, author={Palomo-
+Alonso, A and Salcedo-Sanz, S}, journal={arXiv preprint arXiv:X.Y}, year={2022}
+} ```
```

### Comparing `tensorcro-1.1.2/src/tensorcro.egg-info/SOURCES.txt` & `tensorcro-1.2.0/src/tensorcro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

