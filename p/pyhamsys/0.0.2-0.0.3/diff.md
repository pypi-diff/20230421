# Comparing `tmp/pyhamsys-0.0.2.tar.gz` & `tmp/pyhamsys-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhamsys-0.0.2.tar", last modified: Fri Apr  7 08:41:44 2023, max compression
+gzip compressed data, was "pyhamsys-0.0.3.tar", last modified: Fri Apr 21 06:33:20 2023, max compression
```

## Comparing `pyhamsys-0.0.2.tar` & `pyhamsys-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-07 08:41:44.348867 pyhamsys-0.0.2/
--rw-r--r--   0 cchandre   (503) staff       (20)     1304 2023-04-07 06:56:17.000000 pyhamsys-0.0.2/LICENSE
--rw-r--r--   0 cchandre   (503) staff       (20)     4992 2023-04-07 08:41:44.348572 pyhamsys-0.0.2/PKG-INFO
--rw-r--r--   0 cchandre   (503) staff       (20)     4177 2023-04-07 06:56:17.000000 pyhamsys-0.0.2/README.md
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-07 08:41:44.344852 pyhamsys-0.0.2/pyhamsys/
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-07 08:41:44.346573 pyhamsys-0.0.2/pyhamsys/src/
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-07 08:41:44.348116 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/
--rw-r--r--   0 cchandre   (503) staff       (20)     4992 2023-04-07 08:41:43.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
--rw-r--r--   0 cchandre   (503) staff       (20)      275 2023-04-07 08:41:44.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
--rw-r--r--   0 cchandre   (503) staff       (20)        1 2023-04-07 08:41:43.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
--rw-r--r--   0 cchandre   (503) staff       (20)       12 2023-04-07 08:41:43.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/requires.txt
--rw-r--r--   0 cchandre   (503) staff       (20)        9 2023-04-07 08:41:43.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.egg-info/top_level.txt
--rw-r--r--   0 cchandre   (503) staff       (20)    10952 2023-04-07 06:56:17.000000 pyhamsys-0.0.2/pyhamsys/src/pyhamsys.py
--rw-r--r--   0 cchandre   (503) staff       (20)       38 2023-04-07 08:41:44.348969 pyhamsys-0.0.2/setup.cfg
--rw-r--r--   0 cchandre   (503) staff       (20)     1129 2023-04-07 08:40:20.000000 pyhamsys-0.0.2/setup.py
+drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.774245 pyhamsys-0.0.3/
+-rw-r--r--   0 cchandre   (503) staff       (20)     1304 2023-04-07 06:56:17.000000 pyhamsys-0.0.3/LICENSE
+-rw-r--r--   0 cchandre   (503) staff       (20)     5807 2023-04-21 06:33:20.773885 pyhamsys-0.0.3/PKG-INFO
+-rw-r--r--   0 cchandre   (503) staff       (20)     4992 2023-04-13 08:59:07.000000 pyhamsys-0.0.3/README.md
+drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.769672 pyhamsys-0.0.3/pyhamsys/
+drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.771217 pyhamsys-0.0.3/pyhamsys/src/
+drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.773235 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/
+-rw-r--r--   0 cchandre   (503) staff       (20)     5807 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
+-rw-r--r--   0 cchandre   (503) staff       (20)      275 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
+-rw-r--r--   0 cchandre   (503) staff       (20)        1 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
+-rw-r--r--   0 cchandre   (503) staff       (20)       12 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/requires.txt
+-rw-r--r--   0 cchandre   (503) staff       (20)        9 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/top_level.txt
+-rw-r--r--   0 cchandre   (503) staff       (20)    11726 2023-04-13 08:59:07.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.py
+-rw-r--r--   0 cchandre   (503) staff       (20)       38 2023-04-21 06:33:20.774363 pyhamsys-0.0.3/setup.cfg
+-rw-r--r--   0 cchandre   (503) staff       (20)     1129 2023-04-21 06:31:31.000000 pyhamsys-0.0.3/setup.py
```

### Comparing `pyhamsys-0.0.2/LICENSE` & `pyhamsys-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.0.2/PKG-INFO` & `pyhamsys-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,66 @@
-Metadata-Version: 2.1
-Name: pyhamsys
-Version: 0.0.2
-Summary: Some tools for Hamiltonian systems
-Home-page: http://github.com/cchandre/pyhamsys
-Author: Cristel Chandre
-Author-email: cristel.chandre@cnrs.fr
-License: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyHamSys
-pyHamSys is a Python package for scientific computations involving Hamiltonian systems
+pyHamSys is a Python package for scientific computing involving Hamiltonian systems
+
+![PyPI](https://img.shields.io/pypi/v/pyhamsys)
+![License](https://img.shields.io/badge/license-BSD-lightgray)
+
+Installation: 
+```
+pip install pyhamsys
+```
 
 ## Symplectic Integrators
-PyHamSys includes a class SymplecticIntegrator containing the following integrators:
+pyHamSys includes a class SymplecticIntegrator containing the following symplectic splitting integrators:
 
-Names of integrators include:
-- 'Verlet' (order 2)
-- 'Forest-Ruth' (order 4) from [Forest, Ruth, Physica D 43, 105 (1990)](https://doi.org/10.1016/0167-2789(90)90019-L)
-- 'EFRL', 'PEFRL' or 'VEFRL' (order 4) from [Omelyan, Mryglod, Folk, Comput. Phys. Commun. 146, 188 (2002)](https://doi.org/10.1016/S0010-4655(02)00451-4). Optimized for *H* = *A* + *B*; 'PEFRL' and 'VEFRL' are for splitting *H* = *A*(*p*) + *B*(*q*)
-- 'BM4' (order 4) refers to S<sub>6</sub> from [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7)
-- 'BM6' (order 6) refers to S<sub>10</sub> from [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7)
-- 'RKN4b' (order 4) refers to SRKN<sub>6</sub><sup>*b*</sup> from [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7) for splitting *H* = *A*(*p*) + *B*(*q*)
-- 'RKN6b' (order 6) refers to SRKN<sub>11</sub><sup>*b*</sup> from [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7) for splitting *H* = *A*(*p*) + *B*(*q*)
-- 'RKN6a' (order 6) refers to SRKN<sub>14</sub><sup>*a*</sup> from [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7) for splitting *H* = *A*(*p*) + *B*(*q*)
-- 'ABA104' (order (10,4)) from [S. Blanes, F. Casas, A. Farrés, J. Laskar, J. Makazaga, A. Murua, Appl. Numer. Math. 68, 58 (2013)](http://dx.doi.org/10.1016/j.apnum.2013.01.003) for splitting *H* = *A* + &epsilon; *B*
-- 'ABA864' (order (8,6,4)) from [S. Blanes, F. Casas, A. Farrés, J. Laskar, J. Makazaga, A. Murua, Appl. Numer. Math. 68, 58 (2013)](http://dx.doi.org/10.1016/j.apnum.2013.01.003) for splitting *H* = *A* + &epsilon; *B*
-- 'ABA1064' (order (10,6,4)) from [S. Blanes, F. Casas, A. Farrés, J. Laskar, J. Makazaga, A. Murua, Appl. Numer. Math. 68, 58 (2013)](http://dx.doi.org/10.1016/j.apnum.2013.01.003) for splitting *H* = *A* + &epsilon; *B*
+- `Verlet` (order 2, all purpose), also referred to as Strang or Störmer-Verlet splitting 
+- From [Forest, Ruth, Physica D 43, 105 (1990)](https://doi.org/10.1016/0167-2789(90)90019-L): 
+    - `FR` (order 4, all purpose)
+- From [Yoshida, Phys. Lett. A 150, 262 (1990)](https://doi.org/10.1016/0375-9601(90)90092-3):
+    - `Yo#`: # should be replaced by an even integer, e.g., `Yo6` for 6th order symplectic integrator (all purpose)
+    - `Yos6`: (order 6, all purpose) optimized symplectic integrator (solution A from Table 1)
+- From [McLachlan, SIAM J. Sci. Comp. 16, 151 (1995)](https://doi.org/10.1137/0916010):
+    - `M2` (order 2, all purpose)
+    - `M4` (order 4, all purpose)
+- From [Omelyan, Mryglod, Folk, Comput. Phys. Commun. 146, 188 (2002)](https://doi.org/10.1016/S0010-4655(02)00451-4): 
+    - `EFRL` (order 4) optimized for *H* = *A* + *B*
+    - `PEFRL` and `VEFRL` (order 4) optimized for *H* = *A*(*p*) + *B*(*q*). For `PEFRL`, *chi* should be exp(*h*A)exp(*h*B). For `VEFRL`, *chi* should be exp(*h*B)exp(*h*A).
+- From [Blanes, Moan, J. Comput. Appl. Math. 142, 313 (2002)](https://doi.org/10.1016/S0377-0427(01)00492-7):
+    - `BM4` (order 4, all purpose) refers to S<sub>6</sub> 
+    - `BM6` (order 6, all purpose) refers to S<sub>10</sub>
+    - `RKN4b` (order 4) refers to SRKN<sub>6</sub><sup>*b*</sup> optimized for *H* = *A*(*p*) + *B*(*q*). Here *chi* should be exp(*h*B)exp(*h*A).
+    - `RKN6b` (order 6) refers to SRKN<sub>11</sub><sup>*b*</sup> optimized for *H* = *A*(*p*) + *B*(*q*). Here *chi* should be exp(*h*B)exp(*h*A).
+    - `RKN6a` (order 6) refers to SRKN<sub>14</sub><sup>*a*</sup> optimized for *H* = *A*(*p*) + *B*(*q*). Here *chi* should be exp(*h*A)exp(*h*B).
+- From [Blanes, Casas, Farrés, Laskar, Makazaga, Murua, Appl. Numer. Math. 68, 58 (2013)](http://dx.doi.org/10.1016/j.apnum.2013.01.003):
+    - `ABA104` (order (10,4)) optimized for *H* = *A* + &epsilon; *B*. Here *chi* should be exp(*h*A)exp(*h*B).
+    - `ABA864` (order (8,6,4)) optimized for *H* = *A* + &epsilon; *B*. Here *chi* should be exp(*h*A)exp(*h*B).
+    - `ABA1064` (order (10,6,4)) optimized for *H* = *A* + &epsilon; *B*. Here *chi* should be exp(*h*A)exp(*h*B).
+    
+All purpose integrators are for any splitting of the Hamiltonian *H*=&sum;<sub>*k*</sub> *X*<sub>*k*</sub> in any order of the functions *X*<sub>*k*</sub>. Otherwise, the order of the operators is specified for each integrator.
 
-Usage: *integrator* = SymplecticIntegrator(*name*, *step*, *order*)
-where *name* is one of the names listed above, *step* is the time step of the integrator (float), and *order* is the order of the splitting, so 1 or -1 depending on the order AB or BA of the splitting. 
+Usage: *integrator* = SymplecticIntegrator(*name*, *step*)
+where *name* is one of the names listed above and *step* is the time step of the integrator (float). 
 
 The function *integrator*.`_integrate` integrates the Hamiltonian flow by one step.
 
 The function *integrator*.`integrate` integrates the Hamiltonian flow from the initial conditions specified by the initial state vector *y* using *integrator*, one of the selected symplectic splitting integrators. It returns the value of *y* at times defines by the float, list or array *times*.
 
 Parameters:
-  - chi : function of (*h*, *y*), y being the state vector.
-    Function returning exp(*h* X<sub>*n*</sub>)...exp(*h* X<sub>1</sub>) *y*.
-  - chi_star : function of (*h*, *y*).
-    Function returning exp(*h* X<sub>1</sub>)...exp(*h* X_<sub>*n*</sub>) *y*.
+  - *chi* : function of (*h*, *y*), y being the state vector.
+    Function returning exp(*h* X<sub>*n*</sub>)...exp(*h* X<sub>1</sub>) *y*. If the selected integrator is not all purpose, refer to the list above for the specific ordering of the operators. The operator X<sub>*k*</sub> is the Liouville operator associated with the function *X*<sub>*k*</sub>, i.e., X<sub>*k*</sub> = {*X*<sub>*k*</sub>, &centerdot;}.
+  - *chi_star* : function of (*h*, *y*).
+    Function returning exp(*h* X<sub>1</sub>)...exp(*h* X<sub>*n*</sub>) *y*.
   - *y* : initial state vector (numpy array)
   - *times* : times at which the values of the state vector are computed
   - *command* : function of (*t*, *y*).
     Function to be run at each time step (e.g., plotting an observable associated with the state vector, or register specific events). 
   - *autonomous* : boolean.
     If autonomous is False, the state vector y should be of the form *y* = [*t*, *x*], where the first coordinate is time. 
 
 Returns:
    - If *times* is a float of integer, the output is a tuple (*t*, *y* or *x*) where *y* is the value of the state vector and *y* = [*t*, *x*] if autonomous is False.
    - If *times* is a list or array, returns the times and values of *y* or *x* at *times*. 
    - If *times* is a list or array with a single element, returns the times and values of *y* or *x* at all computed times. 
 
 References:
-  - McLachlan, R.I, 2022, *Tuning symplectic integrators is easy and worthwhile*, [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
-
-
-Installation: 
-```
-pip install pyhamsys
-```
+  - Hairer, Lubich, Wanner, 2003, *Geometric-Preseving Algorithms for Ordinary Differential Equations* (Springer)
+  - McLachlan, 2022, *Tuning symplectic integrators is easy and worthwhile*, [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
```

### Comparing `pyhamsys-0.0.2/pyhamsys/src/pyhamsys.py` & `pyhamsys-0.0.3/pyhamsys/src/pyhamsys.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,56 +111,74 @@
 
     Attributes
     ----------
     name : str
         the name of the symplectic integrator
     step : float
         the time step for the integrator
-    order (default 1) : 1 or -1
-        1 for ABA, -1 for BAB 
 
     Methods
     -------
     _integrate : integrate the state vector y by one step.
 	integrate : integrate the state vector y from 0 to tf.
         if times is int or float : tf = times, and returns only the final value of the state vector y. 
 		if times is a list or numpy array : tf = times[-1]. 
 		if len(times)=1 : returns all intermediate steps. 
 		if len(times)>=2 : returns only the times 
 		specified in times.
     """
 	def __repr__(self) -> str:
-		return f'{self.__class__.__name__}({self.name}, {self.step}, order={self.order})'
+		return f'{self.__class__.__name__}({self.name}, {self.step})'
 	
 	def __str__(self) -> str:
 		return f'{self.name}'
 
-	def __init__(self, name:str, step:float, order:int=1) -> None:
+	def __init__(self, name:str, step:float) -> None:
 		self.name = name
 		self.step = step
-		self.order = order if order in [1, -1] else 1
 		if self.name == 'Verlet':
 			alpha_s = [0.5]
-		elif self.name == 'Forest-Ruth':
-			theta = 1/(2 - 2**(1/3))
+		elif self.name == 'FR':
+			theta = 1 / (2 - 2**(1/3))
 			alpha_s = [theta / 2, theta / 2, 0.5 - theta]
+		elif self.name == 'Yos6':
+			a = [0.784513610477560, 0.235573213359357, -1.17767998417887, 1.31518632068390]
+			alpha_s = [a[0]/2,  a[0]/2, a[1]/2, a[1]/2, a[2]/2, a[2]/2, a[3]/2]
+		elif self.name[:2] == 'Yo':
+			try:
+				N = int(self.name[2:]) // 2
+				alpha_s = xp.asarray([0.5])
+				for n in range(1, N):
+					x1 = 1 / (2 - 2**(1/(2*n+1)))
+					x0 = 1 - 2 * x1
+					alpha_ = xp.concatenate((alpha_s, xp.flip(alpha_s)))
+					alpha_ = xp.concatenate((x1 * alpha_, x0 * alpha_s))
+					alpha_s = alpha_.copy()
+			except:
+				raise NameError(f'{self.name} integrator not defined') 
 		elif self.name.endswith('EFRL'):
 			if self.name.startswith('V'):
 				xi = 0.1644986515575760
 				lam = -0.02094333910398989
 				chi = 1.235692651138917
 			elif self.name.startswith('P'):
 				xi = 0.1786178958448091
 				lam = -0.2123418310626054
 				chi = -0.06626458266981849
 			else:
 				xi = 0.1720865590295143
 				lam = -0.09156203075515678
 				chi = -0.1616217622107222
 			alpha_s = [xi, 0.5 - lam - xi, lam + xi + chi -0.5, 0.5 - chi - xi]
+		elif self.name == 'M2':
+			y = (2*xp.sqrt(326)-36)**(1/3)
+			z = (y**2 + 6 * y -2) / (12 * y)
+			alpha_s = [z, 0.5 - z]
+		elif self.name == 'M4':
+			alpha_s = [(14-xp.sqrt(19))/108, (146+5*xp.sqrt(19))/540, (-23-20*xp.sqrt(19))/270, (-2+10*xp.sqrt(19))/135, 1/5]
 		elif self.name == 'BM4':
 			alpha_s = [0.0792036964311957, 0.1303114101821663, 0.2228614958676077, -0.3667132690474257, 0.3246481886897062, 0.1096884778767498]
 		elif self.name == 'BM6':
 			alpha_s = [0.050262764400392, 0.098553683500650, 0.314960616927694, -0.447346482695478, 0.492426372489876, -0.425118767797691, 0.237063913978122, 0.195602488600053, 0.346358189850727, -0.362762779254345]
 		elif self.name == 'RKN4b':
 			alpha_s = [0.082984406417405, 0.162314550766866, 0.233995250731502, 0.370877414979578, -0.409933719901926, 0.059762097006575]
 		elif self.name == 'RKN6b':
@@ -174,16 +192,17 @@
 		elif self.name == 'ABA1064':
 			alpha_s = [0.03809449742241219, 0.05776438341466301, 0.08753433270225074, 0.116911820440748, 0.0907158752847932, 0.1263544726941979, 0.3095552309573282, -0.3269306129163933]
 		else:
 			raise NameError(f'{self.name} integrator not defined')
 		self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
 		self.alpha_s *= self.step
 		self.alpha_o = xp.tile([1, 0], len(alpha_s))
-		if self.order == -1:
-			self.alpha_o = 1 - self.alpha_o
+		self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
+		self.alpha_s *= self.step
+		self.alpha_o = xp.tile([1, 0], len(alpha_s))
 	
 	def _integrate(self, chi:Callable, chi_star:Callable, y):
 		for h, st in zip(self.alpha_s, self.alpha_o):
 			y = chi(h, y) if st==0 else chi_star(h, y)
 		return y
 	
 	def integrate(self, chi:Callable, chi_star:Callable, y:xp.ndarray, times:Union[int, float, list, xp.ndarray], command:Callable=None, autonomous:bool=True) -> Tuple[Union[float, xp.ndarray], xp.ndarray]:
```

### Comparing `pyhamsys-0.0.2/setup.py` & `pyhamsys-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhamsys',
-    version='0.0.2',
+    version='0.0.3',
     description='Some tools for Hamiltonian systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url='http://github.com/cchandre/pyhamsys',
     classifiers=[
       'Programming Language :: Python :: 3',
```

