# Comparing `tmp/wam2layers-3.0.0b3.tar.gz` & `tmp/wam2layers-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wam2layers-3.0.0b3.tar", last modified: Fri Dec  2 15:44:50 2022, max compression
+gzip compressed data, was "wam2layers-3.0.0b4.tar", last modified: Fri Apr 21 15:34:58 2023, max compression
```

## Comparing `wam2layers-3.0.0b3.tar` & `wam2layers-3.0.0b4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/
--rw-rw-r--   0 peter     (1000) peter     (1000)    11357 2022-05-13 09:49:06.000000 wam2layers-3.0.0b3/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)     2844 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2048 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/README.md
--rw-rw-r--   0 peter     (1000) peter     (1000)     1402 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.797415 wam2layers-3.0.0b3/src/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.797415 wam2layers-3.0.0b3/src/wam2layers/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-09-02 13:39:58.000000 wam2layers-3.0.0b3/src/wam2layers/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.797415 wam2layers-3.0.0b3/src/wam2layers/analysis/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-09-02 13:39:58.000000 wam2layers-3.0.0b3/src/wam2layers/analysis/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5181 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/analysis/checks.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8399 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/analysis/visualization.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      492 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/cli.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/src/wam2layers/preprocessing/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-09-02 13:39:58.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      216 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/cli.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9063 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/ecearth.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    13426 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/era5.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9802 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/shared.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10385 2022-09-02 13:39:58.000000 wam2layers-3.0.0b3/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/src/wam2layers/tracking/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-09-02 13:39:58.000000 wam2layers-3.0.0b3/src/wam2layers/tracking/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    17864 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/tracking/backtrack.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.807415 wam2layers-3.0.0b3/src/wam2layers/utils/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-10-13 13:15:15.000000 wam2layers-3.0.0b3/src/wam2layers/utils/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2458 2022-12-02 15:44:32.000000 wam2layers-3.0.0b3/src/wam2layers/utils/profiling.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 15:44:50.797415 wam2layers-3.0.0b3/src/wam2layers.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2844 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      815 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       50 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/entry_points.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      194 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2022-12-02 15:44:50.000000 wam2layers-3.0.0b3/src/wam2layers.egg-info/top_level.txt
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.606377 wam2layers-3.0.0b4/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    11357 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/LICENSE
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2844 2023-04-21 15:34:58.606377 wam2layers-3.0.0b4/PKG-INFO
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2048 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/README.md
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     1481 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/pyproject.toml
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       38 2023-04-21 15:34:58.608382 wam2layers-3.0.0b4/setup.cfg
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.532774 wam2layers-3.0.0b4/src/
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.557788 wam2layers-3.0.0b4/src/wam2layers/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/__init__.py
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.579906 wam2layers-3.0.0b4/src/wam2layers/analysis/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/__init__.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     5181 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/checks.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     8351 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/visualization.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      492 2023-04-21 10:14:03.000000 wam2layers-3.0.0b4/src/wam2layers/cli.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     8589 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/config.py
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.591905 wam2layers-3.0.0b4/src/wam2layers/preprocessing/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/__init__.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      216 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/cli.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    12555 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/era5.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     9802 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/shared.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    10385 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.594671 wam2layers-3.0.0b4/src/wam2layers/tracking/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/tracking/__init__.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    17248 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/tracking/backtrack.py
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.603574 wam2layers-3.0.0b4/src/wam2layers/utils/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/utils/__init__.py
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2458 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/utils/profiling.py
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.571311 wam2layers-3.0.0b4/src/wam2layers.egg-info/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2844 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/PKG-INFO
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      821 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/SOURCES.txt
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        1 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/dependency_links.txt
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       50 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/entry_points.txt
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      238 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/requires.txt
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       11 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/top_level.txt
+drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.605362 wam2layers-3.0.0b4/tests/
+-rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      442 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/tests/test_config.py
```

### Comparing `wam2layers-3.0.0b3/LICENSE` & `wam2layers-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/PKG-INFO` & `wam2layers-3.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wam2layers
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Atmospheric moisture tracking model
 License: Apache 2.0
 Project-URL: Documentation, https://wam2layers.readthedocs.io/en/latest
 Project-URL: Source code, https://github.com/WAM2layers/WAM2layers
 Keywords: atmospheric rivers,hydrological cycle,meteorology,moisture recycling,moisture tracking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `wam2layers-3.0.0b3/README.md` & `wam2layers-3.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/pyproject.toml` & `wam2layers-3.0.0b4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wam2layers"
 description = "Atmospheric moisture tracking model"
-version = "3.0.0-beta.3"
+version = "3.0.0-beta.4"
 readme = "README.md"
 license = { text = "Apache 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -29,14 +29,15 @@
     "pyyaml",
     "scipy",
     "pandas>=1.4.0",
     "xarray", # or xarray[io,parallel,complete,...]
     "netcdf4",
     "scipy",
     "click",
+    "pydantic",
     "dask>=2022.11",
     "distributed>=2022.11",
     "psutil",
     "matplotlib",
     "cmocean",
 ]
 
@@ -44,15 +45,19 @@
 develop = [
     "black",
     "cffconvert",
     "isort",
     "myst-nb",
     "sphinx_rtd_theme",
     "sphinx",
+    "myst-nb==0.16.0",
     "pytest",
+    "flake8",
+    "build",
+    "twine",
 ]
 
 [project.urls]
 Documentation = "https://wam2layers.readthedocs.io/en/latest"
 "Source code" = "https://github.com/WAM2layers/WAM2layers"
 
 [project.scripts]
```

