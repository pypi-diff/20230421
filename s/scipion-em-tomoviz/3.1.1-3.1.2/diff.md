# Comparing `tmp/scipion-em-tomoviz-3.1.1.tar.gz` & `tmp/scipion-em-tomoviz-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomoviz-3.1.1.tar", last modified: Thu Mar 30 11:21:47 2023, max compression
+gzip compressed data, was "scipion-em-tomoviz-3.1.2.tar", last modified: Thu Apr 20 09:35:46 2023, max compression
```

## Comparing `scipion-em-tomoviz-3.1.1.tar` & `scipion-em-tomoviz-3.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.370855 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 11:21:47.000000 scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/tomoviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)   192251 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/icon_square.png
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/tomoviz/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_mesh_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_particle_pick_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_particle_pick_remove_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/tomoviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/tests/test_tomo3D_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:21:47.374855 scipion-em-tomoviz-3.1.1/tomoviz/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28984 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_triangulations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-03-30 11:20:00.000000 scipion-em-tomoviz-3.1.1/tomoviz/viewers/views_tkinter_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.876229 scipion-em-tomoviz-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-20 09:35:46.876229 scipion-em-tomoviz-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.872229 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 09:35:46.000000 scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:35:46.876229 scipion-em-tomoviz-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.872229 scipion-em-tomoviz-3.1.2/tomoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192251 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/icon_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.872229 scipion-em-tomoviz-3.1.2/tomoviz/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_mesh_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_particle_pick_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_particle_pick_remove_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.872229 scipion-em-tomoviz-3.1.2/tomoviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/tests/test_tomo3D_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:35:46.872229 scipion-em-tomoviz-3.1.2/tomoviz/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30287 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_triangulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-20 09:33:49.000000 scipion-em-tomoviz-3.1.2/tomoviz/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-tomoviz-3.1.1/LICENSE` & `scipion-em-tomoviz-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/PKG-INFO` & `scipion-em-tomoviz-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-tomoviz
-Version: 3.1.1
+Version: 3.1.2
 Summary: Tools for 3D visualization and manipulation of tomography data
 Home-page: https://github.com/scipion-em/scipion-em-tomoviz
 Author: you
 Author-email: you@yourinstitution.email
 License: UNKNOWN
 Description: =======================
         Scipion tomoviz plugin
```

### Comparing `scipion-em-tomoviz-3.1.1/README.rst` & `scipion-em-tomoviz-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/PKG-INFO` & `scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-tomoviz
-Version: 3.1.1
+Version: 3.1.2
 Summary: Tools for 3D visualization and manipulation of tomography data
 Home-page: https://github.com/scipion-em/scipion-em-tomoviz
 Author: you
 Author-email: you@yourinstitution.email
 License: UNKNOWN
 Description: =======================
         Scipion tomoviz plugin
```

### Comparing `scipion-em-tomoviz-3.1.1/scipion_em_tomoviz.egg-info/SOURCES.txt` & `scipion-em-tomoviz-3.1.2/scipion_em_tomoviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/setup.py` & `scipion-em-tomoviz-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/__init__.py` & `scipion-em-tomoviz-3.1.2/tomoviz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.plugin as pwplugin
 
-__version__ = "3.1.1"
+__version__ = "3.1.2"
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwplugin.Plugin):
     pass
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/bibtex.py` & `scipion-em-tomoviz-3.1.2/tomoviz/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/icon.png` & `scipion-em-tomoviz-3.1.2/tomoviz/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/icon_square.png` & `scipion-em-tomoviz-3.1.2/tomoviz/icon_square.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/loading.gif` & `scipion-em-tomoviz-3.1.2/tomoviz/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/protocols/__init__.py` & `scipion-em-tomoviz-3.1.2/tomoviz/protocols/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .protocol_particle_pick_consensus import ProtTomoConsensusPicking
 from .protocol_particle_pick_remove_duplicates import ProtTomoPickingRemoveDuplicates
-from .protocol_mesh_normal import XmippProtFilterbyNormal
+from .protocol_mesh_normal import XmippProtFilterbyNormal, TomovizProtFilterbyNormal
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_mesh_normal.py` & `scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_mesh_normal.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,40 +24,45 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from os import path
 import numpy as np
+
+from pwem.objects import EMSet
 from pyworkflow import BETA
 from pyworkflow.protocol.params import PointerParam, FloatParam, BooleanParam, IntParam
 import pwem.convert.transformations as tfs
 from pwem.protocols import EMProtocol
-from tomo.objects import SubTomogram, Coordinate3D
+from tomo.objects import SetOfCoordinates3D, SubTomogram
 from tomo.protocols import ProtTomoBase
 from tomo.utils import normalFromMatrix
 import tomo.constants as const
 from ..utils import delaunayTriangulation, computeNormals
 
 
-class XmippProtFilterbyNormal(EMProtocol, ProtTomoBase):
+OUTPUT_NAME = 'outputset'
+class TomovizProtFilterbyNormal(EMProtocol, ProtTomoBase):
     """ This protocol takes surfaces or ROIs (SetOfMeshes) and a SetOfSubtomograms or SetOfCoordinates3D with
     transformation matrix and filters them by different criteria related with the normal direction."""
 
     _label = 'filter by normal'
     _devStatus = BETA
+    _possibleOutputs = {OUTPUT_NAME: EMSet}
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
+        self.outputset = None
 
     # --------------------------- DEFINE param functions ------------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('input', PointerParam, pointerClass="SetOfSubTomograms, SetOfCoordinates3D",
