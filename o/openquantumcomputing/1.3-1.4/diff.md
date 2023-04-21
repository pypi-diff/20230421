# Comparing `tmp/openquantumcomputing-1.3.tar.gz` & `tmp/openquantumcomputing-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openquantumcomputing-1.3.tar", last modified: Fri Feb 17 10:24:13 2023, max compression
+gzip compressed data, was "dist/openquantumcomputing-1.4.tar", last modified: Fri Apr 21 12:53:11 2023, max compression
```

## Comparing `openquantumcomputing-1.3.tar` & `openquantumcomputing-1.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-02-17 10:24:13.964614 openquantumcomputing-1.3/
--rw-r--r--   0 franzf    (1000) users      (985)    35149 2022-06-14 18:00:44.000000 openquantumcomputing-1.3/LICENSE
--rw-r--r--   0 franzf    (1000) users      (985)      440 2023-02-17 10:24:13.964614 openquantumcomputing-1.3/PKG-INFO
--rw-r--r--   0 franzf    (1000) users      (985)       99 2022-06-30 13:37:46.000000 openquantumcomputing-1.3/README.md
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-02-17 10:24:13.964614 openquantumcomputing-1.3/openquantumcomputing/
--rw-r--r--   0 franzf    (1000) users      (985)    10439 2022-07-02 08:16:42.000000 openquantumcomputing-1.3/openquantumcomputing/QAOABase.py
--rw-r--r--   0 franzf    (1000) users      (985)     1541 2022-06-30 13:37:38.000000 openquantumcomputing-1.3/openquantumcomputing/QAOAMaxCut.py
--rw-r--r--   0 franzf    (1000) users      (985)    11744 2022-06-17 18:11:46.000000 openquantumcomputing-1.3/openquantumcomputing/QAOAMaxKCutBinary.py
--rw-r--r--   0 franzf    (1000) users      (985)     4426 2022-06-17 18:11:46.000000 openquantumcomputing-1.3/openquantumcomputing/QAOAMaxKCutOnehot.py
--rw-r--r--   0 franzf    (1000) users      (985)      512 2022-07-02 08:13:19.000000 openquantumcomputing-1.3/openquantumcomputing/Statistic.py
--rw-r--r--   0 franzf    (1000) users      (985)        0 2022-06-14 18:07:59.000000 openquantumcomputing-1.3/openquantumcomputing/__init__.py
--rw-r--r--   0 franzf    (1000) users      (985)    14908 2023-02-17 10:17:41.000000 openquantumcomputing-1.3/openquantumcomputing/mixer_utilities.py
--rw-r--r--   0 franzf    (1000) users      (985)    19749 2022-08-11 08:11:30.000000 openquantumcomputing-1.3/openquantumcomputing/utilities.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-02-17 10:24:13.964614 openquantumcomputing-1.3/openquantumcomputing.egg-info/
--rw-r--r--   0 franzf    (1000) users      (985)      440 2023-02-17 10:24:13.000000 openquantumcomputing-1.3/openquantumcomputing.egg-info/PKG-INFO
--rw-r--r--   0 franzf    (1000) users      (985)      538 2023-02-17 10:24:13.000000 openquantumcomputing-1.3/openquantumcomputing.egg-info/SOURCES.txt
--rw-r--r--   0 franzf    (1000) users      (985)        1 2023-02-17 10:24:13.000000 openquantumcomputing-1.3/openquantumcomputing.egg-info/dependency_links.txt
--rw-r--r--   0 franzf    (1000) users      (985)       19 2023-02-17 10:24:13.000000 openquantumcomputing-1.3/openquantumcomputing.egg-info/requires.txt
--rw-r--r--   0 franzf    (1000) users      (985)       21 2023-02-17 10:24:13.000000 openquantumcomputing-1.3/openquantumcomputing.egg-info/top_level.txt
--rw-r--r--   0 franzf    (1000) users      (985)       38 2023-02-17 10:24:13.964614 openquantumcomputing-1.3/setup.cfg
--rw-r--r--   0 franzf    (1000) users      (985)      533 2023-02-17 10:22:36.000000 openquantumcomputing-1.3/setup.py
+drwxr-xr-x   0 franzf    (1000) franzf    (1000)        0 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)    35149 2022-06-11 05:53:22.000000 openquantumcomputing-1.4/LICENSE
+-rw-r--r--   0 franzf    (1000) franzf    (1000)      440 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/PKG-INFO
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)       99 2022-06-28 13:38:08.000000 openquantumcomputing-1.4/README.md
+drwxr-xr-x   0 franzf    (1000) franzf    (1000)        0 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/openquantumcomputing/
+-rw-r--r--   0 franzf    (1000) franzf    (1000)    11497 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/QAOABase.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)     2217 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/QAOAExactCover.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)     1489 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/QAOAMaxCut.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)    11712 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/QAOAMaxKCutBinary.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)     4394 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/QAOAMaxKCutOnehot.py
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)      512 2022-07-02 05:54:18.000000 openquantumcomputing-1.4/openquantumcomputing/Statistic.py
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)        0 2022-06-14 12:45:46.000000 openquantumcomputing-1.4/openquantumcomputing/__init__.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)     3729 2022-08-09 08:30:14.000000 openquantumcomputing-1.4/openquantumcomputing/binsymbols.py
+-rw-r--r--   0 franzf    (1000) franzf    (1000)    14977 2023-03-16 13:52:39.000000 openquantumcomputing-1.4/openquantumcomputing/mixer_utilities.py
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)    19749 2022-08-12 06:59:27.000000 openquantumcomputing-1.4/openquantumcomputing/utilities.py
+drwxr-xr-x   0 franzf    (1000) franzf    (1000)        0 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)      440 2023-04-21 12:53:10.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/PKG-INFO
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)      612 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/SOURCES.txt
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)        1 2023-04-21 12:53:10.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/dependency_links.txt
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)       19 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/requires.txt
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)       21 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/openquantumcomputing.egg-info/top_level.txt
+-rw-r--r--   0 franzf    (1000) franzf    (1000)       38 2023-04-21 12:53:11.000000 openquantumcomputing-1.4/setup.cfg
+-rw-rw-r--   0 franzf    (1000) franzf    (1000)      533 2023-04-21 12:52:27.000000 openquantumcomputing-1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `openquantumcomputing-1.3/LICENSE` & `openquantumcomputing-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openquantumcomputing-1.3/openquantumcomputing/QAOABase.py` & `openquantumcomputing-1.4/openquantumcomputing/QAOABase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from qiskit import *
 import numpy as np
 from scipy.optimize import minimize
+import math
 
 from openquantumcomputing.Statistic import Statistic
 
 class QAOABase:
 
-    def __init__(self):#,params = None):
+    def __init__(self,params = None):
         """
         init function that initializes member variables
 
         :param params: additional parameters
         """
+        self.params=params
         self.E=None
         self.Var=None
         self.current_depth=0 # depth at which local optimization has been done
         self.angles_hist={} # initial and final angles during optimization per depth
         self.num_fval={} # number of function evaluations per depth
         self.num_shots={} # number of total shots taken for local optimization per depth
         self.costval={} # optimal cost values per depth
@@ -27,57 +29,91 @@
         self.g_values={}
         self.g_angles={}
 
 ################################
 # functions to be implemented:
 ################################
 
-    def cost(self, string, params):
+    def cost(self, string):
         """
         implements the cost function
 
         :param string: a binary string
-        :param params: additional parameters
         :return: a scalar value
         """
         raise NotImplementedError
 
-    def createCircuit(self, angles, depth, params={}):
+    def createCircuit(self, angles, depth):
         """
         implements a function to create the circuit
 
-        :param params: additional parameters
         :return: an instance of the qiskti class QuantumCircuit
         """
         raise NotImplementedError
 
 ################################
 # generic functions
 ################################
 
-    def loss(self, angles, backend, depth, shots, precision, noisemodel, params):
+    def isFeasible(self, string):
+        """
+        needs to be implemented to run successProbability
+        """
+        return True
+
+    def successProbability(self, angles, backend, shots, noisemodel=None):
+        """
+        success is defined through cost function to be equal to 0
+        """
+        depth=int(len(angles)/2)
+        circ=self.createCircuit(angles, depth)
+        if backend.configuration().local:
+            job = execute(circ, backend, shots=shots)
+        else:
+            job = start_or_retrieve_job("sprob", backend, circ, options={'shots' : shots})
+
+        jres=job.result()
+        counts_list=jres.get_counts()
+        if isinstance(counts_list, list):
+            s_prob=[]
+            for i, counts in enumerate(counts_list):
+                tmp=0
+                for string in counts:
+                    # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
+                    if self.isFeasible(string[::-1]):
+                        tmp+=counts[string]
+                s_prob.append(tmp)
+        else:
+            s_prob=0
+            for string in counts_list:
+                # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
+                if self.isFeasible(string[::-1]):
+                    s_prob+=counts_list[string]
+        return s_prob/shots
+
+    def loss(self, angles, backend, depth, shots, precision, noisemodel):
         """
         loss function
-        :param params: additional parameters
         :return: an instance of the qiskti class QuantumCircuit
         """
         self.g_it+=1
-        circuit = self.createCircuit(angles, depth, params=params)
+        circuit = self.createCircuit(angles, depth)
 
         n_target=shots
         self.stat.reset()
         shots_taken=0
 
         for i in range(3):
             if backend.configuration().local:
                 job = execute(circuit, backend=backend, noise_model=noisemodel, shots=shots)
             else:
+                name=""
                 job = start_or_retrieve_job(name+"_"+str(opt_iterations), backend, circuit, options={'shots' : shots})
             shots_taken+=shots
-            _,_ = self.measurementStatistics(job, params=params)
+            _,_ = self.measurementStatistics(job)
             if precision is None:
                 break
             else:
                 v=self.stat.get_Variance()
                 shots=int((np.sqrt(v)/precision)**2)-shots_taken
                 if shots<=0:
                     break
@@ -87,15 +123,15 @@
         self.g_values[str(self.g_it)] = -self.stat.get_E()
         self.g_angles[str(self.g_it)] = angles.copy()
 
         #opt_values[str(opt_iterations )] = e[0]
         #opt_angles[str(opt_iterations )] = angles
         return -self.stat.get_E()
 
-    def measurementStatistics(self, job, params):
+    def measurementStatistics(self, job):
         """
         implements a function for expectation value and variance
 
         :param job: job instance derived from BaseJob
         :return: expectation and variance
         """
         jres=job.result()
@@ -103,29 +139,29 @@
         if isinstance(counts_list, list):
             expectations = []
             variances = []
             for i, counts in enumerate(counts_list):
                 self.stat.reset()
                 for string in counts:
                     # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
-                    cost = self.cost(string[::-1], params)
+                    cost = self.cost(string[::-1])
                     self.stat.add_sample(cost, counts[string])
                 expectations.append(self.stat.get_E())
                 variances.append(self.stat.get_Variance())
             return expectations, variances
         else:
             for string in counts_list:
                 # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
-                cost = self.cost(string[::-1], params)
+                cost = self.cost(string[::-1])
                 self.stat.add_sample(cost, counts_list[string])
             return self.stat.get_E(), self.stat.get_Variance()
 
-    def hist(self, angles, backend, shots, noisemodel=None, params={}):
+    def hist(self, angles, backend, shots, noisemodel=None):
         depth=int(len(angles)/2)
-        circ=self.createCircuit(angles, depth, params=params)
+        circ=self.createCircuit(angles, depth)
         if backend.configuration().local:
             job = execute(circ, backend, shots=shots)
         else:
             job = start_or_retrieve_job("hist", backend, circ, options={'shots' : shots})
         return job.result().get_counts()
 
     def random_init(self, gamma_bounds,beta_bounds,depth):
@@ -154,84 +190,83 @@
         """
         depth=len(angles)
         tmp=np.zeros(len(angles)+2)
         tmp[1:-1]=angles.copy()
         w=np.arange(0,depth+1)
         return w/depth*tmp[:-1] + (depth-w)/depth*tmp[1:]
 
-    def sample_cost_landscape(self, backend, shots=1024, noisemodel=None, params={}, verbose=True, angles={"gamma": [0,2*np.pi,20], "beta": [0,2*np.pi,20]}):
+    def sample_cost_landscape(self, backend, shots=1024, noisemodel=None, verbose=True, angles={"gamma": [0,2*np.pi,20], "beta": [0,2*np.pi,20]}):
         if verbose:
             print("Calculating Energy landscape for depth p=1...")
 
         depth=1
 
         tmp=angles["gamma"]
         self.gamma_grid = np.linspace(tmp[0],tmp[1],tmp[2])
         tmp=angles["beta"]
         self.beta_grid = np.linspace(tmp[0],tmp[1],tmp[2])
 
         if backend.configuration().local:
             circuits=[]
             for beta in self.beta_grid:
                 for gamma in self.gamma_grid:
-                    #params['name'] = str(beta_n)+"_"+str(gamma_n)
-                    circuits.append(self.createCircuit(np.array((gamma,beta)), depth, params=params))
+                    circuits.append(self.createCircuit(np.array((gamma,beta)), depth))
             job = execute(circuits, backend, shots=shots)
-            e, v = self.measurementStatistics(job, params=params)
+            e, v = self.measurementStatistics(job)
             self.E = -np.array(e).reshape(angles["beta"][2],angles["gamma"][2])
             self.Var = np.array(v).reshape(angles["beta"][2],angles["gamma"][2])
         else:
             self.E = np.zeros((angles["beta"][2],angles["gamma"][2]))
             self.Var = np.zeros((angles["beta"][2],angles["gamma"][2]))
             b=-1
             for beta in self.beta_grid:
                 b+=1
                 g=-1
                 for gamma in self.gamma_grid:
                     g+=1
-                    params['name'] = str(b)+"_"+str(g)
-                    circuit = createCircuit(np.array((gamma,beta)), depth, params=params)
+                    circuit = createCircuit(np.array((gamma,beta)), depth)
+                    name=""
                     job = start_or_retrieve_job(name+"_"+str(b)+"_"+str(g), backend, circuit, options={'shots' : shots})
-                    e,v = self.measurementStatistics(job, params=params)
+                    e,v = self.measurementStatistics(job)
                     self.E[b,g] = -e[0]
                     self.Var[b,g] = -v[0]
 
         #self.current_depth=1
         if verbose:
             print("Calculating Energy landscape done")
 
     def get_current_deptgh(self):
         return self.current_depth
 
-    def local_opt(self, angles0, backend, shots, precision, noisemodel=None, params={}, method='COBYLA'):
+    def local_opt(self, angles0, backend, shots, precision, noisemodel=None, method='COBYLA'):
         """
 
         :param angles0: initial guess
         """
 
         depth=int(len(angles0)/2)
 
         self.num_shots['d'+str(self.current_depth+1)]=0
         res = minimize(self.loss, x0 = angles0, method = method,
-                       args=(backend, depth, shots, precision, noisemodel, params))
+                       args=(backend, depth, shots, precision, noisemodel))
         return res
 
-    def increase_depth(self, backend, shots=1024, precision=None, noisemodel=None, params={}, method='COBYLA'):
+    def increase_depth(self, backend, shots=1024, precision=None, noisemodel=None, method='COBYLA'):
         """
         sample cost landscape
 
         :param backend: backend
         :param shots: if precision=None, the number of samples taken
                       if precision!=None, the minimum number of samples taken
         :param precision: precision to reach for expectation value based on error=variance/sqrt(shots)
         """
 
         if self.current_depth == 0:
             if self.E is None:
-                self.sample_cost_landscape(backend, shots, noisemodel=noisemodel, params=params, angles={"gamma": [0,2*np.pi,20], "beta": [0,2*np.pi,20]})
+                self.sample_cost_landscape(backend, shots, noisemodel=noisemodel, angles={"gamma": [0,2*np.pi,20], "beta": [0,2*np.pi,20]})
             ind_Emin = np.unravel_index(np.argmin(self.E, axis=None), self.E.shape)
             angles0=np.array((self.gamma_grid[ind_Emin[1]], self.beta_grid[ind_Emin[0]]))
             self.angles_hist['d1_initial']=angles0
         else:
             gamma=self.angles_hist['d'+str(self.current_depth)+'_final'][::2]
             beta=self.angles_hist['d'+str(self.current_depth)+'_final'][1::2]
             gamma_interp=self.interp(gamma)
@@ -241,15 +276,15 @@
             angles0[1::2]=beta_interp
             self.angles_hist['d'+str(self.current_depth+1)+'_initial']=angles0
 
         self.g_it=0
         self.g_values={}
         self.g_angles={}
 
-        res = self.local_opt(angles0, backend, shots, precision, noisemodel=noisemodel, params=params, method=method)
+        res = self.local_opt(angles0, backend, shots, precision, noisemodel=noisemodel, method=method)
         if not res.success:
             raise Warning("Local optimization was not successful.", res)
         self.num_fval['d'+str(self.current_depth+1)]=res.nfev
         print("cost(depth=",self.current_depth+1,")=", res.fun)
 
         ind = min(self.g_values, key=self.g_values.get)
         self.angles_hist['d'+str(self.current_depth+1)+'_final']=self.g_angles[ind]
```

