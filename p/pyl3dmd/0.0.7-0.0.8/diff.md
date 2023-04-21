# Comparing `tmp/pyl3dmd-0.0.7.tar.gz` & `tmp/pyl3dmd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyl3dmd-0.0.7.tar", last modified: Mon Feb 13 18:37:14 2023, max compression
+gzip compressed data, was "pyl3dmd-0.0.8.tar", last modified: Fri Apr 21 18:58:11 2023, max compression
```

## Comparing `pyl3dmd-0.0.7.tar` & `pyl3dmd-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 18:37:14.248786 pyl3dmd-0.0.7/
--rw-rw-rw-   0        0        0      753 2023-02-13 18:37:14.248786 pyl3dmd-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-13 18:37:14.240806 pyl3dmd-0.0.7/pyl3dmd/
--rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.0.7/pyl3dmd/__init__.py
--rw-rw-rw-   0        0        0     6870 2023-01-07 21:43:06.000000 pyl3dmd-0.0.7/pyl3dmd/cpsa.py
--rw-rw-rw-   0        0        0    15385 2023-02-08 02:50:24.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors1set.py
--rw-rw-rw-   0        0        0    24929 2023-02-08 02:54:20.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors2set.py
--rw-rw-rw-   0        0        0    11137 2023-02-08 02:54:29.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors3set.py
--rw-rw-rw-   0        0        0     7700 2023-02-08 02:52:49.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors4set.py
--rw-rw-rw-   0        0        0     3086 2023-02-08 02:52:27.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors5set.py
--rw-rw-rw-   0        0        0     4278 2023-02-08 02:52:17.000000 pyl3dmd-0.0.7/pyl3dmd/descriptors6set.py
--rw-rw-rw-   0        0        0     2146 2022-11-01 17:58:31.000000 pyl3dmd-0.0.7/pyl3dmd/distancedistancematrixdescriptors.py
--rw-rw-rw-   0        0        0     1753 2022-11-23 18:28:22.000000 pyl3dmd-0.0.7/pyl3dmd/geary.py
--rw-rw-rw-   0        0        0    24105 2023-02-02 19:12:07.000000 pyl3dmd-0.0.7/pyl3dmd/geometricdescriptors.py
--rw-rw-rw-   0        0        0     3895 2023-02-08 02:51:59.000000 pyl3dmd-0.0.7/pyl3dmd/getadjacencyanddistancematrices.py
--rw-rw-rw-   0        0        0     8741 2023-02-08 02:53:43.000000 pyl3dmd-0.0.7/pyl3dmd/getatomicproperties.py
--rw-rw-rw-   0        0        0    10313 2023-02-07 08:53:07.000000 pyl3dmd-0.0.7/pyl3dmd/getaway.py
--rw-rw-rw-   0        0        0    10919 2023-02-08 02:55:35.000000 pyl3dmd-0.0.7/pyl3dmd/getinfofromlammpsdatafile.py
--rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.0.7/pyl3dmd/getinfofromlammpstrajfile.py
--rw-rw-rw-   0        0        0     1787 2022-11-23 18:56:51.000000 pyl3dmd-0.0.7/pyl3dmd/moran.py
--rw-rw-rw-   0        0        0     1463 2022-11-23 18:57:26.000000 pyl3dmd-0.0.7/pyl3dmd/moreaubroto.py
--rw-rw-rw-   0        0        0     1593 2022-11-23 18:47:15.000000 pyl3dmd-0.0.7/pyl3dmd/morse.py
--rw-rw-rw-   0        0        0     9558 2023-02-13 17:27:02.000000 pyl3dmd-0.0.7/pyl3dmd/pyl3dmd.py
--rw-rw-rw-   0        0        0     1618 2022-11-24 00:31:54.000000 pyl3dmd-0.0.7/pyl3dmd/rdf.py
--rw-rw-rw-   0        0        0     3271 2023-02-08 02:55:13.000000 pyl3dmd-0.0.7/pyl3dmd/removehydrogenfrommolecule.py
--rw-rw-rw-   0        0        0    14563 2023-02-07 03:57:17.000000 pyl3dmd-0.0.7/pyl3dmd/topologyconnectivity3Ddescriptors.py
--rw-rw-rw-   0        0        0     2262 2022-12-29 23:13:55.000000 pyl3dmd-0.0.7/pyl3dmd/whim.py
-drwxrwxrwx   0        0        0        0 2023-02-13 18:37:14.246790 pyl3dmd-0.0.7/pyl3dmd.egg-info/
--rw-rw-rw-   0        0        0      753 2023-02-13 18:37:14.000000 pyl3dmd-0.0.7/pyl3dmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-02-13 18:37:14.000000 pyl3dmd-0.0.7/pyl3dmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 18:37:14.000000 pyl3dmd-0.0.7/pyl3dmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-13 18:37:14.000000 pyl3dmd-0.0.7/pyl3dmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-13 18:37:14.249781 pyl3dmd-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2272 2023-02-13 18:36:14.000000 pyl3dmd-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:11.332938 pyl3dmd-0.0.8/
+-rw-rw-rw-   0        0        0      753 2023-04-21 18:58:11.331941 pyl3dmd-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:11.322965 pyl3dmd-0.0.8/pyl3dmd/
+-rw-rw-rw-   0        0        0     7978 2023-02-08 04:14:04.000000 pyl3dmd-0.0.8/pyl3dmd/PyL3dMD.py
+-rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.0.8/pyl3dmd/__init__.py
+-rw-rw-rw-   0        0        0    15385 2023-02-08 02:50:24.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors1set.py
+-rw-rw-rw-   0        0        0    24929 2023-02-08 02:54:20.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors2set.py
+-rw-rw-rw-   0        0        0    11137 2023-02-08 02:54:29.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors3set.py
+-rw-rw-rw-   0        0        0     7700 2023-02-08 02:52:49.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors4set.py
+-rw-rw-rw-   0        0        0     3086 2023-02-08 02:52:27.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors5set.py
+-rw-rw-rw-   0        0        0     4278 2023-02-08 02:52:17.000000 pyl3dmd-0.0.8/pyl3dmd/descriptors6set.py
+-rw-rw-rw-   0        0        0     3895 2023-02-08 02:51:59.000000 pyl3dmd-0.0.8/pyl3dmd/getadjacencyanddistancematrices.py
+-rw-rw-rw-   0        0        0     8741 2023-02-08 02:53:43.000000 pyl3dmd-0.0.8/pyl3dmd/getatomicproperties.py
+-rw-rw-rw-   0        0        0    10918 2023-04-21 18:51:02.000000 pyl3dmd-0.0.8/pyl3dmd/getinfofromlammpsdatafile.py
+-rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.0.8/pyl3dmd/getinfofromlammpstrajfile.py
+-rw-rw-rw-   0        0        0     3271 2023-02-08 02:55:13.000000 pyl3dmd-0.0.8/pyl3dmd/removehydrogenfrommolecule.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:11.329946 pyl3dmd-0.0.8/pyl3dmd.egg-info/
+-rw-rw-rw-   0        0        0      753 2023-04-21 18:58:11.000000 pyl3dmd-0.0.8/pyl3dmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-04-21 18:58:11.000000 pyl3dmd-0.0.8/pyl3dmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:58:11.000000 pyl3dmd-0.0.8/pyl3dmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 18:58:11.000000 pyl3dmd-0.0.8/pyl3dmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:58:11.332938 pyl3dmd-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2023-04-21 18:54:36.000000 pyl3dmd-0.0.8/setup.py
```

### Comparing `pyl3dmd-0.0.7/PKG-INFO` & `pyl3dmd-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.0.7/pyl3dmd/__init__.py` & `pyl3dmd-0.0.8/pyl3dmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/cpsa.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors4set.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 # -*- coding: utf-8 -*-
 """
-Created on Sat Nov 26 16:24:36 2022
+Created on Thu December 10 11:41:02 2022
 
-@author: pawan
+@author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 
+
+PyL3dMD: Python LAMMPS 3D Molecular Dynamics/Descriptors
+Copyright (C) 2022  Pawan Panwar, Quanpeng Yang, Ashlie Martini
+
+This file is part of PyL3dMD.
+
+PyL3dMD is free software: you can redistribute it and/or modify 
+it under the terms of the GNU General Public License as published 
+by the Free Software Foundation, either version 3 of the License, 
+or (at your option) any later version.
+
+PyL3dMD is distributed in the hope that it will be useful, but 
+WITHOUT ANY WARRANTY; without even the implied warranty of 
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
+See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+ along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+"""
 This algorithm uses the dot density technique found in:
 
 Shrake, A., and J. A. Rupley. "Environment and Exposure to Solvent
 of Protein Atoms. Lysozyme and Insulin." JMB (1973) 79:351-371.
 
 
 The same approach was used in the Dr. Cao's chemopy package:
