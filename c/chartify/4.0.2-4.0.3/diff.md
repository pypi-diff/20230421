# Comparing `tmp/chartify-4.0.2.tar.gz` & `tmp/chartify-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartify-4.0.2.tar", last modified: Thu Mar 30 11:01:25 2023, max compression
+gzip compressed data, was "chartify-4.0.3.tar", last modified: Fri Apr 21 09:56:15 2023, max compression
```

## Comparing `chartify-4.0.2.tar` & `chartify-4.0.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.206086 chartify-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-30 11:01:11.000000 chartify-4.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-03-30 11:01:11.000000 chartify-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-30 11:01:11.000000 chartify-4.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-03-30 11:01:11.000000 chartify-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-30 11:01:11.000000 chartify-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-30 11:01:11.000000 chartify-4.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-03-30 11:01:25.206086 chartify-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-30 11:01:11.000000 chartify-4.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.186086 chartify-4.0.2/chartify/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.190086 chartify-4.0.2/chartify/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/callout.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29219 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/colour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    88685 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/radar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/_core/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    46517 2023-03-30 11:01:11.000000 chartify-4.0.2/chartify/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.190086 chartify-4.0.2/chartify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-03-30 11:01:25.000000 chartify-4.0.2/chartify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-30 11:01:25.000000 chartify-4.0.2/chartify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:01:25.000000 chartify-4.0.2/chartify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:01:24.000000 chartify-4.0.2/chartify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-30 11:01:25.000000 chartify-4.0.2/chartify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 11:01:25.000000 chartify-4.0.2/chartify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.194086 chartify-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.194086 chartify-4.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   116281 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify1.png
--rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify2.png
--rw-r--r--   0 runner    (1001) docker     (123)    31874 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify3.png
--rw-r--r--   0 runner    (1001) docker     (123)    28399 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify4.png
--rw-r--r--   0 runner    (1001) docker     (123)    31769 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify5.png
--rw-r--r--   0 runner    (1001) docker     (123)    47838 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/chartify6.png
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/_static/coverage.svg
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8398 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-30 11:01:11.000000 chartify-4.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.202086 chartify-4.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-03-30 11:01:11.000000 chartify-4.0.2/examples/Chartify Tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  5316148 2023-03-30 11:01:11.000000 chartify-4.0.2/examples/Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:11.000000 chartify-4.0.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-30 11:01:11.000000 chartify-4.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-30 11:01:11.000000 chartify-4.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-30 11:01:25.206086 chartify-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-30 11:01:11.000000 chartify-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.206086 chartify-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.186086 chartify-4.0.2/tests/outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:01:25.206086 chartify-4.0.2/tests/outputs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/outputs/chart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_callout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_color_palettes_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_colors_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_options_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36651 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-30 11:01:11.000000 chartify-4.0.2/tests/test_style_settings_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-30 11:01:11.000000 chartify-4.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.041937 chartify-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 09:56:02.000000 chartify-4.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-21 09:56:02.000000 chartify-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-21 09:56:02.000000 chartify-4.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-21 09:56:02.000000 chartify-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-21 09:56:02.000000 chartify-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-21 09:56:02.000000 chartify-4.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-21 09:56:15.041937 chartify-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-21 09:56:02.000000 chartify-4.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.025937 chartify-4.0.3/chartify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.025937 chartify-4.0.3/chartify/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/callout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29219 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/colour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88685 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/radar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/_core/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46517 2023-04-21 09:56:02.000000 chartify-4.0.3/chartify/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.025937 chartify-4.0.3/chartify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-21 09:56:15.000000 chartify-4.0.3/chartify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-21 09:56:15.000000 chartify-4.0.3/chartify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:56:15.000000 chartify-4.0.3/chartify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:56:14.000000 chartify-4.0.3/chartify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 09:56:15.000000 chartify-4.0.3/chartify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 09:56:15.000000 chartify-4.0.3/chartify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.029937 chartify-4.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.033937 chartify-4.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   116281 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31874 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28399 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31769 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47838 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/chartify6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/_static/coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8398 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-21 09:56:02.000000 chartify-4.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.037937 chartify-4.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-04-21 09:56:02.000000 chartify-4.0.3/examples/Chartify Tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5316148 2023-04-21 09:56:02.000000 chartify-4.0.3/examples/Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:02.000000 chartify-4.0.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-21 09:56:02.000000 chartify-4.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-21 09:56:02.000000 chartify-4.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 09:56:15.041937 chartify-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-21 09:56:02.000000 chartify-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.041937 chartify-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.021937 chartify-4.0.3/tests/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:56:15.041937 chartify-4.0.3/tests/outputs/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/outputs/chart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_callout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_color_palettes_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_colors_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_options_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36651 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-21 09:56:02.000000 chartify-4.0.3/tests/test_style_settings_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-21 09:56:02.000000 chartify-4.0.3/tox.ini
```

### Comparing `chartify-4.0.2/CONTRIBUTING.rst` & `chartify-4.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/HISTORY.rst` & `chartify-4.0.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+4.0.3 (2023-04-21)
+------------------
+
+* Require jupyter_bokeh to enable html output
+
 4.0.2 (2023-03-30)
 ------------------
 
 * Fix categorical_order_by check for scatter plot
 * Fix categorical_order_by check for _construct_source
 * Refactor category sorting in _construct_source
 * Add tests for categorical_order_by