### Comparing `openquantumcomputing-1.3/openquantumcomputing/QAOAMaxCut.py` & `openquantumcomputing-1.4/openquantumcomputing/QAOAMaxCut.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from qiskit import *
 import numpy as np
 
 from openquantumcomputing.QAOABase import QAOABase
 
 class QAOAMaxCut(QAOABase):
 
-    def cost(self, string, params):
-        G = params.get('G', None)
+    def cost(self, string):
+        G = self.params.get('G', None)
         C = 0
         for edge in G.edges():
             i = int(edge[0])
             j = int(edge[1])
             if string[i] != string[j]:
                 w = G[edge[0]][edge[1]]['weight']
                 C += w
         return C
 
-    def createCircuit(self, angles, depth, params={}):
-        G = params.get('G', None)
-        usebarrier = params.get('usebarrier', False)
-        name= params.get('name', "")
+    def createCircuit(self, angles, depth):
+        G = self.params.get('G', None)
+        usebarrier = self.params.get('usebarrier', False)
 
         num_V = G.number_of_nodes()
 
         q = QuantumRegister(num_V)
         c = ClassicalRegister(num_V)
-        circ = QuantumCircuit(q, c, name=name)
+        circ = QuantumCircuit(q, c)
 
         ### initial state
         circ.h(range(num_V))
 
         if usebarrier:
             circ.barrier()
         for d in range(depth):