```

### Comparing `pyl3dmd-0.0.7/pyl3dmd/descriptors1set.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors1set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/descriptors2set.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors2set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/descriptors3set.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors3set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/descriptors5set.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors5set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/descriptors6set.py` & `pyl3dmd-0.0.8/pyl3dmd/descriptors6set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/getadjacencyanddistancematrices.py` & `pyl3dmd-0.0.8/pyl3dmd/getadjacencyanddistancematrices.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/getatomicproperties.py` & `pyl3dmd-0.0.8/pyl3dmd/getatomicproperties.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/getinfofromlammpsdatafile.py` & `pyl3dmd-0.0.8/pyl3dmd/getinfofromlammpsdatafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
                 if numConnections[k] > 1:
                     if j < k:
                         ii = 0
                         for ii in range (numConnections[j]):
                             i = adjList[j][ii]
                             if i != k:
                                 ll = 0
-                                for ll in range (numConnections[ll]):
+                                for ll in range (numConnections[k]):
                                     l = adjList[k][ll]
                                     if l != j:
                                         dihedrals_list.append([i, j, k, l])
                                     ll = ll+1
                             ii = ii+1
                 kk = kk+1
     dihedrals_list = np.array(dihedrals_list)
```

### Comparing `pyl3dmd-0.0.7/pyl3dmd/getinfofromlammpstrajfile.py` & `pyl3dmd-0.0.8/pyl3dmd/getinfofromlammpstrajfile.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd/pyl3dmd.py` & `pyl3dmd-0.0.8/pyl3dmd/PyL3dMD.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,27 +40,23 @@
 from . import descriptors3set
 from . import descriptors2set
 from . import descriptors1set
 
 import warnings
 warnings.filterwarnings(action='ignore', category=RuntimeWarning)
 
