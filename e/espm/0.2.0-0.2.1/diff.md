# Comparing `tmp/espm-0.2.0.tar.gz` & `tmp/espm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espm-0.2.0.tar", last modified: Thu Apr 20 14:38:31 2023, max compression
+gzip compressed data, was "espm-0.2.1.tar", last modified: Fri Apr 21 09:14:35 2023, max compression
```

## Comparing `espm-0.2.0.tar` & `espm-0.2.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.807454 espm-0.2.0/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.792374 espm-0.2.0/.github/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795137 espm-0.2.0/.github/workflows/
--rw-r--r--   0 nati       (501) staff       (20)     1119 2023-02-23 15:04:13.000000 espm-0.2.0/.github/workflows/python.yml
--rw-r--r--   0 nati       (501) staff       (20)      178 2023-02-21 16:38:53.000000 espm-0.2.0/.readthedocs.yml
--rw-r--r--   0 nati       (501) staff       (20)      583 2023-04-20 13:32:32.000000 espm-0.2.0/CHANGELOG.rst
--rw-r--r--   0 nati       (501) staff       (20)     3993 2023-02-22 09:05:19.000000 espm-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 nati       (501) staff       (20)     1083 2022-12-06 13:16:22.000000 espm-0.2.0/Licence.txt
--rw-r--r--   0 nati       (501) staff       (20)      372 2023-04-18 07:43:05.000000 espm-0.2.0/MANIFEST.in
--rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-20 14:38:31.807301 espm-0.2.0/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     1767 2023-04-20 13:26:45.000000 espm-0.2.0/README.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795785 espm-0.2.0/doc/
--rw-r--r--   0 nati       (501) staff       (20)       30 2020-12-17 09:02:04.000000 espm-0.2.0/doc/changelog.rst
--rw-r--r--   0 nati       (501) staff       (20)     1994 2023-02-23 09:58:20.000000 espm-0.2.0/doc/conf.py
--rw-r--r--   0 nati       (501) staff       (20)       33 2019-04-30 16:36:26.000000 espm-0.2.0/doc/contributing.rst
--rw-r--r--   0 nati       (501) staff       (20)      213 2023-02-23 09:10:02.000000 espm-0.2.0/doc/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.795923 espm-0.2.0/doc/introduction/
--rw-r--r--   0 nati       (501) staff       (20)     4486 2023-04-20 12:54:03.000000 espm-0.2.0/doc/introduction/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.797084 espm-0.2.0/doc/reference/
--rw-r--r--   0 nati       (501) staff       (20)      220 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/datasets.rst
--rw-r--r--   0 nati       (501) staff       (20)      202 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/estimators.rst
--rw-r--r--   0 nati       (501) staff       (20)      156 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/index.rst
--rw-r--r--   0 nati       (501) staff       (20)       58 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/measures.rst
--rw-r--r--   0 nati       (501) staff       (20)      257 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/models.rst
--rw-r--r--   0 nati       (501) staff       (20)       70 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/table_utils.rst
--rw-r--r--   0 nati       (501) staff       (20)       45 2023-02-21 16:38:50.000000 espm-0.2.0/doc/reference/utils.rst
--rw-r--r--   0 nati       (501) staff       (20)      140 2023-04-20 12:35:31.000000 espm-0.2.0/doc/reference/weights.rst
--rw-r--r--   0 nati       (501) staff       (20)       95 2019-04-30 16:36:26.000000 espm-0.2.0/doc/references.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.797235 espm-0.2.0/doc/styles/
--rw-r--r--   0 nati       (501) staff       (20)      332 2023-02-20 15:43:46.000000 espm-0.2.0/doc/styles/sg_gallery.css
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.798332 espm-0.2.0/espm/
--rw-r--r--   0 nati       (501) staff       (20)       21 2023-04-20 13:29:50.000000 espm-0.2.0/espm/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     1385 2023-04-20 12:35:31.000000 espm-0.2.0/espm/conf.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.799758 espm-0.2.0/espm/datasets/
--rw-r--r--   0 nati       (501) staff       (20)     1026 2023-04-20 12:35:31.000000 espm-0.2.0/espm/datasets/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     9637 2023-04-20 13:46:14.000000 espm-0.2.0/espm/datasets/base.py
--rw-r--r--   0 nati       (501) staff       (20)     5738 2023-04-20 12:53:51.000000 espm-0.2.0/espm/datasets/built_in_EDXS_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)    17812 2023-04-20 12:53:51.000000 espm-0.2.0/espm/datasets/eds_spim.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.800038 espm-0.2.0/espm/datasets/toy-problem/
--rw-r--r--   0 nati       (501) staff       (20)     4316 2023-02-21 16:38:50.000000 espm-0.2.0/espm/datasets/toy-problem/phase1.png
--rw-r--r--   0 nati       (501) staff       (20)     6798 2023-02-21 16:38:50.000000 espm-0.2.0/espm/datasets/toy-problem/phase2.png
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.800972 espm-0.2.0/espm/estimators/
--rw-r--r--   0 nati       (501) staff       (20)      529 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    19415 2023-02-23 13:48:32.000000 espm-0.2.0/espm/estimators/base.py
--rw-r--r--   0 nati       (501) staff       (20)     6026 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/dicotomy.py
--rw-r--r--   0 nati       (501) staff       (20)    10252 2023-02-23 14:37:13.000000 espm-0.2.0/espm/estimators/smooth_nmf.py
--rw-r--r--   0 nati       (501) staff       (20)     5700 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/surrogates.py
--rw-r--r--   0 nati       (501) staff       (20)    11222 2023-02-23 09:58:20.000000 espm-0.2.0/espm/estimators/updates.py
--rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.0/espm/hyperspy_extension.yaml
--rw-r--r--   0 nati       (501) staff       (20)    20639 2023-04-20 13:24:00.000000 espm-0.2.0/espm/measures.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.801816 espm-0.2.0/espm/models/
--rw-r--r--   0 nati       (501) staff       (20)    13015 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/EDXS_function.py
--rw-r--r--   0 nati       (501) staff       (20)      500 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    10090 2023-04-20 12:35:31.000000 espm-0.2.0/espm/models/absorption_edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     5682 2023-04-20 13:36:07.000000 espm-0.2.0/espm/models/base.py
--rw-r--r--   0 nati       (501) staff       (20)    17112 2023-04-20 12:53:51.000000 espm-0.2.0/espm/models/edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     6598 2023-04-20 13:17:58.000000 espm-0.2.0/espm/models/generate_EDXS_phases.py
--rw-r--r--   0 nati       (501) staff       (20)     3130 2023-02-23 09:58:20.000000 espm-0.2.0/espm/spectrum_fitting.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.803629 espm-0.2.0/espm/tables/
--rw-r--r--   0 nati       (501) staff       (20)   299008 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/100keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   288577 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/200keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   282569 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/300keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)     6242 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/SDD_efficiency.txt
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)   166571 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/default_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)    11811 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/periodic_table_number.json
--rw-r--r--   0 nati       (501) staff       (20)    11616 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/periodic_table_symbols.json
--rw-r--r--   0 nati       (501) staff       (20)      779 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tables/siegbahn_to_iupac.json
--rw-r--r--   0 nati       (501) staff       (20)     7514 2023-04-20 12:53:51.000000 espm-0.2.0/espm/tables_utils.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.804759 espm-0.2.0/espm/tests/
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.0/espm/tests/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     4910 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_EDXS.py
--rw-r--r--   0 nati       (501) staff       (20)    11339 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)     1073 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_docstring.py
--rw-r--r--   0 nati       (501) staff       (20)     9587 2023-04-18 07:43:05.000000 espm-0.2.0/espm/tests/test_estimators.py
--rw-r--r--   0 nati       (501) staff       (20)     1263 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_laplacian.py
--rw-r--r--   0 nati       (501) staff       (20)     7634 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_measures.py
--rw-r--r--   0 nati       (501) staff       (20)    29130 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_updates.py
--rw-r--r--   0 nati       (501) staff       (20)     3652 2023-02-23 09:58:20.000000 espm-0.2.0/espm/tests/test_utils.py
--rw-r--r--   0 nati       (501) staff       (20)    11669 2023-04-20 12:53:51.000000 espm-0.2.0/espm/utils.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.805166 espm-0.2.0/espm/weights/
--rw-r--r--   0 nati       (501) staff       (20)      258 2023-04-20 12:53:51.000000 espm-0.2.0/espm/weights/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    16957 2023-04-20 13:14:42.000000 espm-0.2.0/espm/weights/abundance.py
--rw-r--r--   0 nati       (501) staff       (20)    11055 2023-04-20 12:53:51.000000 espm-0.2.0/espm/weights/generate_weights.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.799248 espm-0.2.0/espm.egg-info/
--rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     2441 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/SOURCES.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/dependency_links.txt
--rw-r--r--   0 nati       (501) staff       (20)       34 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/entry_points.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/not-zip-safe
--rw-r--r--   0 nati       (501) staff       (20)      207 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/requires.txt
--rw-r--r--   0 nati       (501) staff       (20)        5 2023-04-20 14:38:31.000000 espm-0.2.0/espm.egg-info/top_level.txt
--rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.0/hyperspy_extension.yaml
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.806980 espm-0.2.0/notebooks/
--rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-0.2.0/notebooks/VCA.py
--rw-r--r--   0 nati       (501) staff       (20)     5381 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/api.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17775 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/background_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13661 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/convergence-speed.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     8875 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/generate_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     3204 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/make-plots.ipynb
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-20 14:38:31.807119 espm-0.2.0/notebooks/old/
--rw-r--r--   0 nati       (501) staff       (20)     6289 2022-02-25 16:24:57.000000 espm-0.2.0/notebooks/old/algo-with-negative-variable.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     6820 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/other_algorithms.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17002 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/preprocess_dataset.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     4531 2023-04-20 14:38:30.000000 espm-0.2.0/notebooks/select_spectrum.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    14791 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/simple-test-regularisation.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    31459 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/spectrum_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-0.2.0/notebooks/sunsal.py
--rw-r--r--   0 nati       (501) staff       (20)     7554 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/surrogate-vs-bregmann.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    18735 2023-04-20 14:38:31.000000 espm-0.2.0/notebooks/toy-ML.ipynb
--rw-r--r--   0 nati       (501) staff       (20)      178 2022-12-06 17:40:13.000000 espm-0.2.0/readthedoc.yml
--rw-r--r--   0 nati       (501) staff       (20)       38 2023-04-20 14:38:31.807492 espm-0.2.0/setup.cfg
--rw-r--r--   0 nati       (501) staff       (20)     1800 2023-04-20 13:28:26.000000 espm-0.2.0/setup.py
--rw-r--r--   0 nati       (501) staff       (20)     1120 2023-04-20 13:27:14.000000 espm-0.2.0/todo.md
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.776807 espm-0.2.1/
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.758863 espm-0.2.1/.github/
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.762186 espm-0.2.1/.github/workflows/
+-rw-r--r--   0 nati       (501) staff       (20)      870 2023-04-21 08:29:28.000000 espm-0.2.1/.github/workflows/doc.yml
+-rw-r--r--   0 nati       (501) staff       (20)     1117 2023-04-21 08:28:14.000000 espm-0.2.1/.github/workflows/python.yml
+-rw-r--r--   0 nati       (501) staff       (20)      178 2023-02-21 16:38:53.000000 espm-0.2.1/.readthedocs.yml
+-rw-r--r--   0 nati       (501) staff       (20)      583 2023-04-20 13:32:32.000000 espm-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 nati       (501) staff       (20)     3992 2023-04-20 14:55:38.000000 espm-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 nati       (501) staff       (20)     1083 2022-12-06 13:16:22.000000 espm-0.2.1/Licence.txt
+-rw-r--r--   0 nati       (501) staff       (20)      372 2023-04-18 07:43:05.000000 espm-0.2.1/MANIFEST.in
+-rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-21 09:14:35.776524 espm-0.2.1/PKG-INFO
+-rw-r--r--   0 nati       (501) staff       (20)     1767 2023-04-20 13:26:45.000000 espm-0.2.1/README.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.762879 espm-0.2.1/doc/
+-rw-r--r--   0 nati       (501) staff       (20)       30 2020-12-17 09:02:04.000000 espm-0.2.1/doc/changelog.rst
+-rw-r--r--   0 nati       (501) staff       (20)     1994 2023-02-23 09:58:20.000000 espm-0.2.1/doc/conf.py
+-rw-r--r--   0 nati       (501) staff       (20)       33 2019-04-30 16:36:26.000000 espm-0.2.1/doc/contributing.rst
+-rw-r--r--   0 nati       (501) staff       (20)      213 2023-02-23 09:10:02.000000 espm-0.2.1/doc/index.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.763003 espm-0.2.1/doc/introduction/
+-rw-r--r--   0 nati       (501) staff       (20)     4412 2023-04-21 08:37:45.000000 espm-0.2.1/doc/introduction/index.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.764255 espm-0.2.1/doc/reference/
+-rw-r--r--   0 nati       (501) staff       (20)      220 2023-04-20 12:35:31.000000 espm-0.2.1/doc/reference/datasets.rst
+-rw-r--r--   0 nati       (501) staff       (20)      202 2023-02-21 16:38:50.000000 espm-0.2.1/doc/reference/estimators.rst
+-rw-r--r--   0 nati       (501) staff       (20)      156 2023-04-20 12:35:31.000000 espm-0.2.1/doc/reference/index.rst
+-rw-r--r--   0 nati       (501) staff       (20)       58 2023-02-21 16:38:50.000000 espm-0.2.1/doc/reference/measures.rst
+-rw-r--r--   0 nati       (501) staff       (20)      257 2023-04-20 12:35:31.000000 espm-0.2.1/doc/reference/models.rst
+-rw-r--r--   0 nati       (501) staff       (20)       70 2023-04-20 12:35:31.000000 espm-0.2.1/doc/reference/table_utils.rst
+-rw-r--r--   0 nati       (501) staff       (20)       45 2023-02-21 16:38:50.000000 espm-0.2.1/doc/reference/utils.rst
+-rw-r--r--   0 nati       (501) staff       (20)      140 2023-04-20 12:35:31.000000 espm-0.2.1/doc/reference/weights.rst
+-rw-r--r--   0 nati       (501) staff       (20)       95 2019-04-30 16:36:26.000000 espm-0.2.1/doc/references.rst
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.764380 espm-0.2.1/doc/styles/
+-rw-r--r--   0 nati       (501) staff       (20)      332 2023-02-20 15:43:46.000000 espm-0.2.1/doc/styles/sg_gallery.css
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.765496 espm-0.2.1/espm/
+-rw-r--r--   0 nati       (501) staff       (20)       21 2023-04-21 09:12:59.000000 espm-0.2.1/espm/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     1385 2023-04-20 12:35:31.000000 espm-0.2.1/espm/conf.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.767254 espm-0.2.1/espm/datasets/
+-rw-r--r--   0 nati       (501) staff       (20)     1026 2023-04-20 12:35:31.000000 espm-0.2.1/espm/datasets/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     9637 2023-04-20 13:46:14.000000 espm-0.2.1/espm/datasets/base.py
+-rw-r--r--   0 nati       (501) staff       (20)     5756 2023-04-21 08:05:20.000000 espm-0.2.1/espm/datasets/built_in_EDXS_datasets.py
+-rw-r--r--   0 nati       (501) staff       (20)    19888 2023-04-20 14:51:57.000000 espm-0.2.1/espm/datasets/eds_spim.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.767538 espm-0.2.1/espm/datasets/toy-problem/
+-rw-r--r--   0 nati       (501) staff       (20)     4316 2023-02-21 16:38:50.000000 espm-0.2.1/espm/datasets/toy-problem/phase1.png
+-rw-r--r--   0 nati       (501) staff       (20)     6798 2023-02-21 16:38:50.000000 espm-0.2.1/espm/datasets/toy-problem/phase2.png
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.768492 espm-0.2.1/espm/estimators/
+-rw-r--r--   0 nati       (501) staff       (20)      529 2023-02-23 09:58:20.000000 espm-0.2.1/espm/estimators/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    19415 2023-02-23 13:48:32.000000 espm-0.2.1/espm/estimators/base.py
+-rw-r--r--   0 nati       (501) staff       (20)     6026 2023-02-23 09:58:20.000000 espm-0.2.1/espm/estimators/dicotomy.py
+-rw-r--r--   0 nati       (501) staff       (20)    10252 2023-02-23 14:37:13.000000 espm-0.2.1/espm/estimators/smooth_nmf.py
+-rw-r--r--   0 nati       (501) staff       (20)     5700 2023-02-23 09:58:20.000000 espm-0.2.1/espm/estimators/surrogates.py
+-rw-r--r--   0 nati       (501) staff       (20)    11222 2023-02-23 09:58:20.000000 espm-0.2.1/espm/estimators/updates.py
+-rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.1/espm/hyperspy_extension.yaml
+-rw-r--r--   0 nati       (501) staff       (20)    20639 2023-04-20 13:24:00.000000 espm-0.2.1/espm/measures.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.769298 espm-0.2.1/espm/models/
+-rw-r--r--   0 nati       (501) staff       (20)    13015 2023-04-20 12:35:31.000000 espm-0.2.1/espm/models/EDXS_function.py
+-rw-r--r--   0 nati       (501) staff       (20)      500 2023-04-20 12:35:31.000000 espm-0.2.1/espm/models/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    10090 2023-04-20 12:35:31.000000 espm-0.2.1/espm/models/absorption_edxs.py
+-rw-r--r--   0 nati       (501) staff       (20)     5682 2023-04-20 13:36:07.000000 espm-0.2.1/espm/models/base.py
+-rw-r--r--   0 nati       (501) staff       (20)    17112 2023-04-20 12:53:51.000000 espm-0.2.1/espm/models/edxs.py
+-rw-r--r--   0 nati       (501) staff       (20)     6598 2023-04-20 13:17:58.000000 espm-0.2.1/espm/models/generate_EDXS_phases.py
+-rw-r--r--   0 nati       (501) staff       (20)     3130 2023-02-23 09:58:20.000000 espm-0.2.1/espm/spectrum_fitting.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.771365 espm-0.2.1/espm/tables/
+-rw-r--r--   0 nati       (501) staff       (20)   299008 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/100keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)   288577 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/200keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)   282569 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/300keV_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)     6242 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/SDD_efficiency.txt
+-rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)   166571 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/default_xrays.json
+-rw-r--r--   0 nati       (501) staff       (20)    11811 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/periodic_table_number.json
+-rw-r--r--   0 nati       (501) staff       (20)    11616 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/periodic_table_symbols.json
+-rw-r--r--   0 nati       (501) staff       (20)      779 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tables/siegbahn_to_iupac.json
+-rw-r--r--   0 nati       (501) staff       (20)     7514 2023-04-20 12:53:51.000000 espm-0.2.1/espm/tables_utils.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.772620 espm-0.2.1/espm/tests/
+-rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-0.2.1/espm/tests/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)     4910 2023-04-18 07:43:05.000000 espm-0.2.1/espm/tests/test_EDXS.py
+-rw-r--r--   0 nati       (501) staff       (20)    11339 2023-04-18 07:43:05.000000 espm-0.2.1/espm/tests/test_datasets.py
+-rw-r--r--   0 nati       (501) staff       (20)     1073 2023-02-23 09:58:20.000000 espm-0.2.1/espm/tests/test_docstring.py
+-rw-r--r--   0 nati       (501) staff       (20)     9592 2023-04-20 14:57:35.000000 espm-0.2.1/espm/tests/test_estimators.py
+-rw-r--r--   0 nati       (501) staff       (20)     1263 2023-02-23 09:58:20.000000 espm-0.2.1/espm/tests/test_laplacian.py
+-rw-r--r--   0 nati       (501) staff       (20)     7634 2023-02-23 09:58:20.000000 espm-0.2.1/espm/tests/test_measures.py
+-rw-r--r--   0 nati       (501) staff       (20)    29130 2023-02-23 09:58:20.000000 espm-0.2.1/espm/tests/test_updates.py
+-rw-r--r--   0 nati       (501) staff       (20)     3652 2023-02-23 09:58:20.000000 espm-0.2.1/espm/tests/test_utils.py
+-rw-r--r--   0 nati       (501) staff       (20)    11669 2023-04-20 12:53:51.000000 espm-0.2.1/espm/utils.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.773036 espm-0.2.1/espm/weights/
+-rw-r--r--   0 nati       (501) staff       (20)      258 2023-04-20 12:53:51.000000 espm-0.2.1/espm/weights/__init__.py
+-rw-r--r--   0 nati       (501) staff       (20)    16957 2023-04-20 13:14:42.000000 espm-0.2.1/espm/weights/abundance.py
+-rw-r--r--   0 nati       (501) staff       (20)    11055 2023-04-20 12:53:51.000000 espm-0.2.1/espm/weights/generate_weights.py
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.766699 espm-0.2.1/espm.egg-info/
+-rw-r--r--   0 nati       (501) staff       (20)     2804 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/PKG-INFO
+-rw-r--r--   0 nati       (501) staff       (20)     2467 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/SOURCES.txt
+-rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/dependency_links.txt
+-rw-r--r--   0 nati       (501) staff       (20)       34 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/entry_points.txt
+-rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/not-zip-safe
+-rw-r--r--   0 nati       (501) staff       (20)      207 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/requires.txt
+-rw-r--r--   0 nati       (501) staff       (20)        5 2023-04-21 09:14:35.000000 espm-0.2.1/espm.egg-info/top_level.txt
+-rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-0.2.1/hyperspy_extension.yaml
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.775998 espm-0.2.1/notebooks/
+-rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-0.2.1/notebooks/VCA.py
+-rw-r--r--   0 nati       (501) staff       (20)     5381 2023-04-21 09:14:33.000000 espm-0.2.1/notebooks/api.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    17775 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/background_fit.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    13661 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/convergence-speed.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     8875 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/generate_data.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     3204 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/make-plots.ipynb
+drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 09:14:35.776150 espm-0.2.1/notebooks/old/
+-rw-r--r--   0 nati       (501) staff       (20)     6289 2022-02-25 16:24:57.000000 espm-0.2.1/notebooks/old/algo-with-negative-variable.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     6820 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/other_algorithms.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    17002 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/preprocess_dataset.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)     4531 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/select_spectrum.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    14791 2023-04-21 09:14:34.000000 espm-0.2.1/notebooks/simple-test-regularisation.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    31459 2023-04-21 09:14:35.000000 espm-0.2.1/notebooks/spectrum_fit.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-0.2.1/notebooks/sunsal.py
+-rw-r--r--   0 nati       (501) staff       (20)     7554 2023-04-21 09:14:35.000000 espm-0.2.1/notebooks/surrogate-vs-bregmann.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)    18737 2023-04-21 09:14:35.000000 espm-0.2.1/notebooks/toy-ML.ipynb
+-rw-r--r--   0 nati       (501) staff       (20)      178 2022-12-06 17:40:13.000000 espm-0.2.1/readthedoc.yml
+-rw-r--r--   0 nati       (501) staff       (20)       38 2023-04-21 09:14:35.776869 espm-0.2.1/setup.cfg
+-rw-r--r--   0 nati       (501) staff       (20)     1800 2023-04-21 09:13:09.000000 espm-0.2.1/setup.py
+-rw-r--r--   0 nati       (501) staff       (20)     1120 2023-04-20 13:27:14.000000 espm-0.2.1/todo.md
```

### Comparing `espm-0.2.0/.github/workflows/python.yml` & `espm-0.2.1/.github/workflows/python.yml`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
     #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
     #     flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
       run: |
-        pytest espm
+        make test
```