-                      label='Subtomograms/Coordinates', help='SetOfSubtomograms to filter.')
+                      label='Subtomograms/Coordinates', help='Coordinates to filter.')
         form.addParam('inputMeshes', PointerParam, label="Vesicles", pointerClass='SetOfMeshes',
                       help='Select the vesicles in which the subtomograms/coordinates are.')
         form.addParam('tilt', BooleanParam, default=False,
                       label='Filter by tilt angle',
                       help='Remove items depending on their tilt angle.')
         form.addParam('maxtilt', IntParam, default=150, label='Maximum allowed tilt', condition='tilt',
                       help='Remove the items that have a tilt angle bigger than the one specified in here, '
@@ -83,84 +88,73 @@
         #               help='Remove the subtomograms that are in the missing wedge direction because they are highly '
         #                    'affected by the missing wedge.')
         # form.addParam('mwDir', EnumParam, default=True, label='Missing wedge direction',
         #               help='Missing wedge direction of the tomograms.')
 
     # --------------------------- INSERT steps functions --------------------------------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep('computeNormalStep')
-        self._insertFunctionStep('createOutputStep')
+        self._insertFunctionStep(self.computeNormalStep)
 
     # --------------------------- STEPS functions -------------------------------
     def computeNormalStep(self):
         inSet = self.input.get()
         tiltBool = self.tilt.get()
         normalBool = self.normalDir.get()
         inMeshes = self.inputMeshes.get()
 
         # If filter by normal => create dictionary of input meshes
         if normalBool:
             tol = self.tol.get() * np.pi / 180
             # Create dictionary of meshes:  key = "tomoId_groupId" (each vesicle of each tomogram)
             #                               value = [points, normals] (coordinates with origin, normals of the coords)
             meshDict = {}
+
+            # Get the unique meshes and tomograms
             for meshPoint in inMeshes.iterCoordinates():  # Iterate over points (coordinates) in the input SetOfMeshes
                 tomoId = meshPoint.getTomoId()
                 groupId = meshPoint.getGroupId()
                 key = "%s_%d" % (tomoId, groupId)
                 if key not in meshDict.keys():
+                    self.info("New vesicle (%s) found for tomogram %s" % (groupId, tomoId))
                     meshDict[key] = [[meshPoint.getPosition(const.SCIPION)], 0]
+
                 else:
                     meshDict[key][0].append(meshPoint.getPosition(const.SCIPION))
-            meshPoint.getPosition(const.SCIPION)
+
 
             for meshKey in meshDict:  # iterate over keys
-                meshPoint.getPosition(const.SCIPION)
                 # write normals in position [1] of the value list for each mesh by passing to _getNormalVesicleList
                 # the coordinates in the mesh, that are in position [0] of the value list
                 meshDict[meshKey][1] = self._getNormalVesicleList(np.asarray(meshDict[meshKey][0]))
 
-        # Create corresponding output depending on the input type of object
-        if self._getInputisSubtomo(inSet.getFirstItem()):
-            self.outSet = self._createSetOfSubTomograms()
-        else:
-            self.outSet = self._createSetOfCoordinates3D(inMeshes.getPrecedents())
-        self.outSet.copyInfo(inSet)
+        # Create the set
+        outSet = inSet.create(self.getPath())
+        # Copy set properties
+        outSet.copyInfo(inSet)
 
         # If filter by tilt
         if tiltBool:
-            if self._getInputisSubtomo(inSet.getFirstItem()):
-                for item in inSet:
-                    tilt = self._getTilt(item)
-                    if self.maxtilt.get() > tilt > self.mintilt.get():
-                        # If filter by tilt and normal
-                        if normalBool:
-                            self._filterByNormal(item, tol, meshDict)
-                        else:
-                            self.outSet.append(item)
-            else:
-                for item in inSet.iterCoordinates(volume=None):
-                    tilt = self._getTilt(item)
-                    if self.maxtilt.get() > tilt > self.mintilt.get():
-                        if normalBool:
-                            self._filterByNormal(item, tol, meshDict)
-                        else:
-                            self.outSet.append(item)
+            for item in inSet.iterCoordinates(volume=None):
+                tilt = self._getTilt(item)
+                if self.maxtilt.get() > tilt > self.mintilt.get():
+                    if normalBool:
+                        self._filterByNormal(item, tol, meshDict, outSet)
+                    else:
+                        outSet.append(item)
 
         if normalBool and not tiltBool:
-            if self._getInputisSubtomo(inSet.getFirstItem()):
-                for item in inSet:
-                    self._filterByNormal(item, tol, meshDict)
-            else:
-                for item in inSet.iterCoordinates(volume=None):
-                    self._filterByNormal(item, tol, meshDict)
-
-    def createOutputStep(self):
-        self._defineOutputs(outputset=self.outSet)
-        self._defineSourceRelation(self.input.get(), self.outSet)
+            iterator = inSet.iterCoordinates if isinstance(inSet, SetOfCoordinates3D) else inSet.iterSubtomos
+            for item in iterator(volume=None):
+                self._filterByNormal(item, tol, meshDict, outSet)
+
+        # Register the set
+        self._defineOutputs(**{OUTPUT_NAME:outSet})
+        self._defineSourceRelation(self.input.get(), outSet)
+    def _isInputASetOfCoordinates(self):
+        return isinstance(self.input.get(), SetOfCoordinates3D)
 
     # --------------------------- INFO functions --------------------------------
     def _validate(self):
         validateMsgs = []
         if not self.normalDir.get() and not self.tilt.get():
             validateMsgs.append('Some filter should be switched to "Yes"')
         if not self.input.get().getFirstItem().hasTransform():
@@ -194,58 +188,53 @@
             # if self.topBottom:
             #     methods.append("Particles in the top and bottom parts of the vesicles have been removed.")
             # if self.mwDir:
             #     methods.append("Particles in the missing wedge direction have been removed.")
         return methods
 
     # --------------------------- UTILS functions --------------------------------------------
-    def _getInputisSubtomo(self, item):
-        if isinstance(item, SubTomogram):
-            return True
-        else:
-            return False
-
     def _getVesicleId(self, item):
-        if isinstance(item, SubTomogram):
-            c = item.getCoordinate3D()
-        else:
-            c = item
+
+        c = item
+
         if c.hasGroupId():
             vesicleId = c.getGroupId()
         else:  # For now it works with several vesicles in the same tomo just for input items with groupId
             vesicleId = 1
         return vesicleId
 
     def _getNormalVesicleList(self, points):
         triangulation = delaunayTriangulation(points)
         normalsList = computeNormals(triangulation, associateCoords=True)
         return normalsList
 
-    def _getNormalVesicle(self, normalsList, item):
-        if self._getInputisSubtomo(item):
-            normSubtomo = normalFromMatrix(item.getTransform().getMatrix())
-            coord = item.getCoordinate3D()
-        else:
-            normSubtomo = normalFromMatrix(item.getMatrix())
-            coord = item
+    def _getNormalVesicle(self, normalsList, coord):
+
+        normSubtomo = normalFromMatrix(coord.getMatrix())
         coors = np.asarray([coord.getX(const.SCIPION),
                             coord.getY(const.SCIPION),
                             coord.getZ(const.SCIPION)])
         points, normals = zip(*normalsList)
         points = np.asarray(points)
         idx = np.argmin(np.sum((points - coors) ** 2, axis=1))
         return normSubtomo, normals[idx]
 
     def _getTilt(self, item):
-        if self._getInputisSubtomo(item):
-            _, tilt, _ = tfs.euler_from_matrix(item.getTransform().getMatrix(), axes='szyz')
-        else:
-            _, tilt, _ = tfs.euler_from_matrix(item.getMatrix(), axes='szyz')
+
+        _, tilt, _ = tfs.euler_from_matrix(item.getMatrix(), axes='szyz')
         tilt = -np.rad2deg(tilt)
         return tilt
 
-    def _filterByNormal(self, item, tol, meshDict):
-        meshfromDict = meshDict["%s_%i" % (item.getTomoId(), item.getGroupId())]
-        normSubtomo, normVesicle = self._getNormalVesicle(meshfromDict[1], item)
+    def _filterByNormal(self, item, tol, meshDict,outputSet):
+
+        coord = item.getCoordinate3D() if isinstance(item, SubTomogram) else item
+
+        meshfromDict = meshDict["%s_%i" % (coord.getTomoId(), coord.getGroupId())]
+        normSubtomo, normVesicle = self._getNormalVesicle(meshfromDict[1], coord)
         if abs(normSubtomo[0] - normVesicle[0]) < tol and abs(normSubtomo[1] - normVesicle[1]) < tol and \
                 abs(normSubtomo[2] - normVesicle[2]) < tol:
-            self.outSet.append(item)
+            outputSet.append(item)
+
+class XmippProtFilterbyNormal(TomovizProtFilterbyNormal):
+    @classmethod
+    def isDisabled(cls):
+        return True
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_particle_pick_consensus.py` & `scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_particle_pick_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/protocols/protocol_particle_pick_remove_duplicates.py` & `scipion-em-tomoviz-3.1.2/tomoviz/protocols/protocol_particle_pick_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/tests/__init__.py` & `scipion-em-tomoviz-3.1.2/tomoviz/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/tests/test_tomo3D_base.py` & `scipion-em-tomoviz-3.1.2/tomoviz/tests/test_tomo3D_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/utils.py` & `scipion-em-tomoviz-3.1.2/tomoviz/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/__init__.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_mrc.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_mrc.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
 import pyworkflow.utils as pwutils
 
 from pwem.emlib.image import ImageHandler
 
 import tomoviz
 
+COLOR_MAP = 'gist_rainbow_r' #'terrain'
+
 
 class MrcPlot(object):
     '''
     Class to visualize MRC files
     Input paramters:
          - tomo_mrc (Path (Str) - Optional): File containing a Volume (in MRC format)
          - mask_mrc (Path (Str) - Optional): File containing a Mask (in MRC format)
@@ -68,15 +70,15 @@
     Usage:
          import MRCPlot
          plt = MRCPlot(tomo_mrc=tomo_mrc, mask_mrc=mask_mrc, binning=2)
          plt.initializePlot()
     '''
 
     def __init__(self, tomo_mrc=None, mask_mrc=None, points=None, boxSize=None, normals=None,
-                 binning=None, sigma=1., triangulation=False):
+                 binning=None, sigma=1., triangulation=False, discrete=False):
         if binning is None:
             if tomo_mrc is not None:
                 self.binning = self.getBinning(tomo_mrc)
             elif mask_mrc is not None:
                 self.binning = self.getBinning(mask_mrc)
             else:
                 self.binning = 0
