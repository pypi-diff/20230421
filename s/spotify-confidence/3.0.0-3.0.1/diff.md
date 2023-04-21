# Comparing `tmp/spotify-confidence-3.0.0.tar.gz` & `tmp/spotify-confidence-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/confidence/confidence/dist/.tmp-6ji0f166/spotify-confidence-3.0.0.tar", last modified: Wed Apr  5 15:36:50 2023, max compression
+gzip compressed data, was "/home/runner/work/confidence/confidence/dist/.tmp-at_5yb94/spotify-confidence-3.0.1.tar", last modified: Fri Apr 21 12:14:39 2023, max compression
```

## Comparing `spotify-confidence-3.0.0.tar` & `spotify-confidence-3.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/bayesian_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/bayesian_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/confidence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24538 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/chartify_grapher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/chi_squared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/multiple_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/nims_and_mdes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sample_ratio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sample_size_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sequential_bound_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/t_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/z_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/z_test_linreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/chartgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence/samplesize/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/samplesize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33000 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/spotify_confidence/samplesize/sample_size_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/spotify_confidence.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/bayesian/test_betabinomial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/frequentist/
--rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_chisquared.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_freqsamplesizecalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    34292 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)   132810 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_ztest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/frequentist/test_ztest_linreg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/outputs/precision/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/outputs/precision/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:36:50.000000 spotify-confidence-3.0.0/tests/samplesize/
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/samplesize/test_samplesizecalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-05 15:36:39.000000 spotify-confidence-3.0.0/tests/test_plot_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/confidence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chartify_grapher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chi_squared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/multiple_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/nims_and_mdes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_ratio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_size_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sequential_bound_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/t_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/chartgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33000 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/sample_size_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/bayesian/test_betabinomial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/frequentist/
+-rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_chisquared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_freqsamplesizecalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34292 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132810 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ztest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ztest_linreg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/outputs/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/outputs/precision/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/samplesize/
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/samplesize/test_samplesizecalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/test_plot_precision.py
```

### Comparing `spotify-confidence-3.0.0/LICENSE` & `spotify-confidence-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/PKG-INFO` & `spotify-confidence-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-confidence
-Version: 3.0.0
+Version: 3.0.1
 Summary: Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 Home-page: https://github.com/spotify/confidence
 Author: Per Sillren
 Author-email: pers@spotify.com
 Project-URL: Bug Tracker, https://github.com/spotify/confidence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,19 +14,19 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.0-green.svg "Latest release: 3.0.0")
