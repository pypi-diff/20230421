# Comparing `tmp/element-electrode-localization-0.1.2.tar.gz` & `tmp/element-electrode-localization-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-electrode-localization-0.1.2.tar", last modified: Tue Nov  1 21:40:46 2022, max compression
+gzip compressed data, was "element-electrode-localization-0.1.3.tar", last modified: Fri Apr 21 18:30:19 2023, max compression
```

## Comparing `element-electrode-localization-0.1.2.tar` & `element-electrode-localization-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:46.780070 element-electrode-localization-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-11-01 21:40:46.780070 element-electrode-localization-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:46.780070 element-electrode-localization-0.1.2/element_electrode_localization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/element_electrode_localization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8348 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/element_electrode_localization/coordinate_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     9870 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/element_electrode_localization/electrode_localization.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/element_electrode_localization/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:46.780070 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-11-01 21:40:46.000000 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-01 21:40:46.000000 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:40:46.000000 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-01 21:40:46.000000 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-01 21:40:46.000000 element-electrode-localization-0.1.2/element_electrode_localization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:40:46.780070 element-electrode-localization-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-01 21:40:44.000000 element-electrode-localization-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/element_electrode_localization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/coordinate_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/electrode_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/setup.py
```

### Comparing `element-electrode-localization-0.1.2/LICENSE` & `element-electrode-localization-0.1.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 DataJoint
+Copyright (c) 2023 DataJoint
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `element-electrode-localization-0.1.2/element_electrode_localization/coordinate_framework.py` & `element-electrode-localization-0.1.3/element_electrode_localization/coordinate_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import logging
 import pathlib
-from tqdm import tqdm
+import re
+
 import datajoint as dj
-import pandas as pd
+import nrrd
 import numpy as np
+import pandas as pd
 from tqdm import tqdm
-import nrrd
-import re
-
 
 log = logging.getLogger(__name__)
 schema = dj.schema()
 
 
 def activate(schema_name, *, create_schema=True, create_tables=True):
-    """Activates the schema. 
+    """Activates the schema.
 
     Args:
-        schema_name (str): A string containing the name of the probe scehma.
+        schema_name (str): A string containing the name of the probe schema.
         create_schema (bool): If True, schema will be created in the database.
         create_tables (bool): If True, tables related to the schema will be created in the database.
     """
     schema.activate(
         schema_name, create_schema=create_schema, create_tables=create_tables
     )
 
     # ----------------------------- Table declarations ----------------------
 
 
 @schema
 class CCF(dj.Lookup):
     """Common coordinate framework information.
-    
+
     Attributes:
         ccf_id (foreign key, int): CCF ID/atlas ID.
         ccf_version (varchar(64) ): Allen CCF version.
         ccf_resolution (float): Voxel resolution in microns.
         ccf_description (varchar(255) ): CCF label descriptions.
     """
 
@@ -76,58 +75,59 @@
 
     definition = """
     -> CCF
     """
 
     class BrainRegion(dj.Part):
         """Brain region information.
-        
+
         Attributes:
             BrainRegionAnnotation (foreign key): BrainRegionAnnotation primary key.
             acronym (foreign key, varchar(32) ): Brain region acronym.
             region_name (varchar(128) ): Brain region full name.
             region_id (int): Brain region ID.
-            color_code (varchar(6) ): Hexcode of the color code for this region. 
+            color_code (varchar(6) ): Hex code of the color code for this region.
         """
 
         definition = """
         -> master
         acronym: varchar(32)  # CHARACTER SET utf8 COLLATE utf8_bin
         ---
         region_name: varchar(128)
         region_id=null: int
-        color_code=null: varchar(6)  # hexcode of the color code of this region
+        color_code=null: varchar(6)  # Hex code of the color code of this region
         """
 
     class Voxel(dj.Part):
         """Voxel information from CCF.
 
         Attributes:
             BrainRegion (foreign key): BrainRegionAnnotation.BrainRegion primary key.
             CCF.Voxel (foreign key): CCF.Voxel primary key.
         """
+
         definition = """
         -> master.BrainRegion
         -> CCF.Voxel
         """
 
     @classmethod
     def retrieve_acronym(self, acronym):
         """Retrieve the DataJoint translation of the CCF acronym"""
         return re.sub(r"(?<!^)(?=[A-Z])", "_", acronym).lower()
 
     @classmethod
     def voxel_query(self, x=None, y=None, z=None):
         """Given one or more coordinates, return unique brain regions
-        
+
         Args:
             x (float): x coordinate.
             y (float): y coordinate.
             z (float): z coordinate.
-        
+
         Raises:
             ValueError: Must specificy at least one dimension.
             NotImplementedError: Coming soon.
         """
         if not any(x, y, z):
             raise ValueError("Must specify at least one dimension")
         # query = self.Voxel  #  TODO: add utility function name lookup
@@ -139,15 +139,15 @@
     """Hierarchical structure between the brain regions.
 
     Attributes:
         BrainRegionAnnotation.BrainRegion (foreign key): BrainRegionAnnotation.BrainRegion primary key.
         Parent (query): parent brain region acronym from BrainRegion table
     """
 
-    definition = """ # Hierarchical structure between the brain regionss
+    definition = """ # Hierarchical structure between the brain regions
     -> BrainRegionAnnotation.BrainRegion
     ---
     -> BrainRegionAnnotation.BrainRegion.proj(parent='acronym')
     """
 
 
 # ---- HELPERS ----
```

