# Comparing `tmp/bihc-0.0.4.tar.gz` & `tmp/bihc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-2j0k8b35/bihc-0.0.4.tar", last modified: Wed Mar 29 13:54:10 2023, max compression
+gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-4hn5advy/bihc-0.0.5.tar", last modified: Fri Apr 21 13:32:18 2023, max compression
```

## Comparing `bihc-0.0.4.tar` & `bihc-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-03-29 13:54:10.000000 bihc-0.0.4/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.4/LICENSE
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.4/MANIFEST.in
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-03-29 13:54:10.000000 bihc-0.0.4/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.4/README.md
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.4/bihc/__init__.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    26845 2023-03-29 13:15:01.000000 bihc-0.0.4/bihc/beam.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6251 2023-03-07 19:00:24.000000 bihc-0.0.4/bihc/impedance.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9072 2023-03-28 09:16:31.000000 bihc-0.0.4/bihc/plot.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     4157 2023-03-08 15:02:48.000000 bihc-0.0.4/bihc/power.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      334 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/SOURCES.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/dependency_links.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/requires.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-03-29 13:54:10.000000 bihc-0.0.4/bihc.egg-info/top_level.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.4/pyproject.toml
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-03-29 13:54:10.000000 bihc-0.0.4/setup.cfg
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1080 2023-03-29 13:53:47.000000 bihc-0.0.4/setup.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-03-29 13:54:10.000000 bihc-0.0.4/tests/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.4/tests/test_analyticBunchShapes.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.4/tests/test_numericBunchShapes.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.5/LICENSE
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.5/MANIFEST.in
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-04-21 13:32:18.000000 bihc-0.0.5/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.5/README.md
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.5/bihc/__init__.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    26817 2023-04-21 13:26:41.000000 bihc-0.0.5/bihc/beam.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6251 2023-03-07 19:00:24.000000 bihc-0.0.5/bihc/impedance.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9072 2023-03-28 09:16:31.000000 bihc-0.0.5/bihc/plot.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     4157 2023-03-08 15:02:48.000000 bihc-0.0.5/bihc/power.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      334 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/SOURCES.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/dependency_links.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/requires.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/top_level.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.5/pyproject.toml
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-04-21 13:32:18.000000 bihc-0.0.5/setup.cfg
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1080 2023-04-21 13:31:31.000000 bihc-0.0.5/setup.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/tests/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.5/tests/test_analyticBunchShapes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.5/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.4/LICENSE` & `bihc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/PKG-INFO` & `bihc-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.4
+Version: 0.0.5
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.4/README.md` & `bihc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/bihc/beam.py` & `bihc-0.0.5/bihc/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Beam total longitudinal bunch length in seconds (4*sigma) [s]
     bunchShape : str, default 'GAUSSIAN'
         Beam profile shape : 'GAUSSIAN', 'BINOMIAL' , 'COS2' or 'q-GAUSSIAN'         
     qvalue : float, default 1.2
         q-Gaussian q-value for the 'q-GAUSSIAN' beam profile opt
     phi : float, default 0
         Offset of the bunch profile distribution in time [s]
-    d : float, default 0
+    t0 : float, default 0
         The time length (space) of one bucket
     Np : float, default 2.3e11
         Beam intensity in number of protons per bunch
     beamNumber : int, default 1
         Number of beams for the power loss computation (1 or 2)
     fillNumber : int, default 0
         Fill number relative to a particular beam fill of the machine