### Comparing `espm-0.2.0/CHANGELOG.rst` & `espm-0.2.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/CONTRIBUTING.rst` & `espm-0.2.1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
    GitHub and select the created tag. 
 #. Build the distribution with ``make dist`` and check that the
    ``dist/espm-0.2.0.tar.gz`` source archive contains all required files. The
    binary wheel should be found as ``dist/espm-0.2.0.py3-none-any.whl``.
 #. Test the upload and installation process::
 
     $ twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-    $ pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple emspy
+    $ pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple espm
 
 #. Build and upload the distribution to the real PyPI with ``make release``.
 
 
 Repository organization
 -----------------------
```

### Comparing `espm-0.2.0/Licence.txt` & `espm-0.2.1/Licence.txt`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/PKG-INFO` & `espm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Electron SPectro-Microscopy Python Library
 Home-page: https://github.com/adriente/espm
 Author: Adrien Teurtie, Nathanael Perraudin
 Author-email: nathanael.perraudin@sdsc.ethz.ch
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `espm-0.2.0/README.rst` & `espm-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/doc/conf.py` & `espm-0.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/doc/introduction/index.rst` & `espm-0.2.1/doc/introduction/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,33 +42,32 @@
 >>> ds.generate_built_in_datasets(base_path="generated_samples", seeds_range=1)
 
 Here the object `spim` is of the :class:`hyperspy._signals.signal1d.Signal1D`.
 This object has different useful attributes and methods. For example, 
 @ADRIEN --- summarize here some of them
 
 .. note::
