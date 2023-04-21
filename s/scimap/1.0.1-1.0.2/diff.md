# Comparing `tmp/scimap-1.0.1.tar.gz` & `tmp/scimap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.0.1.tar", max compression
+gzip compressed data, was "scimap-1.0.2.tar", max compression
```

## Comparing `scimap-1.0.1.tar` & `scimap-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.0.1/README.md
--rw-r--r--   0        0        0     2340 2023-04-21 02:04:09.486223 scimap-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.0.1/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.0.1/scimap/cli/test.py
--rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.0.1/scimap/helpers/__init__.py
--rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.0.1/scimap/helpers/_addROI_omero.py
--rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.0.1/scimap/helpers/_add_roi_omero.py
--rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.0.1/scimap/helpers/_animate.py
--rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.0.1/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.0.1/scimap/helpers/_dropFeatures.py
--rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/_merge_adata_obs.py
--rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.0.1/scimap/helpers/_scimap_to_csv.py
--rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0      463 2022-05-29 20:43:39.000000 scimap-1.0.1/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.0.1/scimap/plotting/_addROI_image.py
--rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.0.1/scimap/plotting/_cluster_plots.py
--rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_foldchange.py
--rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.0.1/scimap/plotting/_gate_finder.py
--rw-r--r--   0        0        0     7769 2022-05-26 00:26:12.000000 scimap-1.0.1/scimap/plotting/_image_viewer.py
--rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_pie.py
--rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.0.1/scimap/plotting/_spatial_distance.py
--rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.0.1/scimap/plotting/_spatial_interaction.py
--rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.0.1/scimap/plotting/_spatial_pscore.py
--rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_spatial_scatter.py
--rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.0.1/scimap/plotting/_stacked_barplot.py
--rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.0.1/scimap/plotting/_umap.py
--rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.0.1/scimap/plotting/_voronoi.py
--rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.0.1/scimap/plotting/lasso_selector.py
--rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.0.1/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.0.1/scimap/preprocessing/_combat.py
--rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.0.1/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.0.1/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/phenotype_workflow.csv
--rwxr-xr-x   0        0        0     1269 2022-05-18 01:22:39.000000 scimap-1.0.1/scimap/tests/test_helpers.py
--rwxr-xr-x   0        0        0      985 2022-06-05 16:22:49.000000 scimap-1.0.1/scimap/tests/test_preprocessing.py
--rwxr-xr-x   0        0        0     4674 2022-04-02 14:45:20.000000 scimap-1.0.1/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.0.1/scimap/tools/__init__.py
--rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.0.1/scimap/tools/_cluster.py
--rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.0.1/scimap/tools/_foldchange.py
--rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_phenotype_cells.py
--rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_spatial_aggregate.py
--rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.0.1/scimap/tools/_spatial_cluster.py
--rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_spatial_count.py
--rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.0.1/scimap/tools/_spatial_distance.py
--rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.0.1/scimap/tools/_spatial_expression.py
--rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.0.1/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.0.1/scimap/tools/_spatial_lda.py
--rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.0.1/scimap/tools/_spatial_pscore.py
--rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.0.1/scimap/tools/_spatial_similarity_search.py
--rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.0.1/scimap/tools/_umap.py
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 scimap-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2340 2023-04-21 14:44:10.228845 scimap-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.0.2/README.md
+-rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.000000 scimap-1.0.2/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.000000 scimap-1.0.2/scimap/cli/test.py
+-rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.0.2/scimap/helpers/__init__.py
+-rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.0.2/scimap/helpers/_add_roi_omero.py
+-rw-r--r--   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.0.2/scimap/helpers/_addROI_omero.py
+-rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.0.2/scimap/helpers/_animate.py
+-rw-r--r--   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.0.2/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.0.2/scimap/helpers/_dropFeatures.py
+-rw-r--r--   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/helpers/_merge_adata_obs.py
+-rw-r--r--   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.0.2/scimap/helpers/_scimap_to_csv.py
+-rw-r--r--   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0      463 2022-05-29 20:43:39.000000 scimap-1.0.2/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.0.2/scimap/plotting/_addROI_image.py
+-rw-r--r--   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.0.2/scimap/plotting/_cluster_plots.py
+-rw-r--r--   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/plotting/_foldchange.py
+-rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.0.2/scimap/plotting/_gate_finder.py
+-rw-r--r--   0        0        0     7769 2022-05-26 00:26:12.000000 scimap-1.0.2/scimap/plotting/_image_viewer.py
+-rw-r--r--   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/plotting/_pie.py
+-rw-r--r--   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.0.2/scimap/plotting/_spatial_distance.py
+-rw-r--r--   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.0.2/scimap/plotting/_spatial_interaction.py
+-rw-r--r--   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.0.2/scimap/plotting/_spatial_pscore.py
+-rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/plotting/_spatial_scatter.py
+-rw-r--r--   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.0.2/scimap/plotting/_stacked_barplot.py
+-rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.0.2/scimap/plotting/_umap.py
+-rw-r--r--   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.0.2/scimap/plotting/_voronoi.py
+-rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.0.2/scimap/plotting/lasso_selector.py
+-rw-r--r--   0        0        0      107 2023-04-20 01:30:26.000000 scimap-1.0.2/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.000000 scimap-1.0.2/scimap/preprocessing/_combat.py
+-rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.0.2/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.0.2/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tests/_data/phenotype_workflow.csv
+-rw-r--r--   0        0        0     1269 2022-05-18 01:22:39.000000 scimap-1.0.2/scimap/tests/test_helpers.py
+-rw-r--r--   0        0        0      985 2022-06-05 16:22:49.000000 scimap-1.0.2/scimap/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     4674 2022-04-02 14:45:20.000000 scimap-1.0.2/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.0.2/scimap/tools/__init__.py
+-rw-r--r--   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.0.2/scimap/tools/_cluster.py
+-rw-r--r--   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.0.2/scimap/tools/_foldchange.py
+-rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tools/_phenotype_cells.py
+-rw-r--r--   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tools/_spatial_aggregate.py
+-rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.0.2/scimap/tools/_spatial_cluster.py
+-rw-r--r--   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.0.2/scimap/tools/_spatial_count.py
+-rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.0.2/scimap/tools/_spatial_distance.py
+-rw-r--r--   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.0.2/scimap/tools/_spatial_expression.py
+-rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.0.2/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.0.2/scimap/tools/_spatial_lda.py
+-rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.0.2/scimap/tools/_spatial_pscore.py
+-rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.0.2/scimap/tools/_spatial_similarity_search.py
+-rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.0.2/scimap/tools/_umap.py
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 scimap-1.0.2/PKG-INFO
```

### Comparing `scimap-1.0.1/README.md` & `scimap-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/pyproject.toml` & `scimap-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "1.0.1"
+version = "1.0.2"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -35,15 +35,15 @@
 tifffile = "^2020.6.3"
 numpy = "^1.20.0"
 pytest-xvfb = "^2.0.0"
 matplotlib = "^3.2.1"
 PhenoGraph = "^1.5.7"
 scanpy = "^1.6.0"
 mkdocs = "^1.1.2"