@@ -84,29 +86,28 @@
             self.binning = binning
         self.tomo = (tomo_mrc, triangulation, sigma)
         self.mask = mask_mrc
         self.points = np.loadtxt(points, delimiter=' ') if points is not None else None
         self.normals = np.loadtxt(normals, delimiter=' ') if normals is not None else None
         self.boxSize = boxSize / 2 ** self.binning if boxSize is not None else None
         self.save_basename = pwutils.removeBaseExt(tomo_mrc) if tomo_mrc is not None and points is not None else None
+        self.discrete = discrete
 
         # Get Pyvista Objects
         if isinstance(self.points, np.ndarray):
             self.points_ids = self.points[:, 3]
             self.group_ids = self.points[:, 4]
             self.points = np.column_stack([self.points[:, 1], self.points[:, 0], self.points[:, 2]])
             self.points /= 2 ** self.binning  # Binning Scaling
             self.pv_points = pv.PolyData(self.points)
-            scalar_colors = np.zeros([self.points.shape[0], 4])
-            cmap = matplotlib.cm.get_cmap('gist_rainbow_r')
+            scalar_colors = np.zeros([self.points.shape[0]])
             unique_ids = np.unique(self.group_ids)
-            cmap_ids = np.linspace(0, 1, len(unique_ids))
-            for group_id, cmap_id in zip(unique_ids, cmap_ids):
+            for group_id in unique_ids:
                 idp = np.where(self.group_ids == group_id)
