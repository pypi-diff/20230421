# Comparing `tmp/directdm-2.2.0.tar.gz` & `tmp/directdm-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/directdm-2.2.0.tar", last modified: Mon Nov 30 15:07:43 2020, max compression
+gzip compressed data, was "dist/directdm-2.2.1.tar", last modified: Fri Apr 21 21:17:49 2023, max compression
```

## Comparing `directdm-2.2.0.tar` & `directdm-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/
--rw-r--r--   0 jbrod     (1000) users      (100)      682 2020-11-30 15:07:43.000000 directdm-2.2.0/PKG-INFO
--rw-rw-r--   0 jbrod     (1000) users      (100)     2518 2018-09-13 15:27:57.000000 directdm-2.2.0/README.md
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm/
--rw-r--r--   0 jbrod     (1000) users      (100)      181 2019-05-08 14:58:03.000000 directdm-2.2.0/directdm/__init__.py
--rw-r--r--   0 jbrod     (1000) users      (100)       21 2020-11-30 15:06:11.000000 directdm-2.2.0/directdm/_version.py
--rw-r--r--   0 jbrod     (1000) users      (100)     2636 2019-05-08 14:58:03.000000 directdm-2.2.0/directdm/dm_eft.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm/match/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2018-09-12 06:19:27.000000 directdm-2.2.0/directdm/match/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)     8931 2020-11-22 18:32:18.000000 directdm-2.2.0/directdm/match/dim4_gauge_contribution.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm/num/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.0/directdm/num/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)    13526 2020-11-30 15:06:11.000000 directdm-2.2.0/directdm/num/num_input.py
--rw-r--r--   0 jbrod     (1000) users      (100)    18337 2020-11-30 15:06:11.000000 directdm-2.2.0/directdm/num/single_nucleon_form_factors.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm/run/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.0/directdm/run/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)    39413 2020-01-07 14:49:33.000000 directdm-2.2.0/directdm/run/adm.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   159997 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_g1.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   153526 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_g2.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_yb.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_yc.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_yt.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.0/directdm/run/full_adm_ytau.py
--rw-r--r--   0 jbrod     (1000) users      (100)    27624 2020-11-22 18:32:18.000000 directdm-2.2.0/directdm/run/rge.py
--rw-r--r--   0 jbrod     (1000) users      (100)   244363 2020-11-30 15:06:11.000000 directdm-2.2.0/directdm/wilson_coefficients.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/
--rw-rw-r--   0 jbrod     (1000) users      (100)      682 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/PKG-INFO
--rw-rw-r--   0 jbrod     (1000) users      (100)      669 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/SOURCES.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)        1 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/dependency_links.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)       23 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/requires.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)        9 2020-11-30 15:07:43.000000 directdm-2.2.0/directdm.egg-info/top_level.txt
--rw-r--r--   0 jbrod     (1000) users      (100)       38 2020-11-30 15:07:43.000000 directdm-2.2.0/setup.cfg
--rw-rw-r--   0 jbrod     (1000) users      (100)      885 2018-09-12 06:19:28.000000 directdm-2.2.0/setup.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/
+-rw-r--r--   0 jbrod     (1000) users      (100)      682 2023-04-21 21:17:49.000000 directdm-2.2.1/PKG-INFO
+-rw-rw-r--   0 jbrod     (1000) users      (100)     2518 2018-09-13 15:27:57.000000 directdm-2.2.1/README.md
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/
+-rw-r--r--   0 jbrod     (1000) users      (100)      181 2019-05-08 14:58:03.000000 directdm-2.2.1/directdm/__init__.py
+-rw-r--r--   0 jbrod     (1000) users      (100)       21 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/_version.py
+-rw-r--r--   0 jbrod     (1000) users      (100)     2636 2019-05-08 14:58:03.000000 directdm-2.2.1/directdm/dm_eft.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/match/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2018-09-12 06:19:27.000000 directdm-2.2.1/directdm/match/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)     8931 2020-11-22 18:32:18.000000 directdm-2.2.1/directdm/match/dim4_gauge_contribution.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/num/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.1/directdm/num/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)    17180 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/num/num_input.py
+-rw-r--r--   0 jbrod     (1000) users      (100)    18337 2020-11-30 15:06:11.000000 directdm-2.2.1/directdm/num/single_nucleon_form_factors.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/run/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.1/directdm/run/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)    33119 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/run/adm.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   159997 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_g1.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   153526 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_g2.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yb.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yc.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yt.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_ytau.py
+-rw-r--r--   0 jbrod     (1000) users      (100)    27580 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/run/rge.py
+-rw-r--r--   0 jbrod     (1000) users      (100)   245355 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/wilson_coefficients.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/
+-rw-rw-r--   0 jbrod     (1000) users      (100)      682 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/PKG-INFO
+-rw-rw-r--   0 jbrod     (1000) users      (100)      669 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)        1 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)       23 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/requires.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)        9 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/top_level.txt
+-rw-r--r--   0 jbrod     (1000) users      (100)       38 2023-04-21 21:17:49.000000 directdm-2.2.1/setup.cfg
+-rw-rw-r--   0 jbrod     (1000) users      (100)      885 2018-09-12 06:19:28.000000 directdm-2.2.1/setup.py
```

### Comparing `directdm-2.2.0/PKG-INFO` & `directdm-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: directdm
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python package for dark matter direct detection
 Home-page: https://directdm.github.io
 Author: Fady Bishara, Joachim Brod, Benjamin Grinstein, Jure Zupan
 Author-email: joachim.brod@uc.edu
 License: MIT
 Description:  This package contains classes for Wilson coefficients
                                    for dark matter -- standard model interactions,
```

### Comparing `directdm-2.2.0/README.md` & `directdm-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/dm_eft.py` & `directdm-2.2.1/directdm/dm_eft.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/match/dim4_gauge_contribution.py` & `directdm-2.2.1/directdm/match/dim4_gauge_contribution.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/num/num_input.py` & `directdm-2.2.1/directdm/num/num_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -94,30 +94,30 @@
         # PDG top quark pole mass
         self.input_parameters['mt_pole'] = 172.76
 
         # bottom quark mass, MS-bar
         self.input_parameters['mb_at_mb'] = 4.18
 
         # charm quark mass, MS-bar
-        self.input_parameters['mc_at_mc'] = 1.275
+        self.input_parameters['mc_at_mc'] = 1.27
 
         # strange quark mass, MS-bar at 2 GeV
         self.input_parameters['ms_at_2GeV'] = 0.093
 
         # down quark mass, MS-bar at 2 GeV
         self.input_parameters['md_at_2GeV'] = 0.00467
 
         # up quark mass, MS-bar at 2 GeV
         self.input_parameters['mu_at_2GeV'] = 0.00216
 
 
         ### Low-energy constants for chiral EFT ###
 
         # The strange electric charge radius squared [1/GeV^2]
-        self.input_parameters['rs2'] = -0.115
+        self.input_parameters['rs2'] = -0.114
 
         # gA
         self.input_parameters['gA'] = 1.2756
 
         # Delta u + Delta d
         self.input_parameters['DeltauDeltad'] = 0.440
 
@@ -238,14 +238,35 @@
                               'mub': self.input_parameters['mb_at_mb'],\
                               'muc': self.input_parameters['mc_at_mc']},\
                              self.input_parameters['mt_pole'], 6, 3)
         self.dependent_parameters['mt_at_mt_pole'] = self.input_parameters['mt_pole']\
             * (1 - 4/3*as6/np.pi - 9.125*(as6/np.pi)**2 - 80.405*(as6/np.pi)**3\
                + 0.0664 - 0.00115 * (self.input_parameters['Mh'] - 125))
 