```

### Comparing `openquantumcomputing-1.3/openquantumcomputing/QAOAMaxKCutBinary.py` & `openquantumcomputing-1.4/openquantumcomputing/QAOAMaxKCutBinary.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,38 +12,37 @@
         k_bits = self.kBits_MaxKCut(k_cuts)
         label_list = [int(binstring[j*k_bits:(j+1)*k_bits], 2) for j in range(num_V)]
         label_string = ''
         for label in label_list:
             label_string += str(label)
         return label_string
 
-    def cost(self, string, params):
-        G = params.get('G', None)
-        k_cuts = params.get('k_cuts', None)
+    def cost(self, string):
+        G = self.params.get('G', None)
+        k_cuts = self.params.get('k_cuts', None)
         num_V = G.number_of_nodes()
 
         C = 0
         labels = self.binstringToLabels_MaxKCut(k_cuts,num_V,string)
         for edge in G.edges():
             i = int(edge[0])
             j = int(edge[1])
             li=min(k_cuts-1,int(labels[i]))## e.g. for k_cuts=3, labels 2 and 3 should be equal
             lj=min(k_cuts-1,int(labels[j]))## e.g. for k_cuts=3, labels 2 and 3 should be equal
             if li != lj:
                 w = G[edge[0]][edge[1]]['weight']
                 C += w
         return C
 