-                scalar_colors[idp] = cmap(cmap_id)
+                scalar_colors[idp] = group_id
             self.pv_points["colors"] = scalar_colors
         if isinstance(self.normals, np.ndarray):
             self.normals = np.column_stack([self.normals[:, 1], self.normals[:, 0], self.normals[:, 2]])
             # vecLength = np.amax(pdist(self.pv_points.points))
             self.normals /= np.linalg.norm(self.normals, axis=1)[:, np.newaxis]
             # self.normals *= vecLength
             self.pv_normals = pv.pyvista_ndarray(self.normals)
@@ -116,14 +117,21 @@
         self.mask_actors = []
         self.points_actor = []
         self.normals_actor = None
         self.box_actor = {}
 
         self.first_reset = True
 
+        # Theme
+        from pyvista.themes import DocumentTheme
+        customTheme = DocumentTheme()
+        customTheme.cmap = COLOR_MAP
+        customTheme.color_cycler = 'default'
+        pv.set_plot_theme(customTheme)
+
         self.plt = pvqt.BackgroundPlotter(title='Scipion tomoviz viewer')
         self.plt.main_menu.clear()
         plugin_path = os.path.dirname(tomoviz.__file__)
         self.plt.app.setWindowIcon(QtGui.QIcon(os.path.join(plugin_path, "icon_square.png")))
         self.loading_screen = LoadingScreen()
 
         pos = 0.
@@ -313,15 +321,15 @@
 
         if isinstance(self.normals, np.ndarray):
             pos += 170. if pos != 0 else 45.
             self.plt.add_text('Directions', position=(pos, 65.), font_size=12)
             self.buttonNormals = self.plt.add_checkbox_button_widget(callback=self.plotNormals, position=(pos, 10.))
 
     def getBinning(self, file):
-        dim = ImageHandler().read(file + ':mrc').getDimensions()
+        dim = ImageHandler().read(file).getDimensions()
         return int(np.floor(max(dim) / 400))
 
     def readMRC(self, file, binning=1, order=0, swapaxes=True):
         image = ImageHandler().read(file + ':mrc')
         data = np.squeeze(image.getData())
         data = zoom(data, 1 / (2 ** binning), order=order, prefilter=False)
         data = np.swapaxes(np.swapaxes(data, 0, 2), 1, 0) if swapaxes else data
@@ -340,23 +348,27 @@
         grid = pv.StructuredGrid(x, y, z)
 
         # Set the cell values. Previous reordering of the axis was needed to flatten properly the array
         grid.cell_arrays["values"] = data.flatten(order="K")
 
         return grid
 
-    def surfaceFromMRC(self, data, label=1):
+    def surfaceFromMRC(self, data, binarize=True, label=1):
         '''Function to convert an MRC file into an Structure Surface in VTK'''
 
         # Get Only mesh corresponding to a given label (smooth the result to fill holes in the mask)
-        data = data == label
-        data = binary_erosion(binary_dilation(data, selem=ball(4)), selem=ball(1))
+        if binarize:
+            data = data == label
+            data = binary_erosion(binary_dilation(data, selem=ball(4)), selem=ball(1))
+
+            # Triangulate coordinates using marching cubes algorithm
+            grid = self.marchingCubes(data)
 
-        # Triangulate coordinates using marching cubes algorithm
-        grid = self.marchingCubes(data)
+        else:
+            grid = self.marchingCubes(data, level=label)
 
         # Fix the mesh
         mfix = pm._meshfix.PyTMesh(False)
         mfix.load_array(grid.points, grid.faces.reshape((-1, 4))[:, 1:])
         mfix.join_closest_components()
         mfix.fill_small_boundaries(refine=True)
         vert, faces = mfix.return_arrays()
@@ -381,33 +393,44 @@
     def histogram(self, volume):
         hist, edges = np.histogram(volume, bins=100)
         hist = hist / np.sum(hist)
         bin_centers = np.mean(np.vstack([edges[0:-1], edges[1:]]), axis=0)
         return hist, bin_centers
 
     def contours(self, hist, bin_centers):