-    Please see the review article :cite:p:`teurtrie2023espm`. 
-    `espm : a Python library for the simulation of STEM-EDXS datasets` for an overview of
+    Please see the review article `espm : a Python library for the simulation 
+    of STEM-EDXS datasets` for an overview of
     the simulation methods this package leverages.
 
+
 Factorization
 -------------
 
 Taking the non-negative matrix factorization (NMF) is done with the following:
 
 .. plot::
     :context: close-figs
     
     >>> out = spim.decomposition(3)
     >>> spim.plot_decomposition_loadings(3)
     >>> spim.plot_decomposition_factors(3)
 
-It will use the algorithms developped in this `contribution`_.
-
-.. _contribution: https://link-to-the-paper.com
+BIt will use the algorithms developped in a coming contribution.
 
 These algorithms are an important part of this package. They are specialized to solve regularized Poisson NMF problems. Mathematically, they can be expressed as:
 
 .. math::
     
     \dot{W}, \dot{H} = \arg\min_{W\geq\epsilon, H\geq\epsilon, \sum_i H_{ij}  = 1} D_{GKL}(X || GWH) + \lambda tr ( H^\top \Delta H) + \mu \sum_{i,j} (\log H_{ij} +  \epsilon_{reg})$$
```

### Comparing `espm-0.2.0/espm/conf.py` & `espm-0.2.1/espm/conf.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/datasets/__init__.py` & `espm-0.2.1/espm/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/datasets/base.py` & `espm-0.2.1/espm/datasets/base.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/datasets/built_in_EDXS_datasets.py` & `espm-0.2.1/espm/datasets/built_in_EDXS_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
   'data_folder': 'built_in_grain_boundary',
   'shape_2d': [100, 400],
   'model': 'EDXS',
   'densities': [1, 1]
 }
 
 