@@ -80,15 +80,15 @@
         Beam power spectrum in frequency. Returns the list of numpy arrays [frequency, powerspectrum]
     totalBeamCharge : float
         Beam charge computed from intensity and number of filled slots, in Coulombs [C]
     '''
 
     def __init__(self, M=3564, A=1, fillNumber=0,
                  bunchLength=1.2e-9, phi=0, realMachineLength=True,
-                 ppbk=250, d=None, Np=2.3e11, bunchShape='GAUSSIAN', LPCfile=None, qvalue=1.2, beamNumber=1, 
+                 ppbk=250, t0=None, Np=2.3e11, bunchShape='GAUSSIAN', LPCfile=None, qvalue=1.2, beamNumber=1, 
                  fillMode='FLATTOP', fillingScheme=[False]*3564, machine='LHC', spectrum='numeric', frev=None, 
                  fmax=2e9, exp=2.5, verbose=False):
         
         c = 299792458 # Speed of light in vacuum [m/s]
         
         self.M = M # Default max numebr of buckets
         self.A_GLOBAL = A
@@ -117,16 +117,16 @@
         # Some parameters are set in a different way depending on the machine you are working with
         if self._machine == 'LHC':
             self.BUCKET_MAX = 3564
             RING_CIRCUMFERENCE = 26658.883   #[m]
             GAMMA_R = 7461                   # flat top
                         
         elif self._machine =='SPS':
-            self.BUCKET_MAX = 920 #924 is the correct number
-            RING_CIRCUMFERENCE = 6895          #[m]
+            self.BUCKET_MAX = 924 
+            RING_CIRCUMFERENCE = 6911          #[m]
             if self.fillMode == 'FLATTOP':
                 GAMMA_R = 251    # flat top 450 GeV
             else:
                 GAMMA_R = 27.7   # flat bottom value 26 GeV
 
         elif self._machine == 'PS':
             self.BUCKET_MAX = 21
@@ -139,23 +139,24 @@
         if self.M > self.BUCKET_MAX:
             self.M = self.BUCKET_MAX
             if self.verbose:
                 print('Number of bucket that could be filled set to: ', self.M)
         
         BETA_R = np.sqrt(1 - (1/GAMMA_R**2))
         self.T_1_TURN = RING_CIRCUMFERENCE/(c*BETA_R)
-        
+        if self.frev is None:
+            self.frev = 1/self.T_1_TURN 
 
-        # d is the time (space) of one bucket 
-        if d is None:
-            self.d = self.T_1_TURN/self.BUCKET_MAX #forced to be integer
+        # t0 is the time (space) of one bucket 
+        if t0 is None:
+            self.t0 = self.T_1_TURN/self.BUCKET_MAX #forced to be integer
         else: 
-            self.d = d
+            self.t0 = t0
         
-        self.l = self.d/2
+        self.l = self.t0/2
         self._bunchLength = np.zeros(self.M)
         self.phi = np.zeros(self.M)
         self._spectrum = [np.zeros(self.M), np.zeros(self.M)]    #[f,S]
         self._fillingScheme=fillingScheme[0:self.M]
              
         self._beamNumber = beamNumber # Beam number, either 1 or 2
         self._beamFile = LPCfile
@@ -246,17 +247,15 @@
                 f = np.linspace(-fc/2, fc/2 - deltaF, len(S))      #vector of K point from min_value to max_value (Domain in frequency)
 
             else: #analytic formula (C.Zannini)
                 print('\033[93m'+'Warning -> Analytic FFT might take a long time to be computed'+'\033[0m')
                 from  bihc.plot import progressbar
 
                 an = self._fillingScheme
-                t0 = self.d             #25 ns
-                if self.frev is None:
-                    self.frev = 1/self.T_1_TURN 
+                t0 = self.t0             #25 ns
                 n = np.arange(1,self.M+1)
                 c = 299792458
                 wrev = 2*np.pi*self.frev
                 sigma = self.BUNCH_LENGTH_GLOBAL*c #sigma in m
                 sigmacos= 0.854*sigma #match FWHM to the gaussian sigma
                 sigmapar= 0.744653*sigma
                 F = 1.2413 
@@ -296,32 +295,32 @@
             self.powerSpectrum=[f, np.abs(S)**2]
             self._isSpectrumReady=True
             
             return self._spectrum
         
     @spectrum.setter
     def spectrum(self, newSpectrum): # TODO we want to assign the spectrum
-#        self._spectrum=newSpectrum
-        raise Exception("Spectrum can not be assigned")
+        self._spectrum = newSpectrum
+        #raise Exception("Spectrum can not be assigned")
                        
     def _setBunches(self):
         '''_setBunches method
 
         Computes the longitudinal profile of the bunches 
         with the shape specified in the class instance
 
          'GAUSSIAN', 'BINOMIAL' , 'COS2' or 'q-GAUSSIAN' 
         '''
-        if((self.realMachineLength) and (self.d*self.M>self.T_1_TURN)):
-            self.d=self.T_1_TURN/self.M
+        if((self.realMachineLength) and (self.t0*self.M>self.T_1_TURN)):
+            self.t0=self.T_1_TURN/self.M
             if self.verbose:
-                print("d has been resized to ", self.d ," because it was to big to fill ",self.M," buckets in the real machine length")
+                print("t0 has been resized to ", self.t0 ," because it was to big to fill ",self.M," buckets in the real machine length")
         
-        deltaD=self.d/self.ppbk
-        tTemp = np.arange(-self.d/2, self.d/2 ,deltaD)
+        deltaD=self.t0/self.ppbk
+        tTemp = np.arange(-self.t0/2, self.t0/2 ,deltaD)
         
         print ("Elaborating Data...")
         
         s = np.zeros(len(tTemp)) #[0] * len(t)
         sTemp=np.zeros(len(s))
         H=0
         self.filledSlots=0
@@ -404,20 +403,20 @@
                 sTemp=np.zeros(len(tTemp))
             if(i==0):
                 s=sTemp
             else:
                 s=np.concatenate((s,sTemp),axis=0)
         
         
-        t_max=self.d*self.M-self.d/2
+        t_max=self.t0*self.M-self.t0/2
         
         if(self.realMachineLength):
-            t=np.arange(-self.d/2,self.T_1_TURN -self.d/2,deltaD)     
+            t=np.arange(-self.t0/2,self.T_1_TURN -self.t0/2,deltaD)     
         else:
-            t=np.arange(-self.d/2,t_max,deltaD)
+            t=np.arange(-self.t0/2,t_max,deltaD)
          
         s_end=np.zeros(len(t) - len(s))
         s=np.concatenate((s,s_end),axis=0)
         sTemp=s
         for k in range(1,self.J):
             s=np.concatenate((s,sTemp),axis=0)
```

### Comparing `bihc-0.0.4/bihc/impedance.py` & `bihc-0.0.5/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/bihc/plot.py` & `bihc-0.0.5/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/bihc/power.py` & `bihc-0.0.5/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/bihc.egg-info/PKG-INFO` & `bihc-0.0.5/bihc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.4
+Version: 0.0.5
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.4/setup.py` & `bihc-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.4",
+    version="0.0.5",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.4/tests/test_analyticBunchShapes.py` & `bihc-0.0.5/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.4/tests/test_numericBunchShapes.py` & `bihc-0.0.5/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