-    def createCircuit(self, angles, depth, params={}):
-        G = params.get('G', None)
-        k_cuts = params.get('k_cuts', None)
-        alpha = params.get('alpha', None)
-        version = params.get('version', 2)
-        usebarrier = params.get('usebarrier', False)
-        name= params.get('name', "")
+    def createCircuit(self, angles, depth):
+        G = self.params.get('G', None)
+        k_cuts = self.params.get('k_cuts', None)
+        alpha = self.params.get('alpha', None)
+        version = self.params.get('version', 2)
+        usebarrier = self.params.get('usebarrier', False)
 
         num_V = G.number_of_nodes()
         k_bits = self.kBits_MaxKCut(k_cuts)
         if version==1:
             if k_cuts==2:
                 Hij = np.array((-1, 1,
                                  1,-1,))
@@ -102,15 +101,15 @@
         if version==2 and not k_is_power_of_two:
             num_aux=2
             ind_a1=num_V * k_bits + num_aux - 2
             ind_a2=num_V * k_bits + num_aux - 1
 
         q = QuantumRegister(num_V * k_bits + num_aux)
         c = ClassicalRegister(num_V * k_bits)
-        circ = QuantumCircuit(q, c, name=name)
+        circ = QuantumCircuit(q, c)
         circ.h(range(num_V * k_bits))
 
         if usebarrier:
             circ.barrier()
         for d in range(depth):
             gamma = angles[2 * d]
             beta = angles[2 * d + 1]