+        # The running coupling (at LO, there are no finite threshold effects)
+
+        self.dependent_parameters['as_at_mb'] = rge.AlphaS(self.input_parameters['asMZ'],\
+                              self.input_parameters['Mz']).\
+                              run({'mtmt': self.input_parameters['mt_pole'],\
+                                   'mbmb': self.input_parameters['mb_at_mb'],\
+                                   'mcmc': self.input_parameters['mc_at_mc']},\
+                                  {'mut': self.input_parameters['mt_pole'],\
+                                   'mub': self.input_parameters['mb_at_mb'],\
+                                   'muc': self.input_parameters['mc_at_mc']},\
+                                  self.input_parameters['mb_at_mb'], 5, 1)
+
+        self.dependent_parameters['as_at_2GeV'] = rge.AlphaS(self.input_parameters['asMZ'],\
+                                self.input_parameters['Mz']).\
+                                run({'mtmt': self.input_parameters['mt_pole'],\
+                                     'mbmb': self.input_parameters['mb_at_mb'],\
+                                     'mcmc': self.input_parameters['mc_at_mc']},\
+                                    {'mut': self.input_parameters['mt_pole'],\
+                                     'mub': self.input_parameters['mb_at_mb'],\
+                                     'muc': 2},\
+                                    2, 3, 1)
 
         # The running masses
 
         def mt(mu, mut, mub, muc, nf, loop):
             return rge.M_Quark_MSbar('t', self.dependent_parameters['mt_at_mt_pole'],\
                                      self.input_parameters['mt_pole'],\
                                      self.input_parameters['asMZ'],\
@@ -300,14 +321,15 @@
 
 
         # top quark mass, MS-bar (converted to MSbar QCD and EW, and run to MZ at 1-loop QCD)
         self.dependent_parameters['mt_at_MZ'] = mt(self.input_parameters['Mz'],\
                                                    self.input_parameters['mt_pole'],\
                                                    self.input_parameters['mb_at_mb'],\
                                                    self.input_parameters['mc_at_mc'], 6, 1)
+
         self.dependent_parameters['mb_at_MZ'] = mb(self.input_parameters['Mz'],\
                                                    self.input_parameters['mb_at_mb'],\
                                                    self.input_parameters['mc_at_mc'], 5, 1)
         self.dependent_parameters['mc_at_MZ'] = mc(self.input_parameters['Mz'],\
                                                    self.input_parameters['mb_at_mb'],\
                                                    self.input_parameters['mc_at_mc'], 5, 1)
         self.dependent_parameters['ms_at_MZ'] = ms(self.input_parameters['Mz'],\
@@ -316,14 +338,24 @@
         self.dependent_parameters['md_at_MZ'] = md(self.input_parameters['Mz'],\
                                                    self.input_parameters['mb_at_mb'],\
                                                    self.input_parameters['mc_at_mc'], 5, 1)
         self.dependent_parameters['mu_at_MZ'] = mu(self.input_parameters['Mz'],\
                                                    self.input_parameters['mb_at_mb'],\
                                                    self.input_parameters['mc_at_mc'], 5, 1)
 
+        self.dependent_parameters['ms_at_mb'] = ms(self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mc_at_mc'], 5, 1)
+        self.dependent_parameters['md_at_mb'] = md(self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mc_at_mc'], 5, 1)
+        self.dependent_parameters['mu_at_mb'] = mu(self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mb_at_mb'],\
+                                                   self.input_parameters['mc_at_mc'], 5, 1)
+
 
         # Deltaup
         self.dependent_parameters['Deltaup'] = (   self.input_parameters['gA']\
                                                    + self.input_parameters['DeltauDeltad'])/2
 
         # Deltadp
         self.dependent_parameters['Deltadp'] = ( - self.input_parameters['gA']\
@@ -353,11 +385,46 @@
         # an
         self.dependent_parameters['an'] = self.input_parameters['mun']
 
         # F2sp
         self.dependent_parameters['F2sp'] = self.input_parameters['mus']
 
 
+        # Input parameters at MZ for electroweak RG evolution
+
+        # SU2 coupling
+        self.dependent_parameters['g2_at_MZ']\
+          = np.sqrt(4*np.pi/self.input_parameters['aMZinv']/self.input_parameters['sw2_MSbar'])
+
+        # U1 coupling
+        self.dependent_parameters['g1_at_MZ']\
+          = np.sqrt(self.dependent_parameters['g2_at_MZ']**2/(1/self.input_parameters['sw2_MSbar'] - 1))
+
+        # SU3 coupling
+        self.dependent_parameters['g3_at_MZ']\
+          = np.sqrt(4*np.pi*self.input_parameters['asMZ'])
+
+        # charm Yukawa
+        self.dependent_parameters['yc_at_MZ']\
+          = np.sqrt(np.sqrt(2)*self.input_parameters['GF'])*np.sqrt(2) * self.dependent_parameters['mc_at_MZ']
+
+        # bottom Yukawa
+        self.dependent_parameters['yb_at_MZ']\
+          = np.sqrt(np.sqrt(2)*self.input_parameters['GF'])*np.sqrt(2) * self.dependent_parameters['mb_at_MZ']
+
+        # tau Yukawa
+        self.dependent_parameters['ytau_at_MZ']\
+          = np.sqrt(np.sqrt(2)*self.input_parameters['GF'])*np.sqrt(2) * self.input_parameters['mtau']
+
+        # top Yukawa
+        self.dependent_parameters['yt_at_MZ']\
+          = np.sqrt(np.sqrt(2)*self.input_parameters['GF'])*np.sqrt(2) * self.dependent_parameters['mt_at_MZ']
+
+        # Higgs quartic coupling
+        self.dependent_parameters['lam_at_MZ']\
+          = 2*np.sqrt(2) * self.input_parameters['GF'] * self.input_parameters['Mh']**2
+
+
         # Update the dictionary with the dependent parameters
         self.input_parameters.update(self.dependent_parameters)
```

### Comparing `directdm-2.2.0/directdm/num/single_nucleon_form_factors.py` & `directdm-2.2.1/directdm/num/single_nucleon_form_factors.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/run/adm.py` & `directdm-2.2.1/directdm/run/adm.py`

 * *Files 22% similar despite different names*

```diff
@@ -108,20 +108,24 @@
     else:
         raise Exception("nf has to be 3, 4 or 5")
 
 
 def ADM_QED2(nf):
     """ Return the QED anomalous dimension in the DM-SM sector for nf flavor EFT at alpha^2 """
 
-    # Mixing of Q_{11}^(7) into Q_{5,f}^(7) and Q_{12}^(7) into Q_{6,f}^(7), adapted from Hill et al. [1409.8290]. 
-    gamma_gf = -8
-    gamma_QED2_gf = np.array([5*[gamma_gf]])
+    # Mixing of Q_{11}^(7) into Q_{5,f}^(7) and Q_{12}^(7) into Q_{6,f}^(7),
+    # now correctly adapted from Hill et al. [1409.8290]. 
+    Qu = 2/3
+    Qd = -1/3
+    Qe = -1
+    gamma_QED2_gf = np.array([[8*Qu**2, 8*Qd**2, 8*Qd**2, 8*Qu**2,\
+                              8*Qd**2, 8*Qe**2, 8*Qe**2, 8*Qe**2]])
     gamma_QED2_1 = np.zeros((86,163))
-    gamma_QED2_2 = np.hstack((np.zeros((1,38)),gamma_QED2_gf,np.zeros((1,120))))
-    gamma_QED2_3 = np.hstack((np.zeros((1,46)),gamma_QED2_gf,np.zeros((1,112))))
+    gamma_QED2_2 = np.hstack((np.zeros((1,38)),gamma_QED2_gf,np.zeros((1,117))))
+    gamma_QED2_3 = np.hstack((np.zeros((1,46)),gamma_QED2_gf,np.zeros((1,109))))
     gamma_QED2_4 = np.zeros((75,163))
     gamma_QED2 = np.vstack((gamma_QED2_1, gamma_QED2_2, gamma_QED2_3, gamma_QED2_4))
 
     if nf == 5:
         return gamma_QED2
     elif nf == 4:
         return np.delete(np.delete(gamma_QED2, [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
@@ -681,145 +685,7 @@
     elif nf == 4:
         return np.delete(np.delete(gamma_hat, np.r_[np.s_[24:32], np.s_[48:56],\
                                                     np.s_[64:80]], 1), [4, 9], 2)
     else:
         raise Exception("nf has to be 4 or 5")
 
 
-
-
-def ADT_QCD_LEPTON():
-    """ Return the QCD anomalous dimension tensor for nf flavor EFT,
-        for double insertions of DM-SM and SM-SM operators 
-
-    Our basis of operators below the electroweak scale includes a set of 12 dimension-eight operators,
-    with Wilson coefficients for Dirac DM
-
-    ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s', 'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s']
-
-    and by a subset of 18 SM operators, with Wilson coefficients
-
-    ['P62ue', 'P62umu', 'P62utau', 'P62de', 'P62dmu', 'P62dtau', 'P62se', 'P62smu', 'P62stau',
-     'P63eu', 'P63muu', 'P63tauu', 'P63ed', 'P63mud', 'P63taud', 'P63es', 'P63mus', 'P63taus']
-
-    The anomalous dimension tensor defined below uses the following subset of the dim.6 DM-SM basis,
-
-    ['C63e', 'C63mu', 'C63tau', 'C64e', 'C64mu', 'C64tau']
-
-    and the basis above.
-    """
-
-    # As input for the quark-mass ratios, we use the quark masses at MZ and the lepton masses
-    ip = Num_input()
-
-    mu = ip.mu_at_MZ
-    md = ip.md_at_MZ
-    ms = ip.ms_at_MZ
-    me = ip.me
-    mmu = ip.mmu
-    mtau = ip.mtau
-
-    # Create the ADT:
-
-    gamma_hat_P63eu_Q81u = np.hstack((-16 * me**2/mu**2, np.zeros(5)))
-    gamma_hat_P63muu_Q81u = np.hstack((np.zeros(1), -16 * mmu**2/mu**2, np.zeros(4)))
-    gamma_hat_P63tauu_Q81u = np.hstack((np.zeros(2), -16 * mtau**2/mu**2, np.zeros(3)))
-
-    gamma_hat_P63ed_Q81d = np.hstack((-16 * me**2/md**2, np.zeros(5)))
-    gamma_hat_P63mud_Q81d = np.hstack((np.zeros(1), -16 * mmu**2/md**2, np.zeros(4)))
-    gamma_hat_P63taud_Q81d = np.hstack((np.zeros(2), -16 * mtau**2/md**2, np.zeros(3)))
-
-    gamma_hat_P63es_Q81s = np.hstack((-16 * me**2/ms**2, np.zeros(5)))
-    gamma_hat_P63mus_Q81s = np.hstack((np.zeros(1), -16 * mmu**2/ms**2, np.zeros(4)))
-    gamma_hat_P63taus_Q81s = np.hstack((np.zeros(2), -16 * mtau**2/ms**2, np.zeros(3)))
-
-
-
-    gamma_hat_P63eu_Q82u = np.hstack((np.zeros(3), -16 * me**2/mu**2, np.zeros(2)))
-    gamma_hat_P63muu_Q82u = np.hstack((np.zeros(4), -16 * mmu**2/mu**2, np.zeros(1)))
-    gamma_hat_P63tauu_Q82u = np.hstack((np.zeros(5), -16 * mtau**2/mu**2))
-
-    gamma_hat_P63ed_Q82d = np.hstack((np.zeros(3), -16 * me**2/md**2, np.zeros(2)))
-    gamma_hat_P63mud_Q82d = np.hstack((np.zeros(4), -16 * mmu**2/md**2, np.zeros(1)))
-    gamma_hat_P63taud_Q82d = np.hstack((np.zeros(5), -16 * mtau**2/md**2))
-
-    gamma_hat_P63es_Q82s = np.hstack((np.zeros(3), -16 * me**2/ms**2, np.zeros(2)))
-    gamma_hat_P63mus_Q82s = np.hstack((np.zeros(4), -16 * mmu**2/ms**2, np.zeros(1)))
-    gamma_hat_P63taus_Q82s = np.hstack((np.zeros(5), -16 * mtau**2/ms**2))
-
-
-
-    gamma_hat_P62ue_Q83u = np.hstack((-16 * me**2/mu**2, np.zeros(5)))
-    gamma_hat_P62umu_Q83u = np.hstack((np.zeros(1), -16 * mmu**2/mu**2, np.zeros(4)))
-    gamma_hat_P62utau_Q83u = np.hstack((np.zeros(2), -16 * mtau**2/mu**2, np.zeros(3)))
-
-    gamma_hat_P62de_Q83d = np.hstack((-16 * me**2/md**2, np.zeros(5)))
-    gamma_hat_P62dmu_Q83d = np.hstack((np.zeros(1), -16 * mmu**2/md**2, np.zeros(4)))
-    gamma_hat_P62dtau_Q83d = np.hstack((np.zeros(2), -16 * mtau**2/md**2, np.zeros(3)))
-
-    gamma_hat_P62se_Q83s = np.hstack((-16 * me**2/ms**2, np.zeros(5)))
-    gamma_hat_P62smu_Q83s = np.hstack((np.zeros(1), -16 * mmu**2/ms**2, np.zeros(4)))
-    gamma_hat_P62stau_Q83s = np.hstack((np.zeros(2), -16 * mtau**2/ms**2, np.zeros(3)))
-
-
-
-    gamma_hat_P62ue_Q84u = np.hstack((np.zeros(3), -16 * me**2/mu**2, np.zeros(2)))
-    gamma_hat_P62umu_Q84u = np.hstack((np.zeros(4), -16 * mmu**2/mu**2, np.zeros(1)))
-    gamma_hat_P62utau_Q84u = np.hstack((np.zeros(5), -16 * mtau**2/mu**2))
-
-    gamma_hat_P62de_Q84d = np.hstack((np.zeros(3), -16 * me**2/md**2, np.zeros(2)))
-    gamma_hat_P62dmu_Q84d = np.hstack((np.zeros(4), -16 * mmu**2/md**2, np.zeros(1)))
-    gamma_hat_P62dtau_Q84d = np.hstack((np.zeros(5), -16 * mtau**2/md**2))
-
-    gamma_hat_P62se_Q84s = np.hstack((np.zeros(3), -16 * me**2/ms**2, np.zeros(2)))
-    gamma_hat_P62smu_Q84s = np.hstack((np.zeros(4), -16 * mmu**2/ms**2, np.zeros(1)))
-    gamma_hat_P62stau_Q84s = np.hstack((np.zeros(5), -16 * mtau**2/ms**2))
-
-
-
-    gamma_hat_Q81u = np.vstack((gamma_hat_P63eu_Q81u, gamma_hat_P63muu_Q81u,\
-                                gamma_hat_P63tauu_Q81u, np.zeros((15,6))))
-    gamma_hat_Q81d = np.vstack((np.zeros((3,6)), gamma_hat_P63ed_Q81d,\
-                                gamma_hat_P63mud_Q81d, gamma_hat_P63taud_Q81d, np.zeros((12,6))))
-    gamma_hat_Q81s = np.vstack((np.zeros((6,6)), gamma_hat_P63es_Q81s,\
-                                gamma_hat_P63mus_Q81s, gamma_hat_P63taus_Q81s, np.zeros((9,6))))
-
-    gamma_hat_Q82u = np.vstack((gamma_hat_P63eu_Q82u, gamma_hat_P63muu_Q82u,\
-                                gamma_hat_P63tauu_Q82u, np.zeros((15,6))))
-    gamma_hat_Q82d = np.vstack((np.zeros((3,6)), gamma_hat_P63ed_Q82d,\
-                                gamma_hat_P63mud_Q82d, gamma_hat_P63taud_Q82d, np.zeros((12,6))))
-    gamma_hat_Q82s = np.vstack((np.zeros((6,6)), gamma_hat_P63es_Q82s,\
-                                gamma_hat_P63mus_Q82s, gamma_hat_P63taus_Q82s, np.zeros((9,6))))
-
-    gamma_hat_Q83u = np.vstack((np.zeros((9,6)), gamma_hat_P62ue_Q83u,\
-                                gamma_hat_P62umu_Q83u, gamma_hat_P62utau_Q83u, np.zeros((6,6))))
-    gamma_hat_Q83d = np.vstack((np.zeros((12,6)), gamma_hat_P62de_Q83d,\
-                                gamma_hat_P62dmu_Q83d, gamma_hat_P62dtau_Q83d, np.zeros((3,6))))
-    gamma_hat_Q83s = np.vstack((np.zeros((15,6)), gamma_hat_P62se_Q83s,\
-                                gamma_hat_P62smu_Q83s, gamma_hat_P62stau_Q83s))
-
-    gamma_hat_Q84u = np.vstack((np.zeros((9,6)), gamma_hat_P62ue_Q84u,\
-                                gamma_hat_P62umu_Q84u, gamma_hat_P62utau_Q84u, np.zeros((6,6))))
-    gamma_hat_Q84d = np.vstack((np.zeros((12,6)), gamma_hat_P62de_Q84d,\
-                                gamma_hat_P62dmu_Q84d, gamma_hat_P62dtau_Q84d, np.zeros((3,6))))
-    gamma_hat_Q84s = np.vstack((np.zeros((15,6)), gamma_hat_P62se_Q84s,\
-                                gamma_hat_P62smu_Q84s, gamma_hat_P62stau_Q84s))
-
-
-
-
-    gamma_hat = np.array([gamma_hat_Q81u, gamma_hat_Q81d, gamma_hat_Q81s,\
-                          gamma_hat_Q82u, gamma_hat_Q82d, gamma_hat_Q82s,\
-                          gamma_hat_Q83u, gamma_hat_Q83d, gamma_hat_Q83s,\
-                          gamma_hat_Q84u, gamma_hat_Q84d, gamma_hat_Q84s])
-
-
-    # Return the tensor
-
-    # tensor, zeile, spalte
-
-    return gamma_hat
-
-
-
-
-
```

### Comparing `directdm-2.2.0/directdm/run/full_adm_g1.py` & `directdm-2.2.1/directdm/run/full_adm_g1.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/run/full_adm_g2.py` & `directdm-2.2.1/directdm/run/full_adm_g2.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/run/full_adm_yb.py` & `directdm-2.2.1/directdm/run/full_adm_yb.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/directdm/run/rge.py` & `directdm-2.2.1/directdm/run/rge.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,14 @@
         {'mtmt': 160.0, 'mbmb': 4.18, 'mcmc': 1.275}
 
         A dictionary of scales for each threshold should be given. E.g.
 
         {'mut': 160.0, 'mub': 5, 'muc': 1.3}
 
         (Depending on nf one or zero can be given)
-
-        The decoupling is always at mq(mq)
         """
         if nf == 6:
             as5_mut = self.__solve_rge_nf(self.asMZ, self.MZ, dict_mu['mut'], 5, loop)
             as6_mut = self.decouple_up_MSbar(as5_mut, dict_mu['mut'], dict_mh['mtmt'], 6, loop)
             return self.__solve_rge_nf(as6_mut, dict_mu['mut'], mu0, 6, loop)
         if nf == 5:
             return self.__solve_rge_nf(self.asMZ, self.MZ, mu0, 5, loop)
```

### Comparing `directdm-2.2.0/directdm/wilson_coefficients.py` & `directdm-2.2.1/directdm/wilson_coefficients.py`

 * *Files 18% similar despite different names*

```diff
@@ -309,179 +309,79 @@
         for wc_name in self.sm_lepton_name_list:
             if wc_name in coeff_dict.keys():
                 self.coeff_dict[wc_name] = coeff_dict[wc_name]
             else:
                 pass
 
 
-        # Issue a user warning if certain electron / muon Wilson coefficients are non-zero:
-
-        for wc_name in self.coeff_dict.keys():
-            if DM_type == "D":
-                for wc_name in ['C63e', 'C63mu', 'C64e', 'C64mu']:
-                    if self.coeff_dict[wc_name] != 0.:
-                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
-                    else:
-                        pass
-            elif DM_type == "M":
-                for wc_name in ['C64e', 'C64mu']:
-                    if self.coeff_dict[wc_name] != 0.:
-                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
-                    else:
-                        pass
-            elif DM_type == "C":
-                for wc_name in ['C62e', 'C62mu']:
-                    if self.coeff_dict[wc_name] != 0.:
-                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
-                    else:
-                        pass
-            elif DM_type == "R":
-                pass
-
-        # Create the np.array of coefficients:
-        self.coeff_list_dm_dim5_dim6_dim7 = np.array(dict_to_list(self.coeff_dict, self.wc_name_list))
-        self.coeff_list_dm_dim8 = np.array(dict_to_list(self.coeff_dict, self.wc8_name_list))
-        self.coeff_list_sm_lepton_dim6 = np.array(dict_to_list(self.coeff_dict, self.sm_lepton_name_list))
-
-
-
-        #---------------------------#
-        # The anomalous dimensions: #
-        #---------------------------#
-        if self.DM_type == "D":
-            self.gamma_QED = adm.ADM_QED(3)
-            self.gamma_QED2 = adm.ADM_QED2(3)
-            self.gamma_QCD = adm.ADM_QCD(3)
-            self.gamma_QCD2 = adm.ADM_QCD2(3)
-            self.gamma_QCD_dim8 = adm.ADM_QCD_dim8(3)
-        if self.DM_type == "M":
-            self.gamma_QED = np.delete(np.delete(adm.ADM_QED(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QED2 = np.delete(np.delete(adm.ADM_QED2(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QCD = np.delete(np.delete(adm.ADM_QCD(3), del_ind_list, 1), del_ind_list, 2)
-            self.gamma_QCD2 = np.delete(np.delete(adm.ADM_QCD2(3), del_ind_list, 1), del_ind_list, 2)
-            self.gamma_QCD_dim8 = np.delete(np.delete(adm.ADM_QCD_dim8(3), del_ind_list_dim_8, 0),\
-                                            del_ind_list_dim_8, 1)
-        if self.DM_type == "C":
-            self.gamma_QED = np.delete(np.delete(adm.ADM_QED(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QED2 = np.delete(np.delete(adm.ADM_QED2(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QCD = np.delete(np.delete(adm.ADM_QCD(3), del_ind_list, 1), del_ind_list, 2)
-            self.gamma_QCD2 = np.delete(np.delete(adm.ADM_QCD2(3), del_ind_list, 1), del_ind_list, 2)
-            self.gamma_QCD_dim8 = np.delete(np.delete(adm.ADM_QCD_dim8(3), del_ind_list_dim_8, 0),\
-                                            del_ind_list_dim_8, 1)
-        if self.DM_type == "R":
-            self.gamma_QED = np.delete(np.delete(adm.ADM_QED(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QED2 = np.delete(np.delete(adm.ADM_QED2(3), del_ind_list, 0), del_ind_list, 1)
-            self.gamma_QCD = np.delete(np.delete(adm.ADM_QCD(3), del_ind_list, 1), del_ind_list, 2)
-            self.gamma_QCD2 = np.delete(np.delete(adm.ADM_QCD2(3), del_ind_list, 1), del_ind_list, 2)
-
-
-    def run(self, mu_low=None):
-        """ Running of 3-flavor Wilson coefficients
-
-        Calculate the running from 2 GeV to mu_low [GeV; default 2 GeV] in the three-flavor theory. 
-
-        Return a dictionary of Wilson coefficients for the three-flavor Lagrangian
-        at scale mu_low (this is the default).
-        """
-        if mu_low is None:
-            mu_low=2
-
-        #-------------#
-        # The running #
-        #-------------#
-
-        alpha_at_mu = 1/self.ip['amtauinv']
-
-        as31 = rge.AlphaS(self.ip['asMZ'], self.ip['Mz'])
-        as31_high = as31.run({'mbmb': self.ip['mb_at_mb'], 'mcmc': self.ip['mc_at_mc']},\
-                             {'mub': self.ip['mb_at_mb'], 'muc': self.ip['mc_at_mc']}, 2, 3, 1)
-        as31_low = as31.run({'mbmb': self.ip['mb_at_mb'], 'mcmc': self.ip['mc_at_mc']},\
-                            {'mub': self.ip['mb_at_mb'], 'muc': self.ip['mc_at_mc']}, mu_low, 3, 1)
-        evolve1 = rge.RGE(self.gamma_QCD, 3)
-        evolve2 = rge.RGE(self.gamma_QCD2, 3)
-        if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            evolve8 = rge.RGE([self.gamma_QCD_dim8], 3)
-        else:
-            pass
-
-        C_at_mu_QCD = np.dot(evolve2.U0_as2(as31_high, as31_low),\
-                             np.dot(evolve1.U0(as31_high, as31_low),\
-                                    self.coeff_list_dm_dim5_dim6_dim7))
-        C_at_mu_QED = np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED)\
-                      * np.log(mu_low/2) * alpha_at_mu/(4*np.pi)\
-                    + np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED2)\
-                      * np.log(mu_low/2) * (alpha_at_mu/(4*np.pi))**2
-        if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            C_dim8_at_mu = np.dot(evolve8.U0(as31_high, as31_low), self.coeff_list_dm_dim8)
-        else:
-            pass
-
-        # Revert back to dictionary
-
-        dict_coeff_mu = list_to_dict(C_at_mu_QCD + C_at_mu_QED, self.wc_name_list)
-        if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            dict_dm_dim8 = list_to_dict(C_dim8_at_mu, self.wc8_name_list)
-            dict_coeff_mu.update(dict_dm_dim8)
-
-            dict_sm_lepton_dim6 = list_to_dict(self.coeff_list_sm_lepton_dim6, self.sm_lepton_name_list)
-            dict_coeff_mu.update(dict_sm_lepton_dim6)
-        else:
-            pass
-
-        return dict_coeff_mu
-
-
-
-    def _my_cNR(self, DM_mass, RGE=None, NLO=None, DOUBLE_WEAK=None):
+    def _my_cNR(self, DM_mass, NLO=None):
         """Calculate the coefficients of the NR operators, with momentum dependence factored out.
-    
-        DM_mass is the DM mass in GeV
 
-        RGE is a flag to turn RGE running on (True) or off (False). (Default True)
+        DM_mass is the DM mass in GeV
 
         If NLO is set to True, the coherently enhanced NLO terms for Q_9^(7) are added. (Default False)
 
-        If DOUBLE_WEAK is set to False, the weak mixing below the weak scale is set to zero. (Default True)
-
         Returns a dictionary of coefficients for the NR Lagrangian, 
-        as in 1308.6288, plus coefficients c13 -- c23, c100 for "spurious" long-distance operators
+        as in 1308.6288, plus coefficients for "spurious" long-distance operators
+
+        Note that all dependence on q^2, 1/q^2, 1/(m^2-q^2), q^2/(m^2-q^2) is taken care of
+        by defining spurious operators.
+        
+        Therefore, we need to split some of the coefficients
+        into the "pion part" etc. with the q-dependence factored out,
+        and introduce a few spurious "long-distance" operators.
+        
+        The coefficients cNR1 -- cNR14 correspond to the operators in 1611.00368 and 1308.6288
+        
+        Therefore, we define O6pi     = O6/(mpi^2+q^2); 
+                             O6eta    = O6/(meta^2+q^2);
+                             O6q2pi   = O6*q^2/(mpi^2+q^2);
+                             O6q2eta  = O6*q^2/(meta^2+q^2);
+                             O10pi    = O10/(mpi^2+q^2);
+                             O10eta   = O10/(meta^2+q^2);
+                             O10q2pi  = O10*q^2/(mpi^2+q^2);
+                             O10q2eta = O10*q^2/(meta^2+q^2);
+        
+        For the dipole interactions, these are the ones that have c2p1, c1N2, c2p2 as coefficients. 
+        Therefore, we define O5bq2  = O5/q^2; 
+                             O6bq2  = O6/q^2.
+                             O11bq2 = O11/q^2.
+        
+        For the tensors, O4 * q^2 appears as a leading contribution.
+        Therefore, we define O4q2 = O4 * q^2
+        
+        For the tensors, O1 * q^2 appears as a subleading contribution.
+        Therefore, we define O1q2 = O1 * q^2
 
         The possible names are
 
         ['cNR1p', 'cNR1n', 'cNR2p', 'cNR2n', 'cNR3p', 'cNR3n', 'cNR4p', 'cNR4n', 'cNR5p', 'cNR5n',
          'cNR6p', 'cNR6n', 'cNR7p', 'cNR7n', 'cNR8p', 'cNR8n', 'cNR9p', 'cNR9n', 'cNR10p', 'cNR10n',
-         'cNR11p', 'cNR11n', 'cNR12p', 'cNR12n', 'cNR13p', 'cNR13n', 'cNR14p', 'cNR14n', 'cNR15p', 'cNR15n',
-         'cNR16p', 'cNR16n', 'cNR17p', 'cNR17n', 'cNR18p', 'cNR18n', 'cNR19p', 'cNR19n', 'cNR20p', 'cNR20n',
-         'cNR21p', 'cNR21n', 'cNR22p', 'cNR22n', 'cNR23p', 'cNR23n', 'cNR100p', 'cNR100n', 'cNR104p', 'cNR104n']
+         'cNR11p', 'cNR11n', 'cNR12p', 'cNR12n', 'cNR13p', 'cNR13n', 'cNR14p', 'cNR14n',
+         'cNR6pip', 'cNR6pin', 'cNR6etap', 'cNR6etan',
+         'cNR6q2pip', 'cNR6q2pi', 'cNR6q2etap', 'cNR6q2etan', 'cNR10pip', 'cNR10pin',
+         'cNR10etap', 'cNR10etan', 'cNR10q2pip', 'cNR10q2pin', 'cNR10q2etap', 'cNR10q2etan',
+         'cNR5bq2p', 'cNR5bq2n', 'cNR6bq2p', 'cNR6bq2n', 'cNR11bq2p', 'cNR11bq2n',
+         'cNR1q2p', 'cNR1q2n', 'cNR4q2p', 'cNR4q2n']
         """
-        if RGE is None:
-            RGE = True
         if NLO is None:
             NLO = False
-        if DOUBLE_WEAK is None:
-            DOUBLE_WEAK = True
-
-        if DOUBLE_WEAK:
-            wmws = 1.
-        else:
-            wmws = 0.
 
         ### Input parameters ####
 
         mpi = self.ip['mpi0']
         mp = self.ip['mproton']
         mn = self.ip['mneutron']
         mN = (mp+mn)/2
 
         alpha = 1/self.ip['alowinv']
         GF = self.ip['GF']
 
-        as_2GeV = rge.AlphaS(self.ip['asMZ'],\
-                             self.ip['Mz']).run({'mbmb': self.ip['mb_at_mb'], 'mcmc': self.ip['mc_at_mc']},\
-                                                {'mub': self.ip['mb_at_mb'], 'muc': self.ip['mc_at_mc']}, 2, 3, 1)
+        as_2GeV = self.ip['as_at_2GeV']
+
         gs2_2GeV = 4*np.pi*as_2GeV
 
         # Quark masses at 2GeV
         mu = self.ip['mu_at_2GeV']
         md = self.ip['md_at_2GeV']
         ms = self.ip['ms_at_2GeV']
         mtilde = 1/(1/mu + 1/md + 1/ms)
@@ -603,184 +503,90 @@
         FTW2dn = FTwist2('d', 'n', self.ip).value_zero_mom()
         FTW2sn = FTwist2('s', 'n', self.ip).value_zero_mom()
 
         FTW2gn = FTwist2('g', 'n', self.ip).value_zero_mom()
 
         ### The coefficients ###
         #
-        # Note that all dependence on 1/q^2, 1/(m^2-q^2), q^2/(m^2-q^2) is taken care of
+        # Note that all dependence on q^2, 1/q^2, 1/(m^2-q^2), q^2/(m^2-q^2) is taken care of
         # by defining spurious operators.
         #
         # Therefore, we need to split some of the coefficients
         # into the "pion part" etc. with the q-dependence factored out,
         # and introduce a few spurious "long-distance" operators.
         #
-        # The coefficients cNR1 -- cNR12 correspond to the operators in 1611.00368 and 1308.6288
+        # The coefficients cNR1 -- cNR14 correspond to the operators in 1611.00368 and 1308.6288
         #
-        # Therefore, we define O13 = O6/(mpi^2+q^2); 
-        #                      O14 = O6/(meta^2+q^2);
-        #                      O15 = O6*q^2/(mpi^2+q^2);
-        #                      O16 = O6*q^2/(meta^2+q^2);
-        #                      O17 = O10/(mpi^2+q^2);
-        #                      O18 = O10/(meta^2+q^2);
-        #                      O19 = O10*q^2/(mpi^2+q^2);
-        #                      O20 = O10*q^2/(meta^2+q^2);
+        # Therefore, we define O6pi     = O6/(mpi^2+q^2); 
+        #                      O6eta    = O6/(meta^2+q^2);
+        #                      O6q2pi   = O6*q^2/(mpi^2+q^2);
+        #                      O6q2eta  = O6*q^2/(meta^2+q^2);
+        #                      O10pi    = O10/(mpi^2+q^2);
+        #                      O10eta   = O10/(meta^2+q^2);
+        #                      O10q2pi  = O10*q^2/(mpi^2+q^2);
+        #                      O10q2eta = O10*q^2/(meta^2+q^2);
         #
         # For the dipole interactions, these are the ones that have c2p1, c1N2, c2p2 as coefficients. 
-        # Therefore, we define O21 = O5/q^2; 
-        #                      O22 = O6/q^2.
-        #                      O23 = O11/q^2.
+        # Therefore, we define O5bq2  = O5/q^2; 
+        #                      O6bq2  = O6/q^2.
+        #                      O11bq2 = O11/q^2.
         # 
         # For the tensors, O4 * q^2 appears as a leading contribution.
-        # Therefore, we define O104 = O4 * q^2
+        # Therefore, we define O4q2 = O4 * q^2
         #
         # For the tensors, O1 * q^2 appears as a subleading contribution.
-        # Therefore, we define O100 = O1 * q^2
+        # Therefore, we define O1q2 = O1 * q^2
         #
         # q^2 is here always the spatial part!!! 
         #
 
-        if RGE:
-            c3mu_dict = self.run(2)
-        else:
-            c3mu_dict = self.coeff_dict
+        c3mu_dict = self.coeff_dict
 
         if self.DM_type == "D":
             my_cNR_dict = {
-            'cNR1p' :   F1up*(c3mu_dict['C61u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
-                      + F1dp*(c3mu_dict['C61d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
-                      + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63e'] * c3mu_dict['D63eu'])\
-                      + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63e'] * c3mu_dict['D63ed'])\
-                      + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63mu'] * c3mu_dict['D63muu'])\
-                      + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63mu'] * c3mu_dict['D63mud'])\
-                      + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63tau'] * c3mu_dict['D63tauu'])\
-                      + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63tau'] * c3mu_dict['D63taud'])\
+            'cNR1p' :   F1up*(c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
+                      + F1dp*(c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                       + FGp*c3mu_dict['C71']\
                       + FSup*c3mu_dict['C75u'] + FSdp*c3mu_dict['C75d'] + FSsp*c3mu_dict['C75s']\
                       - alpha/(2*np.pi*DM_mass)*c3mu_dict['C51']\
                       + 2*DM_mass * (F1up*c3mu_dict['C715u'] + F1dp*c3mu_dict['C715d'] + F1sp*c3mu_dict['C715s'])\
                       + FTW2up*c3mu_dict['C723u']\
                       + FTW2dp*c3mu_dict['C723d']\
                       + FTW2sp*c3mu_dict['C723s']\
                       + FTW2gp*c3mu_dict['C725'],
             'cNR2p' : 0,
-            'cNR3p' : F2sp * c3mu_dict['C61s'],
-            'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                           + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                           + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62stau']))\
+            'cNR3p' : F2sp*(c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                           + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                           + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']))\
                       - 2*alpha/np.pi * self.ip['mup']/mN * c3mu_dict['C51']\
                       + 8*(FT0up*c3mu_dict['C79u'] + FT0dp*c3mu_dict['C79d'] + FT0sp*c3mu_dict['C79s']),
             'cNR5p' : - 2*mN * (F1up*c3mu_dict['C719u'] + F1dp*c3mu_dict['C719d'] + F1sp*c3mu_dict['C719s']),
             'cNR6p' : mN/DM_mass * FGtildep * c3mu_dict['C74']\
                       -2*mN*((F1up+F2up)*c3mu_dict['C719u']\
                              + (F1dp+F2dp)*c3mu_dict['C719d']\
-                             + (F1sp+F2dp)*c3mu_dict['C719s'])\
-                      + mN/DM_mass * F2sp * c3mu_dict['C61s'],
-            'cNR7p' : - 2*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
-                           + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                           + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C83s'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62ue'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62de'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62se'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62umu'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62dmu'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62smu'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62utau'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62dtau'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62stau']))\
+                             + (F1sp+F2sp)*c3mu_dict['C719s'])\
+                      + mN/DM_mass*F2sp*(c3mu_dict['C61s']
+                                         - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR7p' : - 2*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
+                           + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
+                           + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
                       - 4*DM_mass * (FAup*c3mu_dict['C717u'] + FAdp*c3mu_dict['C717d'] + FAsp*c3mu_dict['C717s']),
-            'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])),
-            'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + (F1dp+F2dp)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + (F1sp+F2sp)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63es'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mus'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taus']))
-                      + 2*mN*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
-                              + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                              + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C83s'])\
-                              + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62ue'])\
-                              + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62de'])\
-                              + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62se'])\
-                              + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62umu'])\
-                              + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62dmu'])\
-                              + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62smu'])\
-                              + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62utau'])\
-                              + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62dtau'])\
-                              + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62stau']))/DM_mass\
+            'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
+            'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u']\
+                           - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + (F1dp+F2dp)*(c3mu_dict['C62d']\
+                           - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                         + (F1sp+F2sp)*(c3mu_dict['C62s']\
+                           - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s']))\
+                      + 2*mN*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
+                              + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
+                              + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
+                             /DM_mass\
                       - 4*mN * (FAup*c3mu_dict['C721u'] + FAdp*c3mu_dict['C721d'] + FAsp*c3mu_dict['C721s']),
             'cNR10p' : FGtildep * c3mu_dict['C73']\
                        -2*mN/DM_mass * (FT0up*c3mu_dict['C710u']\
                                         + FT0dp*c3mu_dict['C710d']\
                                         + FT0sp*c3mu_dict['C710s']),
             'cNR11p' : - mN/DM_mass * (FSup*c3mu_dict['C76u']\
                                        + FSdp*c3mu_dict['C76d']\
@@ -789,211 +595,90 @@
                         + 2*((FT0up-FT1up)*c3mu_dict['C710u']\
                              + (FT0dp-FT1dp)*c3mu_dict['C710d']\
                              + (FT0sp-FT1sp)*c3mu_dict['C710s'])\
                         - 2*mN * (  F1up*(c3mu_dict['C716u']+c3mu_dict['C720u'])\
                                   + F1dp*(c3mu_dict['C716d']+c3mu_dict['C720d'])\
                                   + F1sp*(c3mu_dict['C716s']+c3mu_dict['C720s'])),
             'cNR12p' : -8*(FT0up*c3mu_dict['C710u'] + FT0dp*c3mu_dict['C710d'] + FT0sp*c3mu_dict['C710s']),
-    
-            'cNR13p' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
-                       + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62dtau']),
-            'cNR14p' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
-                                     + FPdp_eta*c3mu_dict['C78d']\
-                                     + FPsp_eta*c3mu_dict['C78s'])\
-                       + FPpup_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdp_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpsp_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])\
-                       + 4*mN * (  FAup*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
+            'cNR13p' : 0.,
+            'cNR14p' : + 4*mN * (  FAup*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
                                  + FAdp*(c3mu_dict['C718d']+c3mu_dict['C722d'])\
                                  + FAsp*(c3mu_dict['C718s']+c3mu_dict['C722s'])),
-            'cNR15p' : mN/DM_mass * FGtildep_pion * c3mu_dict['C74'],
-            'cNR16p' : mN/DM_mass * FGtildep_eta * c3mu_dict['C74'],
-    
-            'cNR17p' : FPup_pion*c3mu_dict['C77u'] + FPdp_pion*c3mu_dict['C77d'],
-            'cNR18p' : FPup_eta*c3mu_dict['C77u'] + FPdp_eta*c3mu_dict['C77d'] + FPsp_eta*c3mu_dict['C77s'],
-            'cNR19p' : FGtildep_pion * c3mu_dict['C73'],
-            'cNR20p' : FGtildep_eta * c3mu_dict['C73'],
-    
-            'cNR21p' : mN* (2*alpha/np.pi*c3mu_dict['C51']),
-            'cNR22p' : -mN**2* (- 2*alpha/np.pi * self.ip['mup']/mN * c3mu_dict['C51']),
-            'cNR23p' : mN* (2*alpha/np.pi*c3mu_dict['C52']),
 
-            'cNR100p' : (  F1up*c3mu_dict['C719u']\
+            'cNR6pip' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
+                       + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
+            'cNR6etap' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
+                                     + FPdp_eta*c3mu_dict['C78d']\
+                                     + FPsp_eta*c3mu_dict['C78s'])\
+                       + FPpup_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdp_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                       + FPpsp_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']),
+            'cNR6q2pip' : mN/DM_mass * FGtildep_pion * c3mu_dict['C74'],
+            'cNR6q2etap' : mN/DM_mass * FGtildep_eta * c3mu_dict['C74'],
+    
+            'cNR10pip' : FPup_pion*c3mu_dict['C77u'] + FPdp_pion*c3mu_dict['C77d'],
+            'cNR10etap' : FPup_eta*c3mu_dict['C77u'] + FPdp_eta*c3mu_dict['C77d'] + FPsp_eta*c3mu_dict['C77s'],
+            'cNR10q2pip' : FGtildep_pion * c3mu_dict['C73'],
+            'cNR10q2etap' : FGtildep_eta * c3mu_dict['C73'],
+    
+            'cNR5bq2p' : mN* (2*alpha/np.pi*c3mu_dict['C51']),
+            'cNR6bq2p' : -mN**2* (- 2*alpha/np.pi * self.ip['mup']/mN * c3mu_dict['C51']),
+            'cNR11bq2p' : mN* (2*alpha/np.pi*c3mu_dict['C52']),
+
+            'cNR1q2p' : (  F1up*c3mu_dict['C719u']\
                          + F1dp*c3mu_dict['C719d']\
                          + F1sp*c3mu_dict['C719s'])/(2*DM_mass)\
-                        + (F1spslope - F2sp / mN**2/4) * c3mu_dict['C61s'],
-            'cNR104p' : 2*((F1up+F2up)*c3mu_dict['C719u']\
+                        + (F1spslope - F2sp / mN**2/4)
+                          * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4q2p' : 2*((F1up+F2up)*c3mu_dict['C719u']\
                            + (F1dp+F2dp)*c3mu_dict['C719d']\
-                           + (F1sp+F2dp)*c3mu_dict['C719s'])/mN\
-                        - 1/mN/DM_mass * F2sp * c3mu_dict['C61s'],
+                           + (F1sp+F2sp)*c3mu_dict['C719s'])/mN\
+                        - 1/mN/DM_mass * F2sp
+                          * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
 
 
 
 
-            'cNR1n' :   F1un*(c3mu_dict['C61u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
-                      + F1dn*(c3mu_dict['C61d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
+            'cNR1n' :   F1un*(c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
+                      + F1dn*(c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                       + FGn*c3mu_dict['C71']\
                       + FSun*c3mu_dict['C75u'] + FSdn*c3mu_dict['C75d'] + FSsn*c3mu_dict['C75s']\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63e'] * c3mu_dict['D63eu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63e'] * c3mu_dict['D63ed'])\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63mu'] * c3mu_dict['D63muu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63mu'] * c3mu_dict['D63mud'])\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63tau'] * c3mu_dict['D63tauu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C63tau'] * c3mu_dict['D63taud'])\
                       + 2*DM_mass * (F1un*c3mu_dict['C715u'] + F1dn*c3mu_dict['C715d'] + F1sn*c3mu_dict['C715s'])\
                       + FTW2un*c3mu_dict['C723u']\
                       + FTW2dn*c3mu_dict['C723d']\
                       + FTW2sn*c3mu_dict['C723s']\
                       + FTW2gn*c3mu_dict['C725'],
             'cNR2n' : 0,
-            'cNR3n' : F2sn * c3mu_dict['C61s'],
-            'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                           + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                           + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62stau']))\
+            'cNR3n' : F2sn*(c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                           + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                           + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']))\
                       - 2*alpha/np.pi * self.ip['mun']/mN * c3mu_dict['C51']\
                       + 8*(FT0un*c3mu_dict['C79u'] + FT0dn*c3mu_dict['C79d'] + FT0sn*c3mu_dict['C79s']),
             'cNR5n' : - 2*mN * (F1un*c3mu_dict['C719u'] + F1dn*c3mu_dict['C719d'] + F1sn*c3mu_dict['C719s']),
             'cNR6n' : mN/DM_mass * FGtilden * c3mu_dict['C74']\
                       -2*mN*((F1un+F2un)*c3mu_dict['C719u']\
                              + (F1dn+F2dn)*c3mu_dict['C719d']\
-                             + (F1sn+F2dn)*c3mu_dict['C719s'])\
-                      + mN/DM_mass * F2sn * c3mu_dict['C61s'],
-            'cNR7n' : - 2*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
-                           + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                           + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C83s'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62ue'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62de'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63e'] * c3mu_dict['D62se'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62umu'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62dmu'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63mu'] * c3mu_dict['D62smu'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62utau'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62dtau'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C63tau'] * c3mu_dict['D62stau']))\
+                             + (F1sn+F2sn)*c3mu_dict['C719s'])\
+                      + mN/DM_mass * F2sn
+                        * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR7n' : - 2*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
+                           + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
+                           + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
                       - 4*DM_mass * (FAun*c3mu_dict['C717u'] + FAdn*c3mu_dict['C717d']+ FAsn*c3mu_dict['C717s']),
-            'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])),
-            'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                         + (F1un+F2un)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + (F1dn+F2dn)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + (F1sn+F2sn)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63es'])\
-                         + (F1un+F2un)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + (F1dn+F2dn)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + (F1sn+F2sn)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mus'])\
-                         + (F1un+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + (F1dn+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taus']))
-                      + 2*mN*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
-                              + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                              + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C83s'])\
-                              + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62ue'])\
-                              + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62de'])\
-                              + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63e'] * c3mu_dict['D62se'])\
-                              + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62umu'])\
-                              + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62dmu'])\
-                              + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63mu'] * c3mu_dict['D62smu'])\
-                              + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62utau'])\
-                              + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62dtau'])\
-                              + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                      * c3mu_dict['C63tau'] * c3mu_dict['D62stau']))/DM_mass\
+            'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
+            'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                         + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s']))\
+                      + 2*mN*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
+                              + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
+                              + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
+                             /DM_mass\
                       - 4*mN * (FAun*c3mu_dict['C721u']\
                                 + FAdn*c3mu_dict['C721d']\
                                 + FAsn*c3mu_dict['C721s']),
             'cNR10n' : FGtilden * c3mu_dict['C73']\
                      -2*mN/DM_mass * (FT0un*c3mu_dict['C710u']\
                                       + FT0dn*c3mu_dict['C710d']\
                                       + FT0sn*c3mu_dict['C710s']),
@@ -1004,512 +689,281 @@
                        + 2*((FT0un-FT1un)*c3mu_dict['C710u']\
                             + (FT0dn-FT1dn)*c3mu_dict['C710d']\
                             + (FT0sn-FT1sn)*c3mu_dict['C710s'])\
                        - 2*mN * (  F1un*(c3mu_dict['C716u']+c3mu_dict['C720u'])\
                                  + F1dn*(c3mu_dict['C716d']+c3mu_dict['C720d'])\
                                  + F1sn*(c3mu_dict['C716s']+c3mu_dict['C720s'])),
             'cNR12n' : -8*(FT0un*c3mu_dict['C710u'] + FT0dn*c3mu_dict['C710d'] + FT0sn*c3mu_dict['C710s']),
-    
-            'cNR13n' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
-                       + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62dtau']),
-            'cNR14n' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
-                                     + FPdn_eta*c3mu_dict['C78d']\
-                                     + FPsn_eta*c3mu_dict['C78s'])\
-                       + FPpun_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdn_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpsn_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])\
-                       + 4*mN * (  FAun*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
+            'cNR13n' : 0.,
+            'cNR14n' :           + 4*mN * (  FAun*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
                                  + FAdn*(c3mu_dict['C718d']+c3mu_dict['C722d'])\
                                  + FAsn*(c3mu_dict['C718s']+c3mu_dict['C722s'])),
-            'cNR15n' : mN/DM_mass * FGtilden_pion * c3mu_dict['C74'],
-            'cNR16n' : mN/DM_mass * FGtilden_eta * c3mu_dict['C74'],
     
-            'cNR17n' : FPun_pion*c3mu_dict['C77u'] + FPdn_pion*c3mu_dict['C77d'],
-            'cNR18n' : FPun_eta*c3mu_dict['C77u'] + FPdn_eta*c3mu_dict['C77d'] + FPsn_eta*c3mu_dict['C77s'],
-            'cNR19n' : FGtilden_pion * c3mu_dict['C73'],
-            'cNR20n' : FGtilden_eta * c3mu_dict['C73'],
-    
-            'cNR21n' : 0,
-            'cNR22n' : -mN**2 * (- 2*alpha/np.pi * self.ip['mun']/mN * c3mu_dict['C51']),
-            'cNR23n' : 0,
+            'cNR6pin' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
+                       + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
+            'cNR6etan' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
+                                     + FPdn_eta*c3mu_dict['C78d']\
+                                     + FPsn_eta*c3mu_dict['C78s'])\
+                       + FPpun_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdn_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                       + FPpsn_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']),
+            'cNR6q2pin' : mN/DM_mass * FGtilden_pion * c3mu_dict['C74'],
+            'cNR6q2etan' : mN/DM_mass * FGtilden_eta * c3mu_dict['C74'],
+    
+            'cNR10pin' : FPun_pion*c3mu_dict['C77u'] + FPdn_pion*c3mu_dict['C77d'],
+            'cNR10etan' : FPun_eta*c3mu_dict['C77u'] + FPdn_eta*c3mu_dict['C77d'] + FPsn_eta*c3mu_dict['C77s'],
+            'cNR10q2pin' : FGtilden_pion * c3mu_dict['C73'],
+            'cNR10q2etan' : FGtilden_eta * c3mu_dict['C73'],
+    
+            'cNR5bq2n' : 0,
+            'cNR6bq2n' : -mN**2 * (- 2*alpha/np.pi * self.ip['mun']/mN * c3mu_dict['C51']),
+            'cNR11bq2n' : 0,
 
-            'cNR100n' : (  F1un*c3mu_dict['C719u']\
+            'cNR1q2n' : (  F1un*c3mu_dict['C719u']\
                          + F1dn*c3mu_dict['C719d']\
                          + F1sn*c3mu_dict['C719s'])/(2*DM_mass)\
-                        + (F1snslope - F2sn / mN**2/4) * c3mu_dict['C61s'],
-            'cNR104n' : 2*((F1un+F2un)*c3mu_dict['C719u']\
+                        + (F1snslope - F2sn / mN**2/4)
+                          * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4q2n' : 2*((F1un+F2un)*c3mu_dict['C719u']\
                            + (F1dn+F2dn)*c3mu_dict['C719d']\
-                           + (F1sn+F2dn)*c3mu_dict['C719s'])/mN\
-                        - 1/mN/DM_mass * F2sn * c3mu_dict['C61s']
+                           + (F1sn+F2sn)*c3mu_dict['C719s'])/mN\
+                        - 1/mN/DM_mass * F2sn
+                          * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s'])
             }
 
             if NLO:
-                my_cNR_dict['cNR5p'] = - 2*mN * (F1un*c3mu_dict['C719u']\
+                my_cNR_dict['cNR5p'] = my_cNR_dict['cNR5p']\
+                                       - 2*mN * (F1un*c3mu_dict['C719u']\
                                                  + F1dn*c3mu_dict['C719d']\
                                                  + F1sn*c3mu_dict['C719s'])\
                                        + 2*((FT0up-FT1up)*c3mu_dict['C79u']\
                                             + (FT0dp-FT1dp)*c3mu_dict['C79d']\
                                             + (FT0sp-FT1sp)*c3mu_dict['C79s'])
-                my_cNR_dict['cNR100p'] = - ((FT0up-FT1up)*c3mu_dict['C79u']\
+                my_cNR_dict['cNR1q2p'] = my_cNR_dict['cNR1q2p']\
+                                         - ((FT0up-FT1up)*c3mu_dict['C79u']\
                                             + (FT0dp-FT1dp)*c3mu_dict['C79d']\
                                             + (FT0sp-FT1sp)*c3mu_dict['C79s'])/(2*DM_mass*mN)
-                my_cNR_dict['cNR5n'] = - 2*mN * (F1un*c3mu_dict['C719u']\
+                my_cNR_dict['cNR5n'] = my_cNR_dict['cNR5n']\
+                                       - 2*mN * (F1un*c3mu_dict['C719u']\
                                                  + F1dn*c3mu_dict['C719d'] + F1sn*c3mu_dict['C719s'])\
                                        + 2*((FT0un-FT1un)*c3mu_dict['C79u']\
                                             + (FT0dn-FT1dn)*c3mu_dict['C79d']\
                                             + (FT0sn-FT1sn)*c3mu_dict['C79s'])
-                my_cNR_dict['cNR100n'] = - ((FT0un-FT1un)*c3mu_dict['C79u']\
+                my_cNR_dict['cNR1q2n'] = my_cNR_dict['cNR1q2n']\
+                                         - ((FT0un-FT1un)*c3mu_dict['C79u']\
                                             + (FT0dn-FT1dn)*c3mu_dict['C79d']\
                                             + (FT0sn-FT1sn)*c3mu_dict['C79s'])/(2*DM_mass*mN)
 
 
         if self.DM_type == "M":
             my_cNR_dict = {
             'cNR1p' : FGp*c3mu_dict['C71']\
                       + FSup*c3mu_dict['C75u'] + FSdp*c3mu_dict['C75d'] + FSsp*c3mu_dict['C75s']\
                       + 2*DM_mass * (F1up*c3mu_dict['C715u'] + F1dp*c3mu_dict['C715d'] + F1sp*c3mu_dict['C715s']),
             'cNR2p' : 0,
             'cNR3p' : 0,
-            'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                           + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                           + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                           + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                           + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                           + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])),
+            'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                           + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                           + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s'])),
             'cNR5p' : 0,
             'cNR6p' : mN/DM_mass * FGtildep * c3mu_dict['C74'],
             'cNR7p' : - 4*DM_mass * (FAup*c3mu_dict['C717u'] + FAdp*c3mu_dict['C717d'] + FAsp*c3mu_dict['C717s']),
-            'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])),
-            'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + (F1dp+F2dp)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + (F1sp+F2sp)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63es'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mus'])\
-                         + (F1up+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + (F1dp+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taus'])),
+            'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
+            'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + (F1dp+F2dp)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                         + (F1sp+F2sp)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR10p' : FGtildep * c3mu_dict['C73'],
             'cNR11p' : - mN/DM_mass * (FSup*c3mu_dict['C76u']\
                                        + FSdp*c3mu_dict['C76d']\
                                        + FSsp*c3mu_dict['C76s'])\
                        - mN/DM_mass * FGp * c3mu_dict['C72']\
                        - 2*mN * (  F1up*c3mu_dict['C716u']\
                                    + F1dp*c3mu_dict['C716d']\
                                    + F1sp*c3mu_dict['C716s']),
             'cNR12p' : 0,
-    
-            'cNR13p' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
-                       + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpup_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdp_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62dtau']),
-            'cNR14p' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
-                                     + FPdp_eta*c3mu_dict['C78d']\
-                                     + FPsp_eta*c3mu_dict['C78s'])\
-                       + FPpup_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdp_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpsp_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                       + FPpup_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                       + FPpsp_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])\
-                       + 4*mN * (FAup*c3mu_dict['C718u']\
+            'cNR13p' : 0.,
+            'cNR14p' : + 4*mN * (FAup*c3mu_dict['C718u']\
                                  + FAdp*c3mu_dict['C718d']\
                                  + FAsp*c3mu_dict['C718s']),
-            'cNR15p' : mN/DM_mass * FGtildep_pion * c3mu_dict['C74'],
-            'cNR16p' : mN/DM_mass * FGtildep_eta * c3mu_dict['C74'],
     
-            'cNR17p' : FPup_pion*c3mu_dict['C77u'] + FPdp_pion*c3mu_dict['C77d'],
-            'cNR18p' : FPup_eta*c3mu_dict['C77u'] + FPdp_eta*c3mu_dict['C77d'] + FPsp_eta*c3mu_dict['C77s'],
-            'cNR19p' : FGtildep_pion * c3mu_dict['C73'],
-            'cNR20p' : FGtildep_eta * c3mu_dict['C73'],
-    
-            'cNR21p' : 0,
-            'cNR22p' : 0,
-            'cNR23p' : 0,
+            'cNR6pip' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
+                       + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
+            'cNR6etap' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
+                                     + FPdp_eta*c3mu_dict['C78d']\
+                                     + FPsp_eta*c3mu_dict['C78s'])\
+                       + FPpup_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdp_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                       + FPpsp_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']),
+            'cNR6q2pip' : mN/DM_mass * FGtildep_pion * c3mu_dict['C74'],
+            'cNR6q2etap' : mN/DM_mass * FGtildep_eta * c3mu_dict['C74'],
+    
+            'cNR10pip' : FPup_pion*c3mu_dict['C77u'] + FPdp_pion*c3mu_dict['C77d'],
+            'cNR10etap' : FPup_eta*c3mu_dict['C77u'] + FPdp_eta*c3mu_dict['C77d'] + FPsp_eta*c3mu_dict['C77s'],
+            'cNR10q2pip' : FGtildep_pion * c3mu_dict['C73'],
+            'cNR10q2etap' : FGtildep_eta * c3mu_dict['C73'],
+    
+            'cNR5bq2p' : 0,
+            'cNR6bq2p' : 0,
+            'cNR11bq2p' : 0,
 
-            'cNR100p' : 0,
-            'cNR104p' : 0,
+            'cNR1q2p' : 0,
+            'cNR4q2p' : 0,
 
 
 
 
             'cNR1n' :   FGn*c3mu_dict['C71']\
                       + FSun*c3mu_dict['C75u'] + FSdn*c3mu_dict['C75d'] + FSsn*c3mu_dict['C75s']\
                       + 2*DM_mass * (F1un*c3mu_dict['C715u'] + F1dn*c3mu_dict['C715d'] + F1sn*c3mu_dict['C715s']),
             'cNR2n' : 0,
             'cNR3n' : 0,
-            'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                           + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                           + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                           + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                           + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                           + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                   * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])),
+            'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                           + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                           + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s'])),
             'cNR5n' : 0,
             'cNR6n' : mN/DM_mass * FGtilden * c3mu_dict['C74'],
             'cNR7n' : - 4*DM_mass * (FAun*c3mu_dict['C717u'] + FAdn*c3mu_dict['C717d'] + FAsn*c3mu_dict['C717s']),
-            'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                 * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])),
-            'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
-                         + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
-                         + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                         + (F1un+F2un)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63eu'])\
-                         + (F1dn+F2dn)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63ed'])\
-                         + (F1sn+F2sn)*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64e'] * c3mu_dict['D63es'])\
-                         + (F1un+F2un)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63muu'])\
-                         + (F1dn+F2dn)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mud'])\
-                         + (F1sn+F2sn)*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64mu'] * c3mu_dict['D63mus'])\
-                         + (F1un+F2up)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63tauu'])\
-                         + (F1dn+F2dp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taud'])\
-                         + (F1sp+F2sp)*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                        * c3mu_dict['C64tau'] * c3mu_dict['D63taus'])),
+            'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
+            'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                         + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                         + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR10n' : FGtilden * c3mu_dict['C73'],
             'cNR11n' : - mN/DM_mass * (FSun*c3mu_dict['C76u']\
                                        + FSdn*c3mu_dict['C76d']\
                                        + FSsn*c3mu_dict['C76s'])\
                        - mN/DM_mass * FGn * c3mu_dict['C72']\
                        - 2*mN * (  F1un*c3mu_dict['C716u']\
                                    + F1dn*c3mu_dict['C716d']\
                                    + F1sn*c3mu_dict['C716s']),
             'cNR12n' : 0,
-    
-            'cNR13n' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
-                       + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpun_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdn_pion*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                     * c3mu_dict['C64tau'] * c3mu_dict['D62dtau']),
-            'cNR14n' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
-                                     + FPdn_eta*c3mu_dict['C78d']\
-                                     + FPsn_eta*c3mu_dict['C78s'])\
-                       + FPpun_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
-                       + FPpdn_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
-                       + FPpsn_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C84s'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62ue'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62de'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64e'] * c3mu_dict['D62se'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62umu'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62dmu'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64mu'] * c3mu_dict['D62smu'])\
-                       + FPpun_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62utau'])\
-                       + FPpdn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62dtau'])\
-                       + FPpsn_eta*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                    * c3mu_dict['C64tau'] * c3mu_dict['D62stau'])\
-                       + 4*mN * (FAun*c3mu_dict['C718u']\
+            'cNR13p' : 0.,
+            'cNR14n' : + 4*mN * (FAun*c3mu_dict['C718u']\
                                  + FAdn*c3mu_dict['C718d']\
                                  + FAsn*c3mu_dict['C718s']),
-            'cNR15n' : mN/DM_mass * FGtilden_pion * c3mu_dict['C74'],
-            'cNR16n' : mN/DM_mass * FGtilden_eta * c3mu_dict['C74'],
-    
-            'cNR17n' : FPun_pion*c3mu_dict['C77u'] + FPdn_pion*c3mu_dict['C77d'],
-            'cNR18n' : FPun_eta*c3mu_dict['C77u'] + FPdn_eta*c3mu_dict['C77d'] + FPsn_eta*c3mu_dict['C77s'],
-            'cNR19n' : FGtilden_pion * c3mu_dict['C73'],
-            'cNR20n' : FGtilden_eta * c3mu_dict['C73'],
     
-            'cNR21n' : 0,
-            'cNR22n' : 0,
-            'cNR23n' : 0,
+            'cNR6pin' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
+                       + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
+            'cNR6etan' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
+                                     + FPdn_eta*c3mu_dict['C78d']\
+                                     + FPsn_eta*c3mu_dict['C78s'])\
+                       + FPpun_eta*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
+                       + FPpdn_eta*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
+                       + FPpsn_eta*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']),
+            'cNR6q2pin' : mN/DM_mass * FGtilden_pion * c3mu_dict['C74'],
+            'cNR6q2etan' : mN/DM_mass * FGtilden_eta * c3mu_dict['C74'],
+    
+            'cNR10pin' : FPun_pion*c3mu_dict['C77u'] + FPdn_pion*c3mu_dict['C77d'],
+            'cNR10etan' : FPun_eta*c3mu_dict['C77u'] + FPdn_eta*c3mu_dict['C77d'] + FPsn_eta*c3mu_dict['C77s'],
+            'cNR10q2pin' : FGtilden_pion * c3mu_dict['C73'],
+            'cNR10q2etan' : FGtilden_eta * c3mu_dict['C73'],
+    
+            'cNR5bq2n' : 0,
+            'cNR6bq2n' : 0,
+            'cNR11bq2n' : 0,
 
-            'cNR100n' : 0,
-            'cNR104n' : 0
+            'cNR1q2n' : 0,
+            'cNR4q2n' : 0
             }
 
 
         if self.DM_type == "C":
             my_cNR_dict = {
-            'cNR1p' :    F1up * (c3mu_dict['C61u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
-                       + F1dp * (c3mu_dict['C61d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
-                       + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62e'] * c3mu_dict['D63eu'])\
-                       + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62e'] * c3mu_dict['D63ed'])\
-                       + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62mu'] * c3mu_dict['D63muu'])\
-                       + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62mu'] * c3mu_dict['D63mud'])\
-                       + F1up*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62tau'] * c3mu_dict['D63tauu'])\
-                       + F1dp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                               * c3mu_dict['C62tau'] * c3mu_dict['D63taud'])\
+            'cNR1p' :    F1up * (c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
+                       + F1dp * (c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                        + FGp*c3mu_dict['C65']/2/DM_mass\
                        + (FSup*c3mu_dict['C63u'] + FSdp*c3mu_dict['C63d'] + FSsp*c3mu_dict['C63s'])/2/DM_mass,
             'cNR2p' : 0,
-            'cNR3p' : F2sp * c3mu_dict['C61s'],
+            'cNR3p' : F2sp * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR4p' : 0,
             'cNR5p' : 0,
             'cNR6p' : 0,
             'cNR7p' : -2*(  FAup * (c3mu_dict['C62u']\
-                                    - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                                    - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                           + FAdp * (c3mu_dict['C62d']\
-                                    - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                                    - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                           + FAsp * (c3mu_dict['C62s']\
-                                    - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                          + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62ue'])\
-                          + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62de'])\
-                          + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62se'])\
-                          + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62umu'])\
-                          + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62dmu'])\
-                          + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62smu'])\
-                          + FAup*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62utau'])\
-                          + FAdp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62dtau'])\
-                          + FAsp*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62stau'])),
+                                    - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR8p' : 0,
             'cNR9p' : 0,
             'cNR10p' : FGtildep * c3mu_dict['C66']/2/DM_mass,
             'cNR11p' : 0,
             'cNR12p' : 0,
-
-            'cNR13p' : 0,
+            'cNR13p' : 0.,
             'cNR14p' : 0,
-            'cNR15p' : 0,
-            'cNR16p' : 0,
+
+            'cNR6pip' : 0,
+            'cNR6etap' : 0,
+            'cNR6q2pip' : 0,
+            'cNR6q2etap' : 0,
     
-            'cNR17p' : (FPup_pion*c3mu_dict['C64u'] + FPdp_pion*c3mu_dict['C64d'])/2/DM_mass,
-            'cNR18p' : (  FPup_eta*c3mu_dict['C64u']\
+            'cNR10pip' : (FPup_pion*c3mu_dict['C64u'] + FPdp_pion*c3mu_dict['C64d'])/2/DM_mass,
+            'cNR10etap' : (  FPup_eta*c3mu_dict['C64u']\
                         + FPdp_eta*c3mu_dict['C64d']\
                         + FPsp_eta*c3mu_dict['C64s'])/2/DM_mass,
-            'cNR19p' : FGtildep_pion * c3mu_dict['C66']/2/DM_mass,
-            'cNR20p' : FGtildep_eta * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2pip' : FGtildep_pion * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2etap' : FGtildep_eta * c3mu_dict['C66']/2/DM_mass,
     
-            'cNR21p' : 0,
-            'cNR22p' : 0,
-            'cNR23p' : 0,
-
-            'cNR100p' : (F1spslope - 1/mN**2/4 * F2sp) * c3mu_dict['C61s'],
-            'cNR104p' : 0,
+            'cNR5bq2p' : 0,
+            'cNR6bq2p' : 0,
+            'cNR11bq2p' : 0,
+
+            'cNR1q2p' : (F1spslope - 1/mN**2/4 * F2sp)
+                        * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4q2p' : 0,
 
 
 
 
-            'cNR1n' :   F1un * (c3mu_dict['C61u'] - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
-                      + F1dn * (c3mu_dict['C61d'] - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62e'] * c3mu_dict['D63eu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62e'] * c3mu_dict['D63ed'])\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62mu'] * c3mu_dict['D63muu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62mu'] * c3mu_dict['D63mud'])\
-                      + F1un*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62tau'] * c3mu_dict['D63tauu'])\
-                      + F1dn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                              * c3mu_dict['C62tau'] * c3mu_dict['D63taud'])\
+            'cNR1n' :   F1un * (c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
+                      + F1dn * (c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                       + FGn*c3mu_dict['C65']/2/DM_mass\
                       + (FSun*c3mu_dict['C63u'] + FSdn*c3mu_dict['C63d'] + FSsn*c3mu_dict['C63s'])/2/DM_mass,
             'cNR2n' : 0,
-            'cNR3n' : F2sp * c3mu_dict['C61s'],
+            'cNR3n' : F2sp * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR4n' : 0,
             'cNR5n' : 0,
             'cNR6n' : 0,
             'cNR7n' : -2*(  FAun * (c3mu_dict['C62u']\
-                                    - np.sqrt(2)*GF*wmws*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
+                                    - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                           + FAdn * (c3mu_dict['C62d']\
-                                    - np.sqrt(2)*GF*wmws*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
+                                    - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                           + FAsn * (c3mu_dict['C62s']\
-                                    - np.sqrt(2)*GF*wmws*ms**2 / gs2_2GeV * c3mu_dict['C82s'])\
-                          + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62ue'])\
-                          + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62de'])\
-                          + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * me**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62e'] * c3mu_dict['D62se'])\
-                          + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62umu'])\
-                          + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62dmu'])\
-                          + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mmu**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62mu'] * c3mu_dict['D62smu'])\
-                          + FAun*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62utau'])\
-                          + FAdn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62dtau'])\
-                          + FAsn*(np.sqrt(2)*GF*wmws/np.pi**2 * mtau**2 * np.log(2/MZ)\
-                                  * c3mu_dict['C62tau'] * c3mu_dict['D62stau'])),
+                                    - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR8n' : 0,
             'cNR9n' : 0,
             'cNR10n' : FGtilden * c3mu_dict['C66']/2/DM_mass,
             'cNR11n' : 0,
             'cNR12n' : 0,
-
-            'cNR13n' : 0,
+            'cNR13p' : 0.,
             'cNR14n' : 0,
-            'cNR15n' : 0,
-            'cNR16n' : 0,
+
+            'cNR6pin' : 0,
+            'cNR6etan' : 0,
+            'cNR6q2pin' : 0,
+            'cNR6q2etan' : 0,
     
-            'cNR17n' : (FPun_pion*c3mu_dict['C64u'] + FPdn_pion*c3mu_dict['C64d'])/2/DM_mass,
-            'cNR18n' : (  FPun_eta*c3mu_dict['C64u']\
+            'cNR10pin' : (FPun_pion*c3mu_dict['C64u'] + FPdn_pion*c3mu_dict['C64d'])/2/DM_mass,
+            'cNR10etan' : (  FPun_eta*c3mu_dict['C64u']\
                         + FPdn_eta*c3mu_dict['C64d']\
                         + FPsn_eta*c3mu_dict['C64s'])/2/DM_mass,
-            'cNR19n' : FGtilden_pion * c3mu_dict['C66']/2/DM_mass,
-            'cNR20n' : FGtilden_eta * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2pin' : FGtilden_pion * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2etan' : FGtilden_eta * c3mu_dict['C66']/2/DM_mass,
     
-            'cNR21n' : 0,
-            'cNR22n' : 0,
-            'cNR23n' : 0,
-
-            'cNR100n' : (F1snslope - 1/mN**2/4 * F2sn) * c3mu_dict['C61s'],
-            'cNR104n' : 0
+            'cNR5bq2n' : 0,
+            'cNR6bq2n' : 0,
+            'cNR11bq2n' : 0,
+
+            'cNR1q2n' : (F1snslope - 1/mN**2/4 * F2sn)
+                        * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
+            'cNR4q2n' : 0
             }
 
 
         if self.DM_type == "R":
             my_cNR_dict = {
             'cNR1p' :   FSup*c3mu_dict['C63u']/2/DM_mass\
                       + FSdp*c3mu_dict['C63d']/2/DM_mass\
@@ -1522,33 +976,35 @@
             'cNR6p' : 0,
             'cNR7p' : 0,
             'cNR8p' : 0,
             'cNR9p' : 0,
             'cNR10p' : FGtildep * c3mu_dict['C66']/2/DM_mass,
             'cNR11p' : 0,
             'cNR12p' : 0,
-
-            'cNR13p' : 0,
+            'cNR13p' : 0.,
             'cNR14p' : 0,
-            'cNR15p' : 0,
-            'cNR16p' : 0,
+
+            'cNR6pip' : 0,
+            'cNR6etap' : 0,
+            'cNR6q2pip' : 0,
+            'cNR6q2etap' : 0,
     
-            'cNR17p' : (FPup_pion*c3mu_dict['C64u'] + FPdp_pion*c3mu_dict['C64d'])/2/DM_mass,
-            'cNR18p' :   FPup_eta*c3mu_dict['C64u']/2/DM_mass\
+            'cNR10pip' : (FPup_pion*c3mu_dict['C64u'] + FPdp_pion*c3mu_dict['C64d'])/2/DM_mass,
+            'cNR10etap' :   FPup_eta*c3mu_dict['C64u']/2/DM_mass\
                        + FPdp_eta*c3mu_dict['C64d']/2/DM_mass\
                        + FPsp_eta*c3mu_dict['C64s']/2/DM_mass,
-            'cNR19p' : FGtildep_pion * c3mu_dict['C66']/2/DM_mass,
-            'cNR20p' : FGtildep_eta * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2pip' : FGtildep_pion * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2etap' : FGtildep_eta * c3mu_dict['C66']/2/DM_mass,
     
-            'cNR21p' : 0,
-            'cNR22p' : 0,
-            'cNR23p' : 0,
+            'cNR5bq2p' : 0,
+            'cNR6bq2p' : 0,
+            'cNR11bq2p' : 0,
 
-            'cNR100p' : 0,
-            'cNR104p' : 0,
+            'cNR1q2p' : 0,
+            'cNR4q2p' : 0,
 
 
 
 
             'cNR1n' :   FSun*c3mu_dict['C63u']/2/DM_mass\
                       + FSdn*c3mu_dict['C63d']/2/DM_mass\
                       + FSsn*c3mu_dict['C63s']/2/DM_mass\
@@ -1560,176 +1016,176 @@
             'cNR6n' : 0,
             'cNR7n' : 0,
             'cNR8n' : 0,
             'cNR9n' : 0,
             'cNR10n' : FGtilden * c3mu_dict['C66']/2/DM_mass,
             'cNR11n' : 0,
             'cNR12n' : 0,
-
-            'cNR13n' : 0,
+            'cNR13p' : 0.,
             'cNR14n' : 0,
-            'cNR15n' : 0,
-            'cNR16n' : 0,
+
+            'cNR6pin' : 0,
+            'cNR6etan' : 0,
+            'cNR6q2pin' : 0,
+            'cNR6q2etan' : 0,
     
-            'cNR17n' : (FPun_pion*c3mu_dict['C64u'] + FPdn_pion*c3mu_dict['C64d'])/2/DM_mass,
-            'cNR18n' :   FPun_eta*c3mu_dict['C64u']/2/DM_mass\
+            'cNR10pin' : (FPun_pion*c3mu_dict['C64u'] + FPdn_pion*c3mu_dict['C64d'])/2/DM_mass,
+            'cNR10etan' :   FPun_eta*c3mu_dict['C64u']/2/DM_mass\
                        + FPdn_eta*c3mu_dict['C64d']/2/DM_mass\
                        + FPsn_eta*c3mu_dict['C64s']/2/DM_mass,
-            'cNR19n' : FGtilden_pion * c3mu_dict['C66']/2/DM_mass,
-            'cNR20n' : FGtilden_eta * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2pin' : FGtilden_pion * c3mu_dict['C66']/2/DM_mass,
+            'cNR10q2etan' : FGtilden_eta * c3mu_dict['C66']/2/DM_mass,
     
-            'cNR21n' : 0,
-            'cNR22n' : 0,
-            'cNR23n' : 0,
+            'cNR5bq2n' : 0,
+            'cNR6bq2n' : 0,
+            'cNR11bq2n' : 0,
 
-            'cNR100n' : 0,
-            'cNR104n' : 0
+            'cNR1q2n' : 0,
+            'cNR4q2n' : 0
             }
 
 
         return my_cNR_dict
 
 
-    def cNR(self, DM_mass, q, RGE=None, NLO=None, DOUBLE_WEAK=None):
-        """ The operator coefficients of O_1^N -- O_12^N as in 1308.6288 
+    def cNR(self, DM_mass, q, NLO=None):
+        """ The operator coefficients of O_1^N -- O_12^N, O_14^N as in 1308.6288 
 
-        (multiply by propagators and sum up contributions)
+        (including pion propagator contributions)
 
         DM_mass is the DM mass in GeV
 
-        RGE is an optional argument to turn RGE running on (True) or off (False). (Default True)
-
         If NLO is set to True, the coherently enhanced NLO terms for Q_9^(7) are added. (Default False)
 
         Returns a dictionary of coefficients for the NR Lagrangian, 
-        cNR1 -- cNR12, as in 1308.6288
+        cNR1 -- cNR14, as in 1308.6288
 
         The possible names are
 
         ['cNR1p', 'cNR1n', 'cNR2p', 'cNR2n', 'cNR3p', 'cNR3n', 'cNR4p', 'cNR4n', 'cNR5p', 'cNR5n',
          'cNR6p', 'cNR6n', 'cNR7p', 'cNR7n', 'cNR8p', 'cNR8n', 'cNR9p', 'cNR9n', 'cNR10p', 'cNR10n',
-         'cNR11p', 'cNR11n', 'cNR12p', 'cNR12n']
+         'cNR11p', 'cNR11n', 'cNR12p', 'cNR12n', 'cNR13p', 'cNR13n', 'cNR14p', 'cNR14n']
         """
-        if RGE is None:
-            RGE = True
         if NLO is None:
             NLO = False
-        if DOUBLE_WEAK is None:
-            DOUBLE_WEAK = True
 
         meta = self.ip['meta']
         mpi = self.ip['mpi0']
 
         qsq = q**2
 
         # The traditional coefficients, where different from above
         cNR_dict = {}
-        my_cNR = self._my_cNR(DM_mass, RGE, NLO, DOUBLE_WEAK)
+        my_cNR = self._my_cNR(DM_mass, NLO)
 
         # Add meson- / photon-pole contributions
-        cNR_dict['cNR1p'] = my_cNR['cNR1p'] + qsq * my_cNR['cNR100p']
+        cNR_dict['cNR1p'] = my_cNR['cNR1p'] + qsq * my_cNR['cNR1q2p']
         cNR_dict['cNR2p'] = my_cNR['cNR2p']
         cNR_dict['cNR3p'] = my_cNR['cNR3p']
-        cNR_dict['cNR4p'] = my_cNR['cNR4p'] + qsq * my_cNR['cNR104p']
-        cNR_dict['cNR5p'] = my_cNR['cNR5p'] + 1/qsq * my_cNR['cNR21p']
+        cNR_dict['cNR4p'] = my_cNR['cNR4p'] + qsq * my_cNR['cNR4q2p']
+        cNR_dict['cNR5p'] = my_cNR['cNR5p'] + 1/qsq * my_cNR['cNR5bq2p']
         cNR_dict['cNR6p'] = my_cNR['cNR6p']\
-                            + 1/(mpi**2 + qsq) * my_cNR['cNR13p']\
-                            + 1/(meta**2 + qsq) * my_cNR['cNR14p']\
-                            + qsq/(mpi**2 + qsq) * my_cNR['cNR15p']\
-                            + qsq/(meta**2 + qsq) * my_cNR['cNR16p']\
-                            + 1/qsq * my_cNR['cNR22p']
+                            + 1/(mpi**2 + qsq) * my_cNR['cNR6pip']\
+                            + 1/(meta**2 + qsq) * my_cNR['cNR6etap']\
+                            + qsq/(mpi**2 + qsq) * my_cNR['cNR6q2pip']\
+                            + qsq/(meta**2 + qsq) * my_cNR['cNR6q2etap']\
+                            + 1/qsq * my_cNR['cNR6bq2p']
         cNR_dict['cNR7p'] = my_cNR['cNR7p']
         cNR_dict['cNR8p'] = my_cNR['cNR8p']
         cNR_dict['cNR9p'] = my_cNR['cNR9p']
         cNR_dict['cNR10p'] = my_cNR['cNR10p']\
-                             + 1/(mpi**2 + qsq) * my_cNR['cNR17p']\
-                             + 1/(meta**2 + qsq) * my_cNR['cNR18p']\
-                             + qsq/(mpi**2 + qsq) * my_cNR['cNR19p']\
-                             + qsq/(meta**2 + qsq) * my_cNR['cNR20p']
-        cNR_dict['cNR11p'] = my_cNR['cNR11p'] + 1/qsq * my_cNR['cNR23p']
+                             + 1/(mpi**2 + qsq) * my_cNR['cNR10pip']\
+                             + 1/(meta**2 + qsq) * my_cNR['cNR10etap']\
+                             + qsq/(mpi**2 + qsq) * my_cNR['cNR10q2pip']\
+                             + qsq/(meta**2 + qsq) * my_cNR['cNR10q2etap']
+        cNR_dict['cNR11p'] = my_cNR['cNR11p'] + 1/qsq * my_cNR['cNR11bq2p']
         cNR_dict['cNR12p'] = my_cNR['cNR12p']
+        cNR_dict['cNR13p'] = my_cNR['cNR13p']
+        cNR_dict['cNR14p'] = my_cNR['cNR14p']
 
-        cNR_dict['cNR1n'] = my_cNR['cNR1n'] + qsq * my_cNR['cNR100n']
+        cNR_dict['cNR1n'] = my_cNR['cNR1n'] + qsq * my_cNR['cNR1q2n']
         cNR_dict['cNR2n'] = my_cNR['cNR2n']
         cNR_dict['cNR3n'] = my_cNR['cNR3n']
-        cNR_dict['cNR4n'] = my_cNR['cNR4n'] + qsq * my_cNR['cNR104n']
-        cNR_dict['cNR5n'] = my_cNR['cNR5n'] + 1/qsq * my_cNR['cNR21n']
+        cNR_dict['cNR4n'] = my_cNR['cNR4n'] + qsq * my_cNR['cNR4q2n']
+        cNR_dict['cNR5n'] = my_cNR['cNR5n'] + 1/qsq * my_cNR['cNR5bq2n']
         cNR_dict['cNR6n'] = my_cNR['cNR6n']\
-                            + 1/(mpi**2 + qsq) * my_cNR['cNR13n']\
-                            + 1/(meta**2 + qsq) * my_cNR['cNR14n']\
-                            + qsq/(mpi**2 + qsq) * my_cNR['cNR15n']\
-                            + qsq/(meta**2 + qsq) * my_cNR['cNR16n']\
-                            + 1/qsq * my_cNR['cNR22n']
+                            + 1/(mpi**2 + qsq) * my_cNR['cNR6pin']\
+                            + 1/(meta**2 + qsq) * my_cNR['cNR6etan']\
+                            + qsq/(mpi**2 + qsq) * my_cNR['cNR6q2pin']\
+                            + qsq/(meta**2 + qsq) * my_cNR['cNR6q2etan']\
+                            + 1/qsq * my_cNR['cNR6bq2n']
         cNR_dict['cNR7n'] = my_cNR['cNR7n']
         cNR_dict['cNR8n'] = my_cNR['cNR8n']
         cNR_dict['cNR9n'] = my_cNR['cNR9n']
         cNR_dict['cNR10n'] = my_cNR['cNR10n']\
-                             + 1/(mpi**2 + qsq) * my_cNR['cNR17n']\
-                             + 1/(meta**2 + qsq) * my_cNR['cNR18n']\
-                             + qsq/(mpi**2 + qsq) * my_cNR['cNR19n']\
-                             + qsq/(meta**2 + qsq) * my_cNR['cNR20n']
-        cNR_dict['cNR11n'] = my_cNR['cNR11n'] + 1/qsq * my_cNR['cNR23n']
+                             + 1/(mpi**2 + qsq) * my_cNR['cNR10pin']\
+                             + 1/(meta**2 + qsq) * my_cNR['cNR10etan']\
+                             + qsq/(mpi**2 + qsq) * my_cNR['cNR10q2pin']\
+                             + qsq/(meta**2 + qsq) * my_cNR['cNR10q2etan']
+        cNR_dict['cNR11n'] = my_cNR['cNR11n'] + 1/qsq * my_cNR['cNR11bq2n']
         cNR_dict['cNR12n'] = my_cNR['cNR12n']
+        cNR_dict['cNR13n'] = my_cNR['cNR13n']
+        cNR_dict['cNR14n'] = my_cNR['cNR14n']
 
         return cNR_dict
 
 
-    def write_mma(self, DM_mass, qvec, RGE=None, NLO=None, DOUBLE_WEAK=None, path=None, filename=None):
+    def write_mma(self, DM_mass, qvec, NLO=None, path=None, filename=None):
         """ Write a text file with the NR coefficients that can be read into DMFormFactor 
 
         The order is {cNR1p, cNR2p, ... , cNR1n, cNR2n, ... }
 
         Mandatory arguments are the DM mass DM_mass (in GeV) and the spatial momentum transfer qvec (in GeV) 
 
         <path> should be a string with the path (including the trailing "/") where the file should be saved
         (default is './')
 
         <filename> is the filename (default 'cNR.m')
         """
-        if RGE is None:
-            RGE=True
         if NLO is None:
             NLO=False
-        if DOUBLE_WEAK is None:
-            DOUBLE_WEAK = True
         if path is None:
             path = './'
         assert type(path) is str
         if path.endswith('/'):
             pass
         else:
             path += '/'
         if filename is None:
             filename = 'cNR.m'
 
-        val = self.cNR(DM_mass, qvec, RGE, NLO)
+        val = self.cNR(DM_mass, qvec, NLO)
         self.cNR_list_mma = '{' + str(val['cNR1p']) + ', '\
                             + str(val['cNR2p']) + ', '\
                             + str(val['cNR3p']) + ', '\
                             + str(val['cNR4p']) + ', '\
                             + str(val['cNR5p']) + ', '\
                             + str(val['cNR6p']) + ', '\
                             + str(val['cNR7p']) + ', '\
                             + str(val['cNR8p']) + ', '\
                             + str(val['cNR9p']) + ', '\
                             + str(val['cNR10p']) + ', '\
                             + str(val['cNR11p']) + ', '\
                             + str(val['cNR12p']) + ', '\
+                            + str(val['cNR13p']) + ', '\
+                            + str(val['cNR14p']) + ', '\
                             + str(val['cNR1n']) + ', '\
                             + str(val['cNR2n']) + ', '\
                             + str(val['cNR3n']) + ', '\
                             + str(val['cNR4n']) + ', '\
                             + str(val['cNR5n']) + ', '\
                             + str(val['cNR6n']) + ', '\
                             + str(val['cNR7n']) + ', '\
                             + str(val['cNR8n']) + ', '\
                             + str(val['cNR9n']) + ', '\
                             + str(val['cNR10n']) + ', '\
                             + str(val['cNR11n']) + ', '\
-                            + str(val['cNR12n']) + '}' + '\n'
+                            + str(val['cNR12n']) + ', '\
+                            + str(val['cNR13n']) + ', '\
+                            + str(val['cNR14n']) + '}' + '\n'
 
         output_file = str(os.path.expanduser(path)) + filename
 
         with open(output_file,'w') as f:
             f.write(self.cNR_list_mma)
 
 
@@ -1832,15 +1288,15 @@
         The third argument is a dictionary with all input parameters.
 
 
         The class has four methods: 
 
         run
         ---
-        Run the Wilson from mb(mb) to mu_low [GeV; default 2 GeV], with 4 active quark flavors
+        Run the Wilson from mb(mb) to 2 GeV, with 4 active quark flavors
 
         match
         -----
         Match the Wilson coefficients from 4-flavor to 3-flavor QCD, at scale mu [GeV; default 2 GeV]
 
         cNR
         ---
@@ -2061,14 +1517,39 @@
         for wc_name in self.sm_lepton_name_list:
             if wc_name in coeff_dict.keys():
                 self.coeff_dict[wc_name] = coeff_dict[wc_name]
             else:
                 self.coeff_dict[wc_name] = 0.
 
 
+        # Issue a user warning if certain electron / muon Wilson coefficients are non-zero:
+
+        for wc_name in self.coeff_dict.keys():
+            if DM_type == "D":
+                for wc_name in ['C63e', 'C63mu', 'C64e', 'C64mu']:
+                    if self.coeff_dict[wc_name] != 0.:
+                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
+                    else:
+                        pass
+            elif DM_type == "M":
+                for wc_name in ['C64e', 'C64mu']:
+                    if self.coeff_dict[wc_name] != 0.:
+                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
+                    else:
+                        pass
+            elif DM_type == "C":
+                for wc_name in ['C62e', 'C62mu']:
+                    if self.coeff_dict[wc_name] != 0.:
+                        warnings.warn('The RG result for ' + wc_name + ' is incomplete, expect large uncertainties!')
+                    else:
+                        pass
+            elif DM_type == "R":
+                pass
+
+
         # Create the np.array of coefficients:
         self.coeff_list_dm_dim5_dim6_dim7 = np.array(dict_to_list(self.coeff_dict, self.wc_name_list))
         self.coeff_list_dm_dim8 = np.array(dict_to_list(self.coeff_dict, self.wc8_name_list))
         self.coeff_list_sm_dim6 = np.array(dict_to_list(self.coeff_dict, self.sm_name_list))
         self.coeff_list_sm_lepton_dim6 = np.array(dict_to_list(self.coeff_dict, self.sm_lepton_name_list))
 
 
@@ -2128,15 +1609,16 @@
             DM_dim6_init = np.delete(self.coeff_list_dm_dim5_dim6_dim7, np.r_[np.s_[0:7], np.s_[11:86]])
         elif self.DM_type == "C":
             DM_dim6_init = np.delete(self.coeff_list_dm_dim5_dim6_dim7, np.r_[np.s_[0:7], np.s_[11:40]])
 
 
 
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            # The columns of ADM_eff correspond to SM6 operators; the rows of ADM_eff correspond to DM8 operators; 
+            # The columns of ADM_eff correspond to SM6 operators;
+            # the rows of ADM_eff correspond to DM8 operators; 
             C6_dot_ADM_hat = np.transpose(np.tensordot(DM_dim6_init, self.gamma_hat, (0,2)))
 
             # The effective ADM
             #
             # Note that the mixing of the SM operators with four equal flavors
             # does not contribute if we neglect yu, yd, ys! 
             self.ADM_eff = [np.vstack((np.hstack((self.ADM_SM,\
@@ -2146,84 +1628,63 @@
                                                             len(self.coeff_list_sm_dim6))),\
                                                   self.gamma_QCD_dim8))))]
         if self.DM_type == "R":
             pass
 
 
 
-    def run(self, mu_low=None, double_QCD=None):
+    def run(self):
         """ Running of 4-flavor Wilson coefficients
 
         Calculate the running from mb(mb) to mu_low [GeV; default 2 GeV] in the four-flavor theory. 
 
         Return a dictionary of Wilson coefficients for the four-flavor Lagrangian
         at scale mu_low.
         """
-        if mu_low is None:
-            mu_low=2
-        if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            if double_QCD is None:
-                double_QCD=True
-        else:
-            double_QCD=False
+        mu_low=2
 
 
         #-------------#
         # The running #
         #-------------#
 
         mb = self.ip['mb_at_mb']
         alpha_at_mc = 1/self.ip['aMZinv']
-        as_2GeV = rge.AlphaS(self.ip['asMZ'],\
-                             self.ip['Mz']).run({'mbmb': self.ip['mb_at_mb'],\
-                                                 'mcmc': self.ip['mc_at_mc']},\
-                                                {'mub': self.ip['mb_at_mb'],\
-                                                 'muc': self.ip['mc_at_mc']}, 2, 3, 1)
+        as_mb = self.ip['as_at_mb']
+        as_2GeV = self.ip['as_at_2GeV']
         gs2_2GeV = 4*np.pi*as_2GeV
 
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            if double_QCD:
-                adm_eff = self.ADM_eff
-            else:
-                projector = np.vstack((np.hstack((np.zeros((64,64)),\
-                                                  np.ones((64,12)))),\
-                                       np.zeros((12,76))))
-                adm_eff = [np.multiply(projector, self.ADM_eff[0])]
+            adm_eff = self.ADM_eff
         else:
             pass
 
-        as41 = rge.AlphaS(self.ip['asMZ'], self.ip['Mz'])
-        as41_high = as41.run({'mbmb': self.ip['mb_at_mb'], 'mcmc': self.ip['mc_at_mc']},\
-                             {'mub': self.ip['mb_at_mb'], 'muc': self.ip['mc_at_mc']}, mb, 4, 1)
-        as41_low = as41.run({'mbmb': self.ip['mb_at_mb'], 'mcmc': self.ip['mc_at_mc']},\
-                            {'mub': self.ip['mb_at_mb'], 'muc': self.ip['mc_at_mc']}, mu_low, 4, 1)
-
         evolve1 = rge.RGE(self.gamma_QCD, 4)
         evolve2 = rge.RGE(self.gamma_QCD2, 4)
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             evolve8 = rge.RGE(adm_eff, 4)
         else:
             pass
 
         # Mixing in the dim.6 DM-SM sector
         #
-        C_at_mc_QCD = np.dot(evolve2.U0_as2(as41_high, as41_low),\
-                             np.dot(evolve1.U0(as41_high, as41_low),\
+        C_at_mc_QCD = np.dot(evolve2.U0_as2(as_mb, as_2GeV),\
+                             np.dot(evolve1.U0(as_mb, as_2GeV),\
                                     self.coeff_list_dm_dim5_dim6_dim7))
         C_at_mc_QED = np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED)\
                       * np.log(mu_low/mb) * alpha_at_mc/(4*np.pi)\
                       + np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED2)\
                       * np.log(mu_low/mb) * (alpha_at_mc/(4*np.pi))**2
 
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             # Mixing in the dim.6 SM-SM and dim.8 DM-SM sector
 
             DIM6_DIM8_init = np.hstack((self.coeff_list_sm_dim6, self.coeff_list_dm_dim8))
 
-            DIM6_DIM8_at_mb =   np.dot(evolve8.U0(as41_high, as41_low), DIM6_DIM8_init)
+            DIM6_DIM8_at_mb =   np.dot(evolve8.U0(as_mb, as_2GeV), DIM6_DIM8_init)
 
         # Revert back to dictionary
 
         dict_coeff_mc = list_to_dict(C_at_mc_QCD + C_at_mc_QED, self.wc_name_list)
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             dict_dm_dim8 = list_to_dict(np.delete(DIM6_DIM8_at_mb, np.s_[0:64]), self.wc8_name_list)
             dict_sm_dim6 = list_to_dict(np.delete(DIM6_DIM8_at_mb, np.s_[64:70]), self.sm_name_list)
@@ -2233,92 +1694,456 @@
             dict_coeff_mc.update(dict_sm_dim6)
             dict_coeff_mc.update(dict_sm_lepton_dim6)
 
         return dict_coeff_mc
 
 
 
-    def match(self, RGE=None, double_QCD=None, mu=None):
+    def match(self, RGE=None):
         """ Match from four-flavor to three-flavor QCD
 
-        Calculate the matching at mu [GeV; default 2 GeV].
+        Calculate the matching at 2 GeV.
 
         Returns a dictionary of Wilson coefficients for the three-flavor Lagrangian
         at scale mu. The SM-SM Wilson coefficients are NOT returned. 
 
         RGE is an optional argument to turn RGE running on (True) or off (False). (Default True)
+
+
+        ***********************************************************
+
+        Here is an explanation how I implemented the "double weak insertions"
+        for leptons, since these details are not quite spelled out
+        (although implied) in 1801.04240.
+
+        For definiteness, equation numbers correspond to the JHEP version.
+
+        We can just imagine that there is a QCD running in this case
+        (or replace gs by el in all definitions), and then truncate
+        the RG running at the leading term. Effectively, this generates a matching
+        contribution to the dimension-eight operators proportional to a log(mu_high/mu_low).
+
+        We will generate this matching contribution at each of the flavor thresholds
+        (by default, mc, and 2 GeV). This is still not technically correct, as the
+        contribution should only arise via matching to the 3-flavor theory. However,
+        since the dimension-eight Wilson coefficient are not used anywhere else,
+        this should not lead to any problems. Moreover, in this way we automatically
+        obtain the correct logarithm in the NR coefficient when starting at the different
+        EFTs.
+
+        The matching contributions then read explicitly (recall that our DM Wilson
+        coefficients are dimensionful):
+
+        C81q(mu_low) = - 1 / \pi^2 \sum_l m_l^2 \log(mu_low/mu_high)
+                       * C63l(mu_high) * D63lq * gs^2/mq^2
+
+        C82q(mu_low) = - 1 / \pi^2 \sum_l m_l^2 \log(mu_low/mu_high)
+                       * C64l(mu_high) * D63lq * gs^2/mq^2
+
+        C83q(mu_low) = - 1 / \pi^2 \sum_l m_l^2 \log(mu_low/mu_high)
+                       * C63l(mu_high) * D62lq * gs^2/mq^2
+
+        C84q(mu_low) = - 1 / \pi^2 \sum_l m_l^2 \log(mu_low/mu_high)
+                       * C64l(mu_high) * D62lq * gs^2/mq^2
+
+        The NR coefficients are then given by Eq.s (5.5)--(5.10),
+        dropping the factors \sqrt{2}*G_F.
         """
-        if mu is None:
-            mu=2
+        mu=2
         if RGE is None:
             RGE=True
-        if double_QCD is None:
-            double_QCD=True
 
         # The new coefficients
         cdict3f = {}
         if RGE:
-            cdold = self.run(mu, double_QCD)
+            cdold = self.run()
         else:
             cdold = self.coeff_dict
 
-        if self.DM_type == "D" or self.DM_type == "M":
+        if self.DM_type == "D":
             for wcn in self.wc_name_list_3f:
                 cdict3f[wcn] = cdold[wcn]
-            for wcn in self.wc8_name_list:
+
+            cdict3f['C81u'] = cdold['C81u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C81d'] = cdold['C81d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C81s'] = cdold['C81s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C83u'] = cdold['C83u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C83d'] = cdold['C83d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C83s'] = cdold['C83s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C63tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C84u'] = cdold['C84u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C84d'] = cdold['C84d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C84s'] = cdold['C84s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C71'] = cdold['C71'] - cdold['C75c']
+            cdict3f['C72'] = cdold['C72'] - cdold['C76c']
+            cdict3f['C73'] = cdold['C73'] + cdold['C77c']
+            cdict3f['C74'] = cdold['C74'] + cdold['C78c']
+
+
+        if self.DM_type == "M":
+            for wcn in self.wc_name_list_3f:
                 cdict3f[wcn] = cdold[wcn]
+
+            cdict3f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C84u'] = cdold['C84u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C84d'] = cdold['C84d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C84s'] = cdold['C84s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C64tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
             cdict3f['C71'] = cdold['C71'] - cdold['C75c']
             cdict3f['C72'] = cdold['C72'] - cdold['C76c']
             cdict3f['C73'] = cdold['C73'] + cdold['C77c']
             cdict3f['C74'] = cdold['C74'] + cdold['C78c']
 
         if self.DM_type == "C":
             for wcn in self.wc_name_list_3f:
                 cdict3f[wcn] = cdold[wcn]
-            for wcn in self.wc8_name_list:
-                cdict3f[wcn] = cdold[wcn]
+
+            cdict3f['C81u'] = cdold['C81u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C81d'] = cdold['C81d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C81s'] = cdold['C81s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
+
+            cdict3f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['mu_at_2GeV']**2
+            cdict3f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['md_at_2GeV']**2
+            cdict3f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(mu/self.ip['mb_at_mb'])\
+                                * cdold['C62tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_2GeV']) / self.ip['ms_at_2GeV']**2
             cdict3f['C65'] = cdold['C65'] - cdold['C63c']
             cdict3f['C66'] = cdold['C66'] + cdold['C64c']
 
         if self.DM_type == "R":
             for wcn in self.wc_name_list_3f:
                 cdict3f[wcn] = cdold[wcn]
             cdict3f['C65'] = cdold['C65'] - cdold['C63c']
             cdict3f['C66'] = cdold['C66'] + cdold['C64c']
 
 
         # return the 3-flavor coefficients
         return cdict3f
 
 
-    def _my_cNR(self, DM_mass, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None):
+    def _my_cNR(self, DM_mass, RGE=None, NLO=None):
         """ Calculate the NR coefficients from four-flavor theory with meson contributions split off
 
         (mainly for internal use)
         """
-        return WC_3flavor(self.match(RGE, double_QCD, DOUBLE_WEAK), self.DM_type, self.ip)._my_cNR(DM_mass, RGE, NLO)
+        return WC_3flavor(self.match(RGE), self.DM_type, self.ip)._my_cNR(DM_mass, NLO)
 
-    def cNR(self, DM_mass, qvec, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None):
+    def cNR(self, DM_mass, qvec, RGE=None, NLO=None):
         """ Calculate the NR coefficients from four-flavor theory """
-        return WC_3flavor(self.match(RGE, double_QCD), self.DM_type, self.ip).cNR(DM_mass, qvec, RGE, NLO, DOUBLE_WEAK)
+        return WC_3flavor(self.match(RGE), self.DM_type, self.ip).cNR(DM_mass, qvec, NLO)
 
-    def write_mma(self, DM_mass, qvec, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None, path=None, filename=None):
+    def write_mma(self, DM_mass, qvec, RGE=None, NLO=None, path=None, filename=None):
         """ Write a text file with the NR coefficients that can be read into DMFormFactor 
 
         The order is {cNR1p, cNR2p, ... , cNR1n, cNR2n, ... }
 
         Mandatory arguments are the DM mass DM_mass (in GeV) and the spatial momentum transfer qvec (in GeV) 
 
         <path> should be a string with the path (including the trailing "/") where the file should be saved
         (default is './')
 
         <filename> is the filename (default 'cNR.m')
         """
-        WC_3flavor(self.match(RGE, double_QCD), self.DM_type,\
-                   self.ip).write_mma(DM_mass, qvec, RGE, NLO, DOUBLE_WEAK, path, filename)
+        WC_3flavor(self.match(RGE), self.DM_type,\
+                   self.ip).write_mma(DM_mass, qvec, RGE, NLO, path, filename)
 
 
 
 
 class WC_5flavor(object):
     def __init__(self, coeff_dict, DM_type, input_dict=None):
 #    def __init__(self, coeff_dict, DM_type):
@@ -2426,15 +2251,15 @@
         The third argument is a dictionary with all input parameters.
 
 
         The class has four methods: 
 
         run
         ---
-        Run the Wilson from MZ = 91.1876 GeV to mu_low [GeV; default mb(mb)], with 5 active quark flavors
+        Run the Wilson from MZ to mb(mb), with 5 active quark flavors
 
         match
         -----
         Match the Wilson coefficients from 5-flavor to 4-flavor QCD, at scale mu [GeV; default mu = mb(mb)]
 
         cNR
         ---
@@ -2922,84 +2747,65 @@
                             np.hstack((np.zeros((len(self.gamma_QCD_dim8),\
                                                  len(self.coeff_list_sm_dim6))), self.gamma_QCD_dim8))))]
         if self.DM_type == "R":
             pass
 
 
 
-    def run(self, mu_low=None, double_QCD=None):
+    def run(self):
         """ Running of 5-flavor Wilson coefficients
 
         Calculate the running from MZ to mu_low [GeV; default mb(mb)] in the five-flavor theory. 
 
         Return a dictionary of Wilson coefficients for the five-flavor Lagrangian
         at scale mu_low.
         """
 
-        if mu_low is None:
-            mu_low=self.ip['mb_at_mb']
-        if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            if double_QCD is None:
-                double_QCD=True
-        else:
-            double_QCD=False
+        mu_low=self.ip['mb_at_mb']
 
 
         #-------------#
         # The running #
         #-------------#
 
         MZ = self.ip['Mz']
         alpha_at_mb = 1/self.ip['aMZinv']
+        as_MZ = self.ip['asMZ']
+        as_mb = self.ip['as_at_mb']
 
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
-            if double_QCD:
-                adm_eff = self.ADM_eff
-            else:
-                projector = np.vstack((np.hstack((np.zeros((100,100)),\
-                                                  np.ones((100,12)))), np.zeros((12,112))))
-                adm_eff = [np.multiply(projector, self.ADM_eff[0])]
+            adm_eff = self.ADM_eff
         else:
-            double_QCD=False
-
-        as51 = rge.AlphaS(self.ip['asMZ'], self.ip['Mz'])
-        as51_high = as51.run({'mbmb': self.ip['mb_at_mb'],\
-                              'mcmc': self.ip['mc_at_mc']},\
-                             {'mub': self.ip['mb_at_mb'],\
-                              'muc': self.ip['mc_at_mc']}, MZ, 5, 1)
-        as51_low = as51.run({'mbmb': self.ip['mb_at_mb'],\
-                             'mcmc': self.ip['mc_at_mc']},\
-                            {'mub': self.ip['mb_at_mb'],\
-                             'muc': self.ip['mc_at_mc']}, mu_low, 5, 1)
+            pass
 
         evolve1 = rge.RGE(self.gamma_QCD, 5)
         evolve2 = rge.RGE(self.gamma_QCD2, 5)
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             evolve8 = rge.RGE(adm_eff, 5)
         else:
             pass
 
         # Mixing in the dim.6 DM-SM sector
         #
         # Strictly speaking, MZ and mb should be defined at the same scale
         # (however, this is a higher-order difference)
-        C_at_mb_QCD = np.dot(evolve2.U0_as2(as51_high, as51_low),\
-                             np.dot(evolve1.U0(as51_high, as51_low),\
+        C_at_mb_QCD = np.dot(evolve2.U0_as2(as_MZ, as_mb),\
+                             np.dot(evolve1.U0(as_MZ, as_mb),\
                                     self.coeff_list_dm_dim5_dim6_dim7))
         C_at_mb_QED = np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED)\
                       * np.log(mu_low/MZ) * alpha_at_mb/(4*np.pi)\
                       + np.dot(self.coeff_list_dm_dim5_dim6_dim7, self.gamma_QED2)\
                       * np.log(mu_low/MZ) * (alpha_at_mb/(4*np.pi))**2
 
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             # Mixing in the dim.6 SM-SM and dim.8 DM-SM sector
 
             DIM6_DIM8_init = np.hstack((self.coeff_list_sm_dim6, self.coeff_list_dm_dim8))
 
-            DIM6_DIM8_at_mb =   np.dot(evolve8.U0(as51_high, as51_low), DIM6_DIM8_init)
+            DIM6_DIM8_at_mb =   np.dot(evolve8.U0(as_MZ, as_mb), DIM6_DIM8_init)
 
 
         # Revert back to dictionary
 
         dict_coeff_mb = list_to_dict(C_at_mb_QCD + C_at_mb_QED, self.wc_name_list)
         if self.DM_type == "D" or self.DM_type == "M" or self.DM_type == "C":
             dict_dm_dim8 = list_to_dict(np.delete(DIM6_DIM8_at_mb, np.s_[0:100]), self.wc8_name_list)
@@ -3009,57 +2815,385 @@
             dict_coeff_mb.update(dict_dm_dim8)
             dict_coeff_mb.update(dict_sm_dim6)
             dict_coeff_mb.update(dict_sm_lepton_dim6)
 
         return dict_coeff_mb
 
 
-    def match(self, RGE=None, double_QCD=None, mu=None):
+    def match(self, RGE=None):
         """ Match from five-flavor to four-flavor QCD
 
-        Calculate the matching at mu [GeV; default 4.18 GeV].
+        Calculate the matching at mb(mb).
 
         Returns a dictionary of Wilson coefficients for the four-flavor Lagrangian
         at scale mu.
 
         RGE is an optional argument to turn RGE running on (True) or off (False). (Default True)
         """
         if RGE is None:
             RGE=True
-        if mu is None:
-            mu=self.ip['mb_at_mb']
-        if double_QCD is None:
-            double_QCD=True
+        mu=self.ip['mb_at_mb']
 
         # The new coefficients
         cdict4f = {}
         if RGE:
-            cdold = self.run(mu, double_QCD)
+            cdold = self.run()
         else:
             cdold = self.coeff_dict
 
-        if self.DM_type == "D" or self.DM_type == "M":
+        if self.DM_type == "D":
             for wcn in self.wc_name_list_4f:
                 cdict4f[wcn] = cdold[wcn]
-            for wcn in self.wc8_name_list:
+
+            cdict4f['C81u'] = cdold['C81u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C81d'] = cdold['C81d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C81s'] = cdold['C81s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            cdict4f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            cdict4f['C83u'] = cdold['C83u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C83d'] = cdold['C83d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C83s'] = cdold['C83s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C63tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            cdict4f['C84u'] = cdold['C84u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C84d'] = cdold['C84d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C84s'] = cdold['C84s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            for wcn in self.sm_name_list_4f:
+                cdict4f[wcn] = cdold[wcn]
+            for wcn in self.sm_lepton_name_list:
                 cdict4f[wcn] = cdold[wcn]
+            cdict4f['C71'] = cdold['C71'] - cdold['C75b']
+            cdict4f['C72'] = cdold['C72'] - cdold['C76b']
+            cdict4f['C73'] = cdold['C73'] + cdold['C77b']
+            cdict4f['C74'] = cdold['C74'] + cdold['C78b']
+
+        if self.DM_type == "M":
+            for wcn in self.wc_name_list_4f:
+                cdict4f[wcn] = cdold[wcn]
+
+            cdict4f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            cdict4f['C84u'] = cdold['C84u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62ue']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62umu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62utau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C84d'] = cdold['C84d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62de']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62dmu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62dtau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C84s'] = cdold['C84s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64e'] * cdold['D62se']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64mu'] * cdold['D62smu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C64tau'] * cdold['D62stau']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
             for wcn in self.sm_name_list_4f:
                 cdict4f[wcn] = cdold[wcn]
             for wcn in self.sm_lepton_name_list:
                 cdict4f[wcn] = cdold[wcn]
             cdict4f['C71'] = cdold['C71'] - cdold['C75b']
             cdict4f['C72'] = cdold['C72'] - cdold['C76b']
             cdict4f['C73'] = cdold['C73'] + cdold['C77b']
             cdict4f['C74'] = cdold['C74'] + cdold['C78b']
 
         if self.DM_type == "C":
             for wcn in self.wc_name_list_4f:
                 cdict4f[wcn] = cdold[wcn]
-            for wcn in self.wc8_name_list:
-                cdict4f[wcn] = cdold[wcn]
+
+            cdict4f['C81u'] = cdold['C81u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C81d'] = cdold['C81d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C81s'] = cdold['C81s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
+            cdict4f['C82u'] = cdold['C82u']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63eu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63muu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63tauu']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['mu_at_mb']**2
+            cdict4f['C82d'] = cdold['C82d']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63ed']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63mud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63taud']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['md_at_mb']**2
+            cdict4f['C82s'] = cdold['C82s']\
+                              - 1/np.pi**2 * self.ip['me']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62e'] * cdold['D63es']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mmu']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62mu'] * cdold['D63mus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2\
+                              - 1/np.pi**2 * self.ip['mtau']**2\
+                                * np.log(self.ip['mb_at_mb']/self.ip['Mz'])\
+                                * cdold['C62tau'] * cdold['D63taus']\
+                                * (4*np.pi*self.ip['as_at_mb']) / self.ip['ms_at_mb']**2
+
             for wcn in self.sm_name_list_4f:
                 cdict4f[wcn] = cdold[wcn]
             for wcn in self.sm_lepton_name_list:
                 cdict4f[wcn] = cdold[wcn]
             cdict4f['C65'] = cdold['C65'] - cdold['C63b']
             cdict4f['C66'] = cdold['C66'] + cdold['C64b']
 
@@ -3069,41 +3203,41 @@
             cdict4f['C65'] = cdold['C65'] - cdold['C63b']
             cdict4f['C66'] = cdold['C66'] + cdold['C64b']
 
         # return the 4-flavor coefficients
         return cdict4f
 
 
-    def _my_cNR(self, DM_mass, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None):
+    def _my_cNR(self, DM_mass, RGE=None, NLO=None):
         """ Calculate the NR coefficients from four-flavor theory with meson contributions split off
 
         (mainly for internal use) 
         """
-        return WC_4flavor(self.match(RGE, double_QCD), self.DM_type,\
-                     self.ip)._my_cNR(DM_mass, RGE, NLO, double_QCD, DOUBLE_WEAK)
+        return WC_4flavor(self.match(RGE), self.DM_type,\
+                     self.ip)._my_cNR(DM_mass, RGE, NLO)
 
-    def cNR(self, DM_mass, qvec, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None):
+    def cNR(self, DM_mass, qvec, RGE=None, NLO=None):
         """ Calculate the NR coefficients from four-flavor theory """
-        return WC_4flavor(self.match(RGE, double_QCD), self.DM_type,\
-                     self.ip).cNR(DM_mass, qvec, RGE, NLO, double_QCD, DOUBLE_WEAK)
+        return WC_4flavor(self.match(RGE), self.DM_type,\
+                     self.ip).cNR(DM_mass, qvec, RGE, NLO)
 
-    def write_mma(self, DM_mass, qvec, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None, path=None, filename=None):
+    def write_mma(self, DM_mass, qvec, RGE=None, NLO=None, path=None, filename=None):
         """ Write a text file with the NR coefficients that can be read into DMFormFactor 
 
         The order is {cNR1p, cNR2p, ... , cNR1n, cNR2n, ... }
 
         Mandatory arguments are the DM mass DM_mass (in GeV) and the spatial momentum transfer qvec (in GeV) 
 
         <path> should be a string with the path (including the trailing "/") where the file should be saved
         (default is './')
 
         <filename> is the filename (default 'cNR.m')
         """
-        WC_4flavor(self.match(RGE, double_QCD), self.DM_type,\
-                   self.ip).write_mma(DM_mass, qvec, RGE, NLO, double_QCD, DOUBLE_WEAK, path, filename)
+        WC_4flavor(self.match(RGE), self.DM_type,\
+                   self.ip).write_mma(DM_mass, qvec, RGE, NLO, path, filename)
 
 
 
 
 
 
 
@@ -3311,20 +3445,19 @@
         self.ip = input_dict
 
 
     #---------#
     # Running #
     #---------#
 
-    def run(self, mu_Lambda, muz=None):
-        """Calculate the e/w running from scale mu_Lambda (to be given in GeV) to scale muz [muz = MZ by default].
+    def run(self, mu_Lambda):
+        """Calculate the e/w running from scale mu_Lambda (to be given in GeV) to scale muz = MZ.
         
         """
-        if muz is None:
-            muz = self.ip['Mz']+0.01
+        muz = self.ip['Mz']+0.01
 
 
         # Define the dictionary of initial condictions for gauge / Yukawa couplings
         # at the scale mu = MZ (MSbar):
         #
         # (In the future, implement also the "running and matching" of mtop to mu = MZ)
 
@@ -3338,40 +3471,24 @@
 
         def mc(mu, mub, muc, nf, loop):
             return rge.M_Quark_MSbar('c', self.ip['mc_at_mc'], self.ip['mc_at_mc'], self.ip['asMZ'],\
                                      self.ip['Mz']).run(mu, {'mbmb': self.ip['mb_at_mb'],\
                                                              'mcmc': self.ip['mc_at_mc']},\
                                                         {'mub': mub, 'muc': muc}, nf, loop)
 
-        self.mb_at_MZ = mb(self.ip['Mz'], self.ip['mb_at_mb'], self.ip['mc_at_mc'], 5, 1)
-        self.mc_at_MZ = mc(self.ip['Mz'], self.ip['mb_at_mb'], self.ip['mc_at_mc'], 5, 1)
-
-        self.g2_at_MZ   = np.sqrt(4*np.pi/self.ip['aMZinv']/self.ip['sw2_MSbar'])
-        self.g1_at_MZ   = np.sqrt(self.g2_at_MZ**2/(1/self.ip['sw2_MSbar'] - 1))
-        self.g3_at_MZ   = np.sqrt(4*np.pi*self.ip['asMZ'])
-        self.yc_at_MZ   = np.sqrt(np.sqrt(2)*self.ip['GF'])*np.sqrt(2) * self.mc_at_MZ
-        self.yb_at_MZ   = np.sqrt(np.sqrt(2)*self.ip['GF'])*np.sqrt(2) * self.mb_at_MZ
-        self.ytau_at_MZ = np.sqrt(np.sqrt(2)*self.ip['GF'])*np.sqrt(2) * self.ip['mtau']
-        self.yt_at_MZ   = np.sqrt(np.sqrt(2)*self.ip['GF'])*np.sqrt(2) * self.ip['mt_at_MZ']
-        self.lam_at_MZ  = 2*np.sqrt(2) * self.ip['GF'] * self.ip['Mh']**2
-
-        self.coupl_init_dict = {'g1': self.g1_at_MZ,\
-                                'g2': self.g2_at_MZ,\
-                                'gs': self.g3_at_MZ,\
-                                'ytau': self.ytau_at_MZ,\
-                                'yc': self.yc_at_MZ,\
-                                'yb': self.yb_at_MZ,\
-                                'yt': self.yt_at_MZ,\
-                                'lam': self.lam_at_MZ}
-
-
-
-
+        self.coupl_init_dict = {'g1': self.ip['g1_at_MZ'],\
+                                'g2': self.ip['g2_at_MZ'],\
+                                'gs': self.ip['g3_at_MZ'],\
+                                'ytau': self.ip['ytau_at_MZ'],\
+                                'yc': self.ip['yc_at_MZ'],\
+                                'yb': self.ip['yb_at_MZ'],\
+                                'yt': self.ip['yt_at_MZ'],\
+                                'lam': self.ip['lam_at_MZ']}
 
-            
+           
 
         # The full vector of dim.-6 Wilson coefficients
         C6_at_Lambda = np.concatenate((self.coeff_list_dim_6, self.coeff_list_sm_dim_6,\
                                        self.coeff_list_dm_dim_6))
 
         # The vector of rescaled dim.-5 Wilson coefficients
         #
@@ -3533,15 +3650,15 @@
         Mh = self.ip['Mh']
         sw = np.sqrt(self.ip['sw2_MSbar'])
         cw = np.sqrt(1-sw**2)
 
 
         # The Wilson coefficients in the "UV" EFT at scale MZ
         if RUN_EW:
-            wcew_dict = self.run(mu_Lambda, muz=self.ip['Mz'])
+            wcew_dict = self.run(mu_Lambda)
         else:
             wcew_dict = self.coeff_dict
 
 
         # Calculate the physical DM mass in terms of DM_mass and the Wilson coefficients, 
         # and the corresponding shift in the dimension-five Wilson coefficients.
 
@@ -4183,40 +4300,40 @@
         coeff_dict_5f['C722tau'] = 0
 
         coeff_dict_5f['C725'] = 0
 
         return coeff_dict_5f
 
 
-    def _my_cNR(self, DM_mass, mu_Lambda, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None, DM_mass_threshold=None, RUN_EW=None, DIM4=None):
+    def _my_cNR(self, DM_mass, mu_Lambda, RGE=None, NLO=None, DM_mass_threshold=None, RUN_EW=None, DIM4=None):
         """ Calculate the NR coefficients from four-flavor theory
             with meson contributions split off
 
         (mainly for internal use)
         """
         return WC_5flavor(self.match(DM_mass, mu_Lambda, DM_mass_threshold, RUN_EW, DIM4),\
-                          self.DM_type, self.ip)._my_cNR(self.DM_mass_phys, RGE, NLO, double_QCD, DOUBLE_WEAK)
+                          self.DM_type, self.ip)._my_cNR(self.DM_mass_phys, RGE, NLO)
 
-    def cNR(self, DM_mass, qvec, mu_Lambda, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None, DM_mass_threshold=None, RUN_EW=None, DIM4=None):
+    def cNR(self, DM_mass, qvec, mu_Lambda, RGE=None, NLO=None, DM_mass_threshold=None, RUN_EW=None, DIM4=None):
         """ Calculate the NR coefficients from four-flavor theory """
         return WC_5flavor(self.match(DM_mass, mu_Lambda, DM_mass_threshold, RUN_EW, DIM4),\
-                          self.DM_type, self.ip).cNR(DM_mass, qvec, RGE, NLO, double_QCD, DOUBLE_WEAK)
+                          self.DM_type, self.ip).cNR(DM_mass, qvec, RGE, NLO)
 
-    def write_mma(self, DM_mass, qvec, mu_Lambda, RGE=None, NLO=None, double_QCD=None, DOUBLE_WEAK=None,\
+    def write_mma(self, DM_mass, qvec, mu_Lambda, RGE=None, NLO=None,\
                   DM_mass_threshold=None, RUN_EW=None, DIM4=None, path=None, filename=None):
         """ Write a text file with the NR coefficients that can be read into DMFormFactor 
 
         The order is {cNR1p, cNR2p, ... , cNR1n, cNR2n, ... }
 
         Mandatory arguments are the DM mass DM_mass (in GeV) and the momentum transfer qvec (in GeV) 
 
         <path> should be a string with the path (including the trailing "/") where the file should be saved
         (default is '.')
 
         <filename> is the filename (default 'cNR.m')
         """
         WC_5flavor(self.match(DM_mass, mu_Lambda, DM_mass_threshold, RUN_EW, DIM4),\
-                   self.DM_type, self.ip).write_mma(DM_mass, qvec, RGE, NLO, double_QCD, DOUBLE_WEAK, path, filename)
+                   self.DM_type, self.ip).write_mma(DM_mass, qvec, RGE, NLO, path, filename)
```

### Comparing `directdm-2.2.0/directdm.egg-info/PKG-INFO` & `directdm-2.2.1/directdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: directdm
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python package for dark matter direct detection
 Home-page: https://directdm.github.io
 Author: Fady Bishara, Joachim Brod, Benjamin Grinstein, Jure Zupan
 Author-email: joachim.brod@uc.edu
 License: MIT
 Description:  This package contains classes for Wilson coefficients
                                    for dark matter -- standard model interactions,
```

### Comparing `directdm-2.2.0/directdm.egg-info/SOURCES.txt` & `directdm-2.2.1/directdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `directdm-2.2.0/setup.py` & `directdm-2.2.1/setup.py`

 * *Files identical despite different names*