-class pyl3dmd:
-    def __init__(self, datafilename, dumpfilename, numberofcores=None, whichdescriptors=None):
+class PyL3dMD:
+    def __init__(self, datafilename, dumpfilename, numberofcores=None):
         self.datafilename = datafilename
         self.dumpfilename = dumpfilename
         if numberofcores is None:
             self.numberofcores = mp.cpu_count()
         else:
             self.numberofcores = numberofcores
 
-        if whichdescriptors is None:
-            self.whichdescriptors = 'all'
-        else:
-            self.whichdescriptors = whichdescriptors 
         ############################################ PRE-PROCESSING ###########################################
 
         # GET ALL INFORMATIONS FROM LAMMPS DATA FILE
         idAtoms, idMols, atomTypes, atomCharges, atomMasses, atomSection, bondSection = getinfofromlammpsdatafile.getalldatafileinfo(datafilename)
         self.eachMolsNumIdx, self.eachMolsIdx, self.eachMolsMass, self.eachMolsCharge, self.eachMolsBonds, self.eachMolsAngles, self.eachMolsDihedrals = getinfofromlammpsdatafile.arragebymolecule(
             idAtoms, idMols, atomMasses, atomCharges, bondSection)
         numAtoms = len(idAtoms)  # num of atoms in the simulation box
@@ -168,44 +164,19 @@
         apIP = self.eachMolsIP[i]
         apEA = self.eachMolsEA[i]
 
         # calculate Geometric matrix
         G = self.calgeometricdistancematrix(xyz)
 
         # Calculate all descriptors
+        RDF, ATS, GATS, MATS, MoRSE = descriptors6set.getragmmdescriptors(G, charge, apm, apV, apEn, apalapha, apIP, apEA)
+        WHIM = descriptors5set.getwhimdescriptors(xyz, charge, apm, apV, apEn, apalapha, apIP, apEA)
+        CPSA = descriptors4set.getcpsadescriptors(xyz, charge, apRc)
+        GETAWAY = descriptors3set.getgetawayhatsindexes(xyz, mass, bond, charge, apm, apV, apEn, apalapha, apIP, apEA)
+        GMdes, DDMdes = descriptors2set.calgeometricdescriptors(xyz, mass, charge, bond, angle, dihedral, density, disMat)
+        TCdes = descriptors1set.caltopologyconnectivitydescriptors(xyz, mass, bond, angle, dihedral, adjMat, disMat)
+
         others = {'molecule': i + 1, 'Timeframe': j, 'rho': density}