-        logic_slicing = np.where((hist > np.std(hist)) * (hist < np.amax(hist)))
-        sliced_hist = hist[logic_slicing]
-        opacities = 1 - sliced_hist
-        contour_values = bin_centers[logic_slicing]
-        # print(1 - opacities)
-        # print(np.mean(1-opacities))
-        # print(contour_values)
-        logic_slicing_2 = np.where(sliced_hist < np.mean(sliced_hist))
-        contour_values = contour_values[logic_slicing_2]
-        # print(contour_values)
-        opacities = opacities[logic_slicing_2]
+        if self.discrete:
+            logic_slicing = np.where(hist != 0)
+            sliced_hist = hist[logic_slicing]
+            logic_slicing_2 = np.where(sliced_hist != 0)
+            contour_values = bin_centers[logic_slicing]
+            contour_values = contour_values[logic_slicing_2]
+            opacities = np.ones(contour_values.shape) * 0.3
+        else:
+            logic_slicing = np.where((hist > np.std(hist)) * (hist < np.amax(hist)))
+            sliced_hist = hist[logic_slicing]
+            logic_slicing_2 = np.where(sliced_hist < np.mean(sliced_hist))
+            opacities = 1 - sliced_hist
+            contour_values = bin_centers[logic_slicing]
+            # print(1 - opacities)
+            # print(np.mean(1-opacities))
+            # print(contour_values)
+            contour_values = contour_values[logic_slicing_2]
+            # print(contour_values)
+            opacities = opacities[logic_slicing_2]
         return contour_values, opacities
 
     def isovolumes(self, volume, range=0.01, sigma=None, triangulation=True):
         volume = volume if sigma is None else gaussian_filter(volume, sigma=sigma)
         hist, bin_centers = self.histogram(volume)
         contour_values, opacities = self.contours(hist, bin_centers)
