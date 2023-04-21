# Comparing `tmp/seg2map-0.0.8.tar.gz` & `tmp/seg2map-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg2map-0.0.8.tar", last modified: Tue Apr 18 20:22:29 2023, max compression
+gzip compressed data, was "seg2map-0.0.9.tar", last modified: Tue Apr 18 23:59:12 2023, max compression
```

## Comparing `seg2map-0.0.8.tar` & `seg2map-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 20:22:15.000000 seg2map-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-18 20:22:15.000000 seg2map-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 20:22:29.397714 seg2map-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-04-18 20:22:15.000000 seg2map-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 20:22:15.000000 seg2map-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:22:29.397714 seg2map-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 20:22:15.000000 seg2map-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.393713 seg2map-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/src/seg2map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58158 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/log_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/model_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/models_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/new_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42245 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/zoo_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/src/seg2map.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:59:12.340094 seg2map-0.0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 23:59:03.000000 seg2map-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-18 23:59:03.000000 seg2map-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 23:59:12.340094 seg2map-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-04-18 23:59:03.000000 seg2map-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 23:59:03.000000 seg2map-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 23:59:12.340094 seg2map-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 23:59:03.000000 seg2map-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:59:12.336094 seg2map-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:59:12.340094 seg2map-0.0.9/src/seg2map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58183 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/log_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/map_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/map_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/model_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/models_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/new_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44781 2023-04-18 23:59:03.000000 seg2map-0.0.9/src/seg2map/zoo_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:59:12.340094 seg2map-0.0.9/src/seg2map.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 23:59:12.000000 seg2map-0.0.9/src/seg2map.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 23:59:12.000000 seg2map-0.0.9/src/seg2map.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:59:12.000000 seg2map-0.0.9/src/seg2map.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 23:59:12.000000 seg2map-0.0.9/src/seg2map.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 23:59:12.000000 seg2map-0.0.9/src/seg2map.egg-info/top_level.txt
```

### Comparing `seg2map-0.0.8/LICENSE` & `seg2map-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/PKG-INFO` & `seg2map-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `seg2map-0.0.8/README.md` & `seg2map-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/pyproject.toml` & `seg2map-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seg2map"
 dynamic = ["readme"]
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name=" Sharon Fitzpatrick", email="sharon.fitzpatrick23@gmail.com" },
 ]
 # find` directive with `include` or `exclude`
 description = "An interactive jupyter notebook for downloading satellite imagery"
 dependencies = [
   "scikit-image",
```

### Comparing `seg2map-0.0.8/src/seg2map/common.py` & `seg2map-0.0.9/src/seg2map/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,32 +668,33 @@
 
     Args:
         files (List[str]): List of file paths to TIFF files to be converted.
         translateoptions (str, optional): GDAL options for converting TIFF files to JPEG files.
         kwargs(dict, optional): dictionary of GDAL options for converting TIFF files to JPEG files. Options located at:
             https://gdal.org/api/python/osgeo.gdal.html#osgeo.gdal.TranslateOptions
     Returns:
-        List[str]: List of file paths to the newly created JPEG files.
+        List[str]: List of file paths to the JPEG files.
     """
-    new_files = []
+    jpg_files = []
     for file in files:
         jpg_file = file.replace(".tif", ".jpg")
         if os.path.exists(jpg_file):
             logger.info(f"File: {jpg_file} already exists")
+            jpg_files.append(jpg_file)
         else:
             if kwargs:
                 dst = gdal.Translate(jpg_file, file, **kwargs)
-                new_files.append(jpg_file)
+                jpg_files.append(jpg_file)
             elif translateoptions:
                 dst = gdal.Translate(jpg_file, file, options=translateoptions)
-                new_files.append(jpg_file)
+                jpg_files.append(jpg_file)
             else:
                 raise ValueError("Must provide value for kwargs or translateoptions.")
             dst = None  # close and save ds
-    return new_files
+    return jpg_files
 
 
 def rename_files(directory: str, pattern: str, new_name: str, replace_name: str):
     """Rename all files in a directory that match a glob pattern
 
     Args:
         directory (str): the path to the directory containing the files to be renamed
```

### Comparing `seg2map-0.0.8/src/seg2map/downloads.py` & `seg2map-0.0.9/src/seg2map/downloads.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/exception_handler.py` & `seg2map-0.0.9/src/seg2map/exception_handler.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/exceptions.py` & `seg2map-0.0.9/src/seg2map/exceptions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/log_maker.py` & `seg2map-0.0.9/src/seg2map/log_maker.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/map_UI.py` & `seg2map-0.0.9/src/seg2map/map_UI.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/map_functions.py` & `seg2map-0.0.9/src/seg2map/map_functions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/map_interface.py` & `seg2map-0.0.9/src/seg2map/map_interface.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/model_functions.py` & `seg2map-0.0.9/src/seg2map/model_functions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/models_UI.py` & `seg2map-0.0.9/src/seg2map/models_UI.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/new_downloads.py` & `seg2map-0.0.9/src/seg2map/new_downloads.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/roi.py` & `seg2map-0.0.9/src/seg2map/roi.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/sessions.py` & `seg2map-0.0.9/src/seg2map/sessions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.8/src/seg2map/zoo_model.py` & `seg2map-0.0.9/src/seg2map/zoo_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Set
+from typing import Dict, List, Optional, Set
 from typing import Dict, Any
 import requests
 import logging
 import os
 import shutil
 import json
 from pathlib import Path
@@ -84,23 +84,24 @@
     Returns:
         Dict[str, Any]: The updated model dictionary with the new sample directory, or None if input directory is empty.
 
     """
     if len(os.listdir(year_dir)) == 0:
         logger.warning(f"len(os.listdir({year_dir})) == 0")
         return {}
+    # everything after this assumes that the directory is not empty
     # Construct the file path to the original merged multispectral image
     original_merged_tif = os.path.join(year_dir, "merged_multispectral.tif")
     # Create a new "tiles" directory within the year_dir
     tiles_path = common.create_directory(year_dir, "tiles")
     # Generate overlapping tiles from the original merged multispectral image and get the new tiles path
     tiles_path = create_overlapping_tiles(original_merged_tif, tiles_path)
     # Check if the returned tiles_path is empty or None, log a warning and return an empty dictionary if true
-    if tiles_path == "" or tiles_path is None:
-        logger.warning(f"Empty or None tiles_path for {year_dir}")
+    if not tiles_path:
+        logger.warning(f"Overlap operation failed for {year_dir} for merged tif: {original_merged_tif}")
         return {}
     # Create a copy of the model dictionary and update the sample directory with the new tiles path
     model_year_dict = model_dict.copy()
     model_year_dict["sample_direc"] = tiles_path
     return model_year_dict
 
 def get_sorted_files_with_extension(
@@ -255,34 +256,82 @@
     outVRT = os.path.join(tif_location, "Mosaic_greyscale.vrt")
     outTIF = os.path.join(tif_location, "Mosaic_greyscale.tif")
     common.build_vrt(outVRT, imgsToMosaic, resampleAlg="mode")
     # create greyscale tiff
     common.build_tiff(outTIF, outVRT)
     return outTIF
 
+def gdal_retile(tif_path: str, tiles_path: str, OVERLAP_PX: Optional[int] = None, TARGET_SIZE: int = 768)->str:
+    """
+    Retiles a merged GeoTIFF file into smaller overlapping tiles of the specified size.
+
+    Args:
+        tif_path (str): Path to the input GeoTIFF file.
+        tiles_path (str): Output directory where generated tiles will be saved.
+        OVERLAP_PX (int, optional): Number of pixels to overlap between tiles. Defaults to None, which calculates the overlap as half of the target tile size.
+        TARGET_SIZE (int, optional): Target size of each tile in pixels (width and height). Defaults to 768.
+
+    Returns:
+        str: The output directory where the generated tiles are saved.
+
+    Raises:
+        Exception: If an error occurs during the retile process.
+    """
+    try:
+        # retile merged tif and create tiles with overlap
+        if not OVERLAP_PX:
+            OVERLAP_PX = TARGET_SIZE // 2
+        # run retile script with system command. retiles merged_multispectral.tif to become many tif files that overlap each other
+        cmd = f"python gdal_retile.py -r near -ot Byte -ps {TARGET_SIZE} {TARGET_SIZE} -overlap {OVERLAP_PX} -co 'tiled=YES' -targetDir {tiles_path} {tif_path}"
+        os.system(cmd)
+        # return location of tiles that were created
+    except Exception as e:
+        logger.error(f"{e}\ntif_path: {tif_path}\n tiles_path: {tiles_path}\n OVERLAP_PX: {OVERLAP_PX}\n TARGET_SIZE: {TARGET_SIZE}")
+        raise e
+    return tiles_path
 
 def create_overlapping_tiles(
     tif_path: str, tiles_path: str, OVERLAP_PX: int = None, TARGET_SIZE: int = 768
-):
-    # retile merged tif and create jpgs ready for model
-    if not OVERLAP_PX:
-        OVERLAP_PX = TARGET_SIZE // 2
-    # run retile script with system command. retiles merged_multispectral.tif to have overlap
-    cmd = f"python gdal_retile.py -r near -ot Byte -ps {TARGET_SIZE} {TARGET_SIZE} -overlap {OVERLAP_PX} -co 'tiled=YES' -targetDir {tiles_path} {tif_path}"
-    os.system(cmd)
-    tif_files = glob(os.path.join(tiles_path, "*.tif"))
-    kwargs = {"format": "JPEG", "outputType": gdal.GDT_Byte}
-    # create jpgs for new tifs
-    common.gdal_translate_jpegs(tif_files, kwargs=kwargs)
-    # delete tif files
+)->str:
+    """
+    Creates overlapping tiles of a GeoTIFF file and converts them to JPEG format.
+
+    Args:
+        tif_path (str): Path to the input GeoTIFF file.
+        tiles_path (str): Output directory where generated tiles will be saved.
+        OVERLAP_PX (int, optional): Number of pixels to overlap between tiles. Defaults to None, which calculates the overlap as half of the target tile size.
+        TARGET_SIZE (int, optional): Target size of each tile in pixels (width and height). Defaults to 768.
+
+    Returns:
+        str: The output directory where the generated overlapping JPEG tiles are saved.
+
+    Raises:
+        FileNotFoundError: If the input GeoTIFF file is not found.
+    """
+    if not os.path.exists(tif_path):
+        raise FileNotFoundError(f"File {tif_path} does not exist")
+    # retile merged tif to create tifs with overlap
+    tiles_location = gdal_retile(tif_path, tiles_path, OVERLAP_PX, TARGET_SIZE)
+    tif_files = glob(os.path.join(tiles_location, "*.tif"))
+    if not tif_files:
+        logger.error(f"Overlap failed. No tif files were found in {tiles_location}")
+        raise Exception(f"Overlap failed. No tif files were found in {tiles_location}")
+        return ""
+    
+    jpeg_kwargs = {"format": "JPEG", "outputType": gdal.GDT_Byte}
+    # Convert tif files to jpgs
+    jpg_files = common.gdal_translate_jpegs(tif_files, kwargs=jpeg_kwargs)
+    if not jpg_files:
+        logger.error(f"Overlap failed. No jpg files were found in {tiles_location}")
+        raise Exception(f"Overlap failed. No tif files were found in {tiles_location}")
+        return ""
+    # delete tif files to save space
     for file in tif_files:
         os.remove(file)
-    if len(os.listdir(tiles_path)) == 0:
-        logger.warning(f"{tiles_path} is empty. No tiles were created.")
-        return None
+    # return location of overlapping jpgs that were created
     return tiles_path
 
 
 def download_url(
     url: str, save_path: str, progress_bar_name: str = "", chunk_size: int = 1024
 ):
     """Downloads the model from the given url to the save_path location.
```

### Comparing `seg2map-0.0.8/src/seg2map.egg-info/PKG-INFO` & `seg2map-0.0.9/src/seg2map.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `seg2map-0.0.8/src/seg2map.egg-info/SOURCES.txt` & `seg2map-0.0.9/src/seg2map.egg-info/SOURCES.txt`

 * *Files identical despite different names*