```

### Comparing `chartify-4.0.2/LICENSE` & `chartify-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/Makefile` & `chartify-4.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/PKG-INFO` & `chartify-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartify
-Version: 4.0.2
+Version: 4.0.3
 Summary: Python library to make plotting simpler for data scientists
 Home-page: https://github.com/spotify/chartify
 Author: 
 Author-email: chalpert@spotify.com
 License: Apache 2
 Keywords: chartify
 Classifier: Development Status :: 4 - Beta
@@ -20,16 +20,16 @@
 
 Chartify
 ========
 
 |status|  |release|  |python|  |CI|
 
 .. |status| image:: https://img.shields.io/badge/Status-Beta-blue.svg
-.. |release| image:: https://img.shields.io/badge/Release-3.0.5-blue.svg
-.. |python| image:: https://img.shields.io/badge/Python-3.6-blue.svg
+.. |release| image:: https://img.shields.io/badge/Release-4.0.3-blue.svg
+.. |python| image:: https://img.shields.io/badge/Python-3.7-blue.svg
 .. |CI| image:: https://github.com/spotify/chartify/workflows/Tox/badge.svg
         :target: https://github.com/spotify/chartify/actions
 
 Chartify is a Python library that makes it easy for data scientists to create charts.
 
 Why use Chartify?
 -----------------
@@ -100,14 +100,19 @@
 `See the contributing docs <CONTRIBUTING.rst>`_.
 
 
 =======
 History
 =======
 
+4.0.3 (2023-04-21)
+------------------
+
+* Require jupyter_bokeh to enable html output
+
 4.0.2 (2023-03-30)
 ------------------
 
 * Fix categorical_order_by check for scatter plot
 * Fix categorical_order_by check for _construct_source
 * Refactor category sorting in _construct_source
 * Add tests for categorical_order_by
```

### Comparing `chartify-4.0.2/README.rst` & `chartify-4.0.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Chartify
 ========
 
 |status|  |release|  |python|  |CI|
 
 .. |status| image:: https://img.shields.io/badge/Status-Beta-blue.svg
-.. |release| image:: https://img.shields.io/badge/Release-3.0.5-blue.svg
-.. |python| image:: https://img.shields.io/badge/Python-3.6-blue.svg
+.. |release| image:: https://img.shields.io/badge/Release-4.0.3-blue.svg
+.. |python| image:: https://img.shields.io/badge/Python-3.7-blue.svg
 .. |CI| image:: https://github.com/spotify/chartify/workflows/Tox/badge.svg
         :target: https://github.com/spotify/chartify/actions
 
 Chartify is a Python library that makes it easy for data scientists to create charts.
 
 Why use Chartify?
 -----------------
```

### Comparing `chartify-4.0.2/chartify/__init__.py` & `chartify-4.0.3/chartify/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from chartify._core.radar_chart import RadarChart
 from chartify._core.colors import color_palettes
 from chartify._core.options import options
 from chartify import examples
 
 __author__ = """Chris Halpert"""
 __email__ = "chalpert@spotify.com"
-__version__ = "4.0.2"
+__version__ = "4.0.3"
 
 _IPYTHON_INSTANCE = False
 
 
 def set_display_settings():
     """Enable notebook output settings if running in a jupyter notebook"""
     from IPython.core.getipython import get_ipython