-def generate_built_in_datasets (seeds_range = 2) : 
+def generate_built_in_datasets (seeds_range = 10) : 
     r"""
     Generate the two built-in datasets if they are not already present in the datasets folder.
 
     Parameters
     ----------
     seeds_range : int
         The number of seeds to use for the generation of the built-in datasets. The built-in datasets are generated with a base_seed, and then the base_seed + 1, base_seed + 2, etc. up to base_seed + seeds_range -1.
@@ -114,33 +114,32 @@
     """
     if not(os.path.isdir(DATASETS_PATH / Path(particles_misc_dict["data_folder"]))) : 
         print("Generating 2 particles + one matrix built-in dataset. This will take a minute.")
         particle_phases = generate_modular_phases(**particles_phases_dict)
         particles_weights = generate_weights("sphere", particles_misc_dict['shape_2d'], n_phases=3, seed=particles_misc_dict['seed'], radius = 15)
         particles_elements = elts_list_from_dict_list(particles_phases_dict['elts_dicts'])
         generate_dataset(base_seed=particles_misc_dict['seed'],
-                         sample_number=10,
+                         sample_number=seeds_range,
                          model_params = particles_phases_dict['model_params'],
                          misc_params = particles_misc_dict,
                          phases = particle_phases,
                          weights = particles_weights,
                          elements = particles_elements)
     if not(os.path.isdir(DATASETS_PATH / Path(boundary_misc_dict["data_folder"]))) :
         print("Generating a grain boundary with Sr segregation. This will take a minute.")
         boundary_phases = generate_modular_phases(**boundary_phases_dict)
         boundary_weights = generate_weights("gaussian_ripple", boundary_misc_dict['shape_2d'], n_phases=2, seed=boundary_misc_dict['seed'], width = 10)
         boundary_elements = elts_list_from_dict_list(boundary_phases_dict['elts_dicts'])
         generate_dataset(base_seed=boundary_misc_dict['seed'],
-                         sample_number=10,
+                         sample_number=seeds_range,
                          model_params = boundary_phases_dict['model_params'],
                          misc_params = boundary_misc_dict,
                          phases = boundary_phases,
                          weights = boundary_weights,
                          elements = boundary_elements)
