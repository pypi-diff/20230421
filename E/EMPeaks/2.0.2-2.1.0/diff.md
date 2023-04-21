# Comparing `tmp/EMPeaks-2.0.2.tar.gz` & `tmp/EMPeaks-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/yasunobu/Documents/src/published_src/EMPeaks2.0.2/dist/tmppfaxe4h_/EMPeaks-2.0.2.tar", last modified: Tue Dec  7 05:56:15 2021, max compression
+gzip compressed data, was "EMPeaks-2.1.0.tar", last modified: Fri Apr 21 00:40:00 2023, max compression
```

## Comparing `EMPeaks-2.0.2.tar` & `EMPeaks-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.352265 EMPeaks-2.0.2/
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.306170 EMPeaks-2.0.2/EMPeaks/
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.313415 EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/
--rw-r--r--   0 yasunobu   (501) staff       (20)      202 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     5362 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/_doniachsunjic.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     4166 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/_dsmm.py
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.319747 EMPeaks-2.0.2/EMPeaks/GaussianMixture/
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.327370 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/
--rw-r--r--   0 yasunobu   (501) staff       (20)      367 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     1594 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_data 2.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     1594 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_data.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      636 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_em 2.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      636 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_em.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      654 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_exp_data 2.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      654 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_exp_data.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      687 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em 2.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      687 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      459 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     6007 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/_em.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     2147 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gaussian.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     1459 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gmm.py
--rw-r--r--   0 yasunobu   (501) staff       (20)    25027 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gmm2.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     8753 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/GaussianMixture/_spectrum_adapted_em.py
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.330114 EMPeaks-2.0.2/EMPeaks/LorentzianMixture/
--rw-r--r--   0 yasunobu   (501) staff       (20)      178 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/LorentzianMixture/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)    28649 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/LorentzianMixture/_lmm.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     6880 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/LorentzianMixture/_lorentz.py
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.350250 EMPeaks-2.0.2/EMPeaks/PseudoVoigtMixture/
--rw-r--r--   0 yasunobu   (501) staff       (20)      190 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/PseudoVoigtMixture/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)    10509 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/PseudoVoigtMixture/_pseudo_voigt.py
--rw-r--r--   0 yasunobu   (501) staff       (20)    28725 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/PseudoVoigtMixture/_pvmm.py
--rw-r--r--   0 yasunobu   (501) staff       (20)      193 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/__init__.py
--rw-r--r--   0 yasunobu   (501) staff       (20)     1104 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/EMPeaks/file_io.py
-drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2021-12-07 05:56:15.310277 EMPeaks-2.0.2/EMPeaks.egg-info/
--rw-r--r--   0 yasunobu   (501) staff       (20)     2436 2021-12-07 05:56:15.000000 EMPeaks-2.0.2/EMPeaks.egg-info/PKG-INFO
--rw-r--r--   0 yasunobu   (501) staff       (20)     1285 2021-12-07 05:56:15.000000 EMPeaks-2.0.2/EMPeaks.egg-info/SOURCES.txt
--rw-r--r--   0 yasunobu   (501) staff       (20)        1 2021-12-07 05:56:15.000000 EMPeaks-2.0.2/EMPeaks.egg-info/dependency_links.txt
--rw-r--r--   0 yasunobu   (501) staff       (20)        8 2021-12-07 05:56:15.000000 EMPeaks-2.0.2/EMPeaks.egg-info/top_level.txt
--rw-r--r--   0 yasunobu   (501) staff       (20)     1550 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/LICENSE
--rw-r--r--   0 yasunobu   (501) staff       (20)       16 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/MANIFEST.in
--rw-r--r--   0 yasunobu   (501) staff       (20)     2436 2021-12-07 05:56:15.352497 EMPeaks-2.0.2/PKG-INFO
--rw-r--r--   0 yasunobu   (501) staff       (20)     1940 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/README.md
--rw-r--r--   0 yasunobu   (501) staff       (20)      103 2021-12-07 05:50:34.000000 EMPeaks-2.0.2/pyproject.toml
--rw-r--r--   0 yasunobu   (501) staff       (20)      563 2021-12-07 05:56:15.356012 EMPeaks-2.0.2/setup.cfg
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.251003 EMPeaks-2.1.0/
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.125223 EMPeaks-2.1.0/EMPeaks/
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.135809 EMPeaks-2.1.0/EMPeaks/Background/
+-rw-r--r--   0 yasunobu   (501) staff       (20)      225 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/Background/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     5496 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/Background/_background.py
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.147091 EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/
+-rw-r--r--   0 yasunobu   (501) staff       (20)      202 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     5362 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/_doniachsunjic.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     4167 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/_dsmm.py
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.184436 EMPeaks-2.1.0/EMPeaks/GaussianMixture/
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.216105 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/
+-rw-r--r--   0 yasunobu   (501) staff       (20)      367 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1594 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_data 2.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1594 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_data.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      636 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_em 2.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      636 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_em.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      654 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_exp_data 2.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      654 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_exp_data.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      687 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em 2.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      687 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      459 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     6007 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/_em.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     2147 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gaussian.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1459 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gmm.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)    25294 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gmm2.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     8753 2023-04-21 00:38:00.000000 EMPeaks-2.1.0/EMPeaks/GaussianMixture/_spectrum_adapted_em.py
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.234006 EMPeaks-2.1.0/EMPeaks/LorentzianMixture/
+-rw-r--r--   0 yasunobu   (501) staff       (20)      178 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/LorentzianMixture/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     2939 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/LorentzianMixture/_lmm.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     6893 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/LorentzianMixture/_lorentz.py
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.250272 EMPeaks-2.1.0/EMPeaks/PseudoVoigtMixture/
+-rw-r--r--   0 yasunobu   (501) staff       (20)      190 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/PseudoVoigtMixture/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)    10519 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/PseudoVoigtMixture/_pseudo_voigt.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     4200 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/PseudoVoigtMixture/_pvmm.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)      193 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/__init__.py
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1104 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/EMPeaks/file_io.py
+drwxr-xr-x   0 yasunobu   (501) staff       (20)        0 2023-04-21 00:40:00.128455 EMPeaks-2.1.0/EMPeaks.egg-info/
+-rw-r--r--   0 yasunobu   (501) staff       (20)     3211 2023-04-21 00:40:00.000000 EMPeaks-2.1.0/EMPeaks.egg-info/PKG-INFO
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1354 2023-04-21 00:40:00.000000 EMPeaks-2.1.0/EMPeaks.egg-info/SOURCES.txt
+-rw-r--r--   0 yasunobu   (501) staff       (20)        1 2023-04-21 00:40:00.000000 EMPeaks-2.1.0/EMPeaks.egg-info/dependency_links.txt
+-rw-r--r--   0 yasunobu   (501) staff       (20)        8 2023-04-21 00:40:00.000000 EMPeaks-2.1.0/EMPeaks.egg-info/top_level.txt
+-rw-r--r--   0 yasunobu   (501) staff       (20)     1550 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/LICENSE
+-rw-r--r--   0 yasunobu   (501) staff       (20)       16 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/MANIFEST.in
+-rw-r--r--   0 yasunobu   (501) staff       (20)     3211 2023-04-21 00:40:00.251193 EMPeaks-2.1.0/PKG-INFO
+-rw-r--r--   0 yasunobu   (501) staff       (20)     2770 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/README.md
+-rw-r--r--   0 yasunobu   (501) staff       (20)      103 2023-04-21 00:38:01.000000 EMPeaks-2.1.0/pyproject.toml
+-rw-r--r--   0 yasunobu   (501) staff       (20)      563 2023-04-21 00:40:00.255280 EMPeaks-2.1.0/setup.cfg
```

### Comparing `EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/_doniachsunjic.py` & `EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/_doniachsunjic.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/DoniachSunjicMixture/_dsmm.py` & `EMPeaks-2.1.0/EMPeaks/DoniachSunjicMixture/_dsmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from EMPeaks.DoniachSunjicMixture._doniachsunjic import DoniachSunjic
 from EMPeaks.GaussianMixture._gmm2 import GaussianMixtureModel