-![Python](https://img.shields.io/badge/Python-3.6-blue.svg "Python")
+![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
+![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
 Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls.
```

### Comparing `spotify-confidence-3.0.0/README.md` & `spotify-confidence-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.0-green.svg "Latest release: 3.0.0")
-![Python](https://img.shields.io/badge/Python-3.6-blue.svg "Python")
+![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
+![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
 Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls.
```

### Comparing `spotify-confidence-3.0.0/setup.cfg` & `spotify-confidence-3.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spotify-confidence
-version = 3.0.0
+version = 3.0.1
 author = Per Sillren
 author_email = pers@spotify.com
 description = Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spotify/confidence
 project_urls = 
@@ -20,15 +20,15 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	numpy>=1.20.0,<2.0.0
 	scipy>=1.6.0,<1.8.0
 	pandas>=1.2.0,<2.0.0
 	statsmodels>=0.13.0,<1.0.0
-	chartify>=4.0.2
+	chartify>=4.0.3
 	ipywidgets>=8.0.0
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build =
```

### Comparing `spotify-confidence-3.0.0/spotify_confidence/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/bayesian_base.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_base.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/bayesian/bayesian_models.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_models.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/confidence_utils.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/confidence_utils.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/constants.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/constants.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/chartify_grapher.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chartify_grapher.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,27 @@
     listify,
     level2str,
     to_finite,
     de_list_if_length_one,
 )
 from ..constants import (
     POINT_ESTIMATE,
+    ORIGINAL_POINT_ESTIMATE,
     DIFFERENCE,
     CI_LOWER,
     CI_UPPER,
     P_VALUE,
     ADJUSTED_LOWER,
     ADJUSTED_UPPER,
     ADJUSTED_P,
     NULL_HYPOTHESIS,
     NIM,
     NIM_TYPE,
     PREFERENCE,
+    SFX1,
 )
 from ...chartgrid import ChartGrid
 
 
 class ChartifyGrapher(ConfidenceGrapherABC):
     def __init__(
         self,
@@ -180,15 +182,15 @@
         else:
             title = "Change from {} to {}".format(
                 difference_df["level_1"].values[0], difference_df["level_2"].values[0]
             )
 
         y_axis_label = self._get_difference_plot_label(absolute)
         ch = self._ordinal_plot(
-            "difference",
+            DIFFERENCE,
             difference_df,
             groupby=None,
             level_name="",
             remaining_groups=remaining_groups,
             absolute=absolute,
             title=title,
             y_axis_label=y_axis_label,
@@ -377,14 +379,16 @@
         ch = Chart(x_axis_type=self._ordinal_type())
         ch.plot.line(
             data_frame=df.sort_values(self._ordinal_group_column),
             x_column=self._ordinal_group_column,
             y_column=center_name,
             color_column=colors,
         )
+        # Also plot transparent circles, just to be able to show hover box
+        ch.figure.line(source=df, x=self._ordinal_group_column, y=center_name, name="center", line_alpha=0)
         ch.style.color_palette.reset_palette_order()
         ch.plot.area(
             data_frame=(
                 df.assign(**{LOWER: to_finite(df[LOWER], y_min, y_max)})
                 .assign(**{UPPER: to_finite(df[UPPER], y_min, y_max)})
                 .sort_values(self._ordinal_group_column)
             ),
@@ -399,14 +403,23 @@
                 data_frame=df.sort_values(self._ordinal_group_column),
                 x_column=self._ordinal_group_column,
                 y_column=NULL_HYPOTHESIS,
                 color_column=colors,
                 line_dash="dashed",
                 line_width=1,
             )
+            # Also plot named transparent line, just to be able to show hover box
+            ch.figure.line(
+                source=df.sort_values(self._ordinal_group_column),
+                x=self._ordinal_group_column,
+                y=NULL_HYPOTHESIS,
+                line_width=3,
+                line_alpha=0,
+                name="nim",
+            )
         ch.axes.set_yaxis_label(y_axis_label)
         ch.axes.set_xaxis_label(self._ordinal_group_column)
         ch.set_source_label("")
         ch.axes.set_yaxis_range(y_min - 0.05 * (y_max - y_min), y_max + 0.05 * (y_max - y_min))
         ch.axes.set_yaxis_tick_format(axis_format)
         subtitle = "" if not groupby else "{}: {}".format(groupby, level_name)
         ch.set_subtitle(subtitle)
@@ -549,17 +562,19 @@
             if center_name in data.keys() or NULL_HYPOTHESIS in data.keys():
                 index = data["index"]
                 data[LOWER] = np.array(df[LOWER][index])
                 data[UPPER] = np.array(df[UPPER][index])
                 data["color"] = np.array(df[group_col][index])
             if DIFFERENCE in data.keys() or NULL_HYPOTHESIS in data.keys():
                 index = data["index"]
+                data["reference_level"] = np.array(df["level_1"][index])
                 data[DIFFERENCE] = np.array(df[DIFFERENCE][index])
                 data["p_value"] = np.array(df[P_VALUE][index])
                 data["adjusted_p"] = np.array(df[ADJUSTED_P][index])
+                data["reference_level_avg"] = np.array(df[ORIGINAL_POINT_ESTIMATE + SFX1][index])
                 if NULL_HYPOTHESIS in df.columns:
                     data["null_hyp"] = np.array(df[NULL_HYPOTHESIS][index])
 
     def add_tools(
         self,
         chart: Chart,
         df: DataFrame,
@@ -576,38 +591,51 @@
         axis_format, y_min, y_max = axis_format_precision(
             numbers=concat(
                 [df[LOWER], df[center_name], df[UPPER], df[NULL_HYPOTHESIS] if NULL_HYPOTHESIS in df.columns else None]
             ),
             absolute=absolute,
             extra_zeros=2,
         )
+        axis_format_reference_level, _, _ = axis_format_precision(
+            numbers=concat(
+                [df[LOWER], df[center_name], df[UPPER], df[NULL_HYPOTHESIS] if NULL_HYPOTHESIS in df.columns else None]
+            ),
+            absolute=True,
+            extra_zeros=2,
+        )
         ordinal_tool_tip = [] if not ordinal else [(self._ordinal_group_column, f"@{self._ordinal_group_column}")]
         p_value_tool_tip = (
             (
                 [("p-value", "@p_value{0.0000}")]
                 + ([("adjusted p-value", "@adjusted_p{0.0000}")] if len(df) > 1 else [])
             )
             if center_name == DIFFERENCE
             else []
         )
         nim_tool_tip = [("null hypothesis", f"@null_hyp{{{axis_format}}}")] if NULL_HYPOTHESIS in df.columns else []
+        reference_level_tool_tip = (
+            [("reference level", f"@reference_level: @reference_level_avg{{{axis_format_reference_level}}}")]
+            if "level_1" in df.columns
+            else []
+        )
         tooltips = (
             [("group", "@color")]
+            + reference_level_tool_tip
             + ordinal_tool_tip
             + [(f"{center_name}", f"@{center_name}{{{axis_format}}}")]
             + [
                 (
                     ("adjusted " if use_adjusted_intervals else "") + "confidence interval",
                     f"(@{{{LOWER}}}{{{axis_format}}}," f" @{{{UPPER}}}{{{axis_format}}})",
                 )
             ]
             + p_value_tool_tip
             + nim_tool_tip
         )
-        lines_with_hover = [] if ordinal else ["center", "nim"]
+        lines_with_hover = ["center", "nim"]
         renderers = [r for r in chart.figure.renderers if r.name in lines_with_hover]
         hover = tools.HoverTool(tooltips=tooltips, renderers=renderers)
 
         box_zoom = tools.BoxZoomTool()
 
         chart.figure.add_tools(
             hover, tools.ZoomInTool(), tools.ZoomOutTool(), box_zoom, tools.PanTool(), tools.ResetTool()
```

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/chi_squared.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chi_squared.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/experiment.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         difference_df = self.difference(
             level_1=level_1,
             level_2=level_2,
             absolute=absolute,
             groupby=groupby,
             non_inferiority_margins=non_inferiority_margins,
             final_expected_sample_size_column=final_expected_sample_size_column,
+            verbose=True,
         )
         chartgrid = self._confidence_grapher.plot_difference(
             difference_df, absolute, groupby, non_inferiority_margins, use_adjusted_intervals, split_plot_by_groups
         )
         return chartgrid
 
     def differences_plot(
@@ -213,15 +214,15 @@
         groupby: Union[str, Iterable] = None,
         non_inferiority_margins: NIM_TYPE = None,
         use_adjusted_intervals: bool = False,
         final_expected_sample_size_column: str = None,
         split_plot_by_groups: bool = False,
     ) -> ChartGrid:
         difference_df = self.differences(
-            levels, absolute, groupby, non_inferiority_margins, final_expected_sample_size_column
+            levels, absolute, groupby, non_inferiority_margins, final_expected_sample_size_column, verbose=True
         )
         chartgrid = self._confidence_grapher.plot_differences(
             difference_df, absolute, groupby, non_inferiority_margins, use_adjusted_intervals, split_plot_by_groups
         )
         return chartgrid
 
     def multiple_difference_plot(
@@ -238,14 +239,15 @@
         difference_df = self.multiple_difference(
             level=level,
             absolute=absolute,
             groupby=groupby,
             level_as_reference=level_as_reference,
             non_inferiority_margins=non_inferiority_margins,
             final_expected_sample_size_column=final_expected_sample_size_column,
+            verbose=True,
         )
         chartgrid = self._confidence_grapher.plot_multiple_difference(
             difference_df,
             absolute,
             groupby,
             level_as_reference,
             non_inferiority_margins,
```

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/multiple_comparison.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/multiple_comparison.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/nims_and_mdes.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/nims_and_mdes.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sample_ratio_test.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_ratio_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sample_size_calculator.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_size_calculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/sequential_bound_solver.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sequential_bound_solver.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/t_test.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/t_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/z_test.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/analysis/frequentist/z_test_linreg.py` & `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test_linreg.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/chartgrid.py` & `spotify-confidence-3.0.1/spotify_confidence/chartgrid.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/examples.py` & `spotify-confidence-3.0.1/spotify_confidence/examples.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/options.py` & `spotify-confidence-3.0.1/spotify_confidence/options.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/samplesize/__init__.py` & `spotify-confidence-3.0.1/spotify_confidence/samplesize/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence/samplesize/sample_size_calculator.py` & `spotify-confidence-3.0.1/spotify_confidence/samplesize/sample_size_calculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/spotify_confidence.egg-info/PKG-INFO` & `spotify-confidence-3.0.1/spotify_confidence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-confidence
-Version: 3.0.0
+Version: 3.0.1
 Summary: Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 Home-page: https://github.com/spotify/confidence
 Author: Per Sillren
 Author-email: pers@spotify.com
 Project-URL: Bug Tracker, https://github.com/spotify/confidence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,19 +14,19 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.0-green.svg "Latest release: 3.0.0")
-![Python](https://img.shields.io/badge/Python-3.6-blue.svg "Python")
+![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
+![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
 Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls.
```

### Comparing `spotify-confidence-3.0.0/spotify_confidence.egg-info/SOURCES.txt` & `spotify-confidence-3.0.1/spotify_confidence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/bayesian/test_betabinomial.py` & `spotify-confidence-3.0.1/tests/bayesian/test_betabinomial.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_bounds.py` & `spotify-confidence-3.0.1/tests/frequentist/test_bounds.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_chisquared.py` & `spotify-confidence-3.0.1/tests/frequentist/test_chisquared.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_experiment.py` & `spotify-confidence-3.0.1/tests/frequentist/test_experiment.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_freqsamplesizecalculator.py` & `spotify-confidence-3.0.1/tests/frequentist/test_freqsamplesizecalculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_ttest.py` & `spotify-confidence-3.0.1/tests/frequentist/test_ttest.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_ztest.py` & `spotify-confidence-3.0.1/tests/frequentist/test_ztest.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/frequentist/test_ztest_linreg.py` & `spotify-confidence-3.0.1/tests/frequentist/test_ztest_linreg.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/samplesize/test_samplesizecalculator.py` & `spotify-confidence-3.0.1/tests/samplesize/test_samplesizecalculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.0/tests/test_plot_precision.py` & `spotify-confidence-3.0.1/tests/test_plot_precision.py`

 * *Files identical despite different names*

