# Comparing `tmp/pyqt-autotest-0.2.0.tar.gz` & `tmp/pyqt-autotest-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\rober\OneDrive\Documents\Visual Studio Projects\pyqt-autotest\dist\tmpu982n986\pyqt-autotest-0.2.0.tar", last modified: Sun Nov 13 15:40:46 2022, max compression
+gzip compressed data, was "pyqt-autotest-0.2.1.tar", last modified: Fri Apr 21 18:05:30 2023, max compression
```

## Comparing `pyqt-autotest-0.2.0.tar` & `pyqt-autotest-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.996054 pyqt-autotest-0.2.0/
--rw-rw-rw-   0        0        0    35823 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      270 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    51043 2022-11-13 15:40:46.996054 pyqt-autotest-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9131 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/README.md
--rw-rw-rw-   0        0        0      909 2022-11-13 15:39:40.000000 pyqt-autotest-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.933553 pyqt-autotest-0.2.0/pyqt_autotest/
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.964805 pyqt-autotest-0.2.0/pyqt_autotest/cli/
--rw-rw-rw-   0        0        0     3173 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/config.py
--rw-rw-rw-   0        0        0     2524 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/list_tests.py
--rw-rw-rw-   0        0        0     3952 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/main.py
--rw-rw-rw-   0        0        0     3585 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/modules.py
--rw-rw-rw-   0        0        0     5841 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/options.py
--rw-rw-rw-   0        0        0     2989 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/cli/run_tests.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.964805 pyqt-autotest-0.2.0/pyqt_autotest/core/
--rw-rw-rw-   0        0        0      407 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/core/action.py
--rw-rw-rw-   0        0        0     5966 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/core/auto_test.py
--rw-rw-rw-   0        0        0     1834 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/core/exception_handler.py
--rw-rw-rw-   0        0        0     2260 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/core/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.917937 pyqt-autotest-0.2.0/pyqt_autotest/examples/
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.964805 pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/
--rw-rw-rw-   0        0        0      584 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/README.md
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/__init__.py
--rw-rw-rw-   0        0        0     1372 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/test.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.964805 pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/
--rw-rw-rw-   0        0        0      788 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/README.md
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/__init__.py
--rw-rw-rw-   0        0        0     1059 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/test.py
--rw-rw-rw-   0        0        0      213 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/three-body-parameters.txt
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.980429 pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/
--rw-rw-rw-   0        0        0      267 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/README.md
--rw-rw-rw-   0        0        0        0 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/__init__.py
--rw-rw-rw-   0        0        0      713 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/test.py
--rw-rw-rw-   0        0        0      849 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/usercode.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.980429 pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/
--rw-rw-rw-   0        0        0      269 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/README.md
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/__init__.py
--rw-rw-rw-   0        0        0      493 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/test.py
--rw-rw-rw-   0        0        0      849 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/usercode.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.980429 pyqt-autotest-0.2.0/pyqt_autotest/qt/
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/qt/__init__.py
--rw-rw-rw-   0        0        0      995 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/qt/application.py
--rw-rw-rw-   0        0        0     1021 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/qt/modal_unblocker.py
--rw-rw-rw-   0        0        0     1629 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/qt/top_level_widgets.py
--rw-rw-rw-   0        0        0     2082 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/qt/widgets.py
--rw-rw-rw-   0        0        0     1511 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/random_auto_test.py
--rw-rw-rw-   0        0        0     1517 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/repeatable_auto_test.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.996054 pyqt-autotest-0.2.0/pyqt_autotest/results/
--rw-rw-rw-   0        0        0      320 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/results/exit_state.py
--rw-rw-rw-   0        0        0     4630 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/results/json_results_dict.py
--rw-rw-rw-   0        0        0     1196 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/results/print_results.py
--rw-rw-rw-   0        0        0     1046 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/results/result_schema.py
--rw-rw-rw-   0        0        0      766 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/results/statistic_finder.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.996054 pyqt-autotest-0.2.0/pyqt_autotest/utilities/
--rw-rw-rw-   0        0        0        0 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/utilities/__init__.py
--rw-rw-rw-   0        0        0      332 2022-09-11 16:08:54.000000 pyqt-autotest-0.2.0/pyqt_autotest/utilities/print_colors.py
--rw-rw-rw-   0        0        0     1080 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/utilities/randomizer.py
--rw-rw-rw-   0        0        0      409 2022-08-28 16:37:30.000000 pyqt-autotest-0.2.0/pyqt_autotest/utilities/singleton.py
--rw-rw-rw-   0        0        0      739 2022-11-13 13:51:20.000000 pyqt-autotest-0.2.0/pyqt_autotest/utilities/verbosity_controller.py
-drwxrwxrwx   0        0        0        0 2022-11-13 15:40:46.949180 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/
--rw-rw-rw-   0        0        0    51043 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1893 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-11-13 15:40:46.000000 pyqt-autotest-0.2.0/pyqt_autotest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      151 2022-11-13 15:40:46.996054 pyqt-autotest-0.2.0/setup.cfg
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)    35149 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/LICENSE
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      265 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/MANIFEST.in
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)    50190 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/PKG-INFO
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     8968 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/README.md
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      883 2023-04-21 17:24:47.000000 pyqt-autotest-0.2.1/pyproject.toml
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/__init__.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/cli/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     3145 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/config.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     2473 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/list_tests.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     3716 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/main.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     3488 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/modules.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     5676 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/options.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     3098 2023-04-21 17:24:19.000000 pyqt-autotest-0.2.1/pyqt_autotest/cli/run_tests.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/core/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      395 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/core/action.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     5655 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/core/auto_test.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1785 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/core/exception_handler.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     2221 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/core/exceptions.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.981645 pyqt-autotest-0.2.1/pyqt_autotest/examples/
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      569 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/README.md
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1269 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/test.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      770 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/README.md
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1030 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/test.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      210 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/three-body-parameters.txt
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      260 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/README.md
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      695 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/test.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      820 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/usercode.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      262 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/README.md
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      478 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/test.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      820 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/usercode.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/pyqt_autotest/qt/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/qt/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      953 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/qt/application.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      993 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/qt/modal_unblocker.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1586 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/qt/top_level_widgets.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     2032 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/qt/widgets.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1476 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/random_auto_test.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1448 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/repeatable_auto_test.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/pyqt_autotest/results/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      309 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/results/exit_state.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     4479 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/results/json_results_dict.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1183 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/results/print_results.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1001 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/results/result_schema.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      829 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/results/statistic_finder.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/pyqt_autotest/utilities/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        0 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/utilities/__init__.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      324 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/utilities/print_colors.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1053 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/utilities/randomizer.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      400 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/utilities/singleton.py
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      716 2023-04-21 17:03:37.000000 pyqt-autotest-0.2.1/pyqt_autotest/utilities/verbosity_controller.py
+drwxrwxr-x   0 robapp    (1000) robapp    (1000)        0 2023-04-21 18:05:30.985645 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)    50190 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)     1893 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)        1 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)       57 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/entry_points.txt
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)       18 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/requires.txt
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)       14 2023-04-21 18:05:30.000000 pyqt-autotest-0.2.1/pyqt_autotest.egg-info/top_level.txt
+-rw-rw-r--   0 robapp    (1000) robapp    (1000)      140 2023-04-21 18:05:30.989645 pyqt-autotest-0.2.1/setup.cfg
```

### Comparing `pyqt-autotest-0.2.0/LICENSE` & `pyqt-autotest-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pyqt-autotest-0.2.0/PKG-INFO` & `pyqt-autotest-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,836 +1,836 @@
-Metadata-Version: 2.1
-Name: pyqt-autotest
-Version: 0.2.0
-Summary: A command line tool for finding system-level bugs that cause a python Qt application to terminate.
-Author-email: Robert Applin <robertapplin.developer@gmail.com>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://github.com/robertapplin/pyqt-autotest
-Project-URL: Bug Tracker, https://github.com/robertapplin/pyqt-autotest/issues
-Keywords: python,qt,random,auto,test
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyqt-autotest ⚙️🧪
-A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
-
-This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
-
-## Table of contents
-* [Installation](#installation)
-* [Setup](#setup)
-* [Options](#options)
-* [Test class](#test-class)
-* [Built-in Actions](#built-in-actions)
-* [Creating your own Actions](#creating-your-own-actions)
-* [Usage](#usage)
-* [Output](#output)
-
-## Installation
-
-This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
-
-```sh
-pip install pyqt-autotest
-```
-
-## Setup
-
-Create a file named `.autotest` in your home directory with the following contents.
-
-```
-[setup]
-search_directories = /path/to/test/directory1/
-                     /path/to/test/directory2/
-output_directory = /path/to/output/directory/
-```
-
-The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
-
-## Options
-
-The following table details the options that can be provided on the command line.
-
-| Option            | Description                                                                                                                                 | Default                      | Command line option     |
-|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
-| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
-| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
-| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
-| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
-| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
-| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
-| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
-| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
-
-## Test class
-
-The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
-
-```py
-from usercode.model import ExampleModel
-from usercode.presenter import ExamplePresenter
-from usercode.view import ExampleView
-
-from pyqt_autotest.random_auto_test import RandomAutoTest
-
-
-class ExampleTest(RandomAutoTest):
-
-    def setup_widget(self):
-        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
-        self.widget = ExampleView()
-
-        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
-        self.model = ExampleModel()
-        self.presenter = ExamplePresenter(self.widget, self.model)
-        
-        # Your test might be more interesting if you first load data into the widget
-        self.presenter.load_data("fake_data_file.dat")
-```
-
-Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
-
-```py
-    def setup_options(self):
-        self.options.number_of_runs = 2
-        self.options.number_of_actions = 15
-        self.options.wait_time = 200  # milliseconds
-```
-
-## Built-in Actions
-
-The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
-
-| Built-in Action       | Description                                               | Python Callable                                          |
-|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
-| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
-| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
-| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
-
-These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
-
-| Widget type       | Built-in Actions      |
-|-------------------|-----------------------|
-| QPushButton       | Action.MouseLeftClick |
-
-## Creating your own Actions
-This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
-
-The following code provides a basic example for how to define your own custom actions:
-
-```py
-    def setup_options(self):
-        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
-        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
-        actions = {
-            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
-            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
-                                                                    pos=QPoint(2, widget.height() / 2))
-        }
-        
-        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
-        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to 
-        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
-        widget_actions = {
-            QCheckBox: ["Left click in centre"],
-            QLineEdit: ["Enter dummy text"],
-            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
-        }
-
-        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
-        self.options.actions = actions
-        self.options.widget_actions = widget_actions
-```
-
-## Usage
-
-It is trivial to run your test class from the command line as follows (depending on its module location):
-
-```sh
-autotest -R ExampleTest
-```
-or with more arguments:
-```
-autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
-```
-
-## Output
-
-An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
+Metadata-Version: 2.1
+Name: pyqt-autotest
+Version: 0.2.1
+Summary: A command line tool for finding system-level bugs that cause a python Qt application to terminate.
+Author-email: Robert Applin <robertapplin.developer@gmail.com>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://github.com/robertapplin/pyqt-autotest
+Project-URL: Bug Tracker, https://github.com/robertapplin/pyqt-autotest/issues
+Keywords: python,qt,random,auto,test
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyqt-autotest ⚙️🧪
+A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
+
+This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
+
+## Table of contents
+* [Installation](#installation)
+* [Setup](#setup)
+* [Options](#options)
+* [Test class](#test-class)
+* [Built-in Actions](#built-in-actions)
+* [Creating your own Actions](#creating-your-own-actions)
+* [Usage](#usage)
+* [Output](#output)
+
+## Installation
+
+This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
+
+```sh
+pip install pyqt-autotest
+```
+
+## Setup
+
+Create a file named `.autotest` in your home directory with the following contents.
+
+```
+[setup]
+search_directories = /path/to/test/directory1/
+                     /path/to/test/directory2/
+output_directory = /path/to/output/directory/
+```
+
+The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
+
+## Options
+
+The following table details the options that can be provided on the command line.
+
+| Option            | Description                                                                                                                                 | Default                      | Command line option     |
+|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
+| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
+| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
+| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
+| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
+| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
+| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
+| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
+| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
+
+## Test class
+
+The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
+
+```py
+from usercode.model import ExampleModel
+from usercode.presenter import ExamplePresenter
+from usercode.view import ExampleView
+
+from pyqt_autotest.random_auto_test import RandomAutoTest
+
+
+class ExampleTest(RandomAutoTest):
+
+    def setup_widget(self):
+        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
+        self.widget = ExampleView()
+
+        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
+        self.model = ExampleModel()
+        self.presenter = ExamplePresenter(self.widget, self.model)
+
+        # Your test might be more interesting if you first load data into the widget
+        self.presenter.load_data("fake_data_file.dat")
+```
+
+Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
+
+```py
+    def setup_options(self):
+        self.options.number_of_runs = 2
+        self.options.number_of_actions = 15
+        self.options.wait_time = 200  # milliseconds
+```
+
+## Built-in Actions
+
+The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
+
+| Built-in Action       | Description                                               | Python Callable                                          |
+|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
+| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
+| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
+| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
+
+These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
+
+| Widget type       | Built-in Actions      |
+|-------------------|-----------------------|
+| QPushButton       | Action.MouseLeftClick |
+
+## Creating your own Actions
+This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
+
+The following code provides a basic example for how to define your own custom actions:
+
+```py
+    def setup_options(self):
+        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
+        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
+        actions = {
+            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
+            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
+                                                                    pos=QPoint(2, widget.height() / 2))
+        }
+
+        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
+        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to
+        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
+        widget_actions = {
+            QCheckBox: ["Left click in centre"],
+            QLineEdit: ["Enter dummy text"],
+            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
+        }
+
+        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
+        self.options.actions = actions
+        self.options.widget_actions = widget_actions
+```
+
+## Usage
+
+It is trivial to run your test class from the command line as follows (depending on its module location):
+
+```sh
+autotest -R ExampleTest
+```
+or with more arguments:
+```
+autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
+```
+
+## Output
+
+An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
```

### Comparing `pyqt-autotest-0.2.0/README.md` & `pyqt-autotest-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# pyqt-autotest ⚙️🧪
-A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
-
-This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
-
-## Table of contents
-* [Installation](#installation)
-* [Setup](#setup)
-* [Options](#options)
-* [Test class](#test-class)
-* [Built-in Actions](#built-in-actions)
-* [Creating your own Actions](#creating-your-own-actions)
-* [Usage](#usage)
-* [Output](#output)
-
-## Installation
-
-This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
-
-```sh
-pip install pyqt-autotest
-```
-
-## Setup
-
-Create a file named `.autotest` in your home directory with the following contents.
-
-```
-[setup]
-search_directories = /path/to/test/directory1/
-                     /path/to/test/directory2/
-output_directory = /path/to/output/directory/
-```
-
-The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
-
-## Options
-
-The following table details the options that can be provided on the command line.
-
-| Option            | Description                                                                                                                                 | Default                      | Command line option     |
-|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
-| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
-| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
-| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
-| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
-| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
-| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
-| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
-| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
-
-## Test class
-
-The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
-
-```py
-from usercode.model import ExampleModel
-from usercode.presenter import ExamplePresenter
-from usercode.view import ExampleView
-
-from pyqt_autotest.random_auto_test import RandomAutoTest
-
-
-class ExampleTest(RandomAutoTest):
-
-    def setup_widget(self):
-        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
-        self.widget = ExampleView()
-
-        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
-        self.model = ExampleModel()
-        self.presenter = ExamplePresenter(self.widget, self.model)
-        
-        # Your test might be more interesting if you first load data into the widget
-        self.presenter.load_data("fake_data_file.dat")
-```
-
-Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
-
-```py
-    def setup_options(self):
-        self.options.number_of_runs = 2
-        self.options.number_of_actions = 15
-        self.options.wait_time = 200  # milliseconds
-```
-
-## Built-in Actions
-
-The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
-
-| Built-in Action       | Description                                               | Python Callable                                          |
-|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
-| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
-| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
-| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
-
-These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
-
-| Widget type       | Built-in Actions      |
-|-------------------|-----------------------|
-| QPushButton       | Action.MouseLeftClick |
-
-## Creating your own Actions
-This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
-
-The following code provides a basic example for how to define your own custom actions:
-
-```py
-    def setup_options(self):
-        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
-        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
-        actions = {
-            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
-            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
-                                                                    pos=QPoint(2, widget.height() / 2))
-        }
-        
-        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
-        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to 
-        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
-        widget_actions = {
-            QCheckBox: ["Left click in centre"],
-            QLineEdit: ["Enter dummy text"],
-            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
-        }
-
-        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
-        self.options.actions = actions
-        self.options.widget_actions = widget_actions
-```
-
-## Usage
-
-It is trivial to run your test class from the command line as follows (depending on its module location):
-
-```sh
-autotest -R ExampleTest
-```
-or with more arguments:
-```
-autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
-```
-
-## Output
-
-An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
+# pyqt-autotest ⚙️🧪
+A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
+
+This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
+
+## Table of contents
+* [Installation](#installation)
+* [Setup](#setup)
+* [Options](#options)
+* [Test class](#test-class)
+* [Built-in Actions](#built-in-actions)
+* [Creating your own Actions](#creating-your-own-actions)
+* [Usage](#usage)
+* [Output](#output)
+
+## Installation
+
+This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
+
+```sh
+pip install pyqt-autotest
+```
+
+## Setup
+
+Create a file named `.autotest` in your home directory with the following contents.
+
+```
+[setup]
+search_directories = /path/to/test/directory1/
+                     /path/to/test/directory2/
+output_directory = /path/to/output/directory/
+```
+
+The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
+
+## Options
+
+The following table details the options that can be provided on the command line.
+
+| Option            | Description                                                                                                                                 | Default                      | Command line option     |
+|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
+| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
+| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
+| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
+| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
+| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
+| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
+| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
+| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
+
+## Test class
+
+The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
+
+```py
+from usercode.model import ExampleModel
+from usercode.presenter import ExamplePresenter
+from usercode.view import ExampleView
+
+from pyqt_autotest.random_auto_test import RandomAutoTest
+
+
+class ExampleTest(RandomAutoTest):
+
+    def setup_widget(self):
+        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
+        self.widget = ExampleView()
+
+        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
+        self.model = ExampleModel()
+        self.presenter = ExamplePresenter(self.widget, self.model)
+
+        # Your test might be more interesting if you first load data into the widget
+        self.presenter.load_data("fake_data_file.dat")
+```
+
+Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
+
+```py
+    def setup_options(self):
+        self.options.number_of_runs = 2
+        self.options.number_of_actions = 15
+        self.options.wait_time = 200  # milliseconds
+```
+
+## Built-in Actions
+
+The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
+
+| Built-in Action       | Description                                               | Python Callable                                          |
+|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
+| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
+| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
+| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
+
+These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
+
+| Widget type       | Built-in Actions      |
+|-------------------|-----------------------|
+| QPushButton       | Action.MouseLeftClick |
+
+## Creating your own Actions
+This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
+
+The following code provides a basic example for how to define your own custom actions:
+
+```py
+    def setup_options(self):
+        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
+        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
+        actions = {
+            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
+            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
+                                                                    pos=QPoint(2, widget.height() / 2))
+        }
+
+        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
+        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to
+        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
+        widget_actions = {
+            QCheckBox: ["Left click in centre"],
+            QLineEdit: ["Enter dummy text"],
+            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
+        }
+
+        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
+        self.options.actions = actions
+        self.options.widget_actions = widget_actions
+```
+
+## Usage
+
+It is trivial to run your test class from the command line as follows (depending on its module location):
+
+```sh
+autotest -R ExampleTest
+```
+or with more arguments:
+```
+autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
+```
+
+## Output
+
+An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/cli/config.py` & `pyqt-autotest-0.2.1/pyqt_autotest/cli/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,72 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from configparser import ConfigParser
-from os.path import expanduser, isdir
-from typing import List
-
-from pyqt_autotest.utilities.print_colors import PrintColors
-
-HOME_DIR = expanduser("~").replace("\\", "/")
-CONFIG_FILEPATH = f"{HOME_DIR}/.autotest"
-OUTPUT_DIR_OPTION = "output_directory"
-SECTION_HEADING = "setup"
-SEARCH_DIR_OPTION = "search_directories"
-
-
-def _get_multiple_directories_for_option(option_name: str) -> List[str]:
-    """Returns a the output directory set by the user. It searches the config file for this directory."""
-    parser = ConfigParser()
-    if len(parser.read(CONFIG_FILEPATH)) == 0:
-        raise RuntimeError(f"{PrintColors.ERROR}Please create a '{CONFIG_FILEPATH}' file, and specify the "
-                           f"'{SEARCH_DIR_OPTION}' option{PrintColors.END}")
-
-    if SECTION_HEADING not in parser:
-        raise RuntimeError(f"{PrintColors.ERROR}A '{SECTION_HEADING}' section heading was not found in the "
-                           f"'{CONFIG_FILEPATH}' file{PrintColors.END}")
-
-    options = parser[SECTION_HEADING]
-    if option_name not in options:
-        raise RuntimeError(f"{PrintColors.ERROR}A '{option_name}' option was not found in the '{CONFIG_FILEPATH}' "
-                           f"file{PrintColors.END}")
-
-    directories_split = options[option_name].split()
-    # Split by quotes in case a directory has a space inside it and so has been provided with surrounding quotes
-    split_by_quotes = options[option_name].split("\"")
-    # Remove duplicates from list
-    directories_split = list(dict.fromkeys(split_by_quotes + directories_split))
-    # Replace the back-slashes with forward-slashes, and expand '~' and other characters
-    directories_split = [expanduser(directory.replace("\\", "/")) for directory in directories_split]
-    # Remove non-existent directories
-    directories_split = [directory for directory in directories_split if isdir(directory)]
-
-    if len(directories_split) == 0:
-        raise RuntimeError(f"{PrintColors.ERROR}No existing directory found for the '{option_name}' option in the "
-                           f"'{CONFIG_FILEPATH}' file{PrintColors.END}")
-
-    return directories_split
-
-
-def get_search_directories_from_config_file() -> List[str]:
-    """Returns a list of directories to search for test files. It searches the config file for these directories."""
-    return _get_multiple_directories_for_option(SEARCH_DIR_OPTION)
-
-
-def get_output_directory_from_config_file() -> str:
-    """Returns the output directory set by the user. It searches the config file for this directory."""
-    output_directories = _get_multiple_directories_for_option(OUTPUT_DIR_OPTION)
-
-    if len(output_directories) > 1:
-        print(f"{PrintColors.WARNING}PyQtAutoTest Warning: Only one output directory is allowed, but multiple were "
-              f"found. Using the first directory.{PrintColors.END}")
-
-    # Only return the first output directory, as we only output the files in one location
-    return output_directories[0]
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from configparser import ConfigParser
+from os.path import expanduser, isdir
+from typing import List
+
+from pyqt_autotest.utilities.print_colors import PrintColors
+
+HOME_DIR = expanduser("~").replace("\\", "/")
+CONFIG_FILEPATH = f"{HOME_DIR}/.autotest"
+OUTPUT_DIR_OPTION = "output_directory"
+SECTION_HEADING = "setup"
+SEARCH_DIR_OPTION = "search_directories"
+
+
+def _get_multiple_directories_for_option(option_name: str) -> List[str]:
+    """Returns a the output directory set by the user. It searches the config file for this directory."""
+    parser = ConfigParser()
+    if len(parser.read(CONFIG_FILEPATH)) == 0:
+        raise RuntimeError(
+            f"{PrintColors.ERROR}Please create a '{CONFIG_FILEPATH}' file, and specify the "
+            f"'{SEARCH_DIR_OPTION}' option{PrintColors.END}"
+        )
+
+    if SECTION_HEADING not in parser:
+        raise RuntimeError(
+            f"{PrintColors.ERROR}A '{SECTION_HEADING}' section heading was not found in the "
+            f"'{CONFIG_FILEPATH}' file{PrintColors.END}"
+        )
+
+    options = parser[SECTION_HEADING]
+    if option_name not in options:
+        raise RuntimeError(
+            f"{PrintColors.ERROR}A '{option_name}' option was not found in the '{CONFIG_FILEPATH}' " f"file{PrintColors.END}"
+        )
+
+    directories_split = options[option_name].split()
+    # Split by quotes in case a directory has a space inside it and so has been provided with surrounding quotes
+    split_by_quotes = options[option_name].split('"')
+    # Remove duplicates from list
+    directories_split = list(dict.fromkeys(split_by_quotes + directories_split))
+    # Replace the back-slashes with forward-slashes, and expand '~' and other characters
+    directories_split = [expanduser(directory.replace("\\", "/")) for directory in directories_split]
+    # Remove non-existent directories
+    directories_split = [directory for directory in directories_split if isdir(directory)]
+
+    if len(directories_split) == 0:
+        raise RuntimeError(
+            f"{PrintColors.ERROR}No existing directory found for the '{option_name}' option in the "
+            f"'{CONFIG_FILEPATH}' file{PrintColors.END}"
+        )
+
+    return directories_split
+
+
+def get_search_directories_from_config_file() -> List[str]:
+    """Returns a list of directories to search for test files. It searches the config file for these directories."""
+    return _get_multiple_directories_for_option(SEARCH_DIR_OPTION)
+
+
+def get_output_directory_from_config_file() -> str:
+    """Returns the output directory set by the user. It searches the config file for this directory."""
+    output_directories = _get_multiple_directories_for_option(OUTPUT_DIR_OPTION)
+
+    if len(output_directories) > 1:
+        print(
+            f"{PrintColors.WARNING}PyQtAutoTest Warning: Only one output directory is allowed, but multiple were "
+            f"found. Using the first directory.{PrintColors.END}"
+        )
+
+    # Only return the first output directory, as we only output the files in one location
+    return output_directories[0]
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/cli/list_tests.py` & `pyqt-autotest-0.2.1/pyqt_autotest/cli/list_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List, Tuple, Type
-
-from pyqt_autotest.cli.config import get_search_directories_from_config_file
-from pyqt_autotest.cli.modules import (does_module_and_class_match_regex, find_files_in_directories,
-                                       get_test_name, search_file_for_test_classes)
-from pyqt_autotest.qt.application import get_application
-from pyqt_autotest.utilities.print_colors import PrintColors
-from pyqt_autotest.utilities.verbosity_controller import VerbosityController
-
-app = get_application()
-
-
-def _get_module_tests(regex: str, filename: str, test_classes: List[Tuple[str, Type]]) -> List[str]:
-    """Gets the names of tests in a module if the tests match a regex."""
-    test_names = []
-    if test_classes is not None:
-        for test_class in test_classes:
-            test_name = get_test_name(filename, test_class)
-            if regex is None or does_module_and_class_match_regex(regex, test_name):
-                test_names.append(test_name)
-    return test_names
-
-
-def print_matching_tests(regex: str, verbose: bool) -> None:
-    """Print the names of tests matching a regex found in the search directories."""
-    verbosity_controller = VerbosityController(verbose)
-
-    python_files = find_files_in_directories(get_search_directories_from_config_file(), "py")
-
-    found_tests = {}
-    with verbosity_controller:
-        for directory, filenames in python_files.items():
-            found_tests[directory] = []
-            for filename in filenames:
-                _, test_classes, _ = search_file_for_test_classes(f"{directory}/{filename}")
-                found_tests[directory].extend(_get_module_tests(regex, filename, test_classes))
-
-    number_of_tests = sum([len(val) for val in found_tests.values()])
-    print(f"\n{PrintColors.SUCCESS}Found {number_of_tests} test(s):{PrintColors.END}\n" if number_of_tests > 0 else
-          f"\n{PrintColors.WARNING}No regex matches found{PrintColors.END}\n")
-
-    if number_of_tests > 0:
-        # Find the length of the longest test name
-        max_name_len = max([len(max(test_names, key=len)) for test_names in found_tests.values() if len(test_names) > 0])
-
-        for directory, names in found_tests.items():
-            for name in names:
-                print(f"\t{PrintColors.INFO}{name}{' ' * (max_name_len - len(name))}{PrintColors.END}\t{directory}")
-        print("\n")
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List, Tuple, Type
+
+from pyqt_autotest.cli.config import get_search_directories_from_config_file
+from pyqt_autotest.cli.modules import (
+    does_module_and_class_match_regex,
+    find_files_in_directories,
+    get_test_name,
+    search_file_for_test_classes,
+)
+from pyqt_autotest.qt.application import get_application
+from pyqt_autotest.utilities.print_colors import PrintColors
+from pyqt_autotest.utilities.verbosity_controller import VerbosityController
+
+app = get_application()
+
+
+def _get_module_tests(regex: str, filename: str, test_classes: List[Tuple[str, Type]]) -> List[str]:
+    """Gets the names of tests in a module if the tests match a regex."""
+    test_names = []
+    if test_classes is not None:
+        for test_class in test_classes:
+            test_name = get_test_name(filename, test_class)
+            if regex is None or does_module_and_class_match_regex(regex, test_name):
+                test_names.append(test_name)
+    return test_names
+
+
+def print_matching_tests(regex: str, verbose: bool) -> None:
+    """Print the names of tests matching a regex found in the search directories."""
+    verbosity_controller = VerbosityController(verbose)
+
+    python_files = find_files_in_directories(get_search_directories_from_config_file(), "py")
+
+    found_tests = {}
+    with verbosity_controller:
+        for directory, filenames in python_files.items():
+            found_tests[directory] = []
+            for filename in filenames:
+                _, test_classes, _ = search_file_for_test_classes(f"{directory}/{filename}")
+                found_tests[directory].extend(_get_module_tests(regex, filename, test_classes))
+
+    number_of_tests = sum([len(val) for val in found_tests.values()])
+    print(
+        f"\n{PrintColors.SUCCESS}Found {number_of_tests} test(s):{PrintColors.END}\n"
+        if number_of_tests > 0
+        else f"\n{PrintColors.WARNING}No regex matches found{PrintColors.END}\n"
+    )
+
+    if number_of_tests > 0:
+        # Find the length of the longest test name
+        max_name_len = max([len(max(test_names, key=len)) for test_names in found_tests.values() if len(test_names) > 0])
+
+        for directory, names in found_tests.items():
+            for name in names:
+                print(f"\t{PrintColors.INFO}{name}{' ' * (max_name_len - len(name))}{PrintColors.END}\t{directory}")
+        print("\n")
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/cli/modules.py` & `pyqt-autotest-0.2.1/pyqt_autotest/cli/modules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,86 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-import re
-from importlib.util import module_from_spec, spec_from_file_location
-from inspect import getmembers, isclass
-from os import listdir
-from os.path import splitext
-from typing import Dict, List, Tuple, Type
-from pyqt_autotest.random_auto_test import RandomAutoTest
-from pyqt_autotest.repeatable_auto_test import RepeatableAutoTest
-from pyqt_autotest.utilities.print_colors import PrintColors
-
-BASE_TEST_CLASSES = [RandomAutoTest.__name__, RepeatableAutoTest.__name__]
-
-
-def find_files_in_directories(directories: List[str], extension: str) -> Dict[str, List[str]]:
-    """Returns the python files stored in particular directories."""
-    result = {}
-    for directory in directories:
-        result[directory] = [file for file in listdir(directory) if file.endswith(extension)]
-    return result
-
-
-def search_file_for_imports(filepath: str) -> str:
-    """Searches for the imports in a file and returns them as a string."""
-    with open(filepath, "r") as file:
-        all_lines = file.readlines()
-
-    import_lines = ""
-    for line in all_lines:
-        if "import" in line and RandomAutoTest.__name__ not in line:
-            import_lines += line
-    return import_lines
-
-
-def search_file_for_test_classes(filepath: str):
-    """Imports a python module and checks if it contains at least one test class. It returns any found test classes."""
-    print(f"Checking '{filepath}' for test classes...")
-
-    try:
-        # Import module
-        spec = spec_from_file_location("", filepath)
-        module = module_from_spec(spec)
-        spec.loader.exec_module(module)
-    except Exception as ex:
-        print(f"{PrintColors.ERROR}{str(ex)}{PrintColors.END}")
-        return None, None, None
-    else:
-        # Find test classes inside the module
-        test_classes = getmembers(module, lambda member: isclass(member) and (issubclass(member, RandomAutoTest) or
-                                                                              issubclass(member, RepeatableAutoTest)))
-        # Find import lines inside the module
-        import_str = search_file_for_imports(filepath)
-        # Remove classes with a base test type
-        test_classes = [cls for cls in test_classes if cls[0] not in BASE_TEST_CLASSES]
-        if len(test_classes) == 0:
-            print(f"{PrintColors.WARNING}Failed to find a test class which inherits from one of '{BASE_TEST_CLASSES}'."
-                  f"{PrintColors.END}")
-            return None, None, None
-        return module, test_classes, import_str
-
-
-def get_test_name(filename: str, test_class: Tuple[str, Type]) -> str:
-    """Constructs the name of a test"""
-    return f"{splitext(filename)[0]}_{test_class[0]}"
-
-
-def does_module_and_class_match_regex(regex: str, test_name: str) -> bool:
-    """Returns true if the regex is found inside the test name."""
-    pattern = re.compile(regex)
-    return re.search(pattern, test_name)
-
-
-def get_matching_tests_in_module(regex: str, filename: str, test_classes: List[Tuple[str, Type]], import_str: str):
-    """Returns the test classes that match a particular regex."""
-    matching_tests = []
-    if test_classes is not None:
-        for test_class in test_classes:
-            test_name = get_test_name(filename, test_class)
-            if does_module_and_class_match_regex(regex, test_name):
-                matching_tests.append((test_name, test_class, import_str))
-    return matching_tests
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+import re
+from importlib.util import module_from_spec, spec_from_file_location
+from inspect import getmembers, isclass
+from os import listdir
+from os.path import splitext
+from typing import Dict, List, Tuple, Type
+from pyqt_autotest.random_auto_test import RandomAutoTest
+from pyqt_autotest.repeatable_auto_test import RepeatableAutoTest
+from pyqt_autotest.utilities.print_colors import PrintColors
+
+BASE_TEST_CLASSES = [RandomAutoTest.__name__, RepeatableAutoTest.__name__]
+
+
+def find_files_in_directories(directories: List[str], extension: str) -> Dict[str, List[str]]:
+    """Returns the python files stored in particular directories."""
+    result = {}
+    for directory in directories:
+        result[directory] = [file for file in listdir(directory) if file.endswith(extension)]
+    return result
+
+
+def search_file_for_imports(filepath: str) -> str:
+    """Searches for the imports in a file and returns them as a string."""
+    with open(filepath, "r") as file:
+        all_lines = file.readlines()
+
+    import_lines = ""
+    for line in all_lines:
+        if "import" in line and RandomAutoTest.__name__ not in line:
+            import_lines += line
+    return import_lines
+
+
+def search_file_for_test_classes(filepath: str):
+    """Imports a python module and checks if it contains at least one test class. It returns any found test classes."""
+    print(f"Checking '{filepath}' for test classes...")
+
+    try:
+        # Import module
+        spec = spec_from_file_location("", filepath)
+        module = module_from_spec(spec)
+        spec.loader.exec_module(module)
+    except Exception as ex:
+        print(f"{PrintColors.ERROR}{str(ex)}{PrintColors.END}")
+        return None, None, None
+    else:
+        # Find test classes inside the module
+        test_classes = getmembers(
+            module,
+            lambda member: isclass(member) and (issubclass(member, RandomAutoTest) or issubclass(member, RepeatableAutoTest)),
+        )
+        # Find import lines inside the module
+        import_str = search_file_for_imports(filepath)
+        # Remove classes with a base test type
+        test_classes = [cls for cls in test_classes if cls[0] not in BASE_TEST_CLASSES]
+        if len(test_classes) == 0:
+            print(
+                f"{PrintColors.WARNING}Failed to find a test class which inherits from one of '{BASE_TEST_CLASSES}'."
+                f"{PrintColors.END}"
+            )
+            return None, None, None
+        return module, test_classes, import_str
+
+
+def get_test_name(filename: str, test_class: Tuple[str, Type]) -> str:
+    """Constructs the name of a test"""
+    return f"{splitext(filename)[0]}_{test_class[0]}"
+
+
+def does_module_and_class_match_regex(regex: str, test_name: str) -> bool:
+    """Returns true if the regex is found inside the test name."""
+    pattern = re.compile(regex)
+    return re.search(pattern, test_name)
+
+
+def get_matching_tests_in_module(regex: str, filename: str, test_classes: List[Tuple[str, Type]], import_str: str):
+    """Returns the test classes that match a particular regex."""
+    matching_tests = []
+    if test_classes is not None:
+        for test_class in test_classes:
+            test_name = get_test_name(filename, test_class)
+            if does_module_and_class_match_regex(regex, test_name):
+                matching_tests.append((test_name, test_class, import_str))
+    return matching_tests
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/cli/options.py` & `pyqt-autotest-0.2.1/pyqt_autotest/cli/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,148 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import Callable, Dict, List
-
-from pyqt_autotest.core.action import Action
-
-from PyQt5.QtCore import Qt
-from PyQt5.QtTest import QTest
-from PyQt5.QtWidgets import QPushButton
-
-DEFAULT_NUMBER_OF_RUNS = 1
-DEFAULT_NUMBER_OF_ACTIONS = 10
-DEFAULT_SEQUENCE_OF_ACTIONS = []
-DEFAULT_SEQUENCE_OF_WIDGETS = []
-DEFAULT_WAIT_TIME = 50
-DEFAULT_VERBOSE = False
-
-
-class Options:
-    actions: Dict[Action, Callable] = {
-        Action.KeyDownClick: lambda widget: QTest.keyClick(widget, Qt.Key_Down),
-        Action.KeyUpClick: lambda widget: QTest.keyClick(widget, Qt.Key_Up),
-        Action.MouseLeftClick: lambda widget: QTest.mouseClick(widget, Qt.LeftButton)
-    }
-
-    widget_actions = {
-        QPushButton: [Action.MouseLeftClick]
-    }
-
-    def __init__(self, number_of_runs: int = None, number_of_actions: int = None, wait_time: int = None,
-                 verbose: bool = False):
-        self._number_of_runs: int = number_of_runs
-        self._wait_time: int = wait_time
-        self._verbose: bool = verbose
-
-        # Options only used for RandomAutoTest
-        self._number_of_actions: int = number_of_actions
-
-        # Options only used for RepeatableAutoTest
-        self._sequence_of_actions: List[Action] = None
-        self._sequence_of_widgets: List[str] = None
-
-    @property
-    def number_of_runs(self) -> int:
-        """Returns the number_of_runs option, or a default if it hasn't been set."""
-        if self._number_of_runs is None:
-            return DEFAULT_NUMBER_OF_RUNS
-        return int(self._number_of_runs)
-
-    @number_of_runs.setter
-    def number_of_runs(self, n_runs: int) -> None:
-        """Sets the number_of_runs option if it hasn't already been provided on the command line."""
-        if n_runs is None:
-            return
-        if not isinstance(n_runs, int):
-            raise ValueError("The provided 'number_of_runs' option is not an int.")
-
-        if self._number_of_runs is None:
-            self._number_of_runs = n_runs
-
-    @property
-    def number_of_actions(self) -> int:
-        """Returns the number_of_actions option, or a default if it hasn't been set."""
-        if self._number_of_actions is None:
-            return DEFAULT_NUMBER_OF_ACTIONS
-        return int(self._number_of_actions)
-
-    @number_of_actions.setter
-    def number_of_actions(self, n_actions: int) -> None:
-        """Sets the number_of_actions option if it hasn't already been provided on the command line."""
-        if n_actions is None:
-            return
-        if not isinstance(n_actions, int):
-            raise ValueError("The provided 'number_of_actions' option is not an int.")
-
-        if self._number_of_actions is None:
-            self._number_of_actions = n_actions
-
-    @property
-    def wait_time(self) -> int:
-        """Returns the wait_time option, or a default if it hasn't been set."""
-        if self._wait_time is None:
-            return DEFAULT_WAIT_TIME
-        return int(self._wait_time)
-
-    @wait_time.setter
-    def wait_time(self, wait_time: int) -> None:
-        """Sets the wait_time option if it hasn't already been provided on the command line."""
-        if wait_time is None:
-            return
-        if not isinstance(wait_time, int):
-            raise ValueError("The provided 'wait_time' option is not an int.")
-
-        if self._wait_time is None:
-            self._wait_time = wait_time
-
-    @property
-    def sequence_of_actions(self) -> List[Action]:
-        """Returns the sequence_of_actions option, or a default if it hasn't been set."""
-        if self._sequence_of_actions is None:
-            return DEFAULT_SEQUENCE_OF_ACTIONS
-        return self._sequence_of_actions
-
-    @sequence_of_actions.setter
-    def sequence_of_actions(self, actions: List[Action]) -> None:
-        """Sets the sequence_of_actions option if it hasn't already been provided on the command line."""
-        if actions is None:
-            return
-        if not isinstance(actions, list):
-            raise ValueError("The provided 'sequence_of_actions' option is not a list.")
-
-        if self._sequence_of_actions is None:
-            self._sequence_of_actions = [action.strip() for action in actions]
-
-    @property
-    def sequence_of_widgets(self) -> List[str]:
-        """Returns the sequence_of_widgets option, or a default if it hasn't been set."""
-        if self._sequence_of_widgets is None:
-            return DEFAULT_SEQUENCE_OF_WIDGETS
-        return self._sequence_of_widgets
-
-    @sequence_of_widgets.setter
-    def sequence_of_widgets(self, widgets: List[str]) -> None:
-        """Sets the sequence_of_widgets option if it hasn't already been provided on the command line."""
-        if widgets is None:
-            return
-        if not isinstance(widgets, list):
-            raise ValueError("The provided 'sequence_of_widgets' option is not a list.")
-
-        if self._sequence_of_widgets is None:
-            self._sequence_of_widgets = [widget.strip() for widget in widgets]
-
-    @property
-    def verbose(self) -> bool:
-        """Returns the verbose option, or a default if it hasn't been set."""
-        if self._verbose is None:
-            return DEFAULT_VERBOSE
-        return bool(self._verbose)
-
-    @verbose.setter
-    def verbose(self, verbose: bool) -> None:
-        """Sets the verbose option if it hasn't already been provided on the command line."""
-        if verbose is None:
-            return
-        if not isinstance(verbose, bool):
-            raise ValueError("The provided 'verbose' option is not a boolean.")
-
-        if self._verbose is None:
-            self._verbose = verbose
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import Callable, Dict, List
+
+from pyqt_autotest.core.action import Action
+
+from PyQt5.QtCore import Qt
+from PyQt5.QtTest import QTest
+from PyQt5.QtWidgets import QPushButton
+
+DEFAULT_NUMBER_OF_RUNS = 1
+DEFAULT_NUMBER_OF_ACTIONS = 10
+DEFAULT_SEQUENCE_OF_ACTIONS = []
+DEFAULT_SEQUENCE_OF_WIDGETS = []
+DEFAULT_WAIT_TIME = 50
+DEFAULT_VERBOSE = False
+
+
+class Options:
+    actions: Dict[Action, Callable] = {
+        Action.KeyDownClick: lambda widget: QTest.keyClick(widget, Qt.Key_Down),
+        Action.KeyUpClick: lambda widget: QTest.keyClick(widget, Qt.Key_Up),
+        Action.MouseLeftClick: lambda widget: QTest.mouseClick(widget, Qt.LeftButton),
+    }
+
+    widget_actions = {QPushButton: [Action.MouseLeftClick]}
+
+    def __init__(
+        self, number_of_runs: int = None, number_of_actions: int = None, wait_time: int = None, verbose: bool = False
+    ):
+        self._number_of_runs: int = number_of_runs
+        self._wait_time: int = wait_time
+        self._verbose: bool = verbose
+
+        # Options only used for RandomAutoTest
+        self._number_of_actions: int = number_of_actions
+
+        # Options only used for RepeatableAutoTest
+        self._sequence_of_actions: List[Action] = None
+        self._sequence_of_widgets: List[str] = None
+
+    @property
+    def number_of_runs(self) -> int:
+        """Returns the number_of_runs option, or a default if it hasn't been set."""
+        if self._number_of_runs is None:
+            return DEFAULT_NUMBER_OF_RUNS
+        return int(self._number_of_runs)
+
+    @number_of_runs.setter
+    def number_of_runs(self, n_runs: int) -> None:
+        """Sets the number_of_runs option if it hasn't already been provided on the command line."""
+        if n_runs is None:
+            return
+        if not isinstance(n_runs, int):
+            raise ValueError("The provided 'number_of_runs' option is not an int.")
+
+        if self._number_of_runs is None:
+            self._number_of_runs = n_runs
+
+    @property
+    def number_of_actions(self) -> int:
+        """Returns the number_of_actions option, or a default if it hasn't been set."""
+        if self._number_of_actions is None:
+            return DEFAULT_NUMBER_OF_ACTIONS
+        return int(self._number_of_actions)
+
+    @number_of_actions.setter
+    def number_of_actions(self, n_actions: int) -> None:
+        """Sets the number_of_actions option if it hasn't already been provided on the command line."""
+        if n_actions is None:
+            return
+        if not isinstance(n_actions, int):
+            raise ValueError("The provided 'number_of_actions' option is not an int.")
+
+        if self._number_of_actions is None:
+            self._number_of_actions = n_actions
+
+    @property
+    def wait_time(self) -> int:
+        """Returns the wait_time option, or a default if it hasn't been set."""
+        if self._wait_time is None:
+            return DEFAULT_WAIT_TIME
+        return int(self._wait_time)
+
+    @wait_time.setter
+    def wait_time(self, wait_time: int) -> None:
+        """Sets the wait_time option if it hasn't already been provided on the command line."""
+        if wait_time is None:
+            return
+        if not isinstance(wait_time, int):
+            raise ValueError("The provided 'wait_time' option is not an int.")
+
+        if self._wait_time is None:
+            self._wait_time = wait_time
+
+    @property
+    def sequence_of_actions(self) -> List[Action]:
+        """Returns the sequence_of_actions option, or a default if it hasn't been set."""
+        if self._sequence_of_actions is None:
+            return DEFAULT_SEQUENCE_OF_ACTIONS
+        return self._sequence_of_actions
+
+    @sequence_of_actions.setter
+    def sequence_of_actions(self, actions: List[Action]) -> None:
+        """Sets the sequence_of_actions option if it hasn't already been provided on the command line."""
+        if actions is None:
+            return
+        if not isinstance(actions, list):
+            raise ValueError("The provided 'sequence_of_actions' option is not a list.")
+
+        if self._sequence_of_actions is None:
+            self._sequence_of_actions = [action.strip() for action in actions]
+
+    @property
+    def sequence_of_widgets(self) -> List[str]:
+        """Returns the sequence_of_widgets option, or a default if it hasn't been set."""
+        if self._sequence_of_widgets is None:
+            return DEFAULT_SEQUENCE_OF_WIDGETS
+        return self._sequence_of_widgets
+
+    @sequence_of_widgets.setter
+    def sequence_of_widgets(self, widgets: List[str]) -> None:
+        """Sets the sequence_of_widgets option if it hasn't already been provided on the command line."""
+        if widgets is None:
+            return
+        if not isinstance(widgets, list):
+            raise ValueError("The provided 'sequence_of_widgets' option is not a list.")
+
+        if self._sequence_of_widgets is None:
+            self._sequence_of_widgets = [widget.strip() for widget in widgets]
+
+    @property
+    def verbose(self) -> bool:
+        """Returns the verbose option, or a default if it hasn't been set."""
+        if self._verbose is None:
+            return DEFAULT_VERBOSE
+        return bool(self._verbose)
+
+    @verbose.setter
+    def verbose(self, verbose: bool) -> None:
+        """Sets the verbose option if it hasn't already been provided on the command line."""
+        if verbose is None:
+            return
+        if not isinstance(verbose, bool):
+            raise ValueError("The provided 'verbose' option is not a boolean.")
+
+        if self._verbose is None:
+            self._verbose = verbose
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/cli/run_tests.py` & `pyqt-autotest-0.2.1/pyqt_autotest/cli/run_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,74 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import Type
-
-from pyqt_autotest.cli.config import get_output_directory_from_config_file, get_search_directories_from_config_file
-from pyqt_autotest.cli.modules import (find_files_in_directories, get_matching_tests_in_module,
-                                       search_file_for_test_classes)
-from pyqt_autotest.cli.options import Options
-from pyqt_autotest.core.exception_handler import catch_exceptions
-from pyqt_autotest.qt.application import get_application
-from pyqt_autotest.utilities.print_colors import PrintColors
-from pyqt_autotest.utilities.verbosity_controller import VerbosityController
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-from pyqt_autotest.results.print_results import print_results
-
-app = get_application()
-
-
-def _find_matching_tests(regex: str, python_files, verbosity_controller: VerbosityController):
-    """Returns a list of tests that match the provided regex."""
-    matching_tests = []
-    with verbosity_controller:
-        for directory, filenames in python_files.items():
-            for filename in filenames:
-                module, test_classes, import_str = search_file_for_test_classes(f"{directory}/{filename}")
-                matching_tests.extend(get_matching_tests_in_module(regex, filename, test_classes, import_str))
-    return matching_tests
-
-
-def _run_test(test_name: str, test_class: Type, import_str: str, number_of_runs: int, number_of_actions: int,
-              wait_time: int, verbose: bool, verbosity_controller: VerbosityController) -> None:
-    """Runs the tests in a module if the tests match a regex."""
-    print(f"{PrintColors.INFO}Running '{test_name}'...{PrintColors.END}\n")
-    options = Options(number_of_runs, number_of_actions, wait_time, verbose)
-    instance = test_class[1](options, verbosity_controller)
-    instance._run(test_name, import_str)
-
-
-@catch_exceptions
-def run(regex: str, number_of_runs: int, number_of_actions: int, wait_time: int, output_name: str, cautious: bool,
-        verbose: bool) -> None:
-    """Runs the tests with the provided options."""
-    global app
-
-    json_results = JSONResultsDict()
-    json_results.cautious = cautious
-    if output_name is not None:
-        json_results.output_filepath = f"{get_output_directory_from_config_file()}/{output_name}.json"
-
-    verbosity_controller = VerbosityController(verbose)
-
-    python_files = find_files_in_directories(get_search_directories_from_config_file(), "py")
-    matching_tests = _find_matching_tests(regex, python_files, verbosity_controller)
-
-    for test_name, test_class, import_str in matching_tests:
-        _run_test(test_name, test_class, import_str, number_of_runs, number_of_actions, wait_time, verbose,
-                  verbosity_controller)
-
-    json_results.save_to_file()
-    print_results(json_results.output_filepath)
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from os.path import join
+from typing import Type
+
+from pyqt_autotest.cli.config import get_output_directory_from_config_file, get_search_directories_from_config_file
+from pyqt_autotest.cli.modules import find_files_in_directories, get_matching_tests_in_module, search_file_for_test_classes
+from pyqt_autotest.cli.options import Options
+from pyqt_autotest.core.exception_handler import catch_exceptions
+from pyqt_autotest.qt.application import get_application
+from pyqt_autotest.utilities.print_colors import PrintColors
+from pyqt_autotest.utilities.verbosity_controller import VerbosityController
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+from pyqt_autotest.results.print_results import print_results
+
+app = get_application()
+
+
+def _find_matching_tests(regex: str, python_files, verbosity_controller: VerbosityController):
+    """Returns a list of tests that match the provided regex."""
+    matching_tests = []
+    with verbosity_controller:
+        for directory, filenames in python_files.items():
+            for filename in filenames:
+                module, test_classes, import_str = search_file_for_test_classes(f"{directory}/{filename}")
+                matching_tests.extend(get_matching_tests_in_module(regex, filename, test_classes, import_str))
+    return matching_tests
+
+
+def _run_test(
+    test_name: str,
+    test_class: Type,
+    import_str: str,
+    number_of_runs: int,
+    number_of_actions: int,
+    wait_time: int,
+    verbose: bool,
+    verbosity_controller: VerbosityController,
+) -> None:
+    """Runs the tests in a module if the tests match a regex."""
+    print(f"{PrintColors.INFO}Running '{test_name}'...{PrintColors.END}\n")
+    options = Options(number_of_runs, number_of_actions, wait_time, verbose)
+    instance = test_class[1](options, verbosity_controller)
+    instance._run(test_name, import_str)
+
+
+@catch_exceptions
+def run(
+    regex: str, number_of_runs: int, number_of_actions: int, wait_time: int, output_name: str, cautious: bool, verbose: bool
+) -> None:
+    """Runs the tests with the provided options."""
+    global app
+
+    json_results = JSONResultsDict()
+    json_results.cautious = cautious
+    if output_name is not None:
+        json_results.output_filepath = join(get_output_directory_from_config_file(), output_name) + ".json"
+
+    verbosity_controller = VerbosityController(verbose)
+
+    python_files = find_files_in_directories(get_search_directories_from_config_file(), "py")
+    matching_tests = _find_matching_tests(regex, python_files, verbosity_controller)
+
+    if len(matching_tests) == 0:
+        print(f"{PrintColors.ERROR}No matching tests were found for regex '{regex}'." f"{PrintColors.END}")
+        return
+
+    for test_name, test_class, import_str in matching_tests:
+        _run_test(
+            test_name, test_class, import_str, number_of_runs, number_of_actions, wait_time, verbose, verbosity_controller
+        )
+
+    json_results.save_to_file()
+    print_results(json_results.output_filepath)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/core/auto_test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/core/auto_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,133 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-import sys
-from abc import ABCMeta, abstractmethod
-from inspect import getsource
-from typing import List, Tuple
-
-from pyqt_autotest.cli.options import Options
-from pyqt_autotest.core.action import Action
-from pyqt_autotest.core.exception_handler import (catch_exceptions, exception_hook, exit_hook,
-                                                  unraisable_exception_hook)
-from pyqt_autotest.core.exceptions import (ActionDoesNotExist, CloseWidgetError, WidgetDoesNotExist,
-                                           WidgetNotProvidedError)
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-from pyqt_autotest.qt.modal_unblocker import close_modals_if_exist, WindowUnblockFilter
-from pyqt_autotest.qt.top_level_widgets import get_top_level_widget_classes
-from pyqt_autotest.utilities.print_colors import PrintColors
-from pyqt_autotest.utilities.verbosity_controller import VerbosityController
-
-from PyQt5.QtCore import Qt, QTimer
-from PyQt5.QtWidgets import QWidget, QMessageBox
-from PyQt5.QtTest import QTest
-from tqdm import tqdm
-
-
-class _AutoTest(metaclass=ABCMeta):
-
-    def __init__(self, options: Options, verbosity_controller: VerbosityController):
-        super(_AutoTest, self).__init__()
-        self.widget: QWidget = None
-        self.options: Options = options
-
-        self._verbosity_controller = verbosity_controller
-        self._logger = JSONResultsDict()
-
-        # Used to unblock the main widget if a modal QFileDialog opens and blocks further actions
-        self.modal_unblocker = WindowUnblockFilter()
-
-        sys.exit = exit_hook
-        sys.excepthook = exception_hook
-        sys.unraisablehook = unraisable_exception_hook
-
-    def setup_options(self) -> None:
-        """The method used to set the options for the test (optional)."""
-        pass
-
-    @abstractmethod
-    def setup_widget(self) -> None:
-        """The method used to instantiate the users widget."""
-        pass
-
-    @catch_exceptions
-    def _run(self, test_name: str, import_str: str) -> None:
-        """Runs the random widget testing."""
-        self.setup_options()
-        self._logger.init_test(self._test_type(), import_str, getsource(self.setup_widget), test_name, self.options)
-        for run_number in range(1, self.options.number_of_runs + 1):
-            self._logger.init_run()
-            self._run_actions(run_number)
-
-    @catch_exceptions
-    def _run_actions(self, run_number: int) -> None:
-        """Sets up the widget and runs the actions for a single run."""
-        self.setup_widget()
-        if not isinstance(self.widget, QWidget):
-            raise WidgetNotProvidedError()
-        self.widget.setAttribute(Qt.WA_DeleteOnClose)
-        self.widget.installEventFilter(self.modal_unblocker)
-        self.widget.show()
-
-        child_widgets = self._get_child_widgets()
-        with self._verbosity_controller:
-            print(f"\t{PrintColors.INFO}Starting test number "
-                  f"({run_number}/{self.options.number_of_runs})...{PrintColors.END}\n")
-            for action_number in tqdm(range(self._get_number_of_actions()),
-                                      desc=f"\tRunning ({run_number}/{self.options.number_of_runs})",
-                                      disable=self.options.verbose, bar_format="{l_bar}{bar}|", ncols=80):
-                # After a certain timeout, attempt to close any QMessageBox's that could be blocking the main widget
-                QTimer.singleShot(2 * self.options.wait_time, lambda: close_modals_if_exist(QMessageBox))
-                action_name, widget_name, widget = self._get_action_name_widget_name_and_widget(action_number,
-                                                                                                child_widgets)
-                self._logger.save_event(widget_name, str(action_name))
-                # Validate the widget and action exists
-                if widget is None:
-                    raise WidgetDoesNotExist()
-                if action_name not in self.options.actions:
-                    raise ActionDoesNotExist()
-                # Perform action on a child widget
-                self.options.actions[action_name](widget)
-                # Wait for a given number of milliseconds
-                QTest.qWait(self.options.wait_time)
-                # If there was an error which has been caught
-                if not self._logger.is_running():
-                    break
-        self._close_widget()
-
-    @abstractmethod
-    def _test_type(self) -> str:
-        """Returns a string to represent the type of the test. e.g. RandomAutoTest or RepeatableAutoTest."""
-        pass
-
-    @abstractmethod
-    def _get_number_of_actions(self) -> int:
-        """Returns the number of actions to be performed for a run."""
-        pass
-
-    @abstractmethod
-    def _get_child_widgets(self) -> List[QWidget]:
-        """Returns the child widgets which are required for a run."""
-        pass
-
-    @abstractmethod
-    def _get_action_name_widget_name_and_widget(self, action_number: int,
-                                                all_widgets: List[QWidget]) -> Tuple[Action, str, QWidget]:
-        """Returns the action, and widget to perform an action on."""
-        pass
-
-    @catch_exceptions
-    def _close_widget(self) -> None:
-        """Closes the widget and starts the event loop to ensure all events are processed."""
-        self.widget.close()
-        self.widget = None
-        QTest.qWait(self.options.wait_time)
-
-        if self._logger.is_running():
-            if len(get_top_level_widget_classes()) == 0:
-                self._logger.save_run_result(ExitState.Success)
-            else:
-                raise CloseWidgetError()
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+import sys
+from abc import ABCMeta, abstractmethod
+from inspect import getsource
+from typing import List, Tuple
+
+from pyqt_autotest.cli.options import Options
+from pyqt_autotest.core.action import Action
+from pyqt_autotest.core.exception_handler import catch_exceptions, exception_hook, exit_hook, unraisable_exception_hook
+from pyqt_autotest.core.exceptions import ActionDoesNotExist, CloseWidgetError, WidgetDoesNotExist, WidgetNotProvidedError
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+from pyqt_autotest.qt.modal_unblocker import close_modals_if_exist, WindowUnblockFilter
+from pyqt_autotest.qt.top_level_widgets import get_top_level_widget_classes
+from pyqt_autotest.utilities.print_colors import PrintColors
+from pyqt_autotest.utilities.verbosity_controller import VerbosityController
+
+from PyQt5.QtCore import Qt, QTimer
+from PyQt5.QtWidgets import QWidget, QMessageBox
+from PyQt5.QtTest import QTest
+from tqdm import tqdm
+
+
+class _AutoTest(metaclass=ABCMeta):
+    def __init__(self, options: Options, verbosity_controller: VerbosityController):
+        super(_AutoTest, self).__init__()
+        self.widget: QWidget = None
+        self.options: Options = options
+
+        self._verbosity_controller = verbosity_controller
+        self._logger = JSONResultsDict()
+
+        # Used to unblock the main widget if a modal QFileDialog opens and blocks further actions
+        self.modal_unblocker = WindowUnblockFilter()
+
+        sys.exit = exit_hook
+        sys.excepthook = exception_hook
+        sys.unraisablehook = unraisable_exception_hook
+
+    def setup_options(self) -> None:
+        """The method used to set the options for the test (optional)."""
+        pass
+
+    @abstractmethod
+    def setup_widget(self) -> None:
+        """The method used to instantiate the users widget."""
+        pass
+
+    @catch_exceptions
+    def _run(self, test_name: str, import_str: str) -> None:
+        """Runs the random widget testing."""
+        self.setup_options()
+        self._logger.init_test(self._test_type(), import_str, getsource(self.setup_widget), test_name, self.options)
+        for run_number in range(1, self.options.number_of_runs + 1):
+            self._logger.init_run()
+            self._run_actions(run_number)
+
+    @catch_exceptions
+    def _run_actions(self, run_number: int) -> None:
+        """Sets up the widget and runs the actions for a single run."""
+        self.setup_widget()
+        if not isinstance(self.widget, QWidget):
+            raise WidgetNotProvidedError()
+        self.widget.setAttribute(Qt.WA_DeleteOnClose)
+        self.widget.installEventFilter(self.modal_unblocker)
+        self.widget.show()
+
+        child_widgets = self._get_child_widgets()
+        with self._verbosity_controller:
+            print(
+                f"\t{PrintColors.INFO}Starting test number "
+                f"({run_number}/{self.options.number_of_runs})...{PrintColors.END}\n"
+            )
+            for action_number in tqdm(
+                range(self._get_number_of_actions()),
+                desc=f"\tRunning ({run_number}/{self.options.number_of_runs})",
+                disable=self.options.verbose,
+                bar_format="{l_bar}{bar}|",
+                ncols=80,
+            ):
+                # After a certain timeout, attempt to close any QMessageBox's that could be blocking the main widget
+                QTimer.singleShot(2 * self.options.wait_time, lambda: close_modals_if_exist(QMessageBox))
+                action_name, widget_name, widget = self._get_action_name_widget_name_and_widget(action_number, child_widgets)
+                self._logger.save_event(widget_name, str(action_name))
+                # Validate the widget and action exists
+                if widget is None:
+                    raise WidgetDoesNotExist()
+                if action_name not in self.options.actions:
+                    raise ActionDoesNotExist()
+                # Perform action on a child widget
+                self.options.actions[action_name](widget)
+                # Wait for a given number of milliseconds
+                QTest.qWait(self.options.wait_time)
+                # If there was an error which has been caught
+                if not self._logger.is_running():
+                    break
+        self._close_widget()
+
+    @abstractmethod
+    def _test_type(self) -> str:
+        """Returns a string to represent the type of the test. e.g. RandomAutoTest or RepeatableAutoTest."""
+        pass
+
+    @abstractmethod
+    def _get_number_of_actions(self) -> int:
+        """Returns the number of actions to be performed for a run."""
+        pass
+
+    @abstractmethod
+    def _get_child_widgets(self) -> List[QWidget]:
+        """Returns the child widgets which are required for a run."""
+        pass
+
+    @abstractmethod
+    def _get_action_name_widget_name_and_widget(
+        self, action_number: int, all_widgets: List[QWidget]
+    ) -> Tuple[Action, str, QWidget]:
+        """Returns the action, and widget to perform an action on."""
+        pass
+
+    @catch_exceptions
+    def _close_widget(self) -> None:
+        """Closes the widget and starts the event loop to ensure all events are processed."""
+        self.widget.close()
+        self.widget = None
+        QTest.qWait(self.options.wait_time)
+
+        if self._logger.is_running():
+            if len(get_top_level_widget_classes()) == 0:
+                self._logger.save_run_result(ExitState.Success)
+            else:
+                raise CloseWidgetError()
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/core/exception_handler.py` & `pyqt-autotest-0.2.1/pyqt_autotest/core/exception_handler.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from functools import wraps
-from sys import exc_info
-from traceback import format_exception
-
-from pyqt_autotest.core.exceptions import SetupError, WidgetError
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-
-
-def exit_hook(args):
-    """Used to hook a system exit and report the system exit."""
-    message_list = [f"A SystemExit exception was raised with arguments: {str(args)}\n"]
-    print("\n" + "".join(message_list))
-    JSONResultsDict().save_run_result(ExitState.Error, message_list)
-
-
-def exception_hook(type, exception, traceback):
-    """Used to hook an exception and report the exception."""
-    message_list = format_exception(type, exception, traceback)
-    print("\n" + "".join(message_list))
-    JSONResultsDict().save_run_result(ExitState.Error, message_list)
-
-
-def unraisable_exception_hook(unraisable):
-    """Used to hook an unraisable exception and report the unraisable exception."""
-    message_list = format_exception(*exc_info())
-    print("\n" + "".join(message_list))
-    JSONResultsDict().save_run_result(ExitState.Error, message_list)
-
-
-def catch_exceptions(function):
-    """A decorator function used to catch exceptions in a function."""
-
-    @wraps(function)
-    def wrapper(*args, **kwargs):
-        try:
-            return function(*args, **kwargs)
-        except SetupError as ex:
-            ex.report()
-        except WidgetError as ex:
-            ex.report()
-            ex.cleanup()
-        except BaseException as ex:
-            print("\n" + str(ex))
-            JSONResultsDict().save_run_result(ExitState.Error, format_exception(*exc_info()))
-
-    return wrapper
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from functools import wraps
+from sys import exc_info
+from traceback import format_exception
+
+from pyqt_autotest.core.exceptions import SetupError, WidgetError
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+
+
+def exit_hook(args):
+    """Used to hook a system exit and report the system exit."""
+    message_list = [f"A SystemExit exception was raised with arguments: {str(args)}\n"]
+    print("\n" + "".join(message_list))
+    JSONResultsDict().save_run_result(ExitState.Error, message_list)
+
+
+def exception_hook(type, exception, traceback):
+    """Used to hook an exception and report the exception."""
+    message_list = format_exception(type, exception, traceback)
+    print("\n" + "".join(message_list))
+    JSONResultsDict().save_run_result(ExitState.Error, message_list)
+
+
+def unraisable_exception_hook(unraisable):
+    """Used to hook an unraisable exception and report the unraisable exception."""
+    message_list = format_exception(*exc_info())
+    print("\n" + "".join(message_list))
+    JSONResultsDict().save_run_result(ExitState.Error, message_list)
+
+
+def catch_exceptions(function):
+    """A decorator function used to catch exceptions in a function."""
+
+    @wraps(function)
+    def wrapper(*args, **kwargs):
+        try:
+            return function(*args, **kwargs)
+        except SetupError as ex:
+            ex.report()
+        except WidgetError as ex:
+            ex.report()
+            ex.cleanup()
+        except BaseException as ex:
+            print("\n" + str(ex))
+            JSONResultsDict().save_run_result(ExitState.Error, format_exception(*exc_info()))
+
+    return wrapper
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/core/exceptions.py` & `pyqt-autotest-0.2.1/pyqt_autotest/core/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,69 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List
-
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-from pyqt_autotest.qt.top_level_widgets import clear_top_level_widgets, get_top_level_widget_list_as_str
-from pyqt_autotest.utilities.print_colors import PrintColors
-
-"""
-Errors that occur due to invalid data or an setup being passed into pyqt-autotest.
-"""
-
-
-class SetupError(Exception):
-    base_message: str = "\tAn invalid widget setup has been detected, please correct the following:\n\n    "
-    class_message: str = ""
-
-    def report(self):
-        messages = [f"{PrintColors.ERROR}", self.base_message, self.class_message, f"{PrintColors.END}"]
-        print("".join(messages))
-        JSONResultsDict().save_run_result(ExitState.Error, messages)
-
-
-class ActionDoesNotExist(SetupError):
-    class_message: str = "\t\tAn action provided in the RepeatableAutoTest does not exist."
-
-
-class WidgetDoesNotExist(SetupError):
-    class_message: str = "\t\tA widget provided in the RepeatableAutoTest does not exist."
-
-
-class WidgetNotProvidedError(SetupError):
-    class_message: str = "\t\tThe provided user class does not implement a 'self.widget' member which is a QWidget."
-
-
-class NoEnabledChildrenWidgetsError(SetupError):
-    class_message: str = "\t\tThe provided widget does not contain any children widgets which are enabled."
-
-
-"""
-Common errors that are found within a widget.
-"""
-
-
-class WidgetError(Exception):
-    class_message: str = ""
-
-    def report(self, messages: List[str]):
-        print("".join(messages))
-
-    def cleanup(self):
-        pass
-
-
-class CloseWidgetError(WidgetError):
-    class_message: str = "Unexpected top level widget(s) detected after closing your widget:\n\n"
-
-    def report(self):
-        messages = [f"\t{PrintColors.WARNING}", self.class_message,
-                    f"\t\t{get_top_level_widget_list_as_str()}\n{PrintColors.END}"]
-        JSONResultsDict().save_run_result(ExitState.Warning, messages)
-        super().report(messages)
-
-    def cleanup(self):
-        clear_top_level_widgets()
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List
+
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+from pyqt_autotest.qt.top_level_widgets import clear_top_level_widgets, get_top_level_widget_list_as_str
+from pyqt_autotest.utilities.print_colors import PrintColors
+
+"""
+Errors that occur due to invalid data or an setup being passed into pyqt-autotest.
+"""
+
+
+class SetupError(Exception):
+    base_message: str = "\tAn invalid widget setup has been detected, please correct the following:\n\n    "
+    class_message: str = ""
+
+    def report(self):
+        messages = [f"{PrintColors.ERROR}", self.base_message, self.class_message, f"{PrintColors.END}"]
+        print("".join(messages))
+        JSONResultsDict().save_run_result(ExitState.Error, messages)
+
+
+class ActionDoesNotExist(SetupError):
+    class_message: str = "\t\tAn action provided in the RepeatableAutoTest does not exist."
+
+
+class WidgetDoesNotExist(SetupError):
+    class_message: str = "\t\tA widget provided in the RepeatableAutoTest does not exist."
+
+
+class WidgetNotProvidedError(SetupError):
+    class_message: str = "\t\tThe provided user class does not implement a 'self.widget' member which is a QWidget."
+
+
+class NoEnabledChildrenWidgetsError(SetupError):
+    class_message: str = "\t\tThe provided widget does not contain any children widgets which are enabled."
+
+
+"""
+Common errors that are found within a widget.
+"""
+
+
+class WidgetError(Exception):
+    class_message: str = ""
+
+    def report(self, messages: List[str]):
+        print("".join(messages))
+
+    def cleanup(self):
+        pass
+
+
+class CloseWidgetError(WidgetError):
+    class_message: str = "Unexpected top level widget(s) detected after closing your widget:\n\n"
+
+    def report(self):
+        messages = [
+            f"\t{PrintColors.WARNING}",
+            self.class_message,
+            f"\t\t{get_top_level_widget_list_as_str()}\n{PrintColors.END}",
+        ]
+        JSONResultsDict().save_run_result(ExitState.Warning, messages)
+        super().report(messages)
+
+    def cleanup(self):
+        clear_top_level_widgets()
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/README.md` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-To try this usage example, you will need to first install the package on the [transcriber repository](https://github.com/ewancook/transcriber).
-
-This usage example can be executed from the command line as follows:
-
-```sh
-autotest -R test_ComplexRandomTest -n 5 -a 10 -w 100
-```
-
-This test uncovered a QThread termination problem in the transcriber when closing the widget:
-
-```sh
-$ autotest -R test_ComplexRandomTest -n 5 -a 10 -w 100
-Running... (1/5): 100%|########################################################|
-QThread: Destroyed while thread is still running
-```
+To try this usage example, you will need to first install the package on the [transcriber repository](https://github.com/ewancook/transcriber).
+
+This usage example can be executed from the command line as follows:
+
+```sh
+autotest -R test_ComplexRandomTest -n 5 -a 10 -w 100
+```
+
+This test uncovered a QThread termination problem in the transcriber when closing the widget:
+
+```sh
+$ autotest -R test_ComplexRandomTest -n 5 -a 10 -w 100
+Running... (1/5): 100%|########################################################|
+QThread: Destroyed while thread is still running
+```
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/complex/test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/complex/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from transcriber.transcriber import Transcriber
-
-from pyqt_autotest.core.action import Action
-from pyqt_autotest.random_auto_test import RandomAutoTest
-
-from PyQt5.QtCore import Qt, QPoint
-from PyQt5.QtTest import QTest
-from PyQt5.QtWidgets import QCheckBox, QLineEdit, QSpinBox
-
-
-class ComplexRandomTest(RandomAutoTest):
-
-    def setup_options(self):
-        extra_actions = {
-            "Key text": lambda widget: QTest.keyClicks(widget, "dummy text"),
-            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
-                                                                    pos=QPoint(2, widget.height() / 2))
-        }
-        extra_widget_actions = {
-            QCheckBox: ["Left click in centre"],
-            QLineEdit: ["Key text"],
-            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
-        }
-
-        self.options.actions.update(extra_actions)
-        self.options.widget_actions.update(extra_widget_actions)
-
-        self.options.number_of_runs = 1
-        self.options.number_of_actions = 10
-        self.options.wait_time = 300  # milliseconds
-
-    def setup_widget(self):
-        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
-        self.widget = Transcriber()
-
-        # TODO It would be even better to load data before the test begins
+from transcriber.transcriber import Transcriber
+
+from pyqt_autotest.core.action import Action
+from pyqt_autotest.random_auto_test import RandomAutoTest
+
+from PyQt5.QtCore import Qt, QPoint
+from PyQt5.QtTest import QTest
+from PyQt5.QtWidgets import QCheckBox, QLineEdit, QSpinBox
+
+
+class ComplexRandomTest(RandomAutoTest):
+    def setup_options(self):
+        extra_actions = {
+            "Key text": lambda widget: QTest.keyClicks(widget, "dummy text"),
+            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton, pos=QPoint(2, widget.height() / 2)),
+        }
+        extra_widget_actions = {
+            QCheckBox: ["Left click in centre"],
+            QLineEdit: ["Key text"],
+            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick],
+        }
+
+        self.options.actions.update(extra_actions)
+        self.options.widget_actions.update(extra_widget_actions)
+
+        self.options.number_of_runs = 1
+        self.options.number_of_actions = 10
+        self.options.wait_time = 300  # milliseconds
+
+    def setup_widget(self):
+        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
+        self.widget = Transcriber()
+
+        # TODO It would be even better to load data before the test begins
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/README.md` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-To try this usage example, you will need to first install the package on the [N-Body-Simulations github repository](https://github.com/robertapplin/N-Body-Simulations).
-
-This usage example can be executed from the command line as follows:
-
-```sh
-autotest -R test_ModerateRandomTest -n 5 -a 10 -w 300
-```
-
-This test uncovered a previously unknown issue where closing the main widget would leave behind some widgets:
-
-```sh
-$ autotest -R test_ModerateRandomTest -n 5 -a 10 -w 300
-Running... (1/5): 100%|########################################################|
-An exception occurred, please correct the following:
-
-    Unexpected top level widget(s) detected after closing your widget:
-    ['QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget']
-```
+To try this usage example, you will need to first install the package on the [N-Body-Simulations github repository](https://github.com/robertapplin/N-Body-Simulations).
+
+This usage example can be executed from the command line as follows:
+
+```sh
+autotest -R test_ModerateRandomTest -n 5 -a 10 -w 300
+```
+
+This test uncovered a previously unknown issue where closing the main widget would leave behind some widgets:
+
+```sh
+$ autotest -R test_ModerateRandomTest -n 5 -a 10 -w 300
+Running... (1/5): 100%|########################################################|
+An exception occurred, please correct the following:
+
+    Unexpected top level widget(s) detected after closing your widget:
+    ['QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget', 'QWidget']
+```
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/moderate/test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/moderate/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from os.path import abspath, dirname, join
-
-from n_body_simulations.qt.model import NBodySimulationsModel
-from n_body_simulations.qt.presenter import NBodySimulationsPresenter
-from n_body_simulations.qt.view import NBodySimulationsView
-
-from pyqt_autotest.random_auto_test import RandomAutoTest
-
-FILENAME = "three-body-parameters.txt"
-
-
-class ModerateRandomTest(RandomAutoTest):
-
-    def setup_options(self):
-        self.options.number_of_runs = 2
-        self.options.number_of_actions = 10
-        self.options.wait_time = 1000  # milliseconds
-
-    def setup_widget(self):
-        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
-        self.widget = NBodySimulationsView()
-
-        self.model = NBodySimulationsModel()
-        self.presenter = NBodySimulationsPresenter(self.widget, self.model)
-
-        # Load a project file into the widget to make the testing more interesting
-        project_file = join(dirname(abspath(__file__)), FILENAME)
-        self.presenter._load_project(project_file)
+from os.path import abspath, dirname, join
+
+from n_body_simulations.qt.model import NBodySimulationsModel
+from n_body_simulations.qt.presenter import NBodySimulationsPresenter
+from n_body_simulations.qt.view import NBodySimulationsView
+
+from pyqt_autotest.random_auto_test import RandomAutoTest
+
+FILENAME = "three-body-parameters.txt"
+
+
+class ModerateRandomTest(RandomAutoTest):
+    def setup_options(self):
+        self.options.number_of_runs = 2
+        self.options.number_of_actions = 10
+        self.options.wait_time = 1000  # milliseconds
+
+    def setup_widget(self):
+        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
+        self.widget = NBodySimulationsView()
+
+        self.model = NBodySimulationsModel()
+        self.presenter = NBodySimulationsPresenter(self.widget, self.model)
+
+        # Load a project file into the widget to make the testing more interesting
+        project_file = join(dirname(abspath(__file__)), FILENAME)
+        self.presenter._load_project(project_file)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from pyqt_autotest.core.action import Action
-from pyqt_autotest.examples.simple.usercode import UserWidget
-from pyqt_autotest.repeatable_auto_test import RepeatableAutoTest
-
-
-class SimpleRepeatableTest(RepeatableAutoTest):
-
-    def setup_options(self):
-        self.options.number_of_runs = 1
-        self.options.wait_time = 100  # milliseconds
-
-        self.options.sequence_of_actions = [Action.MouseLeftClick, Action.MouseLeftClick, Action.MouseLeftClick]
-        self.options.sequence_of_widgets = ["Success", "Success", "Cause Exception"]
-
-    def setup_widget(self):
-        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
-        self.widget = UserWidget()
+from pyqt_autotest.core.action import Action
+from pyqt_autotest.examples.simple.usercode import UserWidget
+from pyqt_autotest.repeatable_auto_test import RepeatableAutoTest
+
+
+class SimpleRepeatableTest(RepeatableAutoTest):
+    def setup_options(self):
+        self.options.number_of_runs = 1
+        self.options.wait_time = 100  # milliseconds
+
+        self.options.sequence_of_actions = [Action.MouseLeftClick, Action.MouseLeftClick, Action.MouseLeftClick]
+        self.options.sequence_of_widgets = ["Success", "Success", "Cause Exception"]
+
+    def setup_widget(self):
+        # Must instantiate the 'self.widget' member variable, and it must be a QWidget
+        self.widget = UserWidget()
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/repeatable/usercode.py` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/repeatable/usercode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import sys
-
-from PyQt5.QtWidgets import QPushButton, QWidget
-
-
-class UserWidget(QWidget):
-
-    def __init__(self):
-        super(QWidget, self).__init__()
-
-        self.success_button = QPushButton("Success", self)
-        self.cause_exception_button = QPushButton("Cause Exception", self)
-        self.cause_termination_button = QPushButton("Cause Termination", self)
-
-        self.success_button.clicked.connect(self.successful_action)
-        self.cause_exception_button.clicked.connect(self.cause_exception)
-        self.cause_termination_button.clicked.connect(self.cause_termination)
-
-    @staticmethod
-    def successful_action():
-        pass
-
-    def cause_exception(self):
-        raise RuntimeError("This is an exception in the users code.")
-
-    @staticmethod
-    def cause_termination():
-        sys.exit(1)
+import sys
+
+from PyQt5.QtWidgets import QPushButton, QWidget
+
+
+class UserWidget(QWidget):
+    def __init__(self):
+        super(QWidget, self).__init__()
+
+        self.success_button = QPushButton("Success", self)
+        self.cause_exception_button = QPushButton("Cause Exception", self)
+        self.cause_termination_button = QPushButton("Cause Termination", self)
+
+        self.success_button.clicked.connect(self.successful_action)
+        self.cause_exception_button.clicked.connect(self.cause_exception)
+        self.cause_termination_button.clicked.connect(self.cause_termination)
+
+    @staticmethod
+    def successful_action():
+        pass
+
+    def cause_exception(self):
+        raise RuntimeError("This is an exception in the users code.")
+
+    @staticmethod
+    def cause_termination():
+        sys.exit(1)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/examples/simple/usercode.py` & `pyqt-autotest-0.2.1/pyqt_autotest/examples/simple/usercode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import sys
-
-from PyQt5.QtWidgets import QPushButton, QWidget
-
-
-class UserWidget(QWidget):
-
-    def __init__(self):
-        super(QWidget, self).__init__()
-
-        self.success_button = QPushButton("Success", self)
-        self.cause_exception_button = QPushButton("Cause Exception", self)
-        self.cause_termination_button = QPushButton("Cause Termination", self)
-
-        self.success_button.clicked.connect(self.successful_action)
-        self.cause_exception_button.clicked.connect(self.cause_exception)
-        self.cause_termination_button.clicked.connect(self.cause_termination)
-
-    @staticmethod
-    def successful_action():
-        pass
-
-    def cause_exception(self):
-        raise RuntimeError("This is an exception in the users code.")
-
-    @staticmethod
-    def cause_termination():
-        sys.exit(1)
+import sys
+
+from PyQt5.QtWidgets import QPushButton, QWidget
+
+
+class UserWidget(QWidget):
+    def __init__(self):
+        super(QWidget, self).__init__()
+
+        self.success_button = QPushButton("Success", self)
+        self.cause_exception_button = QPushButton("Cause Exception", self)
+        self.cause_termination_button = QPushButton("Cause Termination", self)
+
+        self.success_button.clicked.connect(self.successful_action)
+        self.cause_exception_button.clicked.connect(self.cause_exception)
+        self.cause_termination_button.clicked.connect(self.cause_termination)
+
+    @staticmethod
+    def successful_action():
+        pass
+
+    def cause_exception(self):
+        raise RuntimeError("This is an exception in the users code.")
+
+    @staticmethod
+    def cause_termination():
+        sys.exit(1)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/qt/application.py` & `pyqt-autotest-0.2.1/pyqt_autotest/qt/application.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-import atexit
-import sys
-import traceback
-
-from PyQt5.sip import delete
-from PyQt5.QtWidgets import QApplication
-
-
-# Hold on to QAPP reference to avoid garbage collection
-_QAPP = QApplication.instance()
-
-
-@atexit.register
-def cleanup_qapp_ref():
-    """
-    Remove the global reference to the QApplication object here
-    """
-    global _QAPP
-    if _QAPP is not None:
-        delete(_QAPP)
-    del _QAPP
-
-
-def get_application(name=""):
-    """
-    Initialise and return the global application object
-    :param name: Optional application name
-    :return: Global appliction object
-    """
-    global _QAPP
-
-    def exception_handler(exctype, value, tb):
-        traceback.print_exception(exctype, value, tb)
-        sys.exit(1)
-
-    if _QAPP is None:
-        _QAPP = QApplication([name])
-        sys.excepthook = exception_handler
-
-    return _QAPP
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+import atexit
+import sys
+import traceback
+
+from PyQt5.sip import delete
+from PyQt5.QtWidgets import QApplication
+
+
+# Hold on to QAPP reference to avoid garbage collection
+_QAPP = QApplication.instance()
+
+
+@atexit.register
+def cleanup_qapp_ref():
+    """
+    Remove the global reference to the QApplication object here
+    """
+    global _QAPP
+    if _QAPP is not None:
+        delete(_QAPP)
+    del _QAPP
+
+
+def get_application(name=""):
+    """
+    Initialise and return the global application object
+    :param name: Optional application name
+    :return: Global appliction object
+    """
+    global _QAPP
+
+    def exception_handler(exctype, value, tb):
+        traceback.print_exception(exctype, value, tb)
+        sys.exit(1)
+
+    if _QAPP is None:
+        _QAPP = QApplication([name])
+        sys.excepthook = exception_handler
+
+    return _QAPP
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/qt/modal_unblocker.py` & `pyqt-autotest-0.2.1/pyqt_autotest/qt/modal_unblocker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from PyQt5.QtCore import QObject, Qt
-from PyQt5.QtWidgets import QApplication, QFileDialog
-
-WINDOW_BLOCKED_CODE = 103
-
-
-class WindowUnblockFilter(QObject):
-    """
-    An event filter class to close any modal widgets which are blocking further processing.
-    """
-
-    def eventFilter(self, obj,  event):
-        # QEvent::WindowBlocked - The window is blocked by a modal dialog
-        if event.type() == WINDOW_BLOCKED_CODE:
-            close_modals_if_exist(QFileDialog)
-
-        return super().eventFilter(obj, event)
-
-
-def close_modals_if_exist(widget_type: type) -> None:
-    """Close any top level widgets that are blocking further actions, and have a specific widget type."""
-    for widget in QApplication.topLevelWidgets():
-        if widget.windowModality() == 2 and isinstance(widget, widget_type):
-            widget.setAttribute(Qt.WA_DeleteOnClose)
-            widget.close()
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from PyQt5.QtCore import QObject, Qt
+from PyQt5.QtWidgets import QApplication, QFileDialog
+
+WINDOW_BLOCKED_CODE = 103
+
+
+class WindowUnblockFilter(QObject):
+    """
+    An event filter class to close any modal widgets which are blocking further processing.
+    """
+
+    def eventFilter(self, obj, event):
+        # QEvent::WindowBlocked - The window is blocked by a modal dialog
+        if event.type() == WINDOW_BLOCKED_CODE:
+            close_modals_if_exist(QFileDialog)
+
+        return super().eventFilter(obj, event)
+
+
+def close_modals_if_exist(widget_type: type) -> None:
+    """Close any top level widgets that are blocking further actions, and have a specific widget type."""
+    for widget in QApplication.topLevelWidgets():
+        if widget.windowModality() == 2 and isinstance(widget, widget_type):
+            widget.setAttribute(Qt.WA_DeleteOnClose)
+            widget.close()
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/qt/top_level_widgets.py` & `pyqt-autotest-0.2.1/pyqt_autotest/qt/top_level_widgets.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List, Tuple
-
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QApplication, QWidget
-
-EXCLUDE_TOP_LEVEL_CLASSES = ["QComboBoxPrivateContainer"]
-
-
-def get_widget_class_and_text(widget: QWidget) -> Tuple[str, str]:
-    """Return the widgets class and text."""
-    text = widget.text() if callable(getattr(widget, "text", None)) else ""
-    class_name = widget.metaObject().className()
-    return class_name, text
-
-
-def get_top_level_widget_list_as_str() -> str:
-    """Returns a string listing the top level widgets."""
-    widget_strs = []
-    for widget in QApplication.topLevelWidgets():
-        class_name, text = get_widget_class_and_text(widget)
-        if class_name not in EXCLUDE_TOP_LEVEL_CLASSES:
-            widget_strs.append(class_name if text == "" else f"{class_name} with text '{text}'")
-
-    return "\n\t\t".join(widget_strs)
-
-
-def get_top_level_widget_classes() -> List[str]:
-    """Returns a list of top level widget class names."""
-    top_level_widget_classes = []
-    for widget in QApplication.topLevelWidgets():
-        class_name = widget.metaObject().className()
-        if class_name not in EXCLUDE_TOP_LEVEL_CLASSES:
-            top_level_widget_classes.append(class_name)
-    return top_level_widget_classes
-
-
-def clear_top_level_widgets() -> None:
-    """Close and delete all existing top level widgets."""
-    for widget in QApplication.topLevelWidgets():
-        widget.setAttribute(Qt.WA_DeleteOnClose)
-        widget.close()
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List, Tuple
+
+from PyQt5.QtCore import Qt
+from PyQt5.QtWidgets import QApplication, QWidget
+
+EXCLUDE_TOP_LEVEL_CLASSES = ["QComboBoxPrivateContainer"]
+
+
+def get_widget_class_and_text(widget: QWidget) -> Tuple[str, str]:
+    """Return the widgets class and text."""
+    text = widget.text() if callable(getattr(widget, "text", None)) else ""
+    class_name = widget.metaObject().className()
+    return class_name, text
+
+
+def get_top_level_widget_list_as_str() -> str:
+    """Returns a string listing the top level widgets."""
+    widget_strs = []
+    for widget in QApplication.topLevelWidgets():
+        class_name, text = get_widget_class_and_text(widget)
+        if class_name not in EXCLUDE_TOP_LEVEL_CLASSES:
+            widget_strs.append(class_name if text == "" else f"{class_name} with text '{text}'")
+
+    return "\n\t\t".join(widget_strs)
+
+
+def get_top_level_widget_classes() -> List[str]:
+    """Returns a list of top level widget class names."""
+    top_level_widget_classes = []
+    for widget in QApplication.topLevelWidgets():
+        class_name = widget.metaObject().className()
+        if class_name not in EXCLUDE_TOP_LEVEL_CLASSES:
+            top_level_widget_classes.append(class_name)
+    return top_level_widget_classes
+
+
+def clear_top_level_widgets() -> None:
+    """Close and delete all existing top level widgets."""
+    for widget in QApplication.topLevelWidgets():
+        widget.setAttribute(Qt.WA_DeleteOnClose)
+        widget.close()
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/qt/widgets.py` & `pyqt-autotest-0.2.1/pyqt_autotest/qt/widgets.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List
-
-from pyqt_autotest.core.exceptions import NoEnabledChildrenWidgetsError
-
-from PyQt5.QtWidgets import QWidget
-
-
-def get_widget_identifiers(widget: QWidget) -> List[str]:
-    """Return all the identifiers for a widget"""
-    widget_identifiers = []
-    if callable(getattr(widget, "text", None)):
-        widget_identifiers.append(widget.text())
-    widget_identifiers.append(widget.accessibleName())
-    widget_identifiers.append(widget.objectName())
-    widget_identifiers.append(widget.metaObject().className())
-    # Remove empty strings
-    return [identifier.strip() for identifier in widget_identifiers if identifier.strip() != ""]
-
-
-def get_widget_name(widget: QWidget) -> str:
-    """Returns a string to represent the name of a widget. If a name can't be found, its className is returned."""
-    if callable(getattr(widget, "text", None)) and widget.text().strip() != "":
-        return widget.text()
-    if widget.accessibleName() != "":
-        return widget.accessibleName()
-    if widget.objectName() != "":
-        return widget.objectName()
-    return widget.metaObject().className()
-
-
-def get_widget_from_str(all_widgets: List[QWidget], widget_name: str) -> QWidget:
-    """Search for a widget by name and return it."""
-    for widget in all_widgets:
-        if widget_name in get_widget_identifiers(widget):
-            return widget
-    return None
-
-
-def find_child_widgets(parent_widget: QWidget, available_types: List[QWidget]) -> List[QWidget]:
-    """Find the children widgets within the user's widget."""
-    children_widgets = []
-    for widget_type in available_types:
-        children_widgets.extend(parent_widget.findChildren(widget_type))
-    # Only return the widgets which are enabled
-    enabled_widgets = [widget for widget in children_widgets if widget.isEnabled()]
-    if len(enabled_widgets) == 0:
-        raise NoEnabledChildrenWidgetsError()
-    return enabled_widgets
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List
+
+from pyqt_autotest.core.exceptions import NoEnabledChildrenWidgetsError
+
+from PyQt5.QtWidgets import QWidget
+
+
+def get_widget_identifiers(widget: QWidget) -> List[str]:
+    """Return all the identifiers for a widget"""
+    widget_identifiers = []
+    if callable(getattr(widget, "text", None)):
+        widget_identifiers.append(widget.text())
+    widget_identifiers.append(widget.accessibleName())
+    widget_identifiers.append(widget.objectName())
+    widget_identifiers.append(widget.metaObject().className())
+    # Remove empty strings
+    return [identifier.strip() for identifier in widget_identifiers if identifier.strip() != ""]
+
+
+def get_widget_name(widget: QWidget) -> str:
+    """Returns a string to represent the name of a widget. If a name can't be found, its className is returned."""
+    if callable(getattr(widget, "text", None)) and widget.text().strip() != "":
+        return widget.text()
+    if widget.accessibleName() != "":
+        return widget.accessibleName()
+    if widget.objectName() != "":
+        return widget.objectName()
+    return widget.metaObject().className()
+
+
+def get_widget_from_str(all_widgets: List[QWidget], widget_name: str) -> QWidget:
+    """Search for a widget by name and return it."""
+    for widget in all_widgets:
+        if widget_name in get_widget_identifiers(widget):
+            return widget
+    return None
+
+
+def find_child_widgets(parent_widget: QWidget, available_types: List[QWidget]) -> List[QWidget]:
+    """Find the children widgets within the user's widget."""
+    children_widgets = []
+    for widget_type in available_types:
+        children_widgets.extend(parent_widget.findChildren(widget_type))
+    # Only return the widgets which are enabled
+    enabled_widgets = [widget for widget in children_widgets if widget.isEnabled()]
+    if len(enabled_widgets) == 0:
+        raise NoEnabledChildrenWidgetsError()
+    return enabled_widgets
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/random_auto_test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/random_auto_test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List, Tuple
-
-from pyqt_autotest.core.action import Action
-from pyqt_autotest.core.auto_test import _AutoTest
-from pyqt_autotest.qt.widgets import find_child_widgets, get_widget_name
-from pyqt_autotest.utilities.randomizer import get_random_action, get_random_widget
-
-from PyQt5.QtWidgets import QWidget
-
-
-class RandomAutoTest(_AutoTest):
-    """
-    An auto test class for performing random actions on random widgets within a user widget.
-    """
-
-    def _test_type(self) -> str:
-        """Returns a string to represent the type of the test."""
-        return "RandomAutoTest"
-
-    def _get_number_of_actions(self) -> int:
-        """Returns the number of actions for this test."""
-        return self.options.number_of_actions
-
-    def _get_child_widgets(self) -> List[QWidget]:
-        """Returns the child widgets which are required for a run."""
-        return find_child_widgets(self.widget, list(self.options.widget_actions.keys()))
-
-    def _get_action_name_widget_name_and_widget(self, _, all_widgets: List[QWidget]) -> Tuple[Action, str, QWidget]:
-        """Returns the action, and widget to perform an action on."""
-        widget = get_random_widget(all_widgets)
-        widget_name = get_widget_name(widget)
-        action_name = get_random_action(type(widget), self.options.widget_actions)
-        return action_name, widget_name, widget
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List, Tuple
+
+from pyqt_autotest.core.action import Action
+from pyqt_autotest.core.auto_test import _AutoTest
+from pyqt_autotest.qt.widgets import find_child_widgets, get_widget_name
+from pyqt_autotest.utilities.randomizer import get_random_action, get_random_widget
+
+from PyQt5.QtWidgets import QWidget
+
+
+class RandomAutoTest(_AutoTest):
+    """
+    An auto test class for performing random actions on random widgets within a user widget.
+    """
+
+    def _test_type(self) -> str:
+        """Returns a string to represent the type of the test."""
+        return "RandomAutoTest"
+
+    def _get_number_of_actions(self) -> int:
+        """Returns the number of actions for this test."""
+        return self.options.number_of_actions
+
+    def _get_child_widgets(self) -> List[QWidget]:
+        """Returns the child widgets which are required for a run."""
+        return find_child_widgets(self.widget, list(self.options.widget_actions.keys()))
+
+    def _get_action_name_widget_name_and_widget(self, _, all_widgets: List[QWidget]) -> Tuple[Action, str, QWidget]:
+        """Returns the action, and widget to perform an action on."""
+        widget = get_random_widget(all_widgets)
+        widget_name = get_widget_name(widget)
+        action_name = get_random_action(type(widget), self.options.widget_actions)
+        return action_name, widget_name, widget
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/repeatable_auto_test.py` & `pyqt-autotest-0.2.1/pyqt_autotest/repeatable_auto_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from typing import List, Tuple
-
-from pyqt_autotest.core.action import Action
-from pyqt_autotest.core.auto_test import _AutoTest
-from pyqt_autotest.qt.widgets import find_child_widgets, get_widget_from_str
-
-from PyQt5.QtWidgets import QWidget
-
-
-class RepeatableAutoTest(_AutoTest):
-    """
-    An auto test class for performing a repeatable sequence of actions on widgets within a user widget.
-    """
-
-    def _test_type(self) -> str:
-        """Returns a string to represent the type of the test."""
-        return "RepeatableAutoTest"
-
-    def _get_number_of_actions(self) -> int:
-        """Returns the number of actions for this test."""
-        return len(self.options.sequence_of_actions)
-
-    def _get_child_widgets(self) -> List[QWidget]:
-        """Returns the child widgets which are required for a run."""
-        return find_child_widgets(self.widget, [QWidget])
-
-    def _get_action_name_widget_name_and_widget(self, action_number: int,
-                                                all_widgets: List[QWidget]) -> Tuple[Action, str, QWidget]:
-        """Returns the action, and widget to perform an action on."""
-        action_name = self.options.sequence_of_actions[action_number]
-        widget_name = self.options.sequence_of_widgets[action_number]
-        widget = get_widget_from_str(all_widgets, widget_name)
-        return action_name, widget_name, widget
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from typing import List, Tuple
+
+from pyqt_autotest.core.action import Action
+from pyqt_autotest.core.auto_test import _AutoTest
+from pyqt_autotest.qt.widgets import find_child_widgets, get_widget_from_str
+
+from PyQt5.QtWidgets import QWidget
+
+
+class RepeatableAutoTest(_AutoTest):
+    """
+    An auto test class for performing a repeatable sequence of actions on widgets within a user widget.
+    """
+
+    def _test_type(self) -> str:
+        """Returns a string to represent the type of the test."""
+        return "RepeatableAutoTest"
+
+    def _get_number_of_actions(self) -> int:
+        """Returns the number of actions for this test."""
+        return len(self.options.sequence_of_actions)
+
+    def _get_child_widgets(self) -> List[QWidget]:
+        """Returns the child widgets which are required for a run."""
+        return find_child_widgets(self.widget, [QWidget])
+
+    def _get_action_name_widget_name_and_widget(
+        self, action_number: int, all_widgets: List[QWidget]
+    ) -> Tuple[Action, str, QWidget]:
+        """Returns the action, and widget to perform an action on."""
+        action_name = self.options.sequence_of_actions[action_number]
+        widget_name = self.options.sequence_of_widgets[action_number]
+        widget = get_widget_from_str(all_widgets, widget_name)
+        return action_name, widget_name, widget
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/results/json_results_dict.py` & `pyqt-autotest-0.2.1/pyqt_autotest/results/json_results_dict.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,115 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from json import dump
-from typing import List
-
-from pyqt_autotest.cli.options import Options
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.result_schema import (AUTO_TEST_TYPE_KEY, IMPORTS_KEY, NUMBER_OF_ACTIONS_KEY,
-                                                 NUMBER_OF_RUNS_KEY, RESULT_SCHEMA, RUN_ACTIONS_KEY, RUN_EXIT_STATE_KEY,
-                                                 RUN_MESSAGE_KEY, RUN_WIDGETS_KEY, RUNS_KEY, SETUP_KEY, WAIT_TIME_KEY)
-from pyqt_autotest.utilities.singleton import Singleton
-
-
-class JSONResultsDict(dict, metaclass=Singleton):
-
-    _cautious: bool = False
-
-    _test_running: bool = False
-    _active_test_name: str = None
-
-    _output_filepath: str = None
-
-    @property
-    def cautious(self) -> bool:
-        """Returns the cautious flag value."""
-        return self._cautious
-
-    @cautious.setter
-    def cautious(self, cautious: bool) -> None:
-        """Sets the cautious flag to true or false."""
-        self._cautious = cautious
-
-    @property
-    def output_filepath(self) -> str:
-        """Returns the output filepath of the file to save."""
-        return self._output_filepath
-
-    @output_filepath.setter
-    def output_filepath(self, filepath: str) -> None:
-        """Sets the output filepath of the file to save."""
-        self._output_filepath = filepath
-
-    def init_test(self, test_type: str, import_str: str, setup_str: str, test_name: str, options: Options) -> None:
-        """Initializes a new test result dictionary."""
-        new_test = {
-            AUTO_TEST_TYPE_KEY: test_type,
-            IMPORTS_KEY: import_str,
-            SETUP_KEY: setup_str,
-            NUMBER_OF_RUNS_KEY: options.number_of_runs,
-            NUMBER_OF_ACTIONS_KEY: options.number_of_actions,
-            WAIT_TIME_KEY: options.wait_time,
-            RUNS_KEY: []
-        }
-        self._active_test_name = test_name
-        self[self._active_test_name] = new_test
-
-    def init_run(self) -> None:
-        """Initializes a new run result dictionary."""
-        new_run = {
-            RUN_WIDGETS_KEY: [],
-            RUN_ACTIONS_KEY: [],
-            # If the run terminates, we want to record that there was an error, so set this as the initial state.
-            RUN_EXIT_STATE_KEY: "Error",
-            RUN_MESSAGE_KEY: "The run terminated before completing. Please use the -v, --verbose flag to debug."
-        }
-        self[self._active_test_name][RUNS_KEY].append(new_run)
-        self._test_running = True
-
-    def is_running(self) -> bool:
-        """Returns true if a test run is currently active."""
-        return self._test_running
-
-    def save_run_result(self, exit_state: ExitState, message: List[str] = "") -> None:
-        """Stores the run as a result when the run ends."""
-        if self._active_test_name not in self:
-            raise RuntimeError(f"Something went wrong, the '{self._active_test_name}' property could not be found.")
-        if RUNS_KEY not in self[self._active_test_name]:
-            raise RuntimeError(f"Something went wrong, the '{RUNS_KEY}' property could not be found.")
-
-        self[self._active_test_name][RUNS_KEY][-1][RUN_EXIT_STATE_KEY] = exit_state.value
-        self[self._active_test_name][RUNS_KEY][-1][RUN_MESSAGE_KEY] = f"\n{''.join(message)}"
-
-        # Allow this to fail if the results don't match the schema
-        RESULT_SCHEMA.validate(self[self._active_test_name])
-
-        self._test_running = False
-
-    def save_event(self, widget_name: str, event_name: str) -> None:
-        """Stores an event in the active run."""
-        self[self._active_test_name][RUNS_KEY][-1][RUN_WIDGETS_KEY].append(widget_name)
-        self[self._active_test_name][RUNS_KEY][-1][RUN_ACTIONS_KEY].append(event_name)
-
-        instruction_number = len(self[self._active_test_name][RUNS_KEY][-1][RUN_WIDGETS_KEY])
-        print(f"\t\t{instruction_number}. {event_name} the '{widget_name}' widget")
-
-        # If in cautious mode, save the results after each event is recorded. This is expensive, but might be necessary
-        # to find a bug causing a segmentation or termination fault.
-        if self._cautious:
-            self.save_to_file()
-
-    def save_to_file(self):
-        """Saves the results in this singleton to a json file."""
-        if self.output_filepath is not None:
-            with open(self.output_filepath, "w") as out_file:
-                dump(self, out_file, indent=2)
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from json import dump
+from typing import List
+
+from pyqt_autotest.cli.options import Options
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.result_schema import (
+    AUTO_TEST_TYPE_KEY,
+    IMPORTS_KEY,
+    NUMBER_OF_ACTIONS_KEY,
+    NUMBER_OF_RUNS_KEY,
+    RESULT_SCHEMA,
+    RUN_ACTIONS_KEY,
+    RUN_EXIT_STATE_KEY,
+    RUN_MESSAGE_KEY,
+    RUN_WIDGETS_KEY,
+    RUNS_KEY,
+    SETUP_KEY,
+    WAIT_TIME_KEY,
+)
+from pyqt_autotest.utilities.singleton import Singleton
+
+
+class JSONResultsDict(dict, metaclass=Singleton):
+    _cautious: bool = False
+
+    _test_running: bool = False
+    _active_test_name: str = None
+
+    _output_filepath: str = None
+
+    @property
+    def cautious(self) -> bool:
+        """Returns the cautious flag value."""
+        return self._cautious
+
+    @cautious.setter
+    def cautious(self, cautious: bool) -> None:
+        """Sets the cautious flag to true or false."""
+        self._cautious = cautious
+
+    @property
+    def output_filepath(self) -> str:
+        """Returns the output filepath of the file to save."""
+        return self._output_filepath
+
+    @output_filepath.setter
+    def output_filepath(self, filepath: str) -> None:
+        """Sets the output filepath of the file to save."""
+        self._output_filepath = filepath
+
+    def init_test(self, test_type: str, import_str: str, setup_str: str, test_name: str, options: Options) -> None:
+        """Initializes a new test result dictionary."""
+        new_test = {
+            AUTO_TEST_TYPE_KEY: test_type,
+            IMPORTS_KEY: import_str,
+            SETUP_KEY: setup_str,
+            NUMBER_OF_RUNS_KEY: options.number_of_runs,
+            NUMBER_OF_ACTIONS_KEY: options.number_of_actions,
+            WAIT_TIME_KEY: options.wait_time,
+            RUNS_KEY: [],
+        }
+        self._active_test_name = test_name
+        self[self._active_test_name] = new_test
+
+    def init_run(self) -> None:
+        """Initializes a new run result dictionary."""
+        new_run = {
+            RUN_WIDGETS_KEY: [],
+            RUN_ACTIONS_KEY: [],
+            # If the run terminates, we want to record that there was an error, so set this as the initial state.
+            RUN_EXIT_STATE_KEY: "Error",
+            RUN_MESSAGE_KEY: "The run terminated before completing. Please use the -v, --verbose flag to debug.",
+        }
+        self[self._active_test_name][RUNS_KEY].append(new_run)
+        self._test_running = True
+
+    def is_running(self) -> bool:
+        """Returns true if a test run is currently active."""
+        return self._test_running
+
+    def save_run_result(self, exit_state: ExitState, message: List[str] = "") -> None:
+        """Stores the run as a result when the run ends."""
+        if self._active_test_name not in self:
+            raise RuntimeError(f"Something went wrong, the '{self._active_test_name}' property could not be found.")
+        if RUNS_KEY not in self[self._active_test_name]:
+            raise RuntimeError(f"Something went wrong, the '{RUNS_KEY}' property could not be found.")
+
+        self[self._active_test_name][RUNS_KEY][-1][RUN_EXIT_STATE_KEY] = exit_state.value
+        self[self._active_test_name][RUNS_KEY][-1][RUN_MESSAGE_KEY] = f"\n{''.join(message)}"
+
+        # Allow this to fail if the results don't match the schema
+        RESULT_SCHEMA.validate(self[self._active_test_name])
+
+        self._test_running = False
+
+    def save_event(self, widget_name: str, event_name: str) -> None:
+        """Stores an event in the active run."""
+        self[self._active_test_name][RUNS_KEY][-1][RUN_WIDGETS_KEY].append(widget_name)
+        self[self._active_test_name][RUNS_KEY][-1][RUN_ACTIONS_KEY].append(event_name)
+
+        instruction_number = len(self[self._active_test_name][RUNS_KEY][-1][RUN_WIDGETS_KEY])
+        print(f"\t\t{instruction_number}. {event_name} the '{widget_name}' widget")
+
+        # If in cautious mode, save the results after each event is recorded. This is expensive, but might be necessary
+        # to find a bug causing a segmentation or termination fault.
+        if self._cautious:
+            self.save_to_file()
+
+    def save_to_file(self):
+        """Saves the results in this singleton to a json file."""
+        if self.output_filepath is not None:
+            with open(self.output_filepath, "w") as out_file:
+                dump(self, out_file, indent=2)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/results/print_results.py` & `pyqt-autotest-0.2.1/pyqt_autotest/results/print_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-from pyqt_autotest.results.statistic_finder import StatisticFinder
-from pyqt_autotest.utilities.print_colors import PrintColors
-
-
-def print_results(output_filepath: str = "") -> None:
-    """Prints the results of the tests to the terminal."""
-    stat_finder = StatisticFinder(JSONResultsDict())
-    number_of_successes = stat_finder.count_exit_state(ExitState.Success)
-    number_of_warnings = stat_finder.count_exit_state(ExitState.Warning)
-    number_of_errors = stat_finder.count_exit_state(ExitState.Error)
-
-    print(f"Successes ({PrintColors.SUCCESS}{number_of_successes}{PrintColors.END}) | "
-          f"Warnings ({PrintColors.WARNING}{number_of_warnings}{PrintColors.END}) | "
-          f"Errors ({PrintColors.ERROR}{number_of_errors}{PrintColors.END})\n")
-
-    if output_filepath is None:
-        return
-    if output_filepath != "":
-        print(f"A PyQt AutoTest output file has successfully been created:\n\n\t{output_filepath}\n")
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+from pyqt_autotest.results.statistic_finder import StatisticFinder
+from pyqt_autotest.utilities.print_colors import PrintColors
+
+
+def print_results(output_filepath: str = "") -> None:
+    """Prints the results of the tests to the terminal."""
+    stat_finder = StatisticFinder(JSONResultsDict())
+    number_of_successes = stat_finder.count_exit_state(ExitState.Success)
+    number_of_warnings = stat_finder.count_exit_state(ExitState.Warning)
+    number_of_errors = stat_finder.count_exit_state(ExitState.Error)
+
+    print(
+        f"Successes ({PrintColors.SUCCESS}{number_of_successes}{PrintColors.END}) | "
+        f"Warnings ({PrintColors.WARNING}{number_of_warnings}{PrintColors.END}) | "
+        f"Errors ({PrintColors.ERROR}{number_of_errors}{PrintColors.END})\n"
+    )
+
+    if output_filepath is None:
+        return
+    if output_filepath != "":
+        print(f"A PyQt AutoTest output file has successfully been created:\n\n\t{output_filepath}\n")
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/results/result_schema.py` & `pyqt-autotest-0.2.1/pyqt_autotest/results/result_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from schema import And, Schema, Use
-
-AUTO_TEST_TYPE_KEY = "auto_test_type"
-IMPORTS_KEY = "imports"
-SETUP_KEY = "setup"
-NUMBER_OF_RUNS_KEY = "number_of_runs"
-NUMBER_OF_ACTIONS_KEY = "number_of_actions"
-WAIT_TIME_KEY = "wait_time"
-RUNS_KEY = "runs"
-
-RUN_ACTIONS_KEY = "actions"
-RUN_WIDGETS_KEY = "widgets"
-RUN_EXIT_STATE_KEY = "exit_state"
-RUN_MESSAGE_KEY = "message"
-
-# The schema used for validating the results of a single test (with or without multiple runs)
-RESULT_SCHEMA = Schema({
-    AUTO_TEST_TYPE_KEY: And(Use(str)),
-    IMPORTS_KEY: And(Use(str)),
-    SETUP_KEY: And(Use(str)),
-    NUMBER_OF_RUNS_KEY: And(Use(int)),
-    NUMBER_OF_ACTIONS_KEY: And(Use(int)),
-    WAIT_TIME_KEY: And(Use(int)),
-    RUNS_KEY: [
-        {
-            RUN_ACTIONS_KEY: [str],
-            RUN_WIDGETS_KEY: [str],
-            RUN_EXIT_STATE_KEY: And(Use(str)),
-            RUN_MESSAGE_KEY: And(Use(str))
-        }
-    ]
-})
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from schema import And, Schema, Use
+
+AUTO_TEST_TYPE_KEY = "auto_test_type"
+IMPORTS_KEY = "imports"
+SETUP_KEY = "setup"
+NUMBER_OF_RUNS_KEY = "number_of_runs"
+NUMBER_OF_ACTIONS_KEY = "number_of_actions"
+WAIT_TIME_KEY = "wait_time"
+RUNS_KEY = "runs"
+
+RUN_ACTIONS_KEY = "actions"
+RUN_WIDGETS_KEY = "widgets"
+RUN_EXIT_STATE_KEY = "exit_state"
+RUN_MESSAGE_KEY = "message"
+
+# The schema used for validating the results of a single test (with or without multiple runs)
+RESULT_SCHEMA = Schema(
+    {
+        AUTO_TEST_TYPE_KEY: And(Use(str)),
+        IMPORTS_KEY: And(Use(str)),
+        SETUP_KEY: And(Use(str)),
+        NUMBER_OF_RUNS_KEY: And(Use(int)),
+        NUMBER_OF_ACTIONS_KEY: And(Use(int)),
+        WAIT_TIME_KEY: And(Use(int)),
+        RUNS_KEY: [
+            {RUN_ACTIONS_KEY: [str], RUN_WIDGETS_KEY: [str], RUN_EXIT_STATE_KEY: And(Use(str)), RUN_MESSAGE_KEY: And(Use(str))}
+        ],
+    }
+)
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/results/statistic_finder.py` & `pyqt-autotest-0.2.1/pyqt_autotest/results/statistic_finder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from pyqt_autotest.results.exit_state import ExitState
-from pyqt_autotest.results.json_results_dict import JSONResultsDict
-from pyqt_autotest.results.result_schema import RUN_EXIT_STATE_KEY, RUNS_KEY
-
-
-class StatisticFinder:
-
-    def __init__(self, result_dict: JSONResultsDict):
-        self._results_dict = result_dict
-
-    def count_exit_state(self, exit_state: ExitState) -> int:
-        """Count the number of runs with a particular exit state."""
-        return len([run_result for test_result in self._results_dict.values() for run_result in test_result[RUNS_KEY]
-                    if run_result[RUN_EXIT_STATE_KEY] == exit_state.value])
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from pyqt_autotest.results.exit_state import ExitState
+from pyqt_autotest.results.json_results_dict import JSONResultsDict
+from pyqt_autotest.results.result_schema import RUN_EXIT_STATE_KEY, RUNS_KEY
+
+
+class StatisticFinder:
+    def __init__(self, result_dict: JSONResultsDict):
+        self._results_dict = result_dict
+
+    def count_exit_state(self, exit_state: ExitState) -> int:
+        """Count the number of runs with a particular exit state."""
+        return len(
+            [
+                run_result
+                for test_result in self._results_dict.values()
+                for run_result in test_result[RUNS_KEY]
+                if run_result[RUN_EXIT_STATE_KEY] == exit_state.value
+            ]
+        )
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/utilities/randomizer.py` & `pyqt-autotest-0.2.1/pyqt_autotest/utilities/randomizer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-from random import randint
-from typing import Dict, List, Tuple
-
-from pyqt_autotest.core.action import Action
-
-from PyQt5.QtWidgets import QWidget
-
-
-def get_random_widget(widgets: List[Tuple[str, type]]) -> Tuple[str, str]:
-    """Get a random widget and its type."""
-    number_of_widgets = len(widgets)
-    if number_of_widgets > 0:
-        return widgets[randint(0, number_of_widgets - 1)]
-    else:
-        raise RuntimeError("Failed to find any child widgets within your widget.")
-
-
-def get_random_action(widget_type: type, widget_actions: Dict[QWidget, List[Action]]) -> str:
-    """Get a random action to perform on a specific widget type."""
-    actions_for_widget = widget_actions.get(widget_type, [])
-    number_of_actions = len(actions_for_widget)
-    if number_of_actions == 0:
-        raise RuntimeError(f"Failed to find any actions for a widget of type {widget_type}.")
-
-    return actions_for_widget[randint(0, number_of_actions - 1)]
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+from random import randint
+from typing import Dict, List, Tuple
+
+from pyqt_autotest.core.action import Action
+
+from PyQt5.QtWidgets import QWidget
+
+
+def get_random_widget(widgets: List[Tuple[str, type]]) -> Tuple[str, str]:
+    """Get a random widget and its type."""
+    number_of_widgets = len(widgets)
+    if number_of_widgets > 0:
+        return widgets[randint(0, number_of_widgets - 1)]
+    else:
+        raise RuntimeError("Failed to find any child widgets within your widget.")
+
+
+def get_random_action(widget_type: type, widget_actions: Dict[QWidget, List[Action]]) -> str:
+    """Get a random action to perform on a specific widget type."""
+    actions_for_widget = widget_actions.get(widget_type, [])
+    number_of_actions = len(actions_for_widget)
+    if number_of_actions == 0:
+        raise RuntimeError(f"Failed to find any actions for a widget of type {widget_type}.")
+
+    return actions_for_widget[randint(0, number_of_actions - 1)]
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest/utilities/verbosity_controller.py` & `pyqt-autotest-0.2.1/pyqt_autotest/utilities/verbosity_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# Project Repository : https://github.com/robertapplin/pyqt-autotest
-# Authored by Robert Applin, 2022
-import sys
-from io import StringIO
-
-
-class VerbosityController:
-    """
-    A class to control the amount of debug information is output to the terminal.
-    """
-    def __init__(self, verbose: bool):
-        self._verbose = verbose
-
-    def __enter__(self):
-        """When entering a 'with' statement."""
-        if not self._verbose:
-            self.stdout = sys.stdout
-            sys.stdout = StringIO()
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        """When exiting a 'with' statement."""
-        if not self._verbose:
-            sys.stdout = self.stdout
-            self.stdout = None
+# Project Repository : https://github.com/robertapplin/pyqt-autotest
+# Authored by Robert Applin, 2022
+import sys
+from io import StringIO
+
+
+class VerbosityController:
+    """
+    A class to control the amount of debug information is output to the terminal.
+    """
+
+    def __init__(self, verbose: bool):
+        self._verbose = verbose
+
+    def __enter__(self):
+        """When entering a 'with' statement."""
+        if not self._verbose:
+            self.stdout = sys.stdout
+            sys.stdout = StringIO()
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """When exiting a 'with' statement."""
+        if not self._verbose:
+            sys.stdout = self.stdout
+            self.stdout = None
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest.egg-info/PKG-INFO` & `pyqt-autotest-0.2.1/pyqt_autotest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,836 +1,836 @@
-Metadata-Version: 2.1
-Name: pyqt-autotest
-Version: 0.2.0
-Summary: A command line tool for finding system-level bugs that cause a python Qt application to terminate.
-Author-email: Robert Applin <robertapplin.developer@gmail.com>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://github.com/robertapplin/pyqt-autotest
-Project-URL: Bug Tracker, https://github.com/robertapplin/pyqt-autotest/issues
-Keywords: python,qt,random,auto,test
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyqt-autotest ⚙️🧪
-A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
-
-This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
-
-## Table of contents
-* [Installation](#installation)
-* [Setup](#setup)
-* [Options](#options)
-* [Test class](#test-class)
-* [Built-in Actions](#built-in-actions)
-* [Creating your own Actions](#creating-your-own-actions)
-* [Usage](#usage)
-* [Output](#output)
-
-## Installation
-
-This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
-
-```sh
-pip install pyqt-autotest
-```
-
-## Setup
-
-Create a file named `.autotest` in your home directory with the following contents.
-
-```
-[setup]
-search_directories = /path/to/test/directory1/
-                     /path/to/test/directory2/
-output_directory = /path/to/output/directory/
-```
-
-The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
-
-## Options
-
-The following table details the options that can be provided on the command line.
-
-| Option            | Description                                                                                                                                 | Default                      | Command line option     |
-|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
-| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
-| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
-| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
-| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
-| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
-| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
-| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
-| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
-
-## Test class
-
-The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
-
-```py
-from usercode.model import ExampleModel
-from usercode.presenter import ExamplePresenter
-from usercode.view import ExampleView
-
-from pyqt_autotest.random_auto_test import RandomAutoTest
-
-
-class ExampleTest(RandomAutoTest):
-
-    def setup_widget(self):
-        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
-        self.widget = ExampleView()
-
-        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
-        self.model = ExampleModel()
-        self.presenter = ExamplePresenter(self.widget, self.model)
-        
-        # Your test might be more interesting if you first load data into the widget
-        self.presenter.load_data("fake_data_file.dat")
-```
-
-Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
-
-```py
-    def setup_options(self):
-        self.options.number_of_runs = 2
-        self.options.number_of_actions = 15
-        self.options.wait_time = 200  # milliseconds
-```
-
-## Built-in Actions
-
-The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
-
-| Built-in Action       | Description                                               | Python Callable                                          |
-|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
-| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
-| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
-| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
-
-These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
-
-| Widget type       | Built-in Actions      |
-|-------------------|-----------------------|
-| QPushButton       | Action.MouseLeftClick |
-
-## Creating your own Actions
-This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
-
-The following code provides a basic example for how to define your own custom actions:
-
-```py
-    def setup_options(self):
-        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
-        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
-        actions = {
-            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
-            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
-                                                                    pos=QPoint(2, widget.height() / 2))
-        }
-        
-        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
-        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to 
-        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
-        widget_actions = {
-            QCheckBox: ["Left click in centre"],
-            QLineEdit: ["Enter dummy text"],
-            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
-        }
-
-        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
-        self.options.actions = actions
-        self.options.widget_actions = widget_actions
-```
-
-## Usage
-
-It is trivial to run your test class from the command line as follows (depending on its module location):
-
-```sh
-autotest -R ExampleTest
-```
-or with more arguments:
-```
-autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
-```
-
-## Output
-
-An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
+Metadata-Version: 2.1
+Name: pyqt-autotest
+Version: 0.2.1
+Summary: A command line tool for finding system-level bugs that cause a python Qt application to terminate.
+Author-email: Robert Applin <robertapplin.developer@gmail.com>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://github.com/robertapplin/pyqt-autotest
+Project-URL: Bug Tracker, https://github.com/robertapplin/pyqt-autotest/issues
+Keywords: python,qt,random,auto,test
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyqt-autotest ⚙️🧪
+A command line tool for finding system-level bugs that cause a python Qt application to terminate. This is achieved by simulating user actions on a widget using [QtTest](https://doc.qt.io/qt-5/qtest-overview.html).
+
+This tool requires you to provide a python class which inherits from the provided `RandomAutoTest` class. The widget defined inside this class will be opened a specified number of times, and a random selection of actions is performed on the children widgets within the encompassing widget. The result of each run is recorded, and warnings/errors are captured, before a report is generated to provide reliable instructions for how to reproduce a bug.
+
+## Table of contents
+* [Installation](#installation)
+* [Setup](#setup)
+* [Options](#options)
+* [Test class](#test-class)
+* [Built-in Actions](#built-in-actions)
+* [Creating your own Actions](#creating-your-own-actions)
+* [Usage](#usage)
+* [Output](#output)
+
+## Installation
+
+This package can be installed from [PyPI](https://pypi.org/project/pyqt-autotest/) using pip.
+
+```sh
+pip install pyqt-autotest
+```
+
+## Setup
+
+Create a file named `.autotest` in your home directory with the following contents.
+
+```
+[setup]
+search_directories = /path/to/test/directory1/
+                     /path/to/test/directory2/
+output_directory = /path/to/output/directory/
+```
+
+The `search_directories` option is used to specify the directories to search for python files containing your test classes. The `output_directory` option is used to specify the directory to store the output results in.
+
+## Options
+
+The following table details the options that can be provided on the command line.
+
+| Option            | Description                                                                                                                                 | Default                      | Command line option     |
+|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|-------------------------|
+| Tests regex       | Run tests matching this regular expression. The directories provided in the `.autotest` configuration file are searched for matching tests. |                              | -R, --tests-regex       |
+| List tests        | Flag which lists the tests that are found in the search directories specified by the `.autotest` configuration file. The tests are not run. | False                        | -l, --list-tests        |
+| Number of runs    | The number of times to open the widget and perform a random selection of actions.                                                           | 1                            | -n, --number-of-runs    |
+| Number of actions | The number of random actions to perform each time the widget is opened.                                                                     | 10                           | -a, --number-of-actions |
+| Wait time         | The number of milliseconds to wait between executing two consecutive actions.                                                               | 50                           | -w, --wait-time         |
+| Output name       | The name to give the output file. The output file is stored in the output_directory specified by the `.autotest` configuration file.        | No output file is generated. | -o, --output-name       |
+| Cautious          | Flag which saves the output file before each action is performed. This ensures an output file is still created after a terminating fault.   | False                        | -c, --cautious          |
+| Verbose           | Flag which prints more debug information when supplied. It also prints the actions just before each of them is performed.                   | False                        | -v, --verbose           |
+
+## Test class
+
+The first thing to do is to create a python class which inherits from `RandomAutoTest`, and implement the `setup_widget` method. Inside this method, you should instantiate your `QWidget` and assign it to the member variable `self.widget`as follows. Any additional setup, such as loading data into your widget, should also be done in the same method.
+
+```py
+from usercode.model import ExampleModel
+from usercode.presenter import ExamplePresenter
+from usercode.view import ExampleView
+
+from pyqt_autotest.random_auto_test import RandomAutoTest
+
+
+class ExampleTest(RandomAutoTest):
+
+    def setup_widget(self):
+        # The 'self.widget' member variable MUST be instantiated, and it must be a QWidget.
+        self.widget = ExampleView()
+
+        # Other relevant setup should be done here too. This example refers to the Model-View-Presenter (MVP) pattern
+        self.model = ExampleModel()
+        self.presenter = ExamplePresenter(self.widget, self.model)
+
+        # Your test might be more interesting if you first load data into the widget
+        self.presenter.load_data("fake_data_file.dat")
+```
+
+Optionally, you can also create a `setup_options` method to specify commonly used options. However, these options will be overridden if provided on the command line. Note that the `Output Name` option cannot be provided in this setup method.
+
+```py
+    def setup_options(self):
+        self.options.number_of_runs = 2
+        self.options.number_of_actions = 15
+        self.options.wait_time = 200  # milliseconds
+```
+
+## Built-in Actions
+
+The following actions are built-in to this package. Only these actions can be performed if you do not create your own (see the section below on [how to create your own](#creating-your-own-actions)).
+
+| Built-in Action       | Description                                               | Python Callable                                          |
+|-----------------------|-----------------------------------------------------------|----------------------------------------------------------|
+| Action.KeyDownClick   | Simulates the Down key being pressed on an active widget. | `lambda widget: QTest.keyClick(widget, Qt.Key_Down)`     |
+| Action.KeyUpClick     | Simulates the Up key being pressed on an active widget.   | `lambda widget: QTest.keyClick(widget, Qt.Key_Up)`       |
+| Action.MouseLeftClick | Simulates a widget being left clicked by the mouse.       | `lambda widget: QTest.mouseClick(widget, Qt.LeftButton)` |
+
+These actions will by default be performed for the following widget types. This has been made minimalistic on purpose because this command line tool is arguably more useful if you carefully customize your own actions as seen in the next section.
+
+| Widget type       | Built-in Actions      |
+|-------------------|-----------------------|
+| QPushButton       | Action.MouseLeftClick |
+
+## Creating your own Actions
+This package provides a great amount of flexibility for you to create and customize the actions you want to be available during a 'random auto test'. It also allows you to ignore certain widget types by not providing any actions for them.
+
+The following code provides a basic example for how to define your own custom actions:
+
+```py
+    def setup_options(self):
+        # The 'actions' dictionary requires a string to describe an action, and a callable function which uses QtTest to
+        # perform an action. Note that the 'Left click in centre' action is useful for testing a QCheckBox.
+        actions = {
+            "Enter dummy text": lambda widget: QTest.keyClicks(widget, "dummy text"),
+            "Left click in centre": lambda widget: QTest.mouseClick(widget, Qt.LeftButton,
+                                                                    pos=QPoint(2, widget.height() / 2))
+        }
+
+        # The 'widget_actions' dictionary requires you to specify which actions can be performed on which widget types.
+        # Note that you can use the built-in actions, or create your own with a string name. The string name is used to
+        # describe what an action does when generating the output instructions, so make sure it is short but descriptive.
+        widget_actions = {
+            QCheckBox: ["Left click in centre"],
+            QLineEdit: ["Enter dummy text"],
+            QSpinBox: [Action.KeyDownClick, Action.KeyUpClick]
+        }
+
+        # This will overwrite the built-in actions. You could use 'dict::update' to keep the built-in actions.
+        self.options.actions = actions
+        self.options.widget_actions = widget_actions
+```
+
+## Usage
+
+It is trivial to run your test class from the command line as follows (depending on its module location):
+
+```sh
+autotest -R ExampleTest
+```
+or with more arguments:
+```
+autotest -R ExampleTest -n 5 -a 10 -w 150 -o autotest_results -v
+```
+
+## Output
+
+An output json file will only be generated if an `Output Name` is provided from the command line using the `-o, --output-name` option. Alternatively, you can use the `Verbose` flag to get debug information from your terminal using the `-v, --verbose` option.
```

### Comparing `pyqt-autotest-0.2.0/pyqt_autotest.egg-info/SOURCES.txt` & `pyqt-autotest-0.2.1/pyqt_autotest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

