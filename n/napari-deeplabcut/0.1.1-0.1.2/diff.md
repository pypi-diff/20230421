# Comparing `tmp/napari_deeplabcut-0.1.1.tar.gz` & `tmp/napari_deeplabcut-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_deeplabcut-0.1.1.tar", last modified: Thu Mar  9 13:22:46 2023, max compression
+gzip compressed data, was "napari_deeplabcut-0.1.2.tar", last modified: Fri Apr 21 12:13:50 2023, max compression
```

## Comparing `napari_deeplabcut-0.1.1.tar` & `napari_deeplabcut-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.723922 napari_deeplabcut-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-09 13:22:46.731922 napari_deeplabcut-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.723922 napari_deeplabcut-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/src/napari_deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/src/napari_deeplabcut/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/assets/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/assets/unlock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:22:46.727922 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 13:22:46.000000 napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-09 13:22:24.000000 napari_deeplabcut-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.359644 napari_deeplabcut-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/unlock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/tox.ini
```

### Comparing `napari_deeplabcut-0.1.1/.github/workflows/plugin_preview.yml` & `napari_deeplabcut-0.1.2/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/.github/workflows/test_and_deploy.yml` & `napari_deeplabcut-0.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/.gitignore` & `napari_deeplabcut-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/.napari/DESCRIPTION.md` & `napari_deeplabcut-0.1.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/.pre-commit-config.yaml` & `napari_deeplabcut-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/CODE_OF_CONDUCT.md` & `napari_deeplabcut-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/LICENSE` & `napari_deeplabcut-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/PKG-INFO` & `napari_deeplabcut-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_deeplabcut
-Version: 0.1.1
+Version: 0.1.2
 Summary: napari + DeepLabCut annotation tool
 Home-page: https://github.com/DeepLabCut/napari-deeplabcut
 Author: Jessy Lauer
 Author-email: jessy.lauer@epfl.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/DeepLabCut/napari-deeplabcut/issues
 Project-URL: Documentation, https://github.com/DeepLabCut/napari-deeplabcut#README.md
```

### Comparing `napari_deeplabcut-0.1.1/README.md` & `napari_deeplabcut-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/setup.cfg` & `napari_deeplabcut-0.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 	Source Code = https://github.com/DeepLabCut/napari-deeplabcut
 	User Support = https://github.com/DeepLabCut/napari-deeplabcut/issues
 
 [options]
 packages = find:
 install_requires = 
 	dask-image
-	napari==0.4.17rc8
+	napari==0.4.17
+	natsort
 	numpy
 	opencv-python-headless
 	pandas
 	pyyaml
 	qtpy
 	scikit-image
 	tables
```

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_reader.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import dask.array as da
 import numpy as np
 import pandas as pd
 import yaml
 from dask import delayed
 from dask_image.imread import imread
 from napari.types import LayerData
+from natsort import natsorted
 
 from napari_deeplabcut import misc
 
 SUPPORTED_IMAGES = ".jpg", ".jpeg", ".png"
 SUPPORTED_VIDEOS = ".mp4", ".mov", ".avi"
 
 
@@ -90,15 +91,15 @@
     filepaths = []
     for filepath in glob.iglob(path):
         relpath = Path(filepath).parts[-3:]
         filepaths.append(os.path.join(*relpath))
     params = {
         "name": "images",
         "metadata": {
-            "paths": sorted(filepaths),
+            "paths": natsorted(filepaths),
             "root": os.path.split(path)[0],
         },
     }
     return [(imread(path), params, "image")]
 
 
 def _populate_metadata(
```

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/conftest.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_keypoints.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_keypoints.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_misc.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_reader.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_tests/test_widgets.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_widgets.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     QSizePolicy,
     QStyle,
     QStyleOption,
     QVBoxLayout,
     QWidget,
 )
 