```

### Comparing `openquantumcomputing-1.3/openquantumcomputing/QAOAMaxKCutOnehot.py` & `openquantumcomputing-1.4/openquantumcomputing/QAOAMaxKCutOnehot.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,17 +27,17 @@
             val=self.validcoloring_onehot(ss)
             #print(ss,val)
             if not val:
                 break
         return val
 
 
-    def cost(self, string, params):
-        G = params.get('G', None)
-        k_cuts = params.get('k_cuts', None)
+    def cost(self, string):
+        G = self.params.get('G', None)
+        k_cuts = self.params.get('k_cuts', None)
         num_V = G.number_of_nodes()
 
         C = 0
         if self.validstring_onehot(string, num_V):
             labels = binstringToLabels_MaxKCut_onehot(string, num_V, k_cuts)
             for edge in G.edges():
                 i = int(edge[0])
@@ -45,29 +45,28 @@
                 li=min(k_cuts-1,int(labels[i]))## e.g. for k_cuts=3, labels 2 and 3 should be equal
                 lj=min(k_cuts-1,int(labels[j]))## e.g. for k_cuts=3, labels 2 and 3 should be equal
                 if li != lj:
                     w = G[edge[0]][edge[1]]['weight']
                     C += w
         return C
 
-    def createCircuit(self, angles, depth, params={}):
-        G = params.get('G', None)
-        k_cuts = params.get('k_cuts', None)
-        alpha = params.get('alpha', None)
-        version = params.get('version', 2)
-        usebarrier = params.get('usebarrier', False)
-        name= params.get('name', "")
+    def createCircuit(self, angles, depth):
+        G = self.params.get('G', None)
+        k_cuts = self.params.get('k_cuts', None)
+        alpha = self.params.get('alpha', None)
+        version = self.params.get('version', 2)
+        usebarrier = self.params.get('usebarrier', False)
 
         num_V = G.number_of_nodes()
 
         num_qubits = num_V * k_cuts
 
         q = QuantumRegister(num_qubits)
         c = ClassicalRegister(num_qubits)