-        opacities = (range / (np.amax(opacities) - np.amin(opacities))) * (opacities - np.amin(opacities))
-        return [self.marchingCubes(volume, level, triangulation) for level in contour_values], opacities
+        if not self.discrete:
+            opacities = (range / (np.amax(opacities) - np.amin(opacities))) * (opacities - np.amin(opacities))
+            return [self.marchingCubes(volume, level, triangulation) for level in contour_values], opacities
+        else:
+            return [self.surfaceFromMRC(volume, binarize=False, label=level) for level in contour_values], opacities
 
     def downsamplingPC(self, coords, voxel_size):
         non_empty_voxel_keys, inverse, nb_pts_per_voxel = np.unique(((coords - np.min(coords, axis=0))
                                                                      // voxel_size).astype(int), axis=0,
                                                                     return_inverse=True,
                                                                     return_counts=True)
         idx_pts_vox_sorted = np.argsort(inverse)
@@ -457,21 +480,21 @@
         else:
             for actor in self.mask_actors:
                 self.plt.remove_actor(actor)
             self.graph_actor = []
 
     def plotPoints(self, value):
         if value:
+            reset_camera = False
             if self.first_reset:
                 self.first_reset = False
-                self.points_actor.append(self.plt.add_mesh(self.pv_points, show_scalar_bar=False, scalars="colors",
-                                                           cmap="gist_rainbow_r", render_points_as_spheres=True, reset_camera=True))
-            else:
-                self.points_actor.append(self.plt.add_mesh(self.pv_points, show_scalar_bar=False, scalars="colors",
-                                                           cmap="gist_rainbow_r", render_points_as_spheres=True, reset_camera=False))
+                reset_camera=True
+
+            self.points_actor.append(self.plt.add_mesh(self.pv_points, show_scalar_bar=False, scalars="colors", categories=True,
+                                           render_points_as_spheres=True, reset_camera=reset_camera))
         else:
             for actor in self.points_actor:
                 self.plt.remove_actor(actor)
             self.points_actor = []
 
     def plotBoxes(self, value):
         if value:
@@ -484,21 +507,21 @@
         else:
             for actor in self.box_actor.values():
                 self.plt.remove_actor(actor)
             self.box_actor = {}
 
     def plotNormals(self, value):
         if value:
+            reset_camera = False
             if self.first_reset:
                 self.first_reset = False
-                self.normals_actor = self.plt.add_arrows(self.pv_points.cell_centers().points, self.pv_normals,
-                                                         mag=10, color='red', reset_camera=True)
-            else:
-                self.normals_actor = self.plt.add_arrows(self.pv_points.cell_centers().points, self.pv_normals,
-                                                         mag=10, color='red', reset_camera=False)
+                reset_camera = True
+
+            self.normals_actor = self.plt.add_arrows(self.pv_points.cell_centers().points, self.pv_normals,
+                                                         mag=5, color='red', reset_camera=reset_camera)
         else:
             self.plt.remove_actor(self.normals_actor)
             self.normals_actor = None
 
     def initializePlot(self):
         # By default coordinates button is toggled
         if self.points is not None:
@@ -529,20 +552,30 @@
         self.thread.finished.connect(self.thread.deleteLater)
         self.thread.start()
 
     def showTomogram(self, load=True):
         if load:
             self.tomo, self.pv_tomo, self.opacities, self.pv_tomo_slice = self.worker.output
             self.loading_screen.stopAnimation()
-        cmap = matplotlib.cm.get_cmap('bone')  # Greys also looks nice
-        cmap_ids = np.linspace(0, 1, len(self.pv_tomo))
-        self.tomo_actor = [self.plt.add_mesh(actor, show_scalar_bar=False, opacity=3 * op, color=cmap(cid),
-                                             render_points_as_spheres=True)
-                           for actor, op, cid in zip(self.pv_tomo, self.opacities, cmap_ids)]
-        self.plt.reset_camera()
+        if self.pv_tomo:
+            if self.discrete:
+                cmap = matplotlib.cm.get_cmap('Set3')
+                cmap_ids = np.linspace(0, 1, len(self.pv_tomo))
+                self.tomo_actor = [self.plt.add_mesh(actor, show_scalar_bar=False, opacity=op, color=cmap(cid),
+                                                     render_points_as_spheres=True)
+                                   for actor, op, cid in zip(self.pv_tomo, self.opacities, cmap_ids)]
+            else:
+                cmap = matplotlib.cm.get_cmap('bone')  # Greys also looks nice
+                cmap_ids = np.linspace(0, 1, len(self.pv_tomo))
+                self.tomo_actor = [self.plt.add_mesh(actor, show_scalar_bar=False, opacity=3 * op, color=cmap(cid),
+                                                     render_points_as_spheres=True)
+                                   for actor, op, cid in zip(self.pv_tomo, self.opacities, cmap_ids)]
+            self.plt.reset_camera()
+        else:
+            self.buttonTomo.GetRepresentation().SetState(False)
 
     def showSlices(self, load=True):
         if load:
             self.tomo, self.pv_tomo, self.opacities, self.pv_tomo_slice = self.worker.output
             self.loading_screen.stopAnimation()
         self.tomo_slice_actor = self.plt.add_mesh_slice(self.pv_tomo_slice, normal='z', cmap="gray",
                                                         show_scalar_bar=False,
@@ -597,15 +630,20 @@
 
     def runTomoLoading(self):
         triangulation = self.viewer.tomo[1]
         sigma = self.viewer.tomo[2]
         tomo = self.viewer.readMRC(self.viewer.tomo[0], order=5, binning=self.viewer.binning)
         if isinstance(tomo, np.ndarray):
             pv_tomo_slice = self.viewer.gridFromMRC(tomo)
-            pv_tomo, opacities = self.viewer.isovolumes(tomo, triangulation=triangulation, sigma=sigma)
+            try:
+                pv_tomo, opacities = self.viewer.isovolumes(tomo, triangulation=triangulation, sigma=sigma)
+            except:
+                print("3D Tomogram view could not be computed, only slice mode will be available")
+                pv_tomo = None
+                opacities = None
         self.output = (tomo, pv_tomo, opacities, pv_tomo_slice)
         self.finished.emit()
 
     def runMaskLoading(self):
         mask = self.viewer.readMRC(self.viewer.mask, binning=self.viewer.binning)
         if isinstance(mask, np.ndarray):
             labels = np.unique(mask)[1:]
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_triangulations.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_triangulations.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
+import logging
+logger = logging.getLogger(__name__)
 import pyvista as pv
 import numpy as np
 from scipy.spatial.distance import pdist
 from multiprocessing import Process
 
 from PyQt5.QtWidgets import QApplication, QMainWindow, QDockWidget
 from pyvistaqt.plotting import QtInteractor
@@ -187,22 +188,22 @@
         - methodName (string): Method from the class to be called after the instantiation
         - *args (list): extra argument needed to call the class method
         - **kwargs (dict): arguments to be passed to the contructor of the class
     '''
     try:
         instance = classObj(**kwargs)
         runMethod(instance, methodName, *args)
-    except:
-        print('Cannot create instance of class')
+    except Exception as e:
+        logger.info('Cannot create instance of class %s' % classObj, exc_info=e)
     
 def runMethod(instance, methodName, *args):
     '''
     Execute a method from an instantiated class:
         - instance (obj): object instantiated from a given class
         - methodName (string): method belonging to instance to be called
         - *args (list): extra arguments needed by the method
     '''
     try:
         method = getattr(instance, methodName)
         method(*args)
-    except AttributeError:
-        print(methodName + ' is not a member the class')
+    except AttributeError as e:
+        logger.error(methodName + ' is not a member the class', exc_info=e)
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewer_vtk.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewer_vtk.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/viewers_data.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/viewers_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,94 +23,125 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import os.path
 
 import numpy as np
 import pyworkflow.viewer as pwviewer
-from pyworkflow.object import String
-from pyworkflow.gui.dialog import askYesNo
+from pyworkflow.gui.dialog import askYesNo, showInfo
 from pyworkflow.utils.properties import Message
 import pyworkflow.utils as pwutils
 
 from pwem.protocols import EMProtocol
 import pwem.viewers.views as vi
 from .views_tkinter_tree import Tomo3DTreeProvider
-from .views_tkinter_tree import Tomo3DDialog, ViewerMRCDialog
+from .views_tkinter_tree import ViewerMRCDialog
 
 import tomo.objects
 from ..protocols import XmippProtFilterbyNormal
 
 
 class TomoVizDataViewer(pwviewer.Viewer):
     """ Wrapper to visualize different type of objects
     using pyvista
     """
     _environments = [pwviewer.DESKTOP_TKINTER]
     _targets = [
         tomo.objects.SetOfCoordinates3D,
-        XmippProtFilterbyNormal
+        XmippProtFilterbyNormal,
+        tomo.objects.SetOfTiltSeriesCoordinates,
+        tomo.objects.SetOfSubTomograms
     ]
 
     def __init__(self, **kwargs):
         pwviewer.Viewer.__init__(self, **kwargs)
         self._views = []
 
     def _getObjView(self, obj, fn, viewParams={}):
         return vi.ObjectView(
             self._project, obj.strId(), fn, viewParams=viewParams)
 
     def _visualize(self, obj, **kwargs):
         views = []
         cls = type(obj)
 
+        itemField = tomo.objects.Tomogram.TS_ID_FIELD
+
         if issubclass(cls, tomo.objects.SetOfCoordinates3D):
             outputCoords = obj
+            tomos = outputCoords.getPrecedents()
+            groupAttribute = tomo.objects.Coordinate3D.TOMO_ID_ATTR
+
+        elif issubclass(cls, tomo.objects.SetOfSubTomograms):
+            outputCoords = obj.getCoordinates3D()
+            if outputCoords is None:
+                showInfo("3D coordinates missing",
+                         "This set of subtomograms is not associated with a set of coordinates 3d and cannot be used in this coordinate viewer.",
+                         parent=self.getParent().root)
+                return []
+            tomos = outputCoords.getPrecedents()
+
+            # Keep subtomos as the main collection, since Subtomograms subsets do not affect the coordinates set
+            outputCoords = obj
+            groupAttribute = tomo.objects.SubTomogram.VOL_NAME_FIELD
+
         elif issubclass(cls, EMProtocol):
             outputCoords = obj.inputMeshes.get()
+            tomos = outputCoords.getPrecedents()
+            groupAttribute = "_volId"
 
-        tomos = outputCoords.getPrecedents()
+        elif issubclass(cls, tomo.objects.SetOfTiltSeriesCoordinates):
+            outputCoords = obj
+            tomos = outputCoords.getSetOfTiltSeries()
+            groupAttribute = "_tsId"
+            itemField = groupAttribute
 
-        volIds = outputCoords.aggregate(["MAX", "COUNT"], "_volId", ["_volId"])
-        volIds = [(d['_volId'], d["COUNT"]) for d in volIds]
+        volIds = outputCoords.aggregate(["MAX", "COUNT"], groupAttribute, [groupAttribute])
+        volIds = [(d[groupAttribute], d["COUNT"]) for d in volIds]
 
         tomoList = []
         for objId in volIds:
-            tomogram = tomos[objId[0]].clone()
+            tomogram = tomos[{itemField:objId[0]}].clone()
             tomogram.count = objId[1]
             tomoList.append(tomogram)
                         # tomoList = [String(tomos[objId].getFileName()) for objId in volIds]
         tomoProvider = Tomo3DTreeProvider(tomoList)
-        ViewerMRCDialog(self._tkRoot, outputCoords, provider=tomoProvider)
-
-        import tkinter as tk
-        frame = tk.Frame()
-        if askYesNo(Message.TITLE_SAVE_OUTPUT, Message.LABEL_SAVE_OUTPUT, frame):
-            protocol = self.protocol
-            suffix = protocol._getOutputSuffix(tomo.objects.SetOfCoordinates3D)
-            updated_set = protocol._createSetOfCoordinates3D(tomos, suffix)
-            updated_set.setName("Selected Coordinates")
-            updated_set.setPrecedents(tomos)
-            updated_set.setSamplingRate(tomos.getSamplingRate())
-            updated_set.setBoxSize(outputCoords.getBoxSize())
-            for item in tomoList:
-                basename = pwutils.removeBaseExt(item.getFileName())
-                indices_file = basename + '_indices.txt'
-                if os.path.isfile(indices_file):
-                    indices = np.loadtxt(indices_file, delimiter=' ')
-                    for index in indices:
-                        updated_set.append(outputCoords[index].clone())
-                    pwutils.cleanPath(indices_file)
-            name = protocol.OUTPUT_PREFIX + suffix
-            args = {}
-            args[name] = updated_set
-            protocol._defineOutputs(**args)
-            protocol._defineSourceRelation(tomos, updated_set)
-            protocol._updateOutputSet(name, updated_set, state=updated_set.STREAM_CLOSED)
-        else:
-            for item in tomoList:
-                basename = pwutils.removeBaseExt(item.getFileName())
-                indices_file = basename + '_indices.txt'
-                if os.path.isfile(indices_file):
-                    pwutils.cleanPath(indices_file)
+        viewer = ViewerMRCDialog(self._tkRoot, outputCoords, self.protocol,
+                                 provider=tomoProvider,
+                                 allowSelect= False,
+                                 cancelButton=True)
+
+        # For now we only generate 3d coordinates
+        if viewer.haveCoordinatesChanged() and isinstance(cls, tomo.objects.SetOfCoordinates3D):
+            import tkinter as tk
+            frame = tk.Frame()
+            if askYesNo(Message.TITLE_SAVE_OUTPUT, Message.LABEL_SAVE_OUTPUT, frame):
+                protocol = self.protocol
+                suffix = protocol._getOutputSuffix(tomo.objects.SetOfCoordinates3D)
+                updated_set = protocol._createSetOfCoordinates3D(tomos, suffix)
+                updated_set.setName("Selected Coordinates")
+                updated_set.setPrecedents(tomos)
+                updated_set.setSamplingRate(tomos.getSamplingRate())
+                updated_set.setBoxSize(outputCoords.getBoxSize())
+                for item in tomoList:
+                    basename = pwutils.removeBaseExt(item.getFileName())
+                    indices_file = basename + '_indices.txt'
+                    if os.path.isfile(indices_file):
+                        indices = np.loadtxt(indices_file, delimiter=' ')
+                        for index in indices:
+                            updated_set.append(outputCoords[index].clone())
+                        pwutils.cleanPath(indices_file)
+                name = protocol.OUTPUT_PREFIX + suffix
+                args = {}
+                args[name] = updated_set
+                protocol._defineOutputs(**args)
+                protocol._defineSourceRelation(tomos, updated_set)
+                protocol._updateOutputSet(name, updated_set, state=updated_set.STREAM_CLOSED)
+            else:
+                for item in tomoList:
+                    basename = item.getTsId()
+                    indices_file = basename + '_indices.txt'
+                    if os.path.isfile(indices_file):
+                        pwutils.cleanPath(indices_file)
 
-        return views
+        # TODO: This should return a list of views and not already launching the dialog.
+        return []
```

### Comparing `scipion-em-tomoviz-3.1.1/tomoviz/viewers/views_tkinter_tree.py` & `scipion-em-tomoviz-3.1.2/tomoviz/viewers/views_tkinter_tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,38 +20,41 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import numpy as np
+
+from pyworkflow.protocol import Protocol
 from pyworkflow import utils as pwutils
 from pyworkflow.gui.dialog import ToolbarListDialog
 from pyworkflow.gui.tree import TreeProvider
+from tomo.objects import SetOfTiltSeriesCoordinates
 
 from .viewer_triangulations import TriangulationPlot, guiThread
 from .viewer_mrc import MrcPlot
 from ..utils import delaunayTriangulation
 
 from tomo.utils import extractVesicles, initDictVesicles, normalFromMatrix
 import tomo.constants as const
 
 class Tomo3DTreeProvider(TreeProvider):
-    """ Populate Tree from SetOfTomograms. """
+    """ Populate Tree from SetOfTomograms or SetOfTiltSeries"""
 
     def __init__(self, tomoList):
         TreeProvider.__init__(self)
         self.tomoList = tomoList
 
     def getColumns(self):
-        return [('Tomogram', 300), ("# coords", 100)]
+        return [('Item', 300), ("# coords", 100)]
 
     def getObjectInfo(self, tomo):
-        tomogramName = pwutils.removeBaseExt(tomo.getFileName())
-        # tomogramName = pwutils.removeBaseExt(tomo.get())
+
+        tomogramName = tomo.getTsId()
 
         return {'key': tomogramName, 'parent': None,
                 'text': tomogramName,
                 'values':(tomo.count),
                 'tags': ("done")}
 
     def getObjectPreview(self, obj):
@@ -127,35 +130,63 @@
 
 class ViewerMRCDialog(ToolbarListDialog):
     """
     This class extend from ListDialog to allow calling
     a pyvista viewer subprocess from a list of Tomograms.
     """
 
-    def __init__(self, parent, coords, **kwargs):
+    def __init__(self, parent, coords, protocol:Protocol, **kwargs):
         self.coords = coords
+        self.prot = protocol
         self.provider = kwargs.get("provider", None)
         ToolbarListDialog.__init__(self, parent,
-                                   "Tomogram List",
+                                   "Tomogram list",
                                    allowsEmptySelection=False,
                                    itemDoubleClick=self.doubleClickOnTomogram,
                                    **kwargs)
 
     def doubleClickOnTomogram(self, tomo=None):
         tomo_path = tomo.getFileName()
         coord_list = []
         direction_list = []
-        for coord in self.coords.iterCoordinates(volume=tomo):
-            direction = normalFromMatrix(coord.getMatrix())
-            position = [coord.getX(const.BOTTOM_LEFT_CORNER),
-                        coord.getY(const.BOTTOM_LEFT_CORNER),
-                        coord.getZ(const.BOTTOM_LEFT_CORNER),
-                        coord.getObjId()]
-            position.append(coord.getGroupId()) if coord.getGroupId() is not None else position.append(0)
-            coord_list.append(position)
-            direction_list.append(direction)
-        boxSize = self.coords.getBoxSize()
-        np.savetxt('positions.txt', np.asarray(coord_list))
-        np.savetxt('directions.txt', np.asarray(direction_list))
-        viewer_args = {'tomo_mrc': tomo_path, 'points': 'positions.txt', 'normals': 'directions.txt',
+        boxSize = 32
+
+        def fromCoordinated3D():
+            for coord in self.coords.iterCoordinates(volume=tomo):
+                direction = normalFromMatrix(coord.getMatrix())
+                position = [coord.getX(const.BOTTOM_LEFT_CORNER),
+                            coord.getY(const.BOTTOM_LEFT_CORNER),
+                            coord.getZ(const.BOTTOM_LEFT_CORNER),
+                            coord.getObjId()]
+                position.append(coord.getGroupId()) if coord.getGroupId() is not None else position.append(0)
+                coord_list.append(position)
+                direction_list.append(direction)
+            boxSize = self.coords.getBoxSize()
+
+        def fromTiltSeriesCoordinates():
+            for coord in self.coords.iterItems(where="_tsId='%s'" % tomo.getTsId()):
+                direction = normalFromMatrix(np.eye(4))
+                position = [coord.getX(),
+                            coord.getY(),
+                            coord.getZ(),
+                            coord.getObjId(),
+                            0] # Group Id
+                coord_list.append(position)
+                direction_list.append(direction)
+
+        if not isinstance(self.coords, SetOfTiltSeriesCoordinates):
+            fromCoordinated3D()
+        else:
+            fromTiltSeriesCoordinates()
+
+        posFile = self.prot.getPath('positions.txt')
+        directionsFile= self.prot.getPath('directions.txt')
+        np.savetxt(posFile, np.asarray(coord_list))
+        np.savetxt(directionsFile, np.asarray(direction_list))
+        viewer_args = {'tomo_mrc': tomo_path, 'points': posFile, 'normals': directionsFile,
                        'boxSize': boxSize}
+
         guiThread(MrcPlot, 'initializePlot', **viewer_args)
+
+    def haveCoordinatesChanged(self):
+        # TODO: Add logic to check if coordinates have changed (removed)
+        return False
```