-
 def load_particules (sample = 0) : 
     r"""
     Load the built-in dataset of particles.
 
     Parameters
     ----------
     sample : int
```

### Comparing `espm-0.2.0/espm/datasets/eds_spim.py` & `espm-0.2.1/espm/datasets/eds_spim.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,14 +215,18 @@
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope = width_slope
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept = width_intercept
         self.metadata.xray_db = xray_db
 
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle = take_off_angle(tilt_stage,azimuth_angle,elevation_angle)
 
     def set_additional_parameters(self,thickness = 200e-7, density = 3.5,  detector_type = "SDD_efficiency.txt", width_slope = 0.01, width_intercept = 0.065, xray_db = "default_xrays.json") : 
+        r"""
+        Helper function to set the metadata that are specific to the :mod:`espm` package so that it does not overwrite experimental metadata.
+        See the documentation of the :func:`set_analysis_parameters` function for the meaning of the parameters.
+        """
         self.metadata.Sample.thickness = thickness
         self.metadata.Sample.density = density
         try : 
             del self.metadata.Acquisition_instrument.TEM.Detector.EDS.type
         except AttributeError : 
             pass
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.type = detector_type
@@ -233,33 +237,58 @@
         tilt_stage = self.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha
         azimuth_angle = self.metadata.Acquisition_instrument.TEM.Detector.EDS.azimuth_angle
         elevation_angle = self.metadata.Acquisition_instrument.TEM.Detector.EDS.elevation_angle
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle = take_off_angle(tilt_stage,azimuth_angle,elevation_angle)
 
     @number_to_symbol_list
     def add_elements(self, *, elements = []) :
+        r"""
+        Add elements to the existing list of elements in the metadata.
+
+        Parameters
+        ----------
+        elements : list, optional
+            List of the elements to be added to the existing list of elements in the metadata. They have to be chemical symbols (e.g. ['Si','Fe', 'O']).
+        """
         try : 
             self.metadata.Sample.elements = elements
         except AttributeError :
             self.metadata.Sample = {}
             self.metadata.Sample.elements = elements
 
     def set_microscope_parameters(self, beam_energy = 200, azimuth_angle = 0.0, elevation_angle = 22.0,tilt_stage = 0.0) : 
+        r"""
+        Helper function to set the microscope parameters of the :class:`EDS_espm` object. Be careful, it will overwrite the microscope parameters of the object.
+        See the documentation of the :func:`set_analysis_parameters` function for the meaning of the parameters.
+        """
         self.metadata.Acquisition_instrument = {}
         self.metadata.Acquisition_instrument.TEM = {}
         self.metadata.Acquisition_instrument.TEM.Stage = {}
         self.metadata.Acquisition_instrument.TEM.Detector = {}
         self.metadata.Acquisition_instrument.TEM.Detector.EDS = {}
         self.metadata.Acquisition_instrument.TEM.beam_energy = beam_energy
         self.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha = tilt_stage
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.azimuth_angle = azimuth_angle
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.elevation_angle = elevation_angle
         self.metadata.Acquisition_instrument.TEM.Detector.EDS.energy_resolution_MnKa = 130.0
 
     def set_fixed_W (self,phases_dict) : 
+        r"""
+        Helper function to create a fixed_W matrix. The output matrix will have -1 entries except for the elements (and bremsstrahlung parameters) that are present in the phases_dict dictionary.
+        In the output (fixed_W) matrix, the -1 entries will be ignored during the decomposition using :class:`espm.estimator.NMFEstimator` are normally learned while the non-negative entries will be fixed to the values given in the phases_dict dictionary.
+        Usually, the easiest is to fix some elements to 0.0 in some phases if you want to improve unmixing results. For example, if you have a phase with only Si and O, you can fix the Fe element to 0.0 in this phase.
+
+        Parameters
+        ----------
+        phases_dict : dict
+            Determines which elements of fixed_W are going to be non-negative. The dictionnary has typically the following structure : phases_dict = {"phase1_name" : {"Fe" : 0.0, "O" : 1.25e23}, "phase2_name" : {"Si" : 0.0, "b0" : 0.05}}.
+        Returns
+        -------
+        W : numpy.ndarray
+        """
         elements = self.metadata.Sample.elements
         if self.problem_type == "no_brstlg" : 
             W = -1* np.ones((len(elements), len(phases_dict.keys())))
         elif self.problem_type == "bremsstrahlung" : 
             W = -1* np.ones((len(elements)+2, len(phases_dict.keys())))
         else : 
             raise ValueError("problem type should be either no_brstlg or bremsstrahlung")
@@ -344,14 +373,17 @@
 
 
 ######################
 # Axiliary functions #
 ######################
 
 def get_metadata(spim) : 
+    r"""
+    Get the metadata of the :class:`EDS_espm` object and format it as a model parameters dictionary.
+    """
     mod_pars = {}
     try :
         mod_pars["E0"] = spim.metadata.Acquisition_instrument.TEM.beam_energy
         mod_pars["e_offset"] = spim.axes_manager[-1].offset
         assert mod_pars["e_offset"] > 0.01, "The energy scale can't include 0, it will produce errors elsewhere. Please crop your data."
         mod_pars["e_scale"] = spim.axes_manager[-1].scale
         mod_pars["e_size"] = spim.axes_manager[-1].size
```

### Comparing `espm-0.2.0/espm/datasets/toy-problem/phase1.png` & `espm-0.2.1/espm/datasets/toy-problem/phase1.png`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/datasets/toy-problem/phase2.png` & `espm-0.2.1/espm/datasets/toy-problem/phase2.png`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/__init__.py` & `espm-0.2.1/espm/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/base.py` & `espm-0.2.1/espm/estimators/base.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/dicotomy.py` & `espm-0.2.1/espm/estimators/dicotomy.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/smooth_nmf.py` & `espm-0.2.1/espm/estimators/smooth_nmf.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/surrogates.py` & `espm-0.2.1/espm/estimators/surrogates.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/estimators/updates.py` & `espm-0.2.1/espm/estimators/updates.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/measures.py` & `espm-0.2.1/espm/measures.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/models/EDXS_function.py` & `espm-0.2.1/espm/models/EDXS_function.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/models/absorption_edxs.py` & `espm-0.2.1/espm/models/absorption_edxs.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/models/base.py` & `espm-0.2.1/espm/models/base.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/models/edxs.py` & `espm-0.2.1/espm/models/edxs.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/models/generate_EDXS_phases.py` & `espm-0.2.1/espm/models/generate_EDXS_phases.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/spectrum_fitting.py` & `espm-0.2.1/espm/spectrum_fitting.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/100keV_xrays.json` & `espm-0.2.1/espm/tables/100keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/200keV_xrays.json` & `espm-0.2.1/espm/tables/200keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/300keV_xrays.json` & `espm-0.2.1/espm/tables/300keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/SDD_efficiency.txt` & `espm-0.2.1/espm/tables/SDD_efficiency.txt`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/default_xrays.json` & `espm-0.2.1/espm/tables/default_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/periodic_table_number.json` & `espm-0.2.1/espm/tables/periodic_table_number.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/periodic_table_symbols.json` & `espm-0.2.1/espm/tables/periodic_table_symbols.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables/siegbahn_to_iupac.json` & `espm-0.2.1/espm/tables/siegbahn_to_iupac.json`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tables_utils.py` & `espm-0.2.1/espm/tables_utils.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_EDXS.py` & `espm-0.2.1/espm/tests/test_EDXS.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_datasets.py` & `espm-0.2.1/espm/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_docstring.py` & `espm-0.2.1/espm/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_estimators.py` & `espm-0.2.1/espm/tests/test_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     estimator.fit_transform(X=X)
     P3, A3 = estimator.W_, estimator.H_ 
     np.testing.assert_allclose(G @ P3 @ A3,  Xdot, atol=1)
     L = create_laplacian_matrix(10, 20)
 
     assert(trace_xtLx(L, A3.T) < trace_xtLx(L, A2.T))
     # assert(trace_xtLx(L, A.T) < trace_xtLx(L, A2.T) )
-    assert(trace_xtLx(L, A3.T) < trace_xtLx(L, H.T) )
+    assert(trace_xtLx(L, A3.T) < trace_xtLx(L, H.T)*1.01 )
 
 def test_fixed_mat () :
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
     fW, fH = gen_fixed_mat()
     estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True, fixed_W = fW, hspy_comp = False)
     estimator.fit_transform(X=X)
     P2, A2 = estimator.W_, estimator.H_
```

### Comparing `espm-0.2.0/espm/tests/test_laplacian.py` & `espm-0.2.1/espm/tests/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_measures.py` & `espm-0.2.1/espm/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_updates.py` & `espm-0.2.1/espm/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/tests/test_utils.py` & `espm-0.2.1/espm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/utils.py` & `espm-0.2.1/espm/utils.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/weights/abundance.py` & `espm-0.2.1/espm/weights/abundance.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm/weights/generate_weights.py` & `espm-0.2.1/espm/weights/generate_weights.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/espm.egg-info/PKG-INFO` & `espm-0.2.1/espm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Electron SPectro-Microscopy Python Library
 Home-page: https://github.com/adriente/espm
 Author: Adrien Teurtie, Nathanael Perraudin
 Author-email: nathanael.perraudin@sdsc.ethz.ch
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `espm-0.2.0/espm.egg-info/SOURCES.txt` & `espm-0.2.1/espm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Licence.txt
 MANIFEST.in
 README.rst
 hyperspy_extension.yaml
 readthedoc.yml
 setup.py
 todo.md
+.github/workflows/doc.yml
 .github/workflows/python.yml
 doc/changelog.rst
 doc/conf.py
 doc/contributing.rst
 doc/index.rst
 doc/references.rst
 doc/introduction/index.rst
```

### Comparing `espm-0.2.0/notebooks/VCA.py` & `espm-0.2.1/notebooks/VCA.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/api.ipynb` & `espm-0.2.1/notebooks/api.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/background_fit.ipynb` & `espm-0.2.1/notebooks/background_fit.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/convergence-speed.ipynb` & `espm-0.2.1/notebooks/convergence-speed.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/generate_data.ipynb` & `espm-0.2.1/notebooks/generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/make-plots.ipynb` & `espm-0.2.1/notebooks/make-plots.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/old/algo-with-negative-variable.ipynb` & `espm-0.2.1/notebooks/old/algo-with-negative-variable.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/other_algorithms.ipynb` & `espm-0.2.1/notebooks/other_algorithms.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/preprocess_dataset.ipynb` & `espm-0.2.1/notebooks/preprocess_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/select_spectrum.ipynb` & `espm-0.2.1/notebooks/select_spectrum.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/simple-test-regularisation.ipynb` & `espm-0.2.1/notebooks/simple-test-regularisation.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/spectrum_fit.ipynb` & `espm-0.2.1/notebooks/spectrum_fit.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/sunsal.py` & `espm-0.2.1/notebooks/sunsal.py`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/surrogate-vs-bregmann.ipynb` & `espm-0.2.1/notebooks/surrogate-vs-bregmann.ipynb`

 * *Files identical despite different names*

### Comparing `espm-0.2.0/notebooks/toy-ML.ipynb` & `espm-0.2.1/notebooks/toy-ML.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996511627906977%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(1, 'seed = 42 # for reproducibility\\n')], delete: [1]}}, "*

 * *            "22: {'source': ['lambda_L = 2 # Smoothness of the maps\\n', 'mu = 0.05 # Sparsity of "*

 * *            "the maps']}}"}*

```diff
@@ -99,15 +99,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "seed = 0 # for reproducibility\n",
+                "seed = 42 # for reproducibility\n",
                 "\n",
                 "m = 15 # Number of components\n",
                 "n = 200 # Length of the phases\n",
                 "\n",
                 "n_poisson = 300 # Average poisson number per pixel (this number will be splitted on the m dimension)\n",
                 "\n",
                 "densities = np.random.uniform(0.1, 2.0, 3) # Random densities\n"
@@ -300,16 +300,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lambda_L = 1 # Smoothness of the maps\n",
-                "mu = 0.2 # Sparsity of the maps"
+                "lambda_L = 2 # Smoothness of the maps\n",
+                "mu = 0.05 # Sparsity of the maps"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `espm-0.2.0/setup.py` & `espm-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='espm',
-    version='0.2.0',
+    version='0.2.1',
     description='Electron SPectro-Microscopy Python Library',
     url='https://github.com/adriente/espm',
     author='Adrien Teurtie, Nathanael Perraudin',
     author_email='nathanael.perraudin@sdsc.ethz.ch',
     license='MIT',
     packages=setuptools.find_packages(),
     zip_safe=False,
```

### Comparing `espm-0.2.0/todo.md` & `espm-0.2.1/todo.md`

 * *Files identical despite different names*

