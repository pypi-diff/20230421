# Comparing `tmp/reixs-0.5.5.tar.gz` & `tmp/reixs-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.5.tar", last modified: Thu Apr 13 20:37:48 2023, max compression
+gzip compressed data, was "reixs-0.5.6.tar", last modified: Fri Apr 21 21:34:55 2023, max compression
```

## Comparing `reixs-0.5.5.tar` & `reixs-0.5.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-13 20:37:38.000000 reixs-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 20:37:48.048618 reixs-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-13 20:37:38.000000 reixs-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 20:37:38.000000 reixs-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 20:37:48.048618 reixs-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.044618 reixs-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    57205 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:34:55.534074 reixs-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-21 21:34:41.000000 reixs-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-21 21:34:55.534074 reixs-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-21 21:34:41.000000 reixs-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 21:34:41.000000 reixs-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-21 21:34:55.534074 reixs-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:34:55.526074 reixs-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:34:55.530074 reixs-0.5.6/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    59076 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-21 21:34:41.000000 reixs-0.5.6/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:34:55.534074 reixs-0.5.6/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-21 21:34:55.000000 reixs-0.5.6/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 21:34:55.000000 reixs-0.5.6/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:34:55.000000 reixs-0.5.6/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-21 21:34:55.000000 reixs-0.5.6/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 21:34:55.000000 reixs-0.5.6/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.5/LICENSE` & `reixs-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/PKG-INFO` & `reixs-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.5
+Version: 0.5.6
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.5/README.md` & `reixs-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/setup.cfg` & `reixs-0.5.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.5
+version = 0.5.6
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.5/src/reixs/LoadData.py` & `reixs-0.5.6/src/reixs/LoadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Edge Dict
 from .edges import EdgeDict
 
 # Data Processing Functions
 from .util import COLORP, all_list_entries_equal
 from .xeol import *
-from .add_subtract import ScanAddition, ScanSubtraction, ImageAddition
+from .add_subtract import ScanAddition, ScanSubtraction, ImageAddition, ImageSubtraction
 from .sca import loadSCAscans
 from .mca import loadMCAscans
 from .mesh import loadMeshScans
 from .rsxs_mcp import loadRSXS1dROIscans, loadRSXS2dROIscans, loadRSXSImageStack
 from .beamline_info import loadSCAbeamline, get_single_beamline_value
 
 #########################################################################################
@@ -637,14 +637,49 @@
         self.detector.append(detector)
         self.filename.append(file)
 
         if kwargs['energyloss'] == True:
             self.x_stream[-1] = "Energy loss (eV)"
             self.y_stream[-1] = "Mono Energy (eV)"
 
