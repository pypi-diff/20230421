# Comparing `tmp/dea-tools-0.2.8.dev8.tar.gz` & `tmp/dea-tools-0.2.8.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.2.8.dev8.tar", last modified: Fri Aug 19 05:19:36 2022, max compression
+gzip compressed data, was "dea-tools-0.2.8.dev9.tar", last modified: Tue Aug 30 06:49:00 2022, max compression
```

## Comparing `dea-tools-0.2.8.dev8.tar` & `dea-tools-0.2.8.dev9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-19 05:19:35.000000 dea-tools-0.2.8.dev8/dea_tools/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31477 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (121)    11607 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (121)    19962 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (121)    31368 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (121)    11170 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (121)    19500 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (121)    11754 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (121)    62134 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)    11149 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (121)    40083 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (121)    34879 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (121)    39611 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (121)    42577 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    28904 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)    40780 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (121)    26733 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/dea_tools/waterbodies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-19 05:19:35.000000 dea-tools-0.2.8.dev8/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-19 05:19:36.000000 dea-tools-0.2.8.dev8/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 05:19:35.000000 dea-tools-0.2.8.dev8/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-19 05:19:35.000000 dea-tools-0.2.8.dev8/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-19 05:19:35.000000 dea-tools-0.2.8.dev8/dea_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-19 05:19:36.705079 dea-tools-0.2.8.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-08-19 05:17:32.000000 dea-tools-0.2.8.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31477 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11607 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19962 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31368 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11170 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19500 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11754 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62134 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11149 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40083 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34879 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39611 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42577 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28904 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40832 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26733 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/waterbodies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-30 06:49:00.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/setup.py
```

### Comparing `dea-tools-0.2.8.dev8/LICENSE` & `dea-tools-0.2.8.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/PKG-INFO` & `dea-tools-0.2.8.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev8
+Version: 0.2.8.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: dea@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev8/README.rst` & `dea-tools-0.2.8.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/animations.py` & `dea-tools-0.2.8.dev9/dea_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/changefilmstrips.py` & `dea-tools-0.2.8.dev9/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/crophealth.py` & `dea-tools-0.2.8.dev9/dea_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/deacoastlines.py` & `dea-tools-0.2.8.dev9/dea_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/imageexport.py` & `dea-tools-0.2.8.dev9/dea_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/miningrehab.py` & `dea-tools-0.2.8.dev9/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/app/widgetconstructors.py` & `dea-tools-0.2.8.dev9/dea_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/bandindices.py` & `dea-tools-0.2.8.dev9/dea_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/bom.py` & `dea-tools-0.2.8.dev9/dea_tools/bom.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/classification.py` & `dea-tools-0.2.8.dev9/dea_tools/classification.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/climate.py` & `dea-tools-0.2.8.dev9/dea_tools/climate.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/coastal.py` & `dea-tools-0.2.8.dev9/dea_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/dask.py` & `dea-tools-0.2.8.dev9/dea_tools/dask.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/datahandling.py` & `dea-tools-0.2.8.dev9/dea_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/landcover.py` & `dea-tools-0.2.8.dev9/dea_tools/landcover.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/plotting.py` & `dea-tools-0.2.8.dev9/dea_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/pyfes_model.py` & `dea-tools-0.2.8.dev9/dea_tools/pyfes_model.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/segmentation.py` & `dea-tools-0.2.8.dev9/dea_tools/segmentation.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/spatial.py` & `dea-tools-0.2.8.dev9/dea_tools/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,31 @@
     sun_angles
 
 Last modified: August 2022
 
 '''
 
 # Import required packages
+import fiona
 import collections
 import numpy as np
 import xarray as xr
 import geopandas as gpd
 import rasterio.features
 import scipy.interpolate
+import multiprocessing as mp
 from scipy import ndimage as nd
 from skimage.measure import label
 from rasterstats import zonal_stats
 from skimage.measure import find_contours
 from geopy.geocoders import Nominatim
 from datacube.utils.cog import write_cog
 from datacube.utils.geometry import assign_crs
 from datacube.utils.geometry import CRS, Geometry
-from shapely.geometry import LineString, MultiLineString, shape
+from shapely.geometry import LineString, MultiLineString, shape, mapping
 
 def xr_vectorize(da, 
                  attribute_col='attribute', 
                  transform=None, 
                  crs=None, 
                  dtype='float32',
                  export_shp=False,
@@ -1040,8 +1042,8 @@
     )
 
     # Combine into new xarray.Dataset
     sun_angles_ds = xr.merge(
         [sun_elevation.rename("sun_elevation"), sun_azimuth.rename("sun_azimuth")]
     )
 
-    return sun_angles_ds
+    return sun_angles_ds
```

### Comparing `dea-tools-0.2.8.dev8/dea_tools/temporal.py` & `dea-tools-0.2.8.dev9/dea_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools/waterbodies.py` & `dea-tools-0.2.8.dev9/dea_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/dea_tools.egg-info/PKG-INFO` & `dea-tools-0.2.8.dev9/dea_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev8
+Version: 0.2.8.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: dea@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev8/dea_tools.egg-info/SOURCES.txt` & `dea-tools-0.2.8.dev9/dea_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/index.rst` & `dea-tools-0.2.8.dev9/index.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev8/setup.py` & `dea-tools-0.2.8.dev9/setup.py`

 * *Files identical despite different names*

