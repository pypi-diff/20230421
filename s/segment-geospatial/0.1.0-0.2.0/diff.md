# Comparing `tmp/segment-geospatial-0.1.0.tar.gz` & `tmp/segment-geospatial-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.1.0.tar", last modified: Wed Apr 19 20:24:43 2023, max compression
+gzip compressed data, was "segment-geospatial-0.2.0.tar", last modified: Fri Apr 21 13:57:28 2023, max compression
```

## Comparing `segment-geospatial-0.1.0.tar` & `segment-geospatial-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.742399 segment-geospatial-0.1.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/setup.py
```

### Comparing `segment-geospatial-0.1.0/LICENSE` & `segment-geospatial-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.1.0/PKG-INFO` & `segment-geospatial-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,26 @@
-Metadata-Version: 2.1
-Name: segment-geospatial
-Version: 0.1.0
-Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
-Home-page: https://github.com/opengeos/segment-geospatial
-Author: Qiusheng Wu
-Author-email: giswqs@gmail.com
-License: MIT license
-Keywords: samgeo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # segment-geospatial
 
-[![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/examples/basic_usage.ipynb)
-[![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/examples/basic_usage.ipynb&branch=main)
-[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/examples/basic_usage.ipynb)
+[![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
+[![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
+[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
-**Meta AI' Segment Anything Model (SAM) for Geospatial Data**
+**A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: https://samgeo.gishub.org
 
 ## Features
 
--   TODO
+-   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
+-   Segment GeoTIFF files using the Segment Anything Model (SAM)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.1.0/samgeo/common.py` & `segment-geospatial-0.2.0/samgeo/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,14 +62,144 @@
         extension = "." + extension
     file_id = str(uuid.uuid4())
     file_path = os.path.join(tempfile.gettempdir(), f"{file_id}{extension}")
 
     return file_path
 
 
+def github_raw_url(url):
+    """Get the raw URL for a GitHub file.
+
+    Args:
+        url (str): The GitHub URL.
+    Returns:
+        str: The raw URL.
+    """
+    if isinstance(url, str) and url.startswith("https://github.com/") and "blob" in url:
+        url = url.replace("github.com", "raw.githubusercontent.com").replace(
+            "blob/", ""
+        )
+    return url
+
+
+def download_file(
+    url=None,
+    output=None,
+    quiet=False,
+    proxy=None,
+    speed=None,
+    use_cookies=True,
+    verify=True,
+    id=None,
+    fuzzy=False,
+    resume=False,
+    unzip=True,
+    overwrite=False,
+    subfolder=False,
+):
+    """Download a file from URL, including Google Drive shared URL.
+
+    Args:
+        url (str, optional): Google Drive URL is also supported. Defaults to None.
+        output (str, optional): Output filename. Default is basename of URL.
+        quiet (bool, optional): Suppress terminal output. Default is False.
+        proxy (str, optional): Proxy. Defaults to None.
+        speed (float, optional): Download byte size per second (e.g., 256KB/s = 256 * 1024). Defaults to None.
+        use_cookies (bool, optional): Flag to use cookies. Defaults to True.
+        verify (bool | str, optional): Either a bool, in which case it controls whether the server's TLS certificate is verified, or a string,
+            in which case it must be a path to a CA bundle to use. Default is True.. Defaults to True.
+        id (str, optional): Google Drive's file ID. Defaults to None.
+        fuzzy (bool, optional): Fuzzy extraction of Google Drive's file Id. Defaults to False.
+        resume (bool, optional): Resume the download from existing tmp file if possible. Defaults to False.
+        unzip (bool, optional): Unzip the file. Defaults to True.
+        overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
+        subfolder (bool, optional): Create a subfolder with the same name as the file. Defaults to False.
+
+    Returns:
+        str: The output file path.
+    """
+    import zipfile
+    try:
+        import gdown
+    except ImportError:
+        print(
+            "The gdown package is required for this function. Use `pip install gdown` to install it."
+        )
+        return
+
+    if output is None:
+        if isinstance(url, str) and url.startswith("http"):
+            output = os.path.basename(url)
+
+    out_dir = os.path.abspath(os.path.dirname(output))
+    if not os.path.exists(out_dir):
+        os.makedirs(out_dir)
+
+    if isinstance(url, str):
+        if os.path.exists(os.path.abspath(output)) and (not overwrite):
+            print(
+                f"{output} already exists. Skip downloading. Set overwrite=True to overwrite."
+            )
+            return os.path.abspath(output)
+        else:
+            url = github_raw_url(url)
+
+    if "https://drive.google.com/file/d/" in url:
+        fuzzy = True
+
+    output = gdown.download(
+        url, output, quiet, proxy, speed, use_cookies, verify, id, fuzzy, resume
+    )
+
+    if unzip and output.endswith(".zip"):
+        with zipfile.ZipFile(output, "r") as zip_ref:
+            if not quiet:
+                print("Extracting files...")
+            if subfolder:
+                basename = os.path.splitext(os.path.basename(output))[0]
+
+                output = os.path.join(out_dir, basename)
+                if not os.path.exists(output):
+                    os.makedirs(output)
+                zip_ref.extractall(output)
+            else:
+                zip_ref.extractall(os.path.dirname(output))
+
+    return os.path.abspath(output)
+
+
+def download_checkpoint(url=None, output=None, overwrite=False, **kwargs):
+    """Download a checkpoint from URL. It can be one of the following: sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
+
+    Args:
+        url (str, optional): The checkpoint URL. Defaults to None. 
+        output (str, optional): The output file path. Defaults to None.
+        overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
+
+    Returns:
+        str: The output file path.
+    """
+    checkpoints = {
+        'sam_vit_h_4b8939.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+        'sam_vit_l_0b3195.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
+        'sam_vit_b_01ec64.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+    }
+
+    if isinstance(url, str) and url in checkpoints:
+        url = checkpoints[url]
+
+    if url is None:
+        url = checkpoints['sam_vit_h_4b8939.pth']
+
+    if output is None:
+        output = os.path.basename(url)
+
+    return download_file(url, output,overwrite=overwrite, **kwargs)
+
+
 def image_to_cog(source, dst_path=None, profile="deflate", **kwargs):
     """Converts an image to a COG file.
 
     Args:
         source (str): A dataset path, URL or rasterio.io.DatasetReader object.
         dst_path (str, optional): An output dataset path or or PathLike object. Defaults to None.
         profile (str, optional): COG profile. More at https://cogeotiff.github.io/rio-cogeo/profile. Defaults to "deflate".
@@ -109,14 +239,15 @@
     output,
     bbox,
     zoom=None,
     resolution=None,
     source="OpenStreetMap",
     to_cog=False,
     return_image=False,
+    overwrite=False,
     quiet=False,
     **kwargs,
 ):
     """Download TMS tiles and convert them to a GeoTIFF. The source is adapted from https://github.com/gumblex/tms2geotiff.
         Credits to the GitHub user @gumblex.
 
     Args:
@@ -124,19 +255,21 @@
         bbox (list): The bounding box [minx, miny, maxx, maxy], e.g., [-122.5216, 37.733, -122.3661, 37.8095]
         zoom (int, optional): The map zoom level. Defaults to None.
         resolution (float, optional): The resolution in meters. Defaults to None.
         source (str, optional): The tile source. It can be one of the following: "OPENSTREETMAP", "ROADMAP",
             "SATELLITE", "TERRAIN", "HYBRID", or an HTTP URL. Defaults to "OpenStreetMap".
         to_cog (bool, optional): Convert to Cloud Optimized GeoTIFF. Defaults to False.
         return_image (bool, optional): Return the image as PIL.Image. Defaults to False.
+        overwrite (bool, optional): Overwrite the output file if it already exists. Defaults to False.
         quiet (bool, optional): Suppress output. Defaults to False.
         **kwargs: Additional arguments to pass to gdal.GetDriverByName("GTiff").Create().
 
     """
 
+    import os
     import io
     import math
     import itertools
     import concurrent.futures
 
     import numpy
     from PIL import Image
@@ -151,14 +284,18 @@
 
         SESSION = httpx.Client()
     except ImportError:
         import requests
 
         SESSION = requests.Session()
 
+    if not overwrite and os.path.exists(output):
+        print(f"The output file {output} already exists. Use `overwrite=True` to overwrite it.")
+        return
+
     xyz_tiles = {
         "OPENSTREETMAP": {
             "url": "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
             "attribution": "OpenStreetMap",
             "name": "OpenStreetMap",
         },
         "ROADMAP": {
```

### Comparing `segment-geospatial-0.1.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.1.0
+Version: 0.2.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -17,30 +17,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # segment-geospatial
 
-[![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/examples/basic_usage.ipynb)
-[![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/examples/basic_usage.ipynb&branch=main)
-[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/examples/basic_usage.ipynb)
+[![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
+[![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
+[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
-**Meta AI' Segment Anything Model (SAM) for Geospatial Data**
+**A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: https://samgeo.gishub.org
 
 ## Features
 
--   TODO
+-   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
+-   Segment GeoTIFF files using the Segment Anything Model (SAM)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.1.0/setup.py` & `segment-geospatial-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='samgeo',
     name='segment-geospatial',
     packages=find_packages(include=['samgeo', 'samgeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/segment-geospatial',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