+    def subtract(self, basedir, file, x_stream, y_stream, detector, *args, **kwargs):
+        """
+        Subtract specified images for selected streams.
+
+        Parameters
+        ----------
+        See loader function.
+        Subtracts all imnages from the first element.
+
+        """
+        # Set the defaults if not specified in **kwargs.
+        # Set the defaults if not specified in **kwargs.
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("xoffset", None)
+        kwargs.setdefault("xcoffset", None)
+        kwargs.setdefault("yoffset", None)
+        kwargs.setdefault("ycoffset", None)
+        kwargs.setdefault("background", None)
+        kwargs.setdefault("grid_x", [None, None, None])
+        kwargs.setdefault("grid_y", [None, None, None])
+        kwargs.setdefault("energyloss", False)
+
+        # Append all REIXS scan objects to scan list in current object.
+        self.data.append(ImageSubtraction(basedir, file, x_stream,
+                         y_stream, detector, *args, **kwargs))
+        
+        self.x_stream.append(x_stream)
+        self.y_stream.append(y_stream)
+        self.detector.append(detector)
+        self.filename.append(file)
+
+        if kwargs['energyloss'] == True:
+            self.x_stream[-1] = "Energy loss (eV)"
+            self.y_stream[-1] = "Mono Energy (eV)"
+
     def xlim(self, lower, upper):
         """
         Set x-axis plot window limits.
 
         Parameters
         ----------
         lower : float
@@ -877,28 +912,42 @@
                             self.exportfile.selected_filename)
         self.export(file)
 
 
 class EEMsLoader(Load2d):
     """Specific 2d loader for excitation-emission-maps."""
 
-    def load(self, basedir, file, detector, *args, **kwargs):
-        x_stream = 'Mono Energy'
-
+    def get_scale(self, detector):
         if detector == "MCP":
-            y_stream = "MCP Energy"
+            return "MCP Energy"
         elif detector == "SDD":
-            y_stream = "SDD Energy"
+            return "SDD Energy"
         elif detector == "XEOL":
-            y_stream = "XEOL Energy"
+            return "XEOL Energy"
         else:
             raise TypeError("Detector not defined.")
 
+    def load(self, basedir, file, detector, *args, **kwargs):
+        x_stream = 'Mono Energy'
+        y_stream = self.get_scale(detector)
+
         super().load(basedir, file, x_stream, y_stream, detector, *args, **kwargs)
 
+    def add(self, basedir, file, detector, *args, **kwargs):
+        x_stream = "Mono Energy"
+        y_stream = self.get_scale(detector)
+
+        super().add(basedir, file, x_stream, y_stream, detector, *args, **kwargs)
+
+    def subtract(self, basedir, file, detector, *args, **kwargs):
+        x_stream = "Mono Energy"
+        y_stream = self.get_scale(detector)
+
+        super().subtract(basedir, file, x_stream, y_stream, detector, *args, **kwargs)
+
 #########################################################################################
 
 
 class LoadMesh:
     """Class to display (x,y,z) scatter data."""
 
     def __init__(self):
```

### Comparing `reixs-0.5.5/src/reixs/ReadData.py` & `reixs-0.5.6/src/reixs/ReadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/add_subtract.py` & `reixs-0.5.6/src/reixs/add_subtract.py`

 * *Files 12% similar despite different names*

```diff
@@ -306,8 +306,77 @@
 
     data[0].scan = name
 
     # Normalize data to [0,1]
     if norm == True:
         data[0].MASTER_detector =  data[0].MASTER_detector / max(data[0].MASTER_detector)
 
+    return data
+
+def ImageSubtraction(basedir, file, x_stream, y_stream, detector, *args, norm=True, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None,grid_x=[None, None, None],grid_y=[None, None,None], background=None, energyloss=False):
+    """Internal function to handle image addition.
+
+    Parameters
+    ----------
+    args : Same as for the Load2d class
+    kwargs: See Load2d class
+    """
+
+   # Define generic object in which all data will be stored
+    class added_object:
+        def __init__(self):
+            pass
+
+    # Ensure we only add a unique scan once
+    for i in args:
+        if args.count(i) > 1:
+            raise ValueError("Cannot add the same scan to itself")
+
+    # Get the appropriate data first - same loader as always
+    Scandata =  loadMCAscans(basedir, file, x_stream, y_stream, detector, *args, norm=False, xoffset=xoffset, xcoffset=xcoffset, yoffset=yoffset, ycoffset=ycoffset,grid_x=[None, None, None],grid_y=[None, None, None], background=background, energyloss=False)
+
+    # Iterate over all loaded scans
+    for i, (k, v) in enumerate(Scandata.items()):
+    # Set the first scan as master data
+        if i == 0:
+            MASTER_x_stream = v.new_x
+            MASTER_y_stream = v.new_y
+            MASTER_detector = v.new_z
+            MASTER_xmin = v.xmin
+            MASTER_xmax = v.xmax
+            MASTER_ymin = v.ymin
+            MASTER_ymax = v.ymax
+            name = str(k)+'+'
+        else:
+            # Ensure that we only add emission scans when the spectrometer energy scale is identical
+            if not np.array_equal(MASTER_y_stream, v.new_y):
+                    raise ValueError(
+                        "Cannot add spectra with different energy scales.")
+            
+            interp = interp2d(v.new_x,v.new_y,v.new_z)
+            new_z = interp(MASTER_x_stream,MASTER_y_stream)
+
+            MASTER_detector = np.subtract(MASTER_detector,new_z)
+            
+            name += "_" + str(k)
+
+    if energyloss == True or grid_x!=[None, None, None] or grid_y!=[None, None,None]:
+        MASTER_xmin, MASTER_xmax, MASTER_ymin, MASTER_ymax, MASTER_x_stream, MASTER_y_stream, MASTER_detector = grid_data2d(MASTER_x_stream, MASTER_y_stream, MASTER_detector, grid_x=grid_x,grid_y=grid_y,energyloss=energyloss)
+
+    # Place data in a dictionary with the same structure as a regular Load1d call, so that we can plot it
+    data = dict()
+    data[0] = added_object()
+    data[0].new_x = MASTER_x_stream
+    data[0].new_y = MASTER_y_stream
+    data[0].new_z = MASTER_detector
+    data[0].xmin = MASTER_xmin
+    data[0].xmax = MASTER_xmax
+    data[0].ymin = MASTER_ymin
+    data[0].ymax = MASTER_ymax
+
+    data[0].scan = name
+
+    # Normalize data to [0,1]
+    if norm == True:
+        data[0].MASTER_detector =  data[0].MASTER_detector / max(data[0].MASTER_detector)
+
     return data
```

### Comparing `reixs-0.5.5/src/reixs/beamline_info.py` & `reixs-0.5.6/src/reixs/beamline_info.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/mca.py` & `reixs-0.5.6/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/mesh.py` & `reixs-0.5.6/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/parser.py` & `reixs-0.5.6/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/rixs_readutil.py` & `reixs-0.5.6/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/rsxs_mcp.py` & `reixs-0.5.6/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/rsxs_readutil.py` & `reixs-0.5.6/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/sca.py` & `reixs-0.5.6/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/simplemath.py` & `reixs-0.5.6/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/spec_config.py` & `reixs-0.5.6/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/util.py` & `reixs-0.5.6/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs/xeol.py` & `reixs-0.5.6/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.5/src/reixs.egg-info/PKG-INFO` & `reixs-0.5.6/src/reixs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.5
+Version: 0.5.6
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.5/src/reixs.egg-info/SOURCES.txt` & `reixs-0.5.6/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