### Comparing `wam2layers-3.0.0b3/src/wam2layers/analysis/checks.py` & `wam2layers-3.0.0b4/src/wam2layers/analysis/checks.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/src/wam2layers/analysis/visualization.py` & `wam2layers-3.0.0b4/src/wam2layers/analysis/visualization.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import click
 import matplotlib.pyplot as plt
 import pandas as pd
 import xarray as xr
 from cmocean import cm
 
+from wam2layers.config import Config
 from wam2layers.preprocessing.shared import get_grid_info
-from wam2layers.tracking.backtrack import (input_path, load_region,
-                                           output_path, parse_config)
+from wam2layers.tracking.backtrack import input_path, load_region, output_path
 
 
 def try_import_cartopy():
     """Import cartopy if it is available; else raise."""
     from importlib import import_module
 
     global crs
@@ -36,30 +36,30 @@
 def _plot_precip(config, ax):
     """Return subplot with precip."""
     # Load config and some usful stuf.
     region = load_region(config)
 
     # Load data
     dates = pd.date_range(
-        start=config["preprocess_start_date"],
-        end=config["preprocess_end_date"],
+        start=config.preprocess_start_date,
+        end=config.preprocess_end_date,
         freq=config[
             "output_frequency"
         ],  # Should be output frequency, since this is used to save the data
         inclusive="left",
     )
 
     input_files = []
     for date in dates:
         input_files.append(input_path(date, config))
 
     ds = xr.open_mfdataset(input_files, combine="nested", concat_dim="time")
     # TODO: make region time-dependent
-    start = config["event_start_date"]
-    end = config["event_end_date"]
+    start = config.event_start_date
+    end = config.event_end_date
     subset = ds.precip.sel(time=slice(start, end))
     precip = (subset * region * 3600).sum("time").compute()
 
     # Make figure
     precip.plot(ax=ax, cmap=cm.rain, cbar_kwargs=dict(fraction=0.05, shrink=0.5))
     ax.set_title("Cumulative precipitation during event [mm]", loc="left")
     polish(ax, region.where(region > 0, drop=True))
@@ -68,17 +68,17 @@
 def _plot_evap(config, ax):
     """Return subplot with tracked evaporation."""
     region = load_region(config)
     a_gridcell, lx, ly = get_grid_info(region)
 
     # Load data
     dates = pd.date_range(
-        start=config["track_start_date"],
-        end=config["track_end_date"],
-        freq=config["output_frequency"],
+        start=config.track_start_date,
+        end=config.track_end_date,
+        freq=config.output_frequency,
         inclusive="left",
     )
 
     output_files = []
     for date in dates:
         output_files.append(output_path(date, config))
 