-plotly = "^4.12.0"
+plotly = "^5.14.1"
 TiffFile = "^2020.11.18"
 dask = {extras = ["array"], version = "^2.30.0"}
 zarr = "2.10.3"
 napari = "^0.4.2"
 numba = ">=0.55.0"
 shapely = "^1.7.1"
 gensim = "^4.0"
```

### Comparing `scimap-1.0.1/scimap/cli/_scimap_mcmicro.py` & `scimap-1.0.2/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/cli/test.py` & `scimap-1.0.2/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_addROI_omero.py` & `scimap-1.0.2/scimap/helpers/_addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_add_roi_omero.py` & `scimap-1.0.2/scimap/helpers/_add_roi_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_animate.py` & `scimap-1.0.2/scimap/helpers/_animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_classify.py` & `scimap-1.0.2/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_dropFeatures.py` & `scimap-1.0.2/scimap/helpers/_dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_merge_adata_obs.py` & `scimap-1.0.2/scimap/helpers/_merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_rename.py` & `scimap-1.0.2/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/_scimap_to_csv.py` & `scimap-1.0.2/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/helpers/add_roi_scatter.py` & `scimap-1.0.2/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_addROI_image.py` & `scimap-1.0.2/scimap/plotting/_addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_cluster_plots.py` & `scimap-1.0.2/scimap/plotting/_cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_foldchange.py` & `scimap-1.0.2/scimap/plotting/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_gate_finder.py` & `scimap-1.0.2/scimap/plotting/_gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_image_viewer.py` & `scimap-1.0.2/scimap/plotting/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_pie.py` & `scimap-1.0.2/scimap/plotting/_pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_spatial_distance.py` & `scimap-1.0.2/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_spatial_interaction.py` & `scimap-1.0.2/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_spatial_pscore.py` & `scimap-1.0.2/scimap/plotting/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_spatial_scatter.py` & `scimap-1.0.2/scimap/plotting/_spatial_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_stacked_barplot.py` & `scimap-1.0.2/scimap/plotting/_stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_umap.py` & `scimap-1.0.2/scimap/plotting/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/_voronoi.py` & `scimap-1.0.2/scimap/plotting/_voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/plotting/lasso_selector.py` & `scimap-1.0.2/scimap/plotting/lasso_selector.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/preprocessing/_combat.py` & `scimap-1.0.2/scimap/preprocessing/_combat.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/preprocessing/_mcmicro_to_scimap.py` & `scimap-1.0.2/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/preprocessing/_rescale.py` & `scimap-1.0.2/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/_data/example_data.csv` & `scimap-1.0.2/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/_data/example_data.h5ad` & `scimap-1.0.2/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/_data/phenotype_workflow.csv` & `scimap-1.0.2/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/test_helpers.py` & `scimap-1.0.2/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/test_preprocessing.py` & `scimap-1.0.2/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tests/test_tools.py` & `scimap-1.0.2/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/__init__.py` & `scimap-1.0.2/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_cluster.py` & `scimap-1.0.2/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_foldchange.py` & `scimap-1.0.2/scimap/tools/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_phenotype_cells.py` & `scimap-1.0.2/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_aggregate.py` & `scimap-1.0.2/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_cluster.py` & `scimap-1.0.2/scimap/tools/_spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_count.py` & `scimap-1.0.2/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_distance.py` & `scimap-1.0.2/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_expression.py` & `scimap-1.0.2/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_interaction.py` & `scimap-1.0.2/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_lda.py` & `scimap-1.0.2/scimap/tools/_spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_pscore.py` & `scimap-1.0.2/scimap/tools/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_spatial_similarity_search.py` & `scimap-1.0.2/scimap/tools/_spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/scimap/tools/_umap.py` & `scimap-1.0.2/scimap/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.1/PKG-INFO` & `scimap-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<3.11
@@ -29,15 +29,15 @@
 Requires-Dist: mkdocs (>=1.1.2,<2.0.0)
 Requires-Dist: mkdocs-material (>=7.1.1,<8.0.0)
 Requires-Dist: napari (>=0.4.2,<0.5.0)
 Requires-Dist: napari-ome-zarr (>=0.4.0,<0.5.0)
 Requires-Dist: numba (>=0.55.0)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.4,<2.0.0)
-Requires-Dist: plotly (>=4.12.0,<5.0.0)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pytest (>=5.4.3,<6.0.0)
 Requires-Dist: pytest-xvfb (>=2.0.0,<3.0.0)
 Requires-Dist: scanpy (>=1.6.0,<2.0.0)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Requires-Dist: seaborn (>=0.11.0,<0.12.0)
 Requires-Dist: shapely (>=1.7.1,<2.0.0)
 Requires-Dist: tifffile (>=2020.6.3,<2021.0.0)
```

