# Comparing `tmp/peptide_forest-3.0.2.tar.gz` & `tmp/peptide_forest-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptide_forest-3.0.2.tar", last modified: Wed Mar 15 11:39:04 2023, max compression
+gzip compressed data, was "peptide_forest-3.0.3.tar", last modified: Fri Apr 21 08:27:44 2023, max compression
```

## Comparing `peptide_forest-3.0.2.tar` & `peptide_forest-3.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.144139 peptide_forest-3.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.144139 peptide_forest-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/.github/workflows/pypi_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/.github/workflows/tox_ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.144139 peptide_forest-3.0.2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/config/ursgal_path_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/peptide_forest/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/peptide_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest/training.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-15 11:39:03.000000 peptide_forest-3.0.2/peptide_forest/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/peptide_forest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 11:39:04.000000 peptide_forest-3.0.2/peptide_forest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-15 11:39:04.000000 peptide_forest-3.0.2/peptide_forest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 11:39:04.000000 peptide_forest-3.0.2/peptide_forest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-15 11:39:04.000000 peptide_forest-3.0.2/peptide_forest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 11:39:04.000000 peptide_forest-3.0.2/peptide_forest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/peptide_forest_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/tests/_data/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/_data/mascot_dat2csv_1_0_0.csv
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/_data/omssa_2_1_9.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/_data/path_dict_medium.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/tests/_data/quant_data/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/_data/quant_data/quant_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:39:04.148139 peptide_forest-3.0.2/tests/_data/raw_data/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/_data/raw_data/data_without_mscores.csv
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/test_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-15 11:38:54.000000 peptide_forest-3.0.2/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.692502 peptide_forest-3.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.692502 peptide_forest-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/.github/workflows/pypi_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/.github/workflows/tox_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.692502 peptide_forest-3.0.3/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/config/ursgal_path_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.692502 peptide_forest-3.0.3/peptide_forest/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/peptide_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/peptide_forest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 08:27:44.000000 peptide_forest-3.0.3/peptide_forest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/peptide_forest_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/tests/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/_data/mascot_dat2csv_1_0_0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/_data/omssa_2_1_9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/_data/path_dict_medium.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/tests/_data/quant_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/_data/quant_data/quant_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:27:44.696502 peptide_forest-3.0.3/tests/_data/raw_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/_data/raw_data/data_without_mscores.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/test_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-21 08:27:35.000000 peptide_forest-3.0.3/tests/test_training.py
```

### Comparing `peptide_forest-3.0.2/.github/workflows/tox_ci.yml` & `peptide_forest-3.0.3/.github/workflows/tox_ci.yml`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/.gitignore` & `peptide_forest-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/LICENSE` & `peptide_forest-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/PKG-INFO` & `peptide_forest-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptide_forest
-Version: 3.0.2
+Version: 3.0.3
 Summary: Integrate multiple search engines
 Home-page: https://github.com/peptideforest/peptideForest
 Author: T. Ranff, M. Dennison, J. Bédorf, S. Schulze, N. Zinn, M. Bantscheff, J.J.R.M. van Heugten, C. Fufezan
 Author-email: christian@fufezan.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `peptide_forest-3.0.2/config/ursgal_path_dict.json` & `peptide_forest-3.0.3/config/ursgal_path_dict.json`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest/knowledge_base.py` & `peptide_forest-3.0.3/peptide_forest/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest/peptide_forest.py` & `peptide_forest-3.0.3/peptide_forest/peptide_forest.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest/prep.py` & `peptide_forest-3.0.3/peptide_forest/prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,18 @@
     n = int(delta_col.split("_")[2])
     eng = delta_col[14:]
     score_col = f"score_processed_{eng}"
 
     # Find nth highest score per spectrum
     nth_score = (
         df.sort_values(score_col, ascending=False)
-        .groupby("spectrum_id")[score_col]
+        .groupby("spectrum_id")[["spectrum_id", score_col]]
         .nth(n=(n - 1))
-    )
+        .set_index("spectrum_id")
+    )[score_col]
     # Set to nan if 0
     nth_score.replace(0.0, pd.NA, inplace=True)
     # Calculate different to all other scores in group
     deltas = df.sort_values(score_col)[score_col] - df.sort_values(score_col)[
         "spectrum_id"
     ].map(nth_score)
```

### Comparing `peptide_forest-3.0.2/peptide_forest/results.py` & `peptide_forest-3.0.3/peptide_forest/results.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest/tools.py` & `peptide_forest-3.0.3/peptide_forest/tools.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest/training.py` & `peptide_forest-3.0.3/peptide_forest/training.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest.egg-info/PKG-INFO` & `peptide_forest-3.0.3/peptide_forest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptide-forest
-Version: 3.0.2
+Version: 3.0.3
 Summary: Integrate multiple search engines
 Home-page: https://github.com/peptideforest/peptideForest
 Author: T. Ranff, M. Dennison, J. Bédorf, S. Schulze, N. Zinn, M. Bantscheff, J.J.R.M. van Heugten, C. Fufezan
 Author-email: christian@fufezan.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `peptide_forest-3.0.2/peptide_forest.egg-info/SOURCES.txt` & `peptide_forest-3.0.3/peptide_forest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/peptide_forest_3.py` & `peptide_forest-3.0.3/peptide_forest_3.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/pyproject.toml` & `peptide_forest-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/setup.cfg` & `peptide_forest-3.0.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 	Topic :: Scientific/Engineering :: Chemistry
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 
 [options]
 packages = find:
 install_requires = 
 	numpy>=1.21.5,<1.25.0
-	pandas>=1.3.5,<1.6.0
+	pandas>=1.3.5,<2.1.0
 	uparma>=0.9.14,<1.1.0
-	loguru>=0.5.3,<0.7.0
+	loguru>=0.5.3,<0.8.0
 	scikit-learn~=1.2.0
 	tqdm>=4.62.3,<4.66.0
-	pytest>=6.2.5,<7.3.0
+	pytest>=6.2.5,<7.4.0
 
 [options.package_data]
 * = *.txt
 
 [options.extras_require]
 docs = 
 	sphinx
```

### Comparing `peptide_forest-3.0.2/setup.py` & `peptide_forest-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/tests/_data/mascot_dat2csv_1_0_0.csv` & `peptide_forest-3.0.3/tests/_data/mascot_dat2csv_1_0_0.csv`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/tests/_data/omssa_2_1_9.csv` & `peptide_forest-3.0.3/tests/_data/omssa_2_1_9.csv`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/tests/test_prep.py` & `peptide_forest-3.0.3/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/tests/test_results.py` & `peptide_forest-3.0.3/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `peptide_forest-3.0.2/tests/test_training.py` & `peptide_forest-3.0.3/tests/test_training.py`

 * *Files identical despite different names*