```

### Comparing `chartify-4.0.2/chartify/_core/__init__.py` & `chartify-4.0.3/chartify/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/axes.py` & `chartify-4.0.3/chartify/_core/axes.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/callout.py` & `chartify-4.0.3/chartify/_core/callout.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/chart.py` & `chartify-4.0.3/chartify/_core/chart.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/colors.py` & `chartify-4.0.3/chartify/_core/colors.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/colour.py` & `chartify-4.0.3/chartify/_core/colour.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/options.py` & `chartify-4.0.3/chartify/_core/options.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/plot.py` & `chartify-4.0.3/chartify/_core/plot.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/radar_chart.py` & `chartify-4.0.3/chartify/_core/radar_chart.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/_core/style.py` & `chartify-4.0.3/chartify/_core/style.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify/examples.py` & `chartify-4.0.3/chartify/examples.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/chartify.egg-info/PKG-INFO` & `chartify-4.0.3/chartify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartify
-Version: 4.0.2
+Version: 4.0.3
 Summary: Python library to make plotting simpler for data scientists
 Home-page: https://github.com/spotify/chartify
 Author: 
 Author-email: chalpert@spotify.com
 License: Apache 2
 Keywords: chartify
 Classifier: Development Status :: 4 - Beta
@@ -20,16 +20,16 @@
 
 Chartify
 ========
 
 |status|  |release|  |python|  |CI|
 
 .. |status| image:: https://img.shields.io/badge/Status-Beta-blue.svg
-.. |release| image:: https://img.shields.io/badge/Release-3.0.5-blue.svg
-.. |python| image:: https://img.shields.io/badge/Python-3.6-blue.svg
+.. |release| image:: https://img.shields.io/badge/Release-4.0.3-blue.svg
+.. |python| image:: https://img.shields.io/badge/Python-3.7-blue.svg
 .. |CI| image:: https://github.com/spotify/chartify/workflows/Tox/badge.svg
         :target: https://github.com/spotify/chartify/actions
 
 Chartify is a Python library that makes it easy for data scientists to create charts.
 
 Why use Chartify?
 -----------------
@@ -100,14 +100,19 @@
 `See the contributing docs <CONTRIBUTING.rst>`_.
 
 
 =======
 History
 =======
 
+4.0.3 (2023-04-21)
+------------------
+
+* Require jupyter_bokeh to enable html output
+
 4.0.2 (2023-03-30)
 ------------------
 
 * Fix categorical_order_by check for scatter plot
 * Fix categorical_order_by check for _construct_source
 * Refactor category sorting in _construct_source
 * Add tests for categorical_order_by
```

### Comparing `chartify-4.0.2/chartify.egg-info/SOURCES.txt` & `chartify-4.0.3/chartify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/Makefile` & `chartify-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify1.png` & `chartify-4.0.3/docs/_static/chartify1.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify2.png` & `chartify-4.0.3/docs/_static/chartify2.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify3.png` & `chartify-4.0.3/docs/_static/chartify3.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify4.png` & `chartify-4.0.3/docs/_static/chartify4.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify5.png` & `chartify-4.0.3/docs/_static/chartify5.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/chartify6.png` & `chartify-4.0.3/docs/_static/chartify6.png`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/_static/coverage.svg` & `chartify-4.0.3/docs/_static/coverage.svg`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/conf.py` & `chartify-4.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/installation.rst` & `chartify-4.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/make.bat` & `chartify-4.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/docs/usage.rst` & `chartify-4.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/examples/Chartify Tutorial.ipynb` & `chartify-4.0.3/examples/Chartify Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/examples/Examples.ipynb` & `chartify-4.0.3/examples/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/setup.py` & `chartify-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/__init__.py` & `chartify-4.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_axes.py` & `chartify-4.0.3/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_callout.py` & `chartify-4.0.3/tests/test_callout.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_chart.py` & `chartify-4.0.3/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_color_palettes_config.py` & `chartify-4.0.3/tests/test_color_palettes_config.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_colors.py` & `chartify-4.0.3/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_colors_config.py` & `chartify-4.0.3/tests/test_colors_config.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_examples.py` & `chartify-4.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_options_config.py` & `chartify-4.0.3/tests/test_options_config.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_plots.py` & `chartify-4.0.3/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tests/test_style_settings_config.py` & `chartify-4.0.3/tests/test_style_settings_config.py`

 * *Files identical despite different names*

### Comparing `chartify-4.0.2/tox.ini` & `chartify-4.0.3/tox.ini`

 * *Files identical despite different names*