### Comparing `element-electrode-localization-0.1.2/element_electrode_localization/electrode_localization.py` & `element-electrode-localization-0.1.3/element_electrode_localization/electrode_localization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import inspect
-import pathlib
 import json
 import logging
+import pathlib
+
 import datajoint as dj
 import numpy as np
 
 from . import coordinate_framework
 
 schema = dj.schema()
 
@@ -20,18 +21,18 @@
     electrode_localization_schema_name,
     coordinate_framework_schema_name=None,
     *,
     create_schema=True,
     create_tables=True,
     linking_module=None,
 ):
-    """Activates the `electrode_localization` and `coordinate_framework` schemas. 
+    """Activates the `electrode_localization` and `coordinate_framework` schemas.
 
     Args:
-        electrode_localization_schema_name (str): A string containing the name of the 
+        electrode_localization_schema_name (str): A string containing the name of the
             electrode_localization schema.
         coordinate_framework_schema_name (str): A string containing the name of the coordinate_framework schema.
         create_schema (bool): If True, schema will be created in the database.
         create_tables (bool): If True, tables related to the schema will be created in the database.
         linking_module (str): A string containing the module name or module containing the required dependencies to activate the schema.
     """
 
@@ -63,18 +64,18 @@
 # --------------- Functions required by element-electrode-localization  ----------------
 
 
 def get_electrode_localization_dir(probe_insertion_key: dict) -> str:
     """Retrieve the electrode localization directory associated with a ProbeInsertion.
 
     The directory should contain `channel_locations.json` files (one per shank)for the corresponding `probe_insertion_key`.
-    
+
     Args:
         probe_insertion_key (dict): key of a ProbeInsertion.
-    
+
     Returns:
         The full file-path of the electrode localization dir.
     """
     return _linking_module.get_electrode_localization_dir(probe_insertion_key)
 
 
 # ------------------------------------ Table declarations -----------------------------
@@ -107,16 +108,15 @@
         -> master
         -> probe.ProbeType.Electrode
         ---
         -> coordinate_framework.CCF.Voxel
         """
 
     def make(self, key):
-        """Populates electrode position tables.
-        """
+        """Populates electrode position tables."""
         skipped_electrode_count = 0
         voxel_resolution = (coordinate_framework.CCF & key).fetch1("ccf_resolution")
         electrode_location_dir = pathlib.Path(get_electrode_localization_dir(key))
         assert electrode_location_dir.exists()
 
         channel_locations_files = list(
             electrode_location_dir.glob("*channel_locations*.json")
```

### Comparing `element-electrode-localization-0.1.2/setup.py` & `element-electrode-localization-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
-from setuptools import setup, find_packages
 from os import path
 
+from setuptools import find_packages, setup
+
 pkg_name = next(p for p in find_packages() if "." not in p)
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), "r") as f:
     long_description = f.read()
 
 with open(path.join(here, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 with open(path.join(here, pkg_name, "version.py")) as f:
     exec(f.read())
 
 setup(
     name=pkg_name.replace("_", "-"),
-    version=__version__,
+    version=__version__,  # noqa: F821
     description="Electrode localization DataJoint element",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataJoint",
     author_email="info@datajoint.com",
     license="MIT",
     url=f'https://github.com/datajoint/{pkg_name.replace("_", "-")}',
```