+ICON_FOLDER = os.path.join(os.path.dirname(__file__), "assets")
+
 from napari_deeplabcut import keypoints
 from napari_deeplabcut._reader import _load_config
 from napari_deeplabcut._writer import _write_config, _write_image, _form_df
 from napari_deeplabcut.misc import (
     encode_categories,
     to_os_dir_sep,
     guarantee_multiindex_rows,
@@ -590,15 +592,15 @@
         layout1 = QVBoxLayout()
         layout1.addStretch(1)
         group_box = QGroupBox("Keypoint selection")
         layout2 = QVBoxLayout()
         for menu in self.menus.values():
             layout2.addWidget(menu)
         self.lock_button = QPushButton("Lock selection")
-        self.lock_button.setIcon(QIcon('src/napari_deeplabcut/assets/unlock.svg'))
+        self.lock_button.setIcon(QIcon(os.path.join(ICON_FOLDER, "unlock.svg")))
         self.lock_button.setIconSize(QSize(24, 24))
         self.lock_button.clicked.connect(self._lock_current_keypoint)
         layout2.addWidget(self.lock_button)
         group_box.setLayout(layout2)
         layout1.addWidget(group_box)
         self.setLayout(layout1)
 
@@ -625,18 +627,18 @@
             self.menus["id"].update_items(list(self.id2label))
         self.menus["label"].update_items(self.id2label[id_])
 
     def _lock_current_keypoint(self):
         self._locked = not self._locked
         if self._locked:
             self.lock_button.setText("Unlock selection")
-            self.lock_button.setIcon(QIcon('src/napari_deeplabcut/assets/lock.svg'))
+            self.lock_button.setIcon(QIcon(os.path.join(ICON_FOLDER, "lock.svg")))
         else:
             self.lock_button.setText("Lock selection")
-            self.lock_button.setIcon(QIcon('src/napari_deeplabcut/assets/unlock.svg'))
+            self.lock_button.setIcon(QIcon(os.path.join(ICON_FOLDER, "unlock.svg")))
 
     def update_menus(self, event):
         keypoint = self.store.current_keypoint
         for attr, menu in self.menus.items():
             val = getattr(keypoint, attr)
             if menu.currentText() != val:
                 menu.update_to(val)
```

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/_writer.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from itertools import groupby
+from pathlib import Path
 
 import pandas as pd
 import yaml
 from napari.layers import Shapes
 from napari_builtins.io import napari_write_shapes
 from skimage.io import imsave
 from skimage.util import img_as_ubyte
@@ -62,16 +63,16 @@
             header.scorer = new_scorer
             df.columns = header.columns
             df = pd.concat((df, df_gt))
             df = df[~df.index.duplicated(keep="first")]
             name = os.path.splitext(gt_file)[0]
         else:
             # Let us fetch the config.yaml file to get the scorer name...
-            project_folder = root.rsplit(os.sep, 2)[0]
-            config = _load_config(os.path.join(project_folder, "config.yaml"))
+            project_folder = Path(root).parents[1]
+            config = _load_config(str(project_folder / "config.yaml"))
             new_scorer = config["scorer"]
             header.scorer = new_scorer
             df.columns = header.columns
             name = f"CollectedData_{new_scorer}"
     df.sort_index(inplace=True)
     filename = name + ".h5"
     path = os.path.join(root, filename)
```

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/keypoints.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/keypoints.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/misc.py` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/misc.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut/napari.yaml` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/PKG-INFO` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-deeplabcut
-Version: 0.1.1
+Version: 0.1.2
 Summary: napari + DeepLabCut annotation tool
 Home-page: https://github.com/DeepLabCut/napari-deeplabcut
 Author: Jessy Lauer
 Author-email: jessy.lauer@epfl.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/DeepLabCut/napari-deeplabcut/issues
 Project-URL: Documentation, https://github.com/DeepLabCut/napari-deeplabcut#README.md
```

### Comparing `napari_deeplabcut-0.1.1/src/napari_deeplabcut.egg-info/SOURCES.txt` & `napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.1/tox.ini` & `napari_deeplabcut-0.1.2/tox.ini`

 * *Files identical despite different names*