-# from ..Background import UniformModel, SquareRootModel, LinearModel, TriangleModel, RampModel
-# from scipy import integrate
-# from scipy import optimize
+from EMPeaks.Background import UniformModel, SquareRootModel, LinearModel, TriangleModel, RampModel
+from scipy import integrate
+from scipy import optimize
 import matplotlib.pyplot as plt
 import numpy as np
-# import copy
-# import time
+import copy
+import time
 
 
 class DoniachSunjicMixtureModel(GaussianMixtureModel):
     """
     class Mixture(K, Background)
     K: mixture component of Pseudo Voigt Function
     Background: default 'uniform': including Uniform background model
@@ -84,26 +84,26 @@
 #         return self.LL
 #
 #     def maximum_likelihood_estimation(self, x, weight):
 #         return
 
 
 def main():
-    lmm = DoniachSunjicMixtureModel()
+    dsmm = DoniachSunjicMixtureModel()
     test = DoniachSunjicMixtureModel()
 
     test.model[0].x0 = -100
     test.model[1].x0 = +150
 
     x = np.arange(test.x_min, test.x_max)
     y = test.predict(x) * 10000
 
-    lmm.sampling(x, y, trial=10, r_eps=1.e-6)
-    lmm.fit(x, y, r_eps=1.e-8)
+    dsmm.sampling(x, y, trial=10, r_eps=1.e-6)
+    dsmm.fit(x, y, r_eps=1.e-8)
 
     plt.plot(x, y)
-    plt.plot(x, lmm.predict(x) * lmm.N_tot)
+    plt.plot(x, dsmm.predict(x) * dsmm.N_tot)
     plt.show()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_data 2.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_data 2.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_data.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_data.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_em 2.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_em 2.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_em.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_em.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_exp_data 2.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_exp_data 2.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_exp_data.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_exp_data.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em 2.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em 2.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/Tests/_test_sepctrum_adapted_em.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/_em.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/_em.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gaussian.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gaussian.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gmm.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gmm.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/_gmm2.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/_gmm2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,164 +1,164 @@
 from EMPeaks.GaussianMixture._gaussian import Gaussian
-# from ..Background import UniformModel, SquareRootModel, LinearModel, TriangleModel, RampModel
+from EMPeaks.Background import UniformModel, SquareRootModel, LinearModel, TriangleModel, RampModel
 import numpy as np
 from scipy import integrate
 from scipy import optimize
 import matplotlib.pyplot as plt
 import copy
 import time
 
 
 class GaussianMixtureModel:
     def __init__(self, K=2, x_min=-300, x_max=300, sigma_min=0.1, sigma_max=50,
-                 background='none', k_ramp=0):
+                 background='none', k_ramp=5):
         self.K = K
         self.x_min = x_min
         self.x_max = x_max
         self.sigma_min = sigma_min
         self.sigma_max = sigma_max
         self.background = background
         self.dx = 1.0
 
         self.model = [Gaussian(x_min, x_max, sigma_min, sigma_max) for k in range(self.K)]
         self.pi = np.ones(self.K) / self.K
-        self.N_tot = 1.0
-        self.N = self.pi * self.N_tot
 
         if self.background == 'none':
             self.K_all = K
-        # elif self.background == 'uniform':
-        #     self.K_all = K + 1
-        #     self.pi = np.append(self.pi, 1.0e-4)
-        #     self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        # elif self.background == 'squareroot':
-        #     self.K_all = K + 1
-        #     self.pi = np.append(self.pi, 1.0e-4)
-        #     self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(SquareRootModel(self.x_min, self.x_max))
-        # elif self.background == 'linear':
-        #     self.K_all = K + 1
-        #     self.pi = np.append(self.pi, 1.0e-4)
-        #     self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(LinearModel(self.x_min, self.x_max))
-        # elif self.background == 'ramp_sum':
-        #     print("RampSum Background is set.")
-        #     self.k_ramp = k_ramp
-        #     self.K_all = K + self.k_ramp + 2
-        #     self.ramp_node = np.linspace(self.x_min, self.x_max, self.k_ramp + 1, endpoint=False)
-        #     self.pi = np.append(self.pi, np.random.rand(self.k_ramp + 2))
-        #     self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        #     for k in range(k_ramp):
-        #         self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
-        #     self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
-        # elif self.background == 'sharley':
-        #     print("Sharley Background is set.")
-        #     self.K_all = K + 2
-        #     self.pi = np.append(self.pi, 1.0e-4)
-        #     self.pi = np.append(self.pi, 1.0e-4)
-        #     self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        #     self.model.append(Sharley(self.K, self.x_min, self.x_max))
-        #     self.model[-1].peak_model.model = self.model[0:K]
+        elif self.background == 'uniform':
+            self.K_all = K + 1
+            self.pi = np.append(self.pi, 1.0e-4)
+            self.pi = self.pi / np.sum(self.pi)
+            self.model.append(UniformModel(self.x_min, self.x_max))
+        elif self.background == 'squareroot':
+            self.K_all = K + 1
+            self.pi = np.append(self.pi, 1.0e-4)
+            self.pi = self.pi / np.sum(self.pi)
+            self.model.append(SquareRootModel(self.x_min, self.x_max))
+        elif self.background == 'linear':
+            self.K_all = K + 1
+            self.pi = np.append(self.pi, 1.0e-4)
+            self.pi = self.pi / np.sum(self.pi)
+            self.model.append(LinearModel(self.x_min, self.x_max))
+        elif self.background == 'ramp_sum':
+            print("RampSum Background is set.")
+            self.k_ramp = k_ramp
+            self.K_all = K + self.k_ramp + 2
+            self.ramp_node = np.linspace(self.x_min, self.x_max, self.k_ramp + 1, endpoint=False)
+            self.pi = np.append(self.pi, np.random.rand(self.k_ramp + 2))
+            self.pi = self.pi / np.sum(self.pi)
+            self.model.append(UniformModel(self.x_min, self.x_max))
+            for k in range(k_ramp):
+                 self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
+            self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
+        #elif self.background == 'sharley':
+        #    print("Sharley Background is set.")
+        #    self.K_all = K + 2
+        #    self.pi = np.append(self.pi, 1.0e-4)
+        #    self.pi = np.append(self.pi, 1.0e-4)
+        #    self.pi = self.pi / np.sum(self.pi)
+        #    self.model.append(UniformModel(self.x_min, self.x_max))
+        #    self.model.append(Sharley(self.K, self.x_min, self.x_max))
+        #    self.model[-1].peak_model.model = self.model[0:K]
         else:
             print("Setting Background is not implemented.")
+        self.N_tot = 1.0
         self.N = self.pi * self.N_tot
 
     def set_param(self, **param):
         """
         """
         if not param:
             return self
 
         param_keys = set(param.keys())
         if param_keys >= {'K'}:
             self.K = param['K']
+        else:
+            param['K'] = self.K
 
         self.set_single_params(**param)
         self.set_param_background(**param)
 
         # setting mixture ratio pi, P0, and P0_tot
         if param_keys >= {'N'}:
             self.N = param['N']
             self.N_tot = np.sum(param['N'])
             self.pi = param['N'] / self.N_tot
             return
 
         if param_keys >= {'pi'}:
-            if type(param['pi']) is not list:
+            if type(param['pi']) != list:
                 print("Parameter \"pi\" is not list type. Then pi is uniformly set as default.")
                 self.pi = np.ones(self.K_all) / self.K_all
                 return
-            if len(param["pi"]) is self.K_all:
+            if len(param["pi"]) == self.K_all:
                 self.pi = np.array(param['pi']) / sum(param['pi'])
-                if sum(param["pi"]) is not 1.0:
+                if sum(param["pi"]) != 1.0:
                     print("Sum of \"pi\" must be unity. Then values are normalized as ", self.pi)
                 return
-            elif len(param["pi"]) is self.K:
+            elif len(param["pi"]) == self.K:
                 print("Parameter \"pi\" does not have background ratio. pi for background is set to be 0.1.")
                 self.pi = np.array(param['pi']) / sum(param['pi']) * 0.9
                 self.pi = np.append(self.pi, 0.1)
-                if sum(param["pi"]) is not 1.0:
+                if sum(param["pi"]) != 1.0:
                     print("Sum of \"pi\" must be unity. Then values are normalized as ", self.pi)
                 return
             else:
                 print("Parameter \"pi\" does not have relevant length. Then pi is uniformly set as default.")
                 self.pi = np.ones(self.K_all) / self.K_all
                 return
 
     def set_param_background(self, **param):
         # setting parameters for Background.
         if self.background == 'none':
             self.K_all = self.K
 
-        # elif self.background == 'uniform':
-        #     self.K_all = self.K + 1
-        #
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        # elif self.background == 'squareroot':
-        #     self.K_all = self.K + 1
-        #     self.model.append(SquareRootModel(self.x_min, self.x_max))
-        #
-        # elif self.background == 'linear':
-        #     self.K_all = self.K + 1
-        #     if ('s_tri' in param) and (0 <= param['s_tri'] <= 1.0):
-        #         self.model.append(LinearModel(self.x_min, self.x_max, s_tri=param['s_tri']))
-        #     else:
-        #         self.model.append(LinearModel(self.x_min, self.x_max))
-        #
-        # elif self.background == 'ramp_sum':
-        #     self.K_all = self.K + self.k_ramp + 2
-        #     self.ramp_node = np.linspace(self.x_min, self.x_max, self.k_ramp + 1, endpoint=False)
-        #     # self.pi = np.append(self.pi, np.random.rand(self.k_ramp + 2))
-        #     # self.pi = self.pi / np.sum(self.pi)
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        #     for k in range(self.k_ramp):
-        #         self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
-        #     self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
-        #
+        elif self.background == 'uniform':
+            self.K_all = self.K + 1
+            self.model.append(UniformModel(self.x_min, self.x_max))
+        elif self.background == 'squareroot':
+            self.K_all = self.K + 1
+            self.model.append(SquareRootModel(self.x_min, self.x_max))
+
+        elif self.background == 'linear':
+            self.K_all = self.K + 1
+            if ('s_tri' in param) and (0 <= param['s_tri'] <= 1.0):
+                self.model.append(LinearModel(self.x_min, self.x_max, s_tri=param['s_tri']))
+            else:
+                self.model.append(LinearModel(self.x_min, self.x_max))
+
+        elif self.background == 'ramp_sum':
+            self.K_all = self.K + self.k_ramp + 2
+            self.ramp_node = np.linspace(self.x_min, self.x_max, self.k_ramp + 1, endpoint=False)
+            # self.pi = np.append(self.pi, np.random.rand(self.k_ramp + 2))
+            # self.pi = self.pi / np.sum(self.pi)
+            self.model.append(UniformModel(self.x_min, self.x_max))
+            for k in range(self.k_ramp):
+                self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
+            self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
+
         # elif self.background == 'sharley':
         #     self.K_all = self.K + 2
         #     self.model.append(UniformModel(self.x_min, self.x_max))
         #     self.model.append(Sharley(self.K, self.x_min, self.x_max))
         #     self.model[-1].peak_model.model = self.model[0:self.K]
 
     def extract_single_params(self, param_set, **param):
         org_K = self.K
         param_keys = set(param.keys())
         single_params = []
         for k in range(self.K):
             dict = {}
             for key in param_keys & param_set:
-                if type(param[key]) is not list:
+                if type(param[key]) != list:
                     print("Error: SingleModel parameters must be list type.")
                     self.K = org_K
                     return
-                if len(param[key]) is not param['K']:
+                if len(param[key]) != param['K']:
                     print("Error: length of parameters \"" + key + "\" is not consistent with value K.")
                     self.K = org_K
                     return
                 dict[key] = param[key][k]
             single_params.append(dict)
 
             instance_keys = set(self.__dict__.keys())
@@ -174,19 +174,19 @@
         self.model = [Gaussian(self.x_min, self.x_max, self.sigma_min, self.sigma_max) for k in range(self.K)]
         [self.model[k].set_param(**single_params[k]) for k in range(self.K)]
         return
 
     def export_param(self):
         _tmp_param = self.__dict__
         _tmp_param, _tmp_index = self.export_single_params(_tmp_param)
-        # if self.background is 'linear':
-        #     s_in_linear = [self.model[-1].s_uni, self.model[-1].s_tri]
-        # if self.background is 'linear':
-        #     self.model[-1].s_uni = s_in_linear[0]
-        #     self.model[-1].s_tri = s_in_linear[1]
+        if self.background == 'linear':
+            s_in_linear = [self.model[-1].s_uni, self.model[-1].s_tri]
+        if self.background == 'linear':
+            self.model[-1].s_uni = s_in_linear[0]
+            self.model[-1].s_tri = s_in_linear[1]
         _tmp_param['pi'][0:self.K] = list(np.array(self.pi)[0:self.K][_tmp_index])
         _tmp_param['N'] = list(np.array(_tmp_param['pi']) * self.N_tot)
         self.set_param(**_tmp_param)
         return _tmp_param
 
     def export_single_params(self, _tmp_param):
         """ parameters are sorted in the order of the first element in param_set."""
@@ -212,44 +212,47 @@
         return np.sum([self.pi[k] * self.model[k].predict(x) for k in range(self.K_all)], axis=0)
 
     def log_likelihood(self, x, intensity):
         return np.sum(intensity * np.log(self.predict(x) + 1e-200))
 
     def fit(self, x, intensity, method='adapted_em', max_iter=3000, r_eps=1e-9,
             stdout=True, trial=10, criteria='likelihood'):
+        print("**** Start spectrum fitting via EM algorithm ****")
+        print("background: {}".format(self.background))
+
         self.x_min = np.min(x)
         self.x_max = np.max(x)
-        # if self.background is "uniform":
-        #     self.model[-1] = UniformModel(self.x_min, self.x_max)
-        # if self.background is "squareroot":
-        #     self.model[-1] = SquareRootModel(self.x_min, self.x_max)
-        # if self.background is "linear":
-        #     self.model[-1] = LinearModel(self.x_min, self.x_max)
-        # elif self.background == 'ramp_sum':
-        #     self.model.append(UniformModel(self.x_min, self.x_max))
-        #     for k in range(self.k_ramp):
-        #         self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
-        #     self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
+        if self.background == "uniform":
+            self.model[-1] = UniformModel(self.x_min, self.x_max)
+        if self.background == "squareroot":
+            self.model[-1] = SquareRootModel(self.x_min, self.x_max)
+        if self.background == "linear":
+            self.model[-1] = LinearModel(self.x_min, self.x_max)
+        elif self.background == 'ramp_sum':
+            self.model.append(UniformModel(self.x_min, self.x_max))
+            for k in range(self.k_ramp):
+                self.model.append(RampModel(self.ramp_node[k], self.ramp_node[k + 1], self.x_max))
+            self.model.append(TriangleModel(self.ramp_node[-1], self.x_max))
         # elif self.background == 'sharley':
         #     self.model.append(UniformModel(self.x_min, self.x_max))
         #     self.model.append(Sharley(self.K, self.x_min, self.x_max))
 
-        if method is 'leastsq':
+        if method == 'leastsq':
             info = self.leastsq(x, intensity, stdout)
             return info
 
-        if method is 'l2div':
+        if method == 'l2div':
             info = self.l2_div(x, intensity, stdout)
             return info
 
-        elif method is 'adapted_em':
+        elif method == 'adapted_em':
             info = self.adapted_em(x, intensity, max_iter, r_eps, stdout)
             return info
 
-        elif method is 'smart':
+        elif method == 'smart':
             print('Start smart fitting process.')
             print('>>> Step 1: Sampling {:3d} trials with low threshold of 1.0e-6.'.format(trial))
             info1 = self.sampling(x, intensity, method='adapted_em',
                                   trial=trial, max_iter=max_iter, r_eps=1.0e-6, criteria=criteria, stdout=False)
             self.plot(x, intensity)
             print('>>> Step 2: Adapted_EM estimation with high threshold of {:}.'.format(r_eps))
             info2 = self.adapted_em(x, intensity, max_iter, r_eps, stdout)
@@ -277,18 +280,18 @@
             hist_run_info.append(run_info)
 
         hist_LL = np.array([hist_run_info[i]['LL'] for i in range(trial)])
         hist_RMSE = np.array([hist_run_info[i]['RMSE'] for i in range(trial)])
 
         print('Sampling the different initial guess with {:3d} trial is finished.'.format(trial))
 
-        if criteria is 'likelihood':
+        if criteria == 'likelihood':
             index_best = int(np.nanargmax(hist_LL))
             print('Maximum Log-Likelihood is obtained in trial {:3d}'.format(index_best))
-        elif criteria is 'rmse':
+        elif criteria == 'rmse':
             index_sucess = ~np.isnan(hist_RMSE)
             index_best = int(np.nanargmin(hist_RMSE[index_sucess]))
             print(index_best)
             print('Minimum RMSE is obtained in trial {:3d}'.format(index_best))
         else:
             index_best = 0
 
@@ -336,15 +339,15 @@
             self.e_step(x)
             self.m_step(x, intensity)
 
             ll = self.log_likelihood(x, intensity)
             residual = (ll - ll_0) / np.abs(ll_0)
             t2 = time.time()
 
-            if stdout is True:
+            if stdout == True:
                 if it % 10 == 0:
                     print("> iteration #{:3d}, LL={:10.8e}, residual={:4.3e}, elapsed time: {:5.2f} s"
                           .format(it, ll, residual, t2 - t1))
                     t1 = time.time()
 
             LL_hist.append(ll)
             res_hist.append(residual)
@@ -383,15 +386,15 @@
             'time/iter': t_tot / (it_tot + 1),
             'LL': ll,
             'LL_hist': LL_hist,
             'LL_residual': residual,
             'LL_residual_hist': res_hist,
             'RMSE': rmse
         }
-        if stdout is True:
+        if stdout == True:
             print('Estimated model parameters and scores are following:')
             self.print_param_summary(param)
             print('   LL:      {:12.8e}\n'
                   '   RMSE:     {:12.8e}\n'.format(run_info['LL'], run_info['RMSE'])
                   )
 
         return run_info
@@ -433,15 +436,15 @@
                                     args=(x, intensity),
                                     loss='linear'
                                     )
         self.N_tot = ls.x[0]
         self.N = list(self.pi * self.N_tot)
 
         rmse = np.sqrt((ls['cost']) * 2.0 / x.size)
-        if ls["success"] is True:
+        if ls["success"] == True:
             print("   non-linear least-square optimization is successfully finished.")
             print("            RMSE:      {:12.6e}\n"
                   "    Elapsed time:      {:12.6e} s\n".format(rmse, time.time() - start))
         else:
             print("   Warning: non-linear least-square optimization is failed.")
 
         return rmse
@@ -462,16 +465,16 @@
         Z = freq.sum() * self.dx
 
         def model(x, param):
             dict_param = {"K": self.K, "x0": list(param[0:self.K]),
                           "gamma": list(param[self.K:2 * self.K]),
                           'P0': list(param[2 * self.K:3 * self.K + self.K_all])
                           }
-            # if self.background is 'linear':
-            #     dict_param.update({'s_tri': param[-1]})
+            if self.background == 'linear':
+                dict_param.update({'s_tri': param[-1]})
             self.set_param(**dict_param)
             return self.predict(x) * Z
 
         def residual(param, x, y):
             return y - model(x, param)
 
         init_param = np.zeros(2 * self.K + self.K_all)
@@ -483,18 +486,18 @@
         lb = [self.x_min for i in range(self.K)]
         ub = [self.x_max for i in range(self.K)]
         [lb.append(self.gamma_min) for i in range(self.K)]
         [ub.append(self.gamma_max) for i in range(self.K)]
         [lb.append(0.0) for i in range(self.K_all)]
         [ub.append(np.inf) for i in range(self.K_all)]
 
-        # if self.background is 'linear':
-        #     init_param = np.append(init_param, np.random.rand() * 1000)
-        #     lb.append(-1000)
-        #     ub.append(1000)
+        if self.background == 'linear':
+            init_param = np.append(init_param, np.random.rand() * 1000)
+            lb.append(-1000)
+            ub.append(1000)
 
         bnds = (lb, ub)
 
         try:
             ls = optimize.least_squares(residual, init_param,
                                         args=(x_bin, freq),
                                         bounds=bnds,
@@ -532,15 +535,15 @@
             'LL_hist': np.nan,
             'LL_residual': np.nan,
             'LL_residual_hist': np.nan,
             'RMSE': rmse
         }
 
         param = self.export_param()
-        if flag is True:
+        if flag == True:
             print("   non-linear least-square optimization is successfully finished.")
             print("            RMSE:      {:12.6e}\n"
                   "    Elapsed time:      {:12.6e} s\n".format(run_info['rmse'], run_info['t_tot']))
             print('Estimated model parameters and scores are following:')
             self.print_param_summary(param)
             print('   RMSE:     {:12.8e}\n'.format(run_info['rmse']))
         else:
@@ -554,19 +557,24 @@
         fig = plt.figure(figsize=figsize)
         x = np.arange(self.x_min, self.x_max, self.dx)
 
         ax = fig.add_subplot(1, 1, 1)
         if self.background == 'none':
             for k in range(self.K):
                 ax.plot(x, self.model[k].predict(x) * self.N[k], label='model_' + str(k))
-        elif self.background is 'sharley':
+        elif self.background == 'sharley':
             for k in range(self.K):
                 ax.plot(x, self.model[k].predict(x) * self.N[k], label='model_' + str(k))
             y = self.model[-1].predict(x) * self.N[-1] + self.model[-2].predict(x) * self.N[-2]
             ax.plot(x, y, label=self.background)
+        elif self.background == 'ramp_sum':
+            for k in range(self.K):
+                ax.plot(x, self.model[k].predict(x) * self.N[k], label='model_' + str(k))
+            y = np.sum([self.model[self.K+k].predict(x) * self.N[self.K+k] for k in range(self.k_ramp+2)], axis=0)
+            ax.plot(x, y, label=self.background)
         else:
             for k in range(self.K):
                 ax.plot(x, self.model[k].predict(x) * self.N[k], label='model_' + str(k))
             ax.plot(x, self.model[-1].predict(x) * self.N[-1], label=self.background)
 
         ax.plot(x, self.predict(x) * self.N_tot, 'black', linewidth=3, ls='--', label='full_model')
         ax.scatter(x_data, intensity, label='data')
```

### Comparing `EMPeaks-2.0.2/EMPeaks/GaussianMixture/_spectrum_adapted_em.py` & `EMPeaks-2.1.0/EMPeaks/GaussianMixture/_spectrum_adapted_em.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks/LorentzianMixture/_lorentz.py` & `EMPeaks-2.1.0/EMPeaks/LorentzianMixture/_lorentz.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,11 +164,11 @@
             self.gamma = param[1]
             return - self.log_likelihood(x, intensity)
 
         self.x0 = np.sum(x * intensity) / np.sum(intensity)
         self.gamma = np.sqrt(2.0 * np.log(2.0) * np.sum(x ** 2 * intensity) / np.sum(intensity))
 
         init = [self.x0, self.gamma]
-        info = optimize.minimize(func_ll, x0=init, bounds=[(-200, 200), (0.1, 2000)], method='L-BFGS-B')
+        info = optimize.minimize(func_ll, x0=init, bounds=[(self.x_min, self.x_max), (0.1, 2000)], method='L-BFGS-B')
         self.x0 = info['x'][0]
         self.gamma = info['x'][1]
         return
```

### Comparing `EMPeaks-2.0.2/EMPeaks/PseudoVoigtMixture/_pseudo_voigt.py` & `EMPeaks-2.1.0/EMPeaks/PseudoVoigtMixture/_pseudo_voigt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, x_min=-100, x_max=100, gamma_min=0.01, gamma_max=10):
         self.x_min = x_min
         self.x_max = x_max
         self.gamma_min = gamma_min
         self.gamma_max = gamma_max
         self.x0 = np.random.uniform(x_min, x_max)
         self.gamma = np.random.uniform(gamma_min, gamma_max)
-        self.eta = np.random.uniform()
+        self.eta = np.random.uniform(0.5, 1.0)
         self.interval = (self.x_min, self.x_max)
 
     def set_param(self, **param):
         """
         Tp_min, Tp_maxの代償関係についてのチェックは未実装
         Ea_min, Ea_maxの代償関係についてのチェックは未実装
         """
@@ -177,15 +177,15 @@
             list_ll = np.append(list_ll, (np.log(t) * intensity).sum())
 
         self.x0 = root[np.argmax(list_ll)]
         self.gamma = root2[np.argmax(list_ll)]
         return
 
     def _cm_step_eta(self, x, intensity):
-        eta = np.arange(0, 1, 0.01)
+        eta = np.arange(0.8, 1, 0.01)
         ll = []
         for i in range(eta.size):
             self.eta = eta[i]
             ll.append(self._LL(x, intensity))
         self.eta = eta[np.argmax(np.array(ll))]
         return
```

### Comparing `EMPeaks-2.0.2/EMPeaks/file_io.py` & `EMPeaks-2.1.0/EMPeaks/file_io.py`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/EMPeaks.egg-info/PKG-INFO` & `EMPeaks-2.1.0/EMPeaks.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 Metadata-Version: 2.1
 Name: EMPeaks
-Version: 2.0.2
+Version: 2.1.0
 Summary: 'high-throughput spectrum peak modeling tools by using Spectrum adapted EM algorithms'
-Home-page: UNKNOWN
 Author: Yasunobu Ando
 Author-email: yasunobu.ando@aist.go.jp
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 EMPeaks
 ========================
 
 This package is for high-throughput peak analysis by using Spectrum Adapted EM algorithm.
 Please refer the following paper when using this package:
 [Sci. Tech. Adv. Mater. 20, 733-735 (2019).](https://www.tandfonline.com/doi/full/10.1080/14686996.2019.1620123);
-[STAM-method, in press]()
+[Sci. Tech. Adv. Mater. method 1, 45 (2021).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2021.1899449)
+
+## version 2.1.x (Background Subtraction)
+In version 2.1.x, Automated background subtraction is implemented. Following background models are available now.
+* uniform: uniform background model
+* linear: linear background model (positive gradient)
+* ramp_sum: Ramp-Sum background model
+
+The details of these models are explained in this paper,
+[Sci. Tech. Adv. Mater. Method 3,  2159753 (2023).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2022.2159753)
+
+Background models are easily implemented into model instance as follows;
+```python
+from EMPeaks import GaussianMixture
+gmm = GaussianMixture.GaussianMixtureModel(K=3, background='uniform')
+```
+Keywords to set the background models are ```uniform```, ```linear```, ```ramp_sum```.
 
 ## version 2.0.x
 In version 2.0.x, Gaussian Mixture Model (GMM), Lorentzian Mixture Model (LMM), 
 Pseudo Voigt Mixture model (PVMM), and Doniach-Sunijic Miture model (DSMM).
 In principle, these combination models are also available but not implemented yet.
 
 From this version, each model has the same functions but differ from version 1, 
@@ -65,8 +78,7 @@
 After fitting, you can plot both raw data and fitted model as follows:
 ```python
 gmm.plot(x, y)
 ```
 
 ---------------
 &copy; 2020-2021 National Institute of Advanced Industrial Science and Technology (AIST)
-
```

### Comparing `EMPeaks-2.0.2/EMPeaks.egg-info/SOURCES.txt` & `EMPeaks-2.1.0/EMPeaks.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup.cfg
 ./EMPeaks/__init__.py
 ./EMPeaks/file_io.py
 ./EMPeaks.egg-info/PKG-INFO
 ./EMPeaks.egg-info/SOURCES.txt
 ./EMPeaks.egg-info/dependency_links.txt
 ./EMPeaks.egg-info/top_level.txt
+./EMPeaks/Background/__init__.py
+./EMPeaks/Background/_background.py
 ./EMPeaks/DoniachSunjicMixture/__init__.py
 ./EMPeaks/DoniachSunjicMixture/_doniachsunjic.py
 ./EMPeaks/DoniachSunjicMixture/_dsmm.py
 ./EMPeaks/GaussianMixture/__init__.py
 ./EMPeaks/GaussianMixture/_em.py
 ./EMPeaks/GaussianMixture/_gaussian.py
 ./EMPeaks/GaussianMixture/_gmm.py
```

### Comparing `EMPeaks-2.0.2/LICENSE` & `EMPeaks-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EMPeaks-2.0.2/PKG-INFO` & `EMPeaks-2.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 Metadata-Version: 2.1
 Name: EMPeaks
-Version: 2.0.2
+Version: 2.1.0
 Summary: 'high-throughput spectrum peak modeling tools by using Spectrum adapted EM algorithms'
-Home-page: UNKNOWN
 Author: Yasunobu Ando
 Author-email: yasunobu.ando@aist.go.jp
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 EMPeaks
 ========================
 
 This package is for high-throughput peak analysis by using Spectrum Adapted EM algorithm.
 Please refer the following paper when using this package:
 [Sci. Tech. Adv. Mater. 20, 733-735 (2019).](https://www.tandfonline.com/doi/full/10.1080/14686996.2019.1620123);
-[STAM-method, in press]()
+[Sci. Tech. Adv. Mater. method 1, 45 (2021).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2021.1899449)
+
+## version 2.1.x (Background Subtraction)
+In version 2.1.x, Automated background subtraction is implemented. Following background models are available now.
+* uniform: uniform background model
+* linear: linear background model (positive gradient)
+* ramp_sum: Ramp-Sum background model
+
+The details of these models are explained in this paper,
+[Sci. Tech. Adv. Mater. Method 3,  2159753 (2023).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2022.2159753)
+
+Background models are easily implemented into model instance as follows;
+```python
+from EMPeaks import GaussianMixture
+gmm = GaussianMixture.GaussianMixtureModel(K=3, background='uniform')
+```
+Keywords to set the background models are ```uniform```, ```linear```, ```ramp_sum```.
 
 ## version 2.0.x
 In version 2.0.x, Gaussian Mixture Model (GMM), Lorentzian Mixture Model (LMM), 
 Pseudo Voigt Mixture model (PVMM), and Doniach-Sunijic Miture model (DSMM).
 In principle, these combination models are also available but not implemented yet.
 
 From this version, each model has the same functions but differ from version 1, 
@@ -65,8 +78,7 @@
 After fitting, you can plot both raw data and fitted model as follows:
 ```python
 gmm.plot(x, y)
 ```
 
 ---------------
 &copy; 2020-2021 National Institute of Advanced Industrial Science and Technology (AIST)
-
```

### Comparing `EMPeaks-2.0.2/README.md` & `EMPeaks-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 EMPeaks
 ========================
 
 This package is for high-throughput peak analysis by using Spectrum Adapted EM algorithm.
 Please refer the following paper when using this package:
 [Sci. Tech. Adv. Mater. 20, 733-735 (2019).](https://www.tandfonline.com/doi/full/10.1080/14686996.2019.1620123);
-[STAM-method, in press]()
+[Sci. Tech. Adv. Mater. method 1, 45 (2021).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2021.1899449)
+
+## version 2.1.x (Background Subtraction)
+In version 2.1.x, Automated background subtraction is implemented. Following background models are available now.
+* uniform: uniform background model
+* linear: linear background model (positive gradient)
+* ramp_sum: Ramp-Sum background model
+
+The details of these models are explained in this paper,
+[Sci. Tech. Adv. Mater. Method 3,  2159753 (2023).](https://www.tandfonline.com/doi/abs/10.1080/27660400.2022.2159753)
+
+Background models are easily implemented into model instance as follows;
+```python
+from EMPeaks import GaussianMixture
+gmm = GaussianMixture.GaussianMixtureModel(K=3, background='uniform')
+```
+Keywords to set the background models are ```uniform```, ```linear```, ```ramp_sum```.
 
 ## version 2.0.x
 In version 2.0.x, Gaussian Mixture Model (GMM), Lorentzian Mixture Model (LMM), 
 Pseudo Voigt Mixture model (PVMM), and Doniach-Sunijic Miture model (DSMM).
 In principle, these combination models are also available but not implemented yet.
 
 From this version, each model has the same functions but differ from version 1,
```

### Comparing `EMPeaks-2.0.2/setup.cfg` & `EMPeaks-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EMPeaks
-version = 2.0.2
+version = 2.1.0
 author = Yasunobu Ando
 author_email = yasunobu.ando@aist.go.jp
 description = 'high-throughput spectrum peak modeling tools by using Spectrum adapted EM algorithms'
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

