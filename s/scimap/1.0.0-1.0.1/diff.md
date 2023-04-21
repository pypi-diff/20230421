# Comparing `tmp/scimap-1.0.0.tar.gz` & `tmp/scimap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.0.0.tar", max compression
+gzip compressed data, was "scimap-1.0.1.tar", max compression
```

## Comparing `scimap-1.0.0.tar` & `scimap-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     2327 2023-04-20 02:11:39.705770 scimap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.0.0/README.md
--rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5916 2022-05-22 15:28:25.000000 scimap-1.0.0/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.0.0/scimap/helpers/__init__.py
--rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.0.0/scimap/helpers/_add_roi_omero.py
--rw-r--r--   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.0.0/scimap/helpers/_addROI_omero.py
--rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.0.0/scimap/helpers/_animate.py
--rw-r--r--   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.0.0/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.0.0/scimap/helpers/_dropFeatures.py
--rw-r--r--   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/helpers/_merge_adata_obs.py
--rw-r--r--   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.0.0/scimap/helpers/_scimap_to_csv.py
--rw-r--r--   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0      463 2022-05-29 20:43:39.000000 scimap-1.0.0/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.0.0/scimap/plotting/_addROI_image.py
--rw-r--r--   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.0.0/scimap/plotting/_cluster_plots.py
--rw-r--r--   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/plotting/_foldchange.py
--rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.0.0/scimap/plotting/_gate_finder.py
--rw-r--r--   0        0        0     7769 2022-05-26 00:26:12.000000 scimap-1.0.0/scimap/plotting/_image_viewer.py
--rw-r--r--   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/plotting/_pie.py
--rw-r--r--   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.0.0/scimap/plotting/_spatial_distance.py
--rw-r--r--   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.0.0/scimap/plotting/_spatial_interaction.py
--rw-r--r--   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.0.0/scimap/plotting/_spatial_pscore.py
--rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/plotting/_spatial_scatter.py
--rw-r--r--   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.0.0/scimap/plotting/_stacked_barplot.py
--rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.0.0/scimap/plotting/_umap.py
--rw-r--r--   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.0.0/scimap/plotting/_voronoi.py
--rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.0.0/scimap/plotting/lasso_selector.py
--rw-r--r--   0        0        0      107 2023-04-20 01:30:26.000000 scimap-1.0.0/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     4947 2023-04-20 01:29:14.000000 scimap-1.0.0/scimap/preprocessing/_combat.py
--rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.0.0/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.0.0/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tests/_data/phenotype_workflow.csv
--rw-r--r--   0        0        0     1269 2022-05-18 01:22:39.000000 scimap-1.0.0/scimap/tests/test_helpers.py
--rw-r--r--   0        0        0      985 2022-06-05 16:22:49.000000 scimap-1.0.0/scimap/tests/test_preprocessing.py
--rw-r--r--   0        0        0     4674 2022-04-02 14:45:20.000000 scimap-1.0.0/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.0.0/scimap/tools/__init__.py
--rw-r--r--   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.0.0/scimap/tools/_cluster.py
--rw-r--r--   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.0.0/scimap/tools/_foldchange.py
--rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tools/_phenotype_cells.py
--rw-r--r--   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tools/_spatial_aggregate.py
--rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.0.0/scimap/tools/_spatial_cluster.py
--rw-r--r--   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.0.0/scimap/tools/_spatial_count.py
--rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.0.0/scimap/tools/_spatial_distance.py
--rw-r--r--   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.0.0/scimap/tools/_spatial_expression.py
--rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.0.0/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.0.0/scimap/tools/_spatial_lda.py
--rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.0.0/scimap/tools/_spatial_pscore.py
--rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.0.0/scimap/tools/_spatial_similarity_search.py
--rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.0.0/scimap/tools/_umap.py
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 scimap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.0.1/README.md
+-rw-r--r--   0        0        0     2340 2023-04-21 02:04:09.486223 scimap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.0.1/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.0.1/scimap/cli/test.py
+-rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.0.1/scimap/helpers/__init__.py
+-rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.0.1/scimap/helpers/_addROI_omero.py
+-rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.0.1/scimap/helpers/_add_roi_omero.py
+-rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.0.1/scimap/helpers/_animate.py
+-rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.0.1/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.0.1/scimap/helpers/_dropFeatures.py
+-rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/_merge_adata_obs.py
+-rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.0.1/scimap/helpers/_scimap_to_csv.py
+-rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0      463 2022-05-29 20:43:39.000000 scimap-1.0.1/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.0.1/scimap/plotting/_addROI_image.py
+-rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.0.1/scimap/plotting/_cluster_plots.py
+-rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_foldchange.py
+-rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.0.1/scimap/plotting/_gate_finder.py
+-rw-r--r--   0        0        0     7769 2022-05-26 00:26:12.000000 scimap-1.0.1/scimap/plotting/_image_viewer.py
+-rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_pie.py
+-rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.0.1/scimap/plotting/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.0.1/scimap/plotting/_spatial_interaction.py
+-rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.0.1/scimap/plotting/_spatial_pscore.py
+-rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/plotting/_spatial_scatter.py
+-rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.0.1/scimap/plotting/_stacked_barplot.py
+-rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.0.1/scimap/plotting/_umap.py
+-rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.0.1/scimap/plotting/_voronoi.py
+-rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.0.1/scimap/plotting/lasso_selector.py
+-rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.0.1/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.0.1/scimap/preprocessing/_combat.py
+-rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.0.1/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.0.1/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tests/_data/phenotype_workflow.csv
+-rwxr-xr-x   0        0        0     1269 2022-05-18 01:22:39.000000 scimap-1.0.1/scimap/tests/test_helpers.py
+-rwxr-xr-x   0        0        0      985 2022-06-05 16:22:49.000000 scimap-1.0.1/scimap/tests/test_preprocessing.py
+-rwxr-xr-x   0        0        0     4674 2022-04-02 14:45:20.000000 scimap-1.0.1/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.0.1/scimap/tools/__init__.py
+-rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.0.1/scimap/tools/_cluster.py
+-rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.0.1/scimap/tools/_foldchange.py
+-rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_phenotype_cells.py
+-rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_spatial_aggregate.py
+-rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.0.1/scimap/tools/_spatial_cluster.py
+-rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.0.1/scimap/tools/_spatial_count.py
+-rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.0.1/scimap/tools/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.0.1/scimap/tools/_spatial_expression.py
+-rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.0.1/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.0.1/scimap/tools/_spatial_lda.py
+-rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.0.1/scimap/tools/_spatial_pscore.py
+-rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.0.1/scimap/tools/_spatial_similarity_search.py
+-rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.0.1/scimap/tools/_umap.py
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 scimap-1.0.1/PKG-INFO
```

### Comparing `scimap-1.0.0/pyproject.toml` & `scimap-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "1.0.0"
+version = "1.0.1"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -14,15 +14,15 @@
 documentation = "https://scimap.xyz"
 repository = "https://github.com/labsyspharm/scimap"
 
 keywords = ["image analysis","multiplex imaging","single cell analysis"]
 
 classifiers = [
     # TODO: update this list to match your application: https://pypi.org/pypi?%3Aaction=list_classifiers
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `scimap-1.0.0/README.md` & `scimap-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/cli/_scimap_mcmicro.py` & `scimap-1.0.1/scimap/cli/_scimap_mcmicro.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,210 +6,186 @@
 
 import sys
 import argparse
 import pathlib
 import textwrap
 from joblib import Parallel, delayed
 
+
+# Actual mcmicro code
+
 def mcmicro_wrap(argv=sys.argv):
-    
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         'csv',
         help='single-cell quantification table (CSV file) generated by mcmicro',
     )
-    parser.add_argument(
-        '-o', '--output', default='.',
-        help='output directory'
-    )
+    parser.add_argument('-o', '--output', default='.', help='output directory')
 
     args = parser.parse_args(argv[1:])
 
     run_result = Parallel(n_jobs=-1, verbose=1)(
-        delayed(clustering)([None, args.csv, '-o', args.output, '--clustering-method', m]) 
+        delayed(clustering)(
+            [None, args.csv, '-o', args.output, '--clustering-method', m]
+        )
         for m in ['spatial', 'kmeans', 'phenograph', 'leiden']
     )
 
     print(run_result)
-    
+
     merge([None, args.output, '-o', args.output, '-d', '--csv'])
 
     # move pdf files to output / plots
     output_dir = pathlib.Path(args.output)
     pdfs = sorted(output_dir.rglob('*.pdf'))
     plots_dir = output_dir / 'plots'
     plots_dir.mkdir(exist_ok=True)
 
     if len(pdfs) > 0:
-        print(textwrap.indent(
-            'Moving pdf plots:\n',
-            '    '
-        ))
+        print(textwrap.indent('Moving pdf plots:\n', '    '))
     for p in pdfs:
         if plots_dir not in p.parents:
             move_to = plots_dir / p.parent.name / p.name
-            print(textwrap.indent(
-                f'{str(p)}\n    -> {str(move_to)}',
-                '    '
-            ))
+            print(textwrap.indent(f'{str(p)}\n    -> {str(move_to)}', '    '))
             move_to.parent.mkdir(exist_ok=True, parents=True)
             p.replace(move_to)
     print()
     return 0
 
-def clustering(argv=sys.argv):
 
+def clustering(argv=sys.argv):
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         'csv',
         help='single-cell quantification table (CSV file) generated by mcmicro',
     )
-    parser.add_argument(
-        '-o', '--output', default='.',
-        help='output directory'
-    )
+    parser.add_argument('-o', '--output', default='.', help='output directory')
     clustering_methods = ['all', 'spatial', 'kmeans', 'phenograph', 'leiden', 'pass']
     parser.add_argument(
-        '--clustering-method', default=['all'], choices=clustering_methods, nargs='+', 
-        help='choice of clustering algorithms, "pass": do not run any clustering methods; "all": run all clustering methods; default: "all"'
+        '--clustering-method',
+        default=['all'],
+        choices=clustering_methods,
+        nargs='+',
+        help='choice of clustering algorithms, "pass": do not run any clustering methods; "all": run all clustering methods; default: "all"',
     )
 
     args = parser.parse_args(argv[1:])
 
     _output_dir = pathlib.Path(args.output)
     mcmicro_csv_path = args.csv
     methods = set(args.clustering_method)
 
     assert '.csv' in mcmicro_csv_path, 'input file must be a csv file'
-    
+
     if 'all' in methods:
         methods = clustering_methods[1:-1]
 
     if 'pass' in methods:
         pp.mcmicro_to_scimap(
-            feature_table_path = mcmicro_csv_path, 
-            output_dir = str(_output_dir)
+            feature_table_path=mcmicro_csv_path, output_dir=str(_output_dir)
         )
         return
 
     for method in methods:
-
         output_dir = _output_dir / method
-        
+
         pp.mcmicro_to_scimap(
-            feature_table_path = mcmicro_csv_path, 
-            output_dir = str(output_dir)
+            feature_table_path=mcmicro_csv_path, output_dir=str(output_dir)
         )
 
-        adata_path = pathlib.Path(output_dir) / f'{pathlib.Path(mcmicro_csv_path).stem}.h5ad'
+        adata_path = (
+            pathlib.Path(output_dir) / f'{pathlib.Path(mcmicro_csv_path).stem}.h5ad'
+        )
 
         if method == 'spatial':
             # Spatial clustering
-            tl.spatial_expression(
-                adata = str(adata_path), 
-                output_dir = output_dir
-            )
+            tl.spatial_expression(adata=str(adata_path), output_dir=output_dir)
             tl.spatial_cluster(
-                adata = str(adata_path), 
-                df_name = "spatial_expression",
-                output_dir = output_dir
+                adata=str(adata_path),
+                df_name="spatial_expression",
+                output_dir=output_dir,
             )
-        
+
         else:
             # Expression clustering
-            tl.cluster(
-                adata = str(adata_path), 
-                method = method,
-                output_dir = output_dir
-            )
+            tl.cluster(adata=str(adata_path), method=method, output_dir=output_dir)
 
             # Expression clustering plots
             pl.cluster_plots(
-                adata = str(adata_path), 
-                group_by  = method,
-                output_dir = output_dir
+                adata=str(adata_path), group_by=method, output_dir=output_dir
             )
     return 0
 
+
 def merge(argv=sys.argv):
-    
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         'directory',
         help='recursively search for .h5ad files to merge',
     )
+    parser.add_argument('-o', '--output', default='.', help='output directory')
     parser.add_argument(
-        '-o', '--output', default='.',
-        help='output directory'
+        '-d',
+        '--delete-merged',
+        default=False,
+        action='store_true',
+        help='delete found input files after merging; default: False',
     )
     parser.add_argument(
-        '-d', '--delete-merged', default=False, action='store_true',
-        help='delete found input files after merging; default: False'
-    )
-    parser.add_argument(
-        '--csv', default=False, action='store_true',
-        help='output csv version of the merged h5ad file; default: False'
+        '--csv',
+        default=False,
+        action='store_true',
+        help='output csv version of the merged h5ad file; default: False',
     )
 
     args = parser.parse_args(argv[1:])
 
     input_dir = pathlib.Path(args.directory)
     output_dir = pathlib.Path(args.output)
     delete_after = args.delete_merged
     output_csv = args.csv
 
     input_files = sorted(input_dir.rglob('*.h5ad'))
     output_file = output_dir / input_files[0].name
-    
+
     if len(input_files) == 0:
         print(f'0 .h5ad found in {str(input_dir)}')
         return 1
 
     print_text = '''
         Merging:
 
         {}
 
         Writing:
 
         {}'''
     print_text = textwrap.dedent(print_text).format(
-        "\n".join([str(p) for p in input_files]),
-        str(output_file)
+        "\n".join([str(p) for p in input_files]), str(output_file)
     )
     print(textwrap.indent(print_text, '    '))
     # Merge data
-    hl.merge_adata_obs(
-        adata = [
-            str(p)
-            for p in input_files
-        ],
-        output_dir = output_dir
-    )
+    hl.merge_adata_obs(adata=[str(p) for p in input_files], output_dir=output_dir)
     if output_csv == True:
-        hl.scimap_to_csv(
-            adata = str(output_file),
-            output_dir = output_dir
-        )
-        print(textwrap.indent(
-            str(output_file.parent / f'{output_file.stem}.csv\n'),
-            '    '
-        ))
-    
+        hl.scimap_to_csv(adata=str(output_file), output_dir=output_dir)
+        print(
+            textwrap.indent(
+                str(output_file.parent / f'{output_file.stem}.csv\n'), '    '
+            )
+        )
 
     if delete_after == True:
         if output_file in input_files:
             idx = input_files.index(output_file)
             input_files.pop(idx)
         print(
             textwrap.indent(
-                'Deleting:\n\n' + "\n".join([str(f) for f in input_files]),
-                '    '
+                'Deleting:\n\n' + "\n".join([str(f) for f in input_files]), '    '
             )
         )
         for f in input_files:
             f.unlink()
         print()
-    return 0
+    return 0
```

### Comparing `scimap-1.0.0/scimap/helpers/_add_roi_omero.py` & `scimap-1.0.1/scimap/helpers/_add_roi_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_addROI_omero.py` & `scimap-1.0.1/scimap/helpers/_addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_animate.py` & `scimap-1.0.1/scimap/helpers/_animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_classify.py` & `scimap-1.0.1/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_dropFeatures.py` & `scimap-1.0.1/scimap/helpers/_dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_merge_adata_obs.py` & `scimap-1.0.1/scimap/helpers/_merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_rename.py` & `scimap-1.0.1/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/_scimap_to_csv.py` & `scimap-1.0.1/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/helpers/add_roi_scatter.py` & `scimap-1.0.1/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_addROI_image.py` & `scimap-1.0.1/scimap/plotting/_addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_cluster_plots.py` & `scimap-1.0.1/scimap/plotting/_cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_foldchange.py` & `scimap-1.0.1/scimap/plotting/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_gate_finder.py` & `scimap-1.0.1/scimap/plotting/_gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_image_viewer.py` & `scimap-1.0.1/scimap/plotting/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_pie.py` & `scimap-1.0.1/scimap/plotting/_pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_spatial_distance.py` & `scimap-1.0.1/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_spatial_interaction.py` & `scimap-1.0.1/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_spatial_pscore.py` & `scimap-1.0.1/scimap/plotting/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_spatial_scatter.py` & `scimap-1.0.1/scimap/plotting/_spatial_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_stacked_barplot.py` & `scimap-1.0.1/scimap/plotting/_stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_umap.py` & `scimap-1.0.1/scimap/plotting/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/_voronoi.py` & `scimap-1.0.1/scimap/plotting/_voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/plotting/lasso_selector.py` & `scimap-1.0.1/scimap/plotting/lasso_selector.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/preprocessing/_combat.py` & `scimap-1.0.1/scimap/preprocessing/_combat.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,145 +15,149 @@
 from combat.pycombat import pycombat
 import pandas as pd
 import anndata as ad
 import numpy as np
 import argparse
 
 
+def combat(
+    adata,
+    batch='imageid',
+    layers=None,
+    log=False,
+    replaceOriginal=False,
+    label='combat'):
+    
+    """
+    Parameters:
+
+        adata (AnnData object):  
+            Annotated data matrix.
+
+        batch (str, optional):  
+            The batch key or column in `adata.obs` that indicates the batches for each cell.
+
+        layers (str or None, optional):
+            The layer in `adata.layers` that contains the expression data to correct. If None, 
+            `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`
 
-def combat (adata, 
-            batch='imageid', 
-            layers=None,
-            log=False,
-            replaceOriginal=False, 
-            label='combat'):
-    
-"""
+        log (bool, optional):  
+            Whether to log transform the data before applying ComBat. Generally use it with `raw`.
 
+        replaceOriginal (bool, optional):
+            Whether to replace the original expression data in `adata` with the corrected data.
+
+        label (str, optional):  
+            The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is `True`, this parameter has no effect.  
 
-Parameters:
-    
-    adata (AnnData object):  
-        Annotated data matrix.
-        
-    batch (str, optional):   
-        The batch key or column in `adata.obs` that indicates the batches for each cell.
-        
-    layers (str or None, optional):  
-        The layer in `adata.layers` that contains the expression data to correct.
-        If None, `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`
-        
-    log (bool, optional):  
-        Whether to log transform the data before applying ComBat. Generally use it with `raw`.
-        
-    replaceOriginal (bool, optional):  
-        Whether to replace the original expression data in `adata` with the corrected data.
-        
-    label (str, optional):  
-        The prefix for the key in `adata` that will contain the corrected data.
-        If `replaceOriginal` is True, this parameter has no effect.
-    
     Returns:
-        
-     adata (anndata):  
-        The corrected expression data is stored in a new layer `adata.layers['combat']`.
-    
+
+        adata (anndata):  
+            The corrected expression data is stored in a new layer `adata.layers['combat']`.
+
     Examples:
-        
+
         ```python
-        
+
         # applying batch correction using raw data
-        adata = combat (adata, 
-                    batch='imageid', 
-                    layers='raw',
-                    log=True,
-                    replaceOriginal=False, 
-                    label='combat')
-        
+        adata = combat (adata,
+                        batch='imageid',
+                        layers='raw',
+                        log=True,
+                        replaceOriginal=False,
+                        label='combat')
+
         # results will be available in adata.layers['combat']
-        
+
         ```
-"""
-    
+    """
+
     # isolate the data
     if layers is None:
         data = pd.DataFrame(adata.X, index=adata.obs.index, columns=adata.var.index)
     elif layers == 'raw':
         data = pd.DataFrame(adata.raw.X, index=adata.obs.index, columns=adata.var.index)
     else:
-        data = pd.DataFrame(adata.layers[layers], index=adata.obs.index, columns=adata.var.index)
-    
+        data = pd.DataFrame(
+            adata.layers[layers], index=adata.obs.index, columns=adata.var.index
+        )
+
     # log the data if requested
     if log is True:
         data = np.log1p(data)
-    
+
     # isolate batch
     batchData = adata.obs[batch]
-    
-    #convert to category
+
+    # convert to category
     batchData = batchData.astype('category')
-    
+
     # make sure there are atleast two batches
     if len(batchData.unique()) < 2:
-        raise Exception("Sorry a minimum of 2 batches is required. Please check the '" + str(batch) + "' column")
-    
+        raise Exception(
+            "Sorry a minimum of 2 batches is required. Please check the '"
+            + str(batch)
+            + "' column"
+        )
+
     # perform batch correction
-    batchCorrected = pycombat(data.T,batchData).T
-    
+    batchCorrected = pycombat(data.T, batchData).T
+
     # add as a specific layer
     adata.layers[label] = batchCorrected
-    
+
     # replace original
     if replaceOriginal is True:
         if layers is None:
             adata.X = batchCorrected
         elif layers == 'raw':
             del adata.raw
             adata.raw = ad.AnnData(batchCorrected, obs=adata.obs)
         else:
             adata.layers[layers] = batchCorrected
-    
+
     # return adata
     return adata
-    
+
 
 # Make the Function CLI compatable
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Run ComBat batch correction.')
     parser.add_argument('--adata', type=str, help='Annotated data matrix.')
-    parser.add_argument('--batch', type=str, default='imageid', help='The batch key or column in `adata.obs` that indicates the batches for each cell.')
-    parser.add_argument('--layers', type=str, default=None, help='The layer in `adata.layers` that contains the expression data to correct. If None, `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`')
-    parser.add_argument('--log', type=bool, default=False, help='Whether to log transform the data before applying ComBat. Generally use it with `raw`.')
-    parser.add_argument('--replaceOriginal', type=bool, default=False, help='Whether to replace the original expression data in `adata` with the corrected data.')
-    parser.add_argument('--label', type=str, default='combat', help='The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is True, this parameter has no effect.')
-    args = parser.parse_args()    
-    combat(adata=args.adata, 
-           batch=args.batch, 
-           layers=args.layers, 
-           log=args.log, 
-           replaceOriginal=args.replaceOriginal, 
-           label=args.label)
-
-    
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    parser.add_argument(
+        '--batch',
+        type=str,
+        default='imageid',
+        help='The batch key or column in `adata.obs` that indicates the batches for each cell.',
+    )
+    parser.add_argument(
+        '--layers',
+        type=str,
+        default=None,
+        help='The layer in `adata.layers` that contains the expression data to correct. If None, `adata.X` is used. use `raw` to use the data stored in `adata.raw.X`',
+    )
+    parser.add_argument(
+        '--log',
+        type=bool,
+        default=False,
+        help='Whether to log transform the data before applying ComBat. Generally use it with `raw`.',
+    )
+    parser.add_argument(
+        '--replaceOriginal',
+        type=bool,
+        default=False,
+        help='Whether to replace the original expression data in `adata` with the corrected data.',
+    )
+    parser.add_argument(
+        '--label',
+        type=str,
+        default='combat',
+        help='The prefix for the key in `adata` that will contain the corrected data. If `replaceOriginal` is True, this parameter has no effect.',
+    )
+    args = parser.parse_args()
+    combat(
+        adata=args.adata,
+        batch=args.batch,
+        layers=args.layers,
+        log=args.log,
+        replaceOriginal=args.replaceOriginal,
+        label=args.label)
```

### Comparing `scimap-1.0.0/scimap/preprocessing/_mcmicro_to_scimap.py` & `scimap-1.0.1/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/preprocessing/_rescale.py` & `scimap-1.0.1/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/_data/example_data.csv` & `scimap-1.0.1/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/_data/example_data.h5ad` & `scimap-1.0.1/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/_data/phenotype_workflow.csv` & `scimap-1.0.1/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/test_helpers.py` & `scimap-1.0.1/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/test_preprocessing.py` & `scimap-1.0.1/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tests/test_tools.py` & `scimap-1.0.1/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/__init__.py` & `scimap-1.0.1/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_cluster.py` & `scimap-1.0.1/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_foldchange.py` & `scimap-1.0.1/scimap/tools/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_phenotype_cells.py` & `scimap-1.0.1/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_aggregate.py` & `scimap-1.0.1/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_cluster.py` & `scimap-1.0.1/scimap/tools/_spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_count.py` & `scimap-1.0.1/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_distance.py` & `scimap-1.0.1/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_expression.py` & `scimap-1.0.1/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_interaction.py` & `scimap-1.0.1/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_lda.py` & `scimap-1.0.1/scimap/tools/_spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_pscore.py` & `scimap-1.0.1/scimap/tools/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_spatial_similarity_search.py` & `scimap-1.0.1/scimap/tools/_spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/scimap/tools/_umap.py` & `scimap-1.0.1/scimap/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.0.0/PKG-INFO` & `scimap-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<3.11
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