-        circ = QuantumCircuit(q, c, name=name)
+        circ = QuantumCircuit(q, c)
         if version==1:
             circ.h(range(num_qubits))
         else:
             for v in range(num_V):
                 I = v*k_cuts
                 Wn(circ, [i for i in range(I, I+k_cuts)])
                 #circ.initialize(W, [q[i] for i in range(I, I+k_cuts)])
```

### Comparing `openquantumcomputing-1.3/openquantumcomputing/Statistic.py` & `openquantumcomputing-1.4/openquantumcomputing/Statistic.py`

 * *Files identical despite different names*

### Comparing `openquantumcomputing-1.3/openquantumcomputing/mixer_utilities.py` & `openquantumcomputing-1.4/openquantumcomputing/mixer_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from sympy.physics.quantum import TensorProduct
 from sympy.physics.paulialgebra import Pauli, evaluate_pauli_product
-from binsymbols import *
+from openquantumcomputing.binsymbols import binsymbols
 from sympy import *
+from sympy.core.numbers import One as sympyOne
 from openquantumcomputing.utilities import decompose
 import itertools
 import math
 
 X=Pauli(1)
 Y=Pauli(2)
 Z=Pauli(3)
@@ -372,15 +373,15 @@
                     self.__add_middle_part(array, operators, angle)
                     self.__add_U_dagger(array, operators)
         return array
 
     def __get_operators_from_tensor_product(self, tensor_product):
         """ split tensor product expr on each tensor product """
         operators=[]