-        
-        if self.whichdescriptors == 'all':
-            RDF, ATS, GATS, MATS, MoRSE = descriptors6set.getragmmdescriptors(G, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            WHIM = descriptors5set.getwhimdescriptors(xyz, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            CPSA = descriptors4set.getcpsadescriptors(xyz, charge, apRc)
-            GETAWAY = descriptors3set.getgetawayhatsindexes(xyz, mass, bond, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            GMdes, DDMdes = descriptors2set.calgeometricdescriptors(xyz, mass, charge, bond, angle, dihedral, density, disMat)
-            TCdes = descriptors1set.caltopologyconnectivitydescriptors(xyz, mass, bond, angle, dihedral, adjMat, disMat)
-            
-            # Combine all dictionaries into a single dictionary to return/store
-            res = {**others, **TCdes, **GMdes, **DDMdes, **GETAWAY, **CPSA, **WHIM, **RDF, **MoRSE, **ATS, **GATS, **MATS}
-            
-        elif self.whichdescriptors == 'set6':
-            RDF, ATS, GATS, MATS, MoRSE = descriptors6set.getragmmdescriptors(G, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            res = {**others, **RDF, **MoRSE, **ATS, **GATS, **MATS}
-        
-        elif self.whichdescriptors == 'set5':
-            WHIM = descriptors5set.getwhimdescriptors(xyz, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            res = {**others, **WHIM}
-        
-        elif self.whichdescriptors == 'set4':
-            CPSA = descriptors4set.getcpsadescriptors(xyz, charge, apRc)
-            res = {**others, **CPSA}
-        
-        elif self.whichdescriptors == 'set3':
-            GETAWAY = descriptors3set.getgetawayhatsindexes(xyz, mass, bond, charge, apm, apV, apEn, apalapha, apIP, apEA)
-            res = {**others, **GETAWAY}
-            
-        elif self.whichdescriptors == 'set2':
-            GMdes, DDMdes = descriptors2set.calgeometricdescriptors(xyz, mass, charge, bond, angle, dihedral, density, disMat)
-            res = {**others, **GMdes, **DDMdes}
-            
-        elif self.whichdescriptors == 'set1':
-            TCdes = descriptors1set.caltopologyconnectivitydescriptors(xyz, mass, bond, angle, dihedral, adjMat, disMat)
-            res = {**others, **TCdes}
+
+        # Combine all dictionaries into a single dictionary to return/store
+        res = {**others, **GMdes, **DDMdes, **TCdes, **RDF, **MoRSE, **ATS, **GATS, **MATS, **WHIM, **GETAWAY, **CPSA}
         return res
```

### Comparing `pyl3dmd-0.0.7/pyl3dmd/removehydrogenfrommolecule.py` & `pyl3dmd-0.0.8/pyl3dmd/removehydrogenfrommolecule.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.7/pyl3dmd.egg-info/PKG-INFO` & `pyl3dmd-0.0.8/pyl3dmd.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.0.7/pyl3dmd.egg-info/SOURCES.txt` & `pyl3dmd-0.0.8/pyl3dmd.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 setup.py
+pyl3dmd/PyL3dMD.py
 pyl3dmd/__init__.py
-pyl3dmd/cpsa.py
 pyl3dmd/descriptors1set.py
 pyl3dmd/descriptors2set.py
 pyl3dmd/descriptors3set.py
 pyl3dmd/descriptors4set.py
 pyl3dmd/descriptors5set.py
 pyl3dmd/descriptors6set.py
-pyl3dmd/distancedistancematrixdescriptors.py
-pyl3dmd/geary.py
-pyl3dmd/geometricdescriptors.py
 pyl3dmd/getadjacencyanddistancematrices.py
 pyl3dmd/getatomicproperties.py
-pyl3dmd/getaway.py
 pyl3dmd/getinfofromlammpsdatafile.py
 pyl3dmd/getinfofromlammpstrajfile.py
-pyl3dmd/moran.py
-pyl3dmd/moreaubroto.py
-pyl3dmd/morse.py
-pyl3dmd/pyl3dmd.py
-pyl3dmd/rdf.py
 pyl3dmd/removehydrogenfrommolecule.py
-pyl3dmd/topologyconnectivity3Ddescriptors.py
-pyl3dmd/whim.py
 pyl3dmd.egg-info/PKG-INFO
 pyl3dmd.egg-info/SOURCES.txt
 pyl3dmd.egg-info/dependency_links.txt
 pyl3dmd.egg-info/top_level.txt
```

### Comparing `pyl3dmd-0.0.7/setup.py` & `pyl3dmd-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors'
 LONG_DESCRIPTION = 'PyL3dMD stands for Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors, a python package for 3D descriptors calculation'
 
 # setup
 setup(
        # name has to be identical with the name of the folder where the package is
         name="pyl3dmd",
```