@@ -98,80 +98,80 @@
 
 
 def visualize_input_data(config_file):
     """An figure showing the cumulative moisture inputs.
 
     TODO: make figure creation independent of case.
     """
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
 
     # Make figure
     fig = plt.figure(figsize=(16, 10))
     ax = fig.add_subplot(111, projection=crs.PlateCarree())
 
     _plot_precip(config, ax)
 
     # Save
-    out_dir = Path(config["output_folder"]) / "figures"
+    out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
     fig.savefig(out_dir / "input_event.png", dpi=200)
 
 
 def visualize_output_data(config_file):
     """An figure showing the cumulative moisture origins.
 
     TODO: make figure creation independent of case.
     """
     # Load config and some usful stuf.
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
 
     # Make figure
     fig = plt.figure(figsize=(16, 10))
     ax = fig.add_subplot(111, projection=crs.PlateCarree())
 
     _plot_evap(config, ax)
 
     # Save
-    out_dir = Path(config["output_folder"]) / "figures"
+    out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
     fig.savefig(out_dir / "cumulative_sources.png", dpi=200)
 
 
 def visualize_both(config_file):
     """Diagnostic figure with four subplots combining input and output data."""
     # Load config and some usful stuf.
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
 
     # Make figure
     fig, [ax1, ax2] = plt.subplots(
         2, 1, figsize=(16, 10), subplot_kw=dict(projection=crs.PlateCarree())
     )
 
     _plot_precip(config, ax1)
     _plot_evap(config, ax2)
 
     # Save
-    out_dir = Path(config["output_folder"]) / "figures"
+    out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
     fig.savefig(out_dir / "summary_subplots.png", dpi=200)
 
 
 def visualize_snapshots(config_file):
     """Diagnostic figure with four subplots combining input and output data."""
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
     dates = pd.date_range(
-        start=config["track_start_date"],
-        end=config["track_end_date"],
-        freq=config["output_frequency"],
+        start=config.track_start_date,
+        end=config.track_end_date,
+        freq=config.output_frequency,
         inclusive="left",
     )
     region = load_region(config)
     a_gridcell, lx, ly = get_grid_info(region)
 
-    out_dir = Path(config["output_folder"]) / "figures"
+    out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
 
     for date in dates:
         print(date)
         ds_in = xr.open_dataset(input_path(date, config))
         ds_out = xr.open_dataset(output_path(date, config))
```

### Comparing `wam2layers-3.0.0b3/src/wam2layers/preprocessing/era5.py` & `wam2layers-3.0.0b4/src/wam2layers/preprocessing/era5.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,56 @@
 import click
 import numpy as np
 import pandas as pd
 import xarray as xr
 import yaml
 
 from wam2layers.analysis.checks import check_input
-from wam2layers.preprocessing.shared import (accumulation_to_flux,
-                                             calculate_humidity, insert_level,
-                                             interpolate, sortby_ndarray)
-
-
-class InvalidConfig(Exception):
-    pass
+from wam2layers.config import Config
+from wam2layers.preprocessing.shared import (
+    accumulation_to_flux,
+    calculate_humidity,
+    insert_level,
+    interpolate,
+    sortby_ndarray,
+)
 
 
 def load_data(variable, date, config):
     """Load data for given variable and date."""
-    template = config["filename_template"]
+    template = config.filename_template
 
     # If it's a 4d variable, we need to set the level type
     if variable in ["u", "v", "q"]:
-        if config["level_type"] == "model_levels":
+        if config.level_type == "model_levels":
             prefix = "_ml"
-        elif config["level_type"] == "pressure_levels":
+        elif config.level_type == "pressure_levels":
             prefix = "_pl"
     # If it's a 3d variable we do not need to set the level type
     else:
         prefix = ""
 
     # Load data
     filepath = template.format(
         year=date.year,
         month=date.month,
         day=date.day,
         levtype=prefix,
         variable=variable,
     )