-        while not isinstance(tensor_product, (Pauli, core.numbers.One)):
+        while not isinstance(tensor_product, (Pauli, sympyOne)):
             tensor_product, operator = tensor_product.args
             operators.insert(0, operator)
         operators.insert(0, tensor_product)
         return operators
 
     def __add_U(self, array, operators):
         """ add gates corresponding to block U in eq. 33 """
```

### Comparing `openquantumcomputing-1.3/openquantumcomputing/utilities.py` & `openquantumcomputing-1.4/openquantumcomputing/utilities.py`

 * *Files identical despite different names*

### Comparing `openquantumcomputing-1.3/openquantumcomputing.egg-info/SOURCES.txt` & `openquantumcomputing-1.4/openquantumcomputing.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.py
 openquantumcomputing/QAOABase.py
+openquantumcomputing/QAOAExactCover.py
 openquantumcomputing/QAOAMaxCut.py
 openquantumcomputing/QAOAMaxKCutBinary.py
 openquantumcomputing/QAOAMaxKCutOnehot.py
 openquantumcomputing/Statistic.py
 openquantumcomputing/__init__.py
+openquantumcomputing/binsymbols.py
 openquantumcomputing/mixer_utilities.py
 openquantumcomputing/utilities.py
 openquantumcomputing.egg-info/PKG-INFO
 openquantumcomputing.egg-info/SOURCES.txt
 openquantumcomputing.egg-info/dependency_links.txt
 openquantumcomputing.egg-info/requires.txt
 openquantumcomputing.egg-info/top_level.txt
```

### Comparing `openquantumcomputing-1.3/setup.py` & `openquantumcomputing-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='openquantumcomputing',
-    version='1.3',
+    version='1.4',
     license='GNU General Public License v3.0',
     author="Franz Georg Fuchs",
     author_email='franzgeorgfuchs@gmail.com',
     description='Tools for quantum computing',
     long_description=open('README.md').read(),
     url='https://github.com/OpenQuantumComputing/OpenQuantumComputing',
     packages=['openquantumcomputing'],
```