-    da = xr.open_dataset(filepath, chunks=config["chunks"]).sel(
+    da = xr.open_dataset(filepath, chunks=config.chunks).sel(
         time=date.strftime("%Y%m%d")
     )[variable]
 
     if "lev" in da.coords:
         da = da.rename(lev="level")
 
     # If it's 4d data we want to select a subset of the levels
-    if variable in ["u", "v", "q"] and isinstance(config["levels"], list):
-        return da.sel(level=config["levels"])
+    if variable in ["u", "v", "q"] and isinstance(config.levels, list):
+        return da.sel(level=config.levels)
 
     return da
 
 
 def preprocess_precip_and_evap(date, config):
     """Load and pre-process precipitation and evaporation."""
     # All incoming units are accumulations (in m) since previous time step
@@ -188,30 +189,21 @@
     v = v.where(above_surface)
     q = q.where(above_surface)
     p = p.where(above_surface)
 
     return dp, p, q, u, v, p_boundary
 
 
-def parse_config(config_file):
-    """Read and parse case configuration file."""
-    with open(config_file) as f:
-        config = yaml.safe_load(f)
-
-    # Create the preprocessed data folder if it does not exist yet
-    config["output_dir"] = Path(config["preprocessed_data_folder"]).expanduser()
-    config["output_dir"].mkdir(exist_ok=True, parents=True)
-
-    config["datelist"] = pd.date_range(
-        start=config["preprocess_start_date"],
-        end=config["preprocess_end_date"],
-        freq="d",
-        inclusive="left",
+def get_input_dates(config):
+    """Dates for pre-processing."""
+    return pd.date_range(
+        start=config.preprocess_start_date,
+        end=config.preprocess_end_date,
+        freq="1d",
     )
-    return config
 
 
 def prep_experiment(config_file):
     """Pre-process all data for a given config file.
 
     This function expects the following configuration settings:
 
@@ -227,37 +219,37 @@
       /home/peter/WAM2layers/preprocessed_data_2021
     - filename_prefix: Fixed part of filename. This function will infer the
       variable name and add _ml for model level data. E.g. with prefix =
       "FloodCase_202107" this function will be able to find
       FloodCase_202107_ml_u.nc or FloodCase_202107_u.nc and
       FloodCase_202107_sp.nc
     """
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
 
-    if config["chunks"] is not None:
+    if config.chunks is not None:
         print("Starting dask cluster")
         from dask.distributed import Client
 
         client = Client()
         print(f"To see the dask dashboard, go to {client.dashboard_link}")
 
-    for date in config["datelist"]:
+    for date in get_input_dates(config):
         print(date)
 
         # 4d fields
-        levels = config["levels"]
+        levels = config.levels
         q = load_data("q", date, config)  # in kg kg-1
         u = load_data("u", date, config)  # in m/s
         v = load_data("v", date, config)  # in m/s
         sp = load_data("sp", date, config)  # in Pa
 
-        if config["level_type"] == "model_levels":
+        if config.level_type == "model_levels":
             dp = get_dp_modellevels(sp, levels)
 
-        if config["level_type"] == "pressure_levels":
+        if config.level_type == "pressure_levels":
             d2m = load_data("d2m", date, config)  # Dew point in K
             q2m = calculate_humidity(d2m, sp)  # kg kg-1
             u10 = load_data("u10", date, config)  # in m/s
             v10 = load_data("v10", date, config)  # in m/s
             dp, p, q, u, v, pb = get_dp_pressurelevels(q, u, v, sp, q2m, u10, v10)
 
         # Calculate column water vapour
@@ -274,44 +266,37 @@
             cw = cwv
 
         # Determine the fluxes
         fx = u * cw  # eastward atmospheric moisture flux (kg m-1 s-1)
         fy = v * cw  # northward atmospheric moisture flux (kg m-1 s-1)
 
         # Integrate fluxes and states to upper and lower layer
-        if config["level_type"] == "model_levels":
+        if config.level_type == "model_levels":
             # TODO: Check if this is a reasonable choice for boundary
             boundary = 111
-            idx = dp.level.searchsorted(boundary, side="right")
-            upper = np.s_[:, :idx, :, :]
-            lower = np.s_[:, idx:, :, :]
-            s_lower = cw[lower].sum(dim="level")
-            s_upper = cw[upper].sum(dim="level")
-            fx_lower = fx[lower].sum(dim="level")  # kg m-1 s-1
-            fy_lower = fy[lower].sum(dim="level")  # kg m-1 s-1
-            fx_upper = fx[upper].sum(dim="level")  # kg m-1 s-1
-            fy_upper = fy[upper].sum(dim="level")  # kg m-1 s-1
+            lower_layer = dp.level > boundary
+            upper_layer = ~lower_layer
 
-        elif config["level_type"] == "pressure_levels":
+        if config.level_type == "pressure_levels":
             upper_layer = p < pb[:, None, :, :]
             lower_layer = pb[:, None, :, :] < p
 
-            # Vertically integrate state over two layers
-            s_lower = cw.where(lower_layer).sum(dim="level")
-            s_upper = cw.where(upper_layer).sum(dim="level")
-            fx_lower = fx.where(lower_layer).sum(dim="level")  # kg m-1 s-1
-            fy_lower = fy.where(lower_layer).sum(dim="level")  # kg m-1 s-1
-            fx_upper = fx.where(upper_layer).sum(dim="level")  # kg m-1 s-1
-            fy_upper = fy.where(upper_layer).sum(dim="level")  # kg m-1 s-1
-
-        else:
-            raise InvalidConfig(
-                "Expected config level_type to be one of ['model_level', "
-                f"'pressure_level'], but got {config['level_type']}."
-            )
+        # Vertically integrate state over two layers
+        s_lower = cw.where(lower_layer).sum(dim="level")
+        s_upper = cw.where(upper_layer).sum(dim="level")
+
+        # Determine the fluxes
+        fx = u * cw  # eastward atmospheric moisture flux (kg m-1 s-1)
+        fy = v * cw  # northward atmospheric moisture flux (kg m-1 s-1)
+
+        # Vertically integrate fluxes over two layers
+        fx_lower = fx.where(lower_layer).sum(dim="level")  # kg m-1 s-1
+        fy_lower = fy.where(lower_layer).sum(dim="level")  # kg m-1 s-1
+        fx_upper = fx.where(upper_layer).sum(dim="level")  # kg m-1 s-1
+        fy_upper = fy.where(upper_layer).sum(dim="level")  # kg m-1 s-1
 
         precip, evap = preprocess_precip_and_evap(date, config)
 
         # Combine everything into one dataset
         ds = xr.Dataset(
             {
                 "fx_upper": fx_upper.assign_attrs(units="kg m-1 s-1"),
@@ -326,19 +311,19 @@
         )
 
         # Verify that the data meets all the requirements for the model
         # check_input(ds)
 
         # Save preprocessed data
         filename = f"{date.strftime('%Y-%m-%d')}_fluxes_storages.nc"
-        output_path = config["output_dir"] / filename
+        output_path = config.preprocessed_data_folder / filename
         ds.astype("float32").to_netcdf(output_path)
 
     # Close the dask cluster when done
-    if config["chunks"] is not None:
+    if config.chunks is not None:
         client.shutdown()
 
 
 ################################################################################
 # To run this script interactively in e.g. Spyder, uncomment the following line:
 # prep_experiment("../../cases/era5_2021.yaml")
 ################################################################################
```

### Comparing `wam2layers-3.0.0b3/src/wam2layers/preprocessing/shared.py` & `wam2layers-3.0.0b4/src/wam2layers/preprocessing/shared.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv` & `wam2layers-3.0.0b4/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/src/wam2layers/tracking/backtrack.py` & `wam2layers-3.0.0b4/src/wam2layers/tracking/backtrack.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,63 +3,44 @@
 
 import click
 import numpy as np
 import pandas as pd
 import xarray as xr
 import yaml
 
+from wam2layers.config import Config
 from wam2layers.preprocessing.shared import get_grid_info
 from wam2layers.utils.profiling import Profiler, ProgressTracker
 
 
-def parse_config(config_file):
-    """Load and parse config file into dictionary."""
-    with open(config_file) as f:
-        config = yaml.safe_load(f)
-
-    # Add datelist
+def get_tracking_dates(config):
+    """Dates for tracking."""
+    # E.g. if data from 00:00 to 23:00
+    # Using target freq directly would end at 23:45 or so
     input_dates = pd.date_range(
-        start=config["track_start_date"],
-        end=config["track_end_date"],
-        freq=config["input_frequency"],
-        inclusive="left",
+        start=config.track_start_date,
+        end=config.track_end_date,
+        freq=config.input_frequency,
     )
-    config["datelist"] = pd.date_range(
+
+    return pd.date_range(
         start=input_dates[0],
         end=input_dates[-1],
-        freq=config["target_frequency"],
+        freq=config.target_frequency,
         inclusive="right",
     )
 
-    # Parse directories with pathlib
-    config["preprocessed_data_folder"] = Path(
-        config["preprocessed_data_folder"]
-    ).expanduser()
-    config["output_folder"] = Path(config["output_folder"]).expanduser() / "backtrack"
-
-    # Check if input dir exists
-    if not config["preprocessed_data_folder"].exists():
-        raise ValueError(
-            "Please create the preprocessed_data_folder before running the script"
-        )
-
-    # Create output dir if it doesn't exist yet
-    if not config["output_folder"].exists():
-        config["output_folder"].mkdir(parents=True)
-
-    return config
-
 
 def input_path(date, config):
-    input_dir = config["preprocessed_data_folder"]
+    input_dir = config.preprocessed_data_folder
     return f"{input_dir}/{date.strftime('%Y-%m-%d')}_fluxes_storages.nc"
 
 
 def output_path(date, config):
-    output_dir = config["output_folder"]
+    output_dir = config.output_folder
     return f"{output_dir}/{date.strftime('%Y-%m-%d')}_s_track.nc"
 
 
 # LRU Cache keeps the file open so we save a bit on I/O
 @lru_cache(maxsize=2)
 def read_data_at_date(d):
     """Load input data for given date."""
@@ -77,49 +58,49 @@
 def load_data(t, subset="fluxes"):
     """Load variable at t, interpolate if needed."""
     variables = {
         "fluxes": ["fx_upper", "fx_lower", "fy_upper", "fy_lower", "evap", "precip"],
         "states": ["s_upper", "s_lower"],
     }
 
-    t1 = t.ceil(config["input_frequency"])
+    t1 = t.ceil(config.input_frequency)
     da1 = read_data_at_time(t1)[variables[subset]]
     if t == t1:
         # this saves a lot of work if times are aligned with input
         return da1
 
-    t0 = t.floor(config["input_frequency"])
+    t0 = t.floor(config.input_frequency)
     da0 = read_data_at_time(t0)[variables[subset]]
     if t == t0:
         return da0
 
     return da0 + (t - t0) / (t1 - t0) * (da1 - da0)
 
 
 def load_fluxes(t):
-    t_current = t - pd.Timedelta(config["target_frequency"]) / 2
+    t_current = t - pd.Timedelta(config.target_frequency) / 2
     return load_data(t_current, "fluxes")
 
 
 def load_states(t):
     t_prev = t
-    t_next = t - pd.Timedelta(config["target_frequency"])
+    t_next = t - pd.Timedelta(config.target_frequency)
     states_prev = load_data(t_prev, "states")
     states_next = load_data(t_next, "states")
     return states_prev, states_next
 
 
 def time_in_range(start, end, current):
     """Returns whether current is in the range [start, end]"""
     return start <= current <= end
 
 
 def load_region(config):
     # TODO: make variable name more generic
-    return xr.open_dataset(config["region"]).source_region
+    return xr.open_dataset(config.region).source_region
 
 
 def to_edges_zonal(fx, periodic_boundary=False):
     """Define the horizontal fluxes over the east/west boundaries."""
     fe = np.zeros_like(fx)
     fe[:, :-1] = 0.5 * (fx[:, :-1] + fx[:, 1:])
     if periodic_boundary:
@@ -283,15 +264,15 @@
 
     # compute the resulting vertical moisture flux; the vertical velocity so
     # that the new residual_lower/s_lower = residual_upper/s_upper (positive downward)
     fv = s_rel.s_lower * (residual_upper + residual_lower) - residual_lower
 
     # stabilize the outfluxes / influxes; during the reduced timestep the
     # vertical flux can maximally empty/fill 1/x of the top or down storage
-    stab = 1.0 / (config["kvf"] + 1.0)
+    stab = 1.0 / (config.kvf + 1.0)
     flux_limit = np.minimum(s_mean.s_upper, s_mean.s_lower)
     fv_stable = np.minimum(np.abs(fv), stab * flux_limit)
 
     # Reinstate the sign
     return np.sign(fv) * fv_stable
 
 
@@ -317,22 +298,22 @@
     s_track_upper = output["s_track_upper_restart"].values
     s_track_lower = output["s_track_lower_restart"].values
 
     tagged_precip = region * precip
     s_total = s_upper + s_lower
 
     # separate the direction of the vertical flux and make it absolute
-    f_downward, f_upward = split_vertical_flux(config["kvf"], f_vert)
+    f_downward, f_upward = split_vertical_flux(config.kvf, f_vert)
 
     # Determine horizontal fluxes over the grid-cell boundaries
     f_e_lower_we, f_e_lower_ew, f_w_lower_we, f_w_lower_ew = to_edges_zonal(
-        fx_lower, config["periodic_boundary"]
+        fx_lower, config.periodic_boundary
     )
     f_e_upper_we, f_e_upper_ew, f_w_upper_we, f_w_upper_ew = to_edges_zonal(
-        fx_upper, config["periodic_boundary"]
+        fx_upper, config.periodic_boundary
     )
 
     (
         fy_n_lower_sn,
         fy_n_lower_ns,
         fy_s_lower_sn,
         fy_s_lower_ns,
@@ -343,15 +324,15 @@
         fy_s_upper_sn,
         fy_s_upper_ns,
     ) = to_edges_meridional(fy_upper)
 
     # Short name for often used expressions
     s_track_relative_lower = s_track_lower / s_lower
     s_track_relative_upper = s_track_upper / s_upper
-    if config["periodic_boundary"]:
+    if config.periodic_boundary:
         inner = np.s_[1:-1, :]
     else:
         inner = np.s_[1:-1, 1:-1]
 
     # Actual tracking (note: backtracking, all terms have been negated)
     s_track_lower[inner] += (
         +f_e_lower_we * look_east(s_track_relative_lower)
@@ -393,15 +374,15 @@
     output["north_loss"] += (
         fy_n_upper_ns * s_track_relative_upper + fy_n_lower_ns * s_track_relative_lower
     )[1, :]
     output["south_loss"] += (
         fy_s_upper_sn * s_track_relative_upper + fy_s_lower_sn * s_track_relative_lower
     )[-2, :]
 
-    if config["periodic_boundary"] == False:
+    if config.periodic_boundary == False:
         output["east_loss"] += (
             f_e_upper_ew * s_track_relative_upper
             + f_e_lower_ew * s_track_relative_lower
         )[:, -2]
         output["west_loss"] += (
             f_w_upper_we * s_track_relative_upper
             + f_w_lower_we * s_track_relative_lower
@@ -412,28 +393,29 @@
     output["tagged_precip"] += tagged_precip
 
 
 def initialize(config_file):
     """Read config, region, and initial states."""
     print(f"Initializing experiment with config file {config_file}")
 
-    config = parse_config(config_file)
+    config = Config.from_yaml(config_file)
     region = load_region(config)
 
     output = initialize_outputs(region)
     region = region.values
 
-    if config["restart"]:
+    if config.restart:
         # Reload last state from existing output
-        date = config["datelist"][-1] + pd.Timedelta(days=1)
+        tracking_dates = get_tracking_dates(config)
+        date = tracking_dates[-1] + pd.Timedelta(days=1)
         ds = xr.open_dataset(output_path(date, config))
         output["s_track_upper_restart"].values = ds.s_track_upper_restart.values
         output["s_track_lower_restart"].values = ds.s_track_lower_restart.values
 
-    print(f"Output will be written to {config['output_folder']}.")
+    print(f"Output will be written to {config.output_folder}.")
     return config, region, output
 
 
 def initialize_outputs(region):
     """Allocate output arrays."""
 
     proto = region
@@ -480,52 +462,54 @@
 
 def run_experiment(config_file):
     """Run a backtracking experiment from start to finish."""
     global config
 
     config, region, output = initialize(config_file)
 
+    tracking_dates = get_tracking_dates(config)
+
     progress_tracker = ProgressTracker(output)
-    for t in reversed(config["datelist"]):
+    for t in reversed(tracking_dates):
 
         fluxes = load_fluxes(t)
         states_prev, states_next = load_states(t)
 
         # Convert data to volumes
-        change_units(states_prev, config["target_frequency"])
-        change_units(states_next, config["target_frequency"])
-        change_units(fluxes, config["target_frequency"])
+        change_units(states_prev, config.target_frequency)
+        change_units(states_next, config.target_frequency)
+        change_units(fluxes, config.target_frequency)
 
         # Apply a stability correction if needed
         stabilize_fluxes(fluxes, states_next)
 
         # Determine the vertical moisture flux
         fluxes["f_vert"] = calculate_fv(fluxes, states_prev, states_next)
 
-        # Only track the precipitation at certain dates
+        # Only track the precipitation at certain timesteps
         if (
             time_in_range(
-                config["event_start_date"],
-                config["event_end_date"],
-                t.strftime("%Y%m%d"),
+                config.event_start_date,
+                config.event_end_date,
+                t,
             )
             == False
         ):
             fluxes["precip"] = 0
 
         backtrack(
             fluxes,
             states_prev,
             states_next,
             region,
             output,
         )
 
         # Daily output
-        if t == t.floor(config["output_frequency"]):
+        if t == t.floor(config.output_frequency):
             progress_tracker.print_progress(t, output)
             progress_tracker.store_intermediate_states(output)
             write_output(output, t)
 
 
 ###########################################################################
 # The code below makes it possible to run wam2layers from the command line:
```

### Comparing `wam2layers-3.0.0b3/src/wam2layers/utils/profiling.py` & `wam2layers-3.0.0b4/src/wam2layers/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b3/src/wam2layers.egg-info/PKG-INFO` & `wam2layers-3.0.0b4/src/wam2layers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wam2layers
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Atmospheric moisture tracking model
 License: Apache 2.0
 Project-URL: Documentation, https://wam2layers.readthedocs.io/en/latest
 Project-URL: Source code, https://github.com/WAM2layers/WAM2layers
 Keywords: atmospheric rivers,hydrological cycle,meteorology,moisture recycling,moisture tracking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `wam2layers-3.0.0b3/src/wam2layers.egg-info/SOURCES.txt` & `wam2layers-3.0.0b4/src/wam2layers.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 src/wam2layers/__init__.py
 src/wam2layers/cli.py
+src/wam2layers/config.py
 src/wam2layers.egg-info/PKG-INFO
 src/wam2layers.egg-info/SOURCES.txt
 src/wam2layers.egg-info/dependency_links.txt
 src/wam2layers.egg-info/entry_points.txt
 src/wam2layers.egg-info/requires.txt
 src/wam2layers.egg-info/top_level.txt
 src/wam2layers/analysis/__init__.py
 src/wam2layers/analysis/checks.py
 src/wam2layers/analysis/visualization.py
 src/wam2layers/preprocessing/__init__.py
 src/wam2layers/preprocessing/cli.py
-src/wam2layers/preprocessing/ecearth.py
 src/wam2layers/preprocessing/era5.py
 src/wam2layers/preprocessing/shared.py
 src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
 src/wam2layers/tracking/__init__.py
 src/wam2layers/tracking/backtrack.py
 src/wam2layers/utils/__init__.py
-src/wam2layers/utils/profiling.py
+src/wam2layers/utils/profiling.py
+tests/test_config.py
```

