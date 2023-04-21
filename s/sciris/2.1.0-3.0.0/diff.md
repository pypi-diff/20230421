# Comparing `tmp/sciris-2.1.0.tar.gz` & `tmp/sciris-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciris-2.1.0.tar", last modified: Sat Dec 24 04:13:27 2022, max compression
+gzip compressed data, was "sciris-3.0.0.tar", last modified: Fri Apr 21 07:06:40 2023, max compression
```

## Comparing `sciris-2.1.0.tar` & `sciris-3.0.0.tar`

### file list

```diff
@@ -1,53 +1,352 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1209 2022-08-19 06:28:28.000000 sciris-2.1.0/.gitignore
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1092 2022-10-23 20:14:34.000000 sciris-2.1.0/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19096 2022-12-24 04:13:27.400382 sciris-2.1.0/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18198 2022-10-24 07:44:29.000000 sciris-2.1.0/README.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/docs/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       20 2018-11-23 04:31:03.000000 sciris-2.1.0/docs/.gitignore
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      737 2022-08-19 06:28:28.000000 sciris-2.1.0/docs/Makefile
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3330 2022-12-24 04:13:18.000000 sciris-2.1.0/docs/conf.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      674 2022-08-19 06:28:28.000000 sciris-2.1.0/docs/index.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      752 2018-11-23 04:31:03.000000 sciris-2.1.0/docs/make.bat
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      224 2021-12-20 17:43:24.000000 sciris-2.1.0/readthedocs.yml
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/sciris/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      852 2022-08-19 06:28:28.000000 sciris-2.1.0/sciris/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11573 2022-08-19 06:28:28.000000 sciris-2.1.0/sciris/ansicolors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14485 2022-10-24 07:44:29.000000 sciris-2.1.0/sciris/sc_asd.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    41888 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_colors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    25374 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_dataframe.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42023 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_datetime.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    80132 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_fileio.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15478 2022-08-19 06:28:28.000000 sciris-2.1.0/sciris/sc_legacy.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45390 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_math.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9419 2022-08-19 06:28:28.000000 sciris-2.1.0/sciris/sc_nested.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    56013 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_odict.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22799 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_parallel.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    76039 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    39068 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_printing.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24197 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_profiling.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    25510 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    78625 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      273 2022-12-24 04:13:18.000000 sciris-2.1.0/sciris/sc_version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/sciris.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19096 2022-12-24 04:13:27.000000 sciris-2.1.0/sciris.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      917 2022-12-24 04:13:27.000000 sciris-2.1.0/sciris.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2022-12-24 04:13:27.000000 sciris-2.1.0/sciris.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      230 2022-12-24 04:13:27.000000 sciris-2.1.0/sciris.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2022-12-24 04:13:27.000000 sciris-2.1.0/sciris.egg-info/top_level.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2022-12-24 04:13:27.400382 sciris-2.1.0/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2948 2022-12-24 04:13:18.000000 sciris-2.1.0/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/tests/
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2022-12-24 04:13:27.400382 sciris-2.1.0/tests/files/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)       80 2019-09-19 23:00:18.000000 sciris-2.1.0/tests/files/deadclass.obj
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)    51539 2019-09-19 23:00:18.000000 sciris-2.1.0/tests/files/exampledata.xlsx
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1817 2022-01-08 10:13:41.000000 sciris-2.1.0/tests/run_all_tests.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1444 2022-12-24 04:13:18.000000 sciris-2.1.0/tests/showcase_vanilla.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2558 2022-01-08 10:13:41.000000 sciris-2.1.0/tests/test_asd.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3681 2022-10-23 20:14:34.000000 sciris-2.1.0/tests/test_dataframe.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8789 2022-12-24 04:13:18.000000 sciris-2.1.0/tests/test_fileio.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6243 2022-10-24 07:50:39.000000 sciris-2.1.0/tests/test_math.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7655 2022-01-12 06:57:55.000000 sciris-2.1.0/tests/test_odict.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3638 2022-08-19 06:28:28.000000 sciris-2.1.0/tests/test_parallel.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5947 2022-12-24 04:13:18.000000 sciris-2.1.0/tests/test_plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10635 2022-12-24 04:13:18.000000 sciris-2.1.0/tests/test_utils.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    52027 2023-04-21 07:02:08.000000 sciris-3.0.0/CHANGELOG.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3510 2022-12-27 06:15:14.000000 sciris-3.0.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1137 2023-04-21 07:02:08.000000 sciris-3.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1092 2022-12-27 06:15:14.000000 sciris-3.0.0/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      160 2023-04-21 07:02:08.000000 sciris-3.0.0/MANIFEST.in
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2936 2023-04-21 07:06:40.573511 sciris-3.0.0/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1987 2023-04-21 07:02:08.000000 sciris-3.0.0/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15052 2023-04-21 07:02:08.000000 sciris-3.0.0/STYLE_GUIDE.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/_static/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/_static/scripts/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      237 2023-04-14 01:21:03.000000 sciris-3.0.0/docs/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/_static/vendor/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/_static/vendor/fontawesome/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7427 2023-04-14 01:21:03.000000 sciris-3.0.0/docs/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/_templates/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      512 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/_templates/custom-class-template.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/_templates/custom-function-template.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1294 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/_templates/custom-module-template.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.561512 sciris-3.0.0/docs/api/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/docs/api/_autosummary/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      538 2023-04-20 04:17:11.000000 sciris-3.0.0/docs/api/_autosummary/sciris.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       75 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_asd.asd.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      251 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_asd.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.alpinecolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      102 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.arraycolors.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.bandedcolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.bicolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.colormapdemo.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.gridcolors.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.hex2rgb.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.hsv2rgb.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.midpointnorm.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.orangebluecolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.parulacolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.rgb2hex.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.rgb2hsv.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      556 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      108 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.sanitizecolor.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.shifthue.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      108 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.turbocolormap.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_colors.vectocolor.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      726 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_dataframe.dataframe.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      270 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_dataframe.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      358 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.Timer.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.date.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.datedelta.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.daterange.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.datetoyear.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.day.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.daydiff.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.elapsedtimestr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.getdate.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.now.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.randsleep.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.readdate.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      633 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.tic.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.time.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.timedsleep.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      358 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.timer.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.toc.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_datetime.toctic.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      217 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.Blobject.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      208 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.Empty.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      293 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.Failed.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      226 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.Spreadsheet.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.dumpstr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      102 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.getfilelist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.getfilepaths.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.ispath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.jsonify.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.jsonpickle.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.jsonunpickle.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       81 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.load.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadjson.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadspreadsheet.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadstr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadtext.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadyaml.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.loadzip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.makefilepath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.makepath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       81 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.path.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.printjson.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.readjson.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.readyaml.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.rmpath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1013 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      117 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.sanitizefilename.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.sanitizejson.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.sanitizepath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       81 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.save.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.savejson.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.saveobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.savespreadsheet.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.savetext.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.saveyaml.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.savezip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.thisdir.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.thisfile.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.thispath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       84 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.unzip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       84 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_fileio.zsave.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       85 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.approx.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       76 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.cat.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.convolve.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       82 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.count.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.dataindex.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.fillnans.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.findfirst.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.findinds.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.findlast.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.findnans.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      100 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.findnearest.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.gauss1d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.gauss2d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.getvaliddata.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.getvalidinds.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.inclusiverange.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.isprime.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.linregress.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.normalize.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.normsum.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.numdigits.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.perturb.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.randround.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       85 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.rmnans.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       88 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.rolling.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      689 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.safedivide.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.sanitize.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       85 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.smooth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_math.smoothinterp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      102 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.flattendict.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.getnested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.iternested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.iterobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.makenested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      102 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.mergenested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.nestedloop.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      396 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.search.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_nested.setnested.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_odict.asobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      213 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_odict.dictobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      213 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_odict.objdict.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      207 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_odict.odict.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      431 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_odict.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      343 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_parallel.Parallel.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_parallel.parallelize.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      421 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_parallel.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.SIticks.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      371 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.ScirisDateFormatter.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      328 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.animation.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.ax3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.bar3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.boxoff.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.commaticks.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.dateformatter.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.datenumformatter.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.emptyfig.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.fig3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.figlayout.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.fonts.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.get_rows_cols.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.getrowscols.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.loadfig.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.maximize.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.orderlegend.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.plot3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      850 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.savefig.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.savefigs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.savemovie.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.scatter3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.separatelegend.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.setaxislim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.setxlim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.setylim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.stackedbar.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_plotting.surf3d.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.arraymean.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.arraymedian.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.blank.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.capture.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.colorize.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.createcollist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.heading.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      115 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.humanize_bytes.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.indent.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.objatt.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.objectid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.objmeth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.objprop.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.objrepr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      116 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.percentcomplete.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       77 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.pr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.prepr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printarr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printblue.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printcyan.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printdata.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printgreen.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printmagenta.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printmean.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printmedian.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printred.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printtologfile.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printv.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printvars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.printyellow.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.progressbar.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      231 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.progressbars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      948 2023-04-20 04:17:12.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.sigfig.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.sigfigs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_printing.slacknotification.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      143 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.LimitExceeded.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       99 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.benchmark.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.checkmem.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.checkram.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.cpu_count.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.cpuload.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      108 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.loadbalancer.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.memload.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.mprofile.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.profile.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      241 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.resourcemonitor.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      642 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_profiling.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      234 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_settings.ScirisOptions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_settings.help.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      100 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_settings.parse_env.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      435 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_settings.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.KeyNotFoundError.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      222 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.LazyModule.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      204 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.Link.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      131 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.LinkException.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.asciify.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.autolist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.checktype.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       74 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.cp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       77 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.dcp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.download.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.fast_uuid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.flexstr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.getplatform.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.getuser.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.htmlify.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.importbyname.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.importbypath.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.isarray.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.isiterable.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.islinux.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.ismac.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.isnumber.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.isstring.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.iswindows.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.mergedicts.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.mergelists.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.newlinejoin.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       74 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.pp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      219 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.prettyobj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.promotetoarray.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.promotetolist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1170 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.runcommand.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.sanitizestr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       77 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.sha.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.strjoin.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.strsplit.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.suggest.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.swapdict.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.toarray.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.tolist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.traceback.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.transposelist.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      296 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.tryexcept.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.uniquename.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       89 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.urlopen.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.uuid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       80 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_utils.wget.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      116 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_version.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.compareversions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       91 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.freeze.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      100 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.getcaller.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.gitinfo.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.loadarchive.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.loadmetadata.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.metadata.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       94 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.require.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      411 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2023-04-20 04:17:13.000000 sciris-3.0.0/docs/api/_autosummary/sciris.sc_versioning.savearchive.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      432 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/all.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      717 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/containers.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      869 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/files.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      457 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      550 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/math.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      867 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/parallel.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      752 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/printing.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      725 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/api/utils.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       35 2022-12-27 06:15:14.000000 sciris-3.0.0/docs/code_of_conduct.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       32 2022-12-27 06:15:14.000000 sciris-3.0.0/docs/contributing.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1122 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9323 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/overview.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/requirements.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       31 2022-12-27 06:15:14.000000 sciris-3.0.0/docs/style_guide.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/docs/tutorials/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4035 2023-04-21 07:02:08.000000 sciris-3.0.0/docs/tutorials/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-12-27 06:15:14.000000 sciris-3.0.0/docs/whatsnew.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      901 2023-04-21 07:02:08.000000 sciris-3.0.0/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/sciris/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1350 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/__init__.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/sciris/_extras/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      343 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/_extras/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/_extras/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11573 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/_extras/ansicolors.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21606 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/_extras/legacy.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      270 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/fancy.mplstyle
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14576 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_asd.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42573 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_colors.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    41026 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_dataframe.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    50754 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_datetime.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    91697 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_fileio.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    47823 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_math.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15297 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_nested.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    59323 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_odict.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    34005 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_parallel.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    76970 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_plotting.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    50919 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_printing.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    30700 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_profiling.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28154 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    83595 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      273 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_version.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    31575 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/sc_versioning.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2023-04-21 07:02:08.000000 sciris-3.0.0/sciris/simple.mplstyle
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/sciris.egg-info/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2936 2023-04-21 07:06:40.000000 sciris-3.0.0/sciris.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15736 2023-04-21 07:06:40.000000 sciris-3.0.0/sciris.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-04-21 07:06:40.000000 sciris-3.0.0/sciris.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      204 2023-04-21 07:06:40.000000 sciris-3.0.0/sciris.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2023-04-21 07:06:40.000000 sciris-3.0.0/sciris.egg-info/top_level.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-04-21 07:06:40.573511 sciris-3.0.0/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1909 2023-04-21 07:02:08.000000 sciris-3.0.0/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-04-21 07:06:40.573511 sciris-3.0.0/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      430 2023-04-21 07:02:08.000000 sciris-3.0.0/tests/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       65 2023-04-21 07:02:08.000000 sciris-3.0.0/tests/requirements.txt
```

### Comparing `sciris-2.1.0/LICENSE` & `sciris-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sciris-2.1.0/sciris/ansicolors.py` & `sciris-3.0.0/sciris/_extras/ansicolors.py`

 * *Files identical despite different names*

### Comparing `sciris-2.1.0/sciris/sc_asd.py` & `sciris-3.0.0/sciris/sc_asd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 '''
-Adaptive stochastic descent optimization algorithm, building on scipy.optimize.
+Adaptive stochastic descent optimization algorithm, building on :mod:`scipy.optimize`.
 
-This algorithm is published as "Optimization by adaptive stochastic descent" by
-Kerr et al. (2018) (DOI: https://doi.org/10.1371/journal.pone.0192944).
+This algorithm is published as:
+
+  Kerr CC, Dura-Bernal S, Smolinski TG, Chadderdon GL, Wilson DP (2018).
+  **Optimization by Adaptive Stochastic Descent**. *PLoS ONE* 13(3): e0192944. 
+  https://doi.org/10.1371/journal.pone.0192944
 '''
 
+import time
 import numpy as np
-import numpy.random as nr
-from time import time
 from . import sc_utils as scu
 from . import sc_printing as scp
 from . import sc_odict as sco
 
 __all__ = ['asd']
 
 def asd(function, x, args=None, stepsize=0.1, sinc=2, sdec=2, pinc=2, pdec=2,
     pinitial=None, sinitial=None, xmin=None, xmax=None, maxiters=None, maxtime=None,
     abstol=1e-6, reltol=1e-3, stalliters=None, stoppingfunc=None, randseed=None,
     label=None, verbose=1, **kwargs):
     """
     Optimization using adaptive stochastic descent (ASD). Can be used as a faster
-    and more powerful alternative to e.g. ``scipy.optimize.minimize()``.
+    and more powerful alternative to e.g. :func:`scipy.optimize.minimize()`.
 
     ASD starts at ``x0`` and attempts to find a local minimizer ``x`` of the function ``func()``.
     ``func()`` accepts input ``x`` and returns a scalar function value evaluated at ``x``.
     ``x0`` can be a scalar, list, or Numpy array of any size.
 
     Args:
         function     (func):  The function to minimize
@@ -86,19 +88,18 @@
 
     Please use the following citation for this method:
 
         CC Kerr, S Dura-Bernal, TG Smolinski, GL Chadderdon, DP Wilson (2018).
         Optimization by adaptive stochastic descent.
         PLOS ONE 13 (3), e0192944.
 
-    Version: 2019jul08
+    *New in version 3.0.0:* Uses its own random number stream
     """
-    if randseed is not None:
-        nr.seed(int(randseed)) # Don't reset it if not supplied
-        if verbose >= 2: print(f'ASD: Launching with random seed is {randseed}; sample: {nr.random()}')
+    rng = np.random.default_rng(randseed)
+    if verbose >= 2: print(f'ASD: Launching with random seed {randseed}')
 
     def consistentshape(userinput, origshape=False):
         """
         Make sure inputs have the right shape and data type.
         """
         output = np.reshape(np.array(userinput, dtype='float'), -1)
         if origshape: return output, np.shape(userinput)
@@ -171,27 +172,27 @@
     fvals = np.zeros(maxiters + 1) # Store all objective function values
     allsteps = np.zeros((maxiters + 1, nparams)) # Store all parameters
     fvals[0] = fvalorig # Store initial function output
     allsteps[0, :] = xorig # Store initial input vector
 
     # Loop
     count = 0 # Keep track of how many iterations have occurred
-    start = time() # Keep track of when we begin looping
+    start = time.time() # Keep track of when we begin looping
     offset = ' ' * 4 # Offset the print statements
     exitreason = 'Unknown exit reason' # Catch everything else
     while True:
         count += 1 # Increment the count
         if verbose >= 3: print(f'\n\n Count={count} \n x={x} \n probabilities={probabilities} \n stepsizes={stepsizes}')
 
         # Calculate next parameters
         probabilities = probabilities / sum(probabilities) # Normalize probabilities
         cumprobs = np.cumsum(probabilities) # Calculate the cumulative distribution
         inrange = False
         for r in range(maxrangeiters): # Try to find parameters within range
-            choice = np.flatnonzero(cumprobs > nr.random())[0] # Choose a parameter and upper/lower at random
+            choice = np.flatnonzero(cumprobs > rng.random())[0] # Choose a parameter and upper/lower at random
             par = np.mod(choice, nparams) # Which parameter was chosen
             pm = np.floor((choice) / nparams) # Plus or minus
             newval = x[par] + ((-1)**pm) * stepsizes[choice] # Calculate the new vector
             if newval<xmin[par]: newval = xmin[par] # Reset to the lower limit
             if newval>xmax[par]: newval = xmax[par] # Reset to the upper limit
             inrange = (newval != x[par])
             if verbose >= 3: print(offset*2 + f'count={count} r={r}, choice={choice}, par={par}, x[par]={x[par]}, pm={(-1)**pm}, step={stepsizes[choice]}, newval={newval}, xmin={xmin[par]}, xmax={xmax[par]}, inrange={inrange}')
@@ -225,37 +226,37 @@
             probabilities[choice] = probabilities[choice] / pdec # Decrease probability of picking this parameter again
             stepsizes[choice] = stepsizes[choice] / sdec # Decrease size of step for next time
             flag = '--' # Marks no change
             if np.isnan(fvalnew):
                 if verbose >= 1: print('ASD: Warning, objective function returned NaN')
         if verbose > 0 and not (count % max(1, int(1.0/verbose))): # Print out every 1/verbose steps
             orig, best, new, diff = scp.sigfig([fvalorig, fvalold, fvalnew, fvalnew-fvalold])
-            print(offset + label + f' step {count} ({time()-start:0.1f} s) {flag} (orig:{orig} | best:{best} | new:{new} | diff:{diff})')
+            print(offset + label + f' step {count} ({time.time()-start:0.1f} s) {flag} (orig:{orig} | best:{best} | new:{new} | diff:{diff})')
 
         # Store output information
         fvals[count] = fval # Store objective function evaluations
         allsteps[count, :] = x # Store parameters
 
         # Stopping criteria
-        if count >= maxiters: # Stop if the iteration limit is exceeded
+        if count >= maxiters: # Stop if the iteration limit is exceeded # pragma: no cover
             exitreason = 'Maximum iterations reached'
             break
-        if (time() - start) > maxtime:
-            strtime, strmax = scp.sigfig([(time()-start), maxtime])
+        if (time.time() - start) > maxtime: # pragma: no cover
+            strtime, strmax = scp.sigfig([(time.time()-start), maxtime])
             exitreason = f'Time limit reached ({strtime} > {strmax})'
             break
         if (count > stalliters) and (abs(np.mean(abserrorhistory)) < abstol): # Stop if improvement is too small
             strabs, strtol = scp.sigfig([np.mean(abserrorhistory), abstol])
             exitreason = f'Absolute improvement too small ({strabs} < {strtol})'
             break
         if (count > stalliters) and (sum(relerrorhistory) < reltol): # Stop if improvement is too small
             strrel, strtol = scp.sigfig([np.mean(relerrorhistory), reltol])
             exitreason = f'Relative improvement too small ({strrel} < {strtol})'
             break
-        if stoppingfunc and stoppingfunc():
+        if stoppingfunc and stoppingfunc(): # pragma: no cover
             exitreason = 'Stopping function called'
             break
 
     # Return
     if verbose > 0:
         orig, best, ratio = scp.sigfig([fvals[0], fvals[-1], fvals[-1]/fvals[0]])
         print(f'=== {label} {exitreason} ({count} steps, orig: {orig} | best: {best} | ratio: {ratio}) ===')
@@ -264,8 +265,8 @@
     output['fval'] = fvals[count]
     output['exitreason'] = exitreason
     output['details'] = sco.objdict()
     output['details']['fvals'] = fvals[:count+1] # Function evaluations
     output['details']['xvals'] = allsteps[:count+1, :]
     output['details']['probabilities'] = probabilities
     output['details']['stepsizes'] = stepsizes
-    return output # Return parameter vector as well as details about run
+    return output # Return parameter vector as well as details about run
```

### Comparing `sciris-2.1.0/sciris/sc_colors.py` & `sciris-3.0.0/sciris/sc_colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Handle colors and colormaps.
 
 Highlights:
     - Adds colormaps including ``'turbo'``, ``'parula'``, and ``'orangeblue'``
-    - :func:`hex2rgb`/:func:`rgb2hex`: convert between different color conventions
-    - :func:`vectocolor`: map a list of sequential values onto a list of colors
-    - :func:`gridcolors`: map a list of qualitative categories onto a list of colors
+    - :func:`sc.hex2rgb() <hex2rgb>`/:func:`sc.rgb2hex() <rgb2hex>`: convert between different color conventions
+    - :func:`sc.vectocolor() <vectocolor>`: map a list of sequential values onto a list of colors
+    - :func:`sc.gridcolors() <gridcolors>`: map a list of qualitative categories onto a list of colors
 '''
 
 ##############################################################################
 #%% Imports
 ##############################################################################
 
 import struct
 import pylab as pl
 import numpy as np
-from matplotlib import colors as mplc
+from matplotlib import colors as mplc, colormaps as mplcm
 from . import sc_utils as scu
 from . import sc_math as scm
 
 
 ##############################################################################
 #%% Color functions
 ##############################################################################
@@ -40,15 +40,15 @@
         if origndim==1:
             colors = colors[0] # Pull it out again
         return colors
 
 
 def sanitizecolor(color, asarray=False, alpha=None, normalize=True):
     '''
-    Alias to ``matplotlib.colors.to_rgb``, but also handles numeric inputs.
+    Alias to :func:`matplotlib.colors.to_rgb`, but also handles numeric inputs.
     
     Arg:
         color (str/list/etc): the input color to sanitize into an RGB tuple (or array)
         asarray (bool): whether to return an array instead of a tuple
         alpha (float): if not None, include the alpha channel with this value
         normalize (bool): whether to divide by 255 if any values are greater than 1
     
@@ -66,15 +66,15 @@
         except ValueError as E:
             errormsg = f'Could not understand "{color}" as a valid color: must be a standard Matplotlib color string'
             raise ValueError(errormsg) from E
     elif isinstance(color, float):
         color = [color]*3 # Consider it grey
             
     color = scu.toarray(color).astype(float) # Get it into consistent format for further operations
-    if len(color) not in [3,4]:
+    if len(color) not in [3,4]: # pragma: no cover
         errormsg = f'Cannot parse {color} as a color: expecting length 3 (RGB) or 4 (RGBA)'
         raise ValueError(errormsg)
     if normalize and color.max()>1:
         color /= 255
     if alpha is not None and len(color) == 3:
         color = scm.cat(color, float(alpha))
     if not asarray:
@@ -91,17 +91,17 @@
     if asarray:
         output = colors
         if reverse: output = output[::-1] # Reverse the array
     else:
         output = []
         for c in colors: # Gather output
             output.append(tuple(c))
-        if reverse: # Reverse the list
+        if reverse: # Reverse the list # pragma: no cover
             output.reverse()
-        if ashex:
+        if ashex: # pragma: no cover
             for c,color in enumerate(output):
                 output[c] = rgb2hex(color)
     return output
 
 
 def shifthue(colors=None, hueshift=0.0):
     '''
@@ -145,17 +145,17 @@
 
     **Example**::
 
         rgb = sc.hex2rgb('#87bc26') # Returns array([0.52941176, 0.7372549 , 0.14901961])
     '''
     if string[0] == '#':
         string = string[1:] # Trim leading #, if it exists
-    if len(string)==3:
-        string = string[0]*2+string[1]*2+string[2]*2 # Convert e.g. '8b2' to '88bb22'
-    if len(string)!=6: # pragma: no cover
+    if len(string) == 3:
+        string = string[0]*2 + string[1]*2 + string[2]*2 # Convert e.g. '8b2' to '88bb22'
+    if len(string) != 6: # pragma: no cover
         errormsg = f'Cannot convert "{string}" to an RGB color: must be 3 or 6 characters long'
         raise ValueError(errormsg)
     hexstring = bytes.fromhex(string) # Ensure it's the right type
     rgb = np.array(struct.unpack('BBB',hexstring),dtype=float)/255.
     return rgb
 
 
@@ -225,16 +225,17 @@
 
         n = 1000
         x = pl.randn(n,1);
         y = pl.randn(n,1);
         c = sc.vectocolor(y);
         pl.scatter(x, y, c=c, s=50)
 
-    | New in version 1.2.0: midpoint argument.
-    | New in version 2.1.0: nancolor argument and remove nans by default
+    | *New in version 1.2.0:* midpoint argument.
+    | *New in version 2.1.0:* nancolor argument and remove nans by default
+    | *New in version 3.0.0:* correct "midpoint" argument
     """
 
     from numpy import array, zeros
 
     if cmap is None:
         cmap = pl.get_cmap() # Get current colormap
     elif isinstance(cmap, str):
@@ -246,25 +247,27 @@
 
     # If a scalar is supplied, convert it to a vector instead
     if scu.isnumber(vector):
         vector = np.linspace(0, 1, vector)
 
     # Usual situation -- the vector has elements
     vector = scu.dcp(vector) # To avoid in-place modification
-    vector = np.array(vector) # Just to be sure
+    vector = np.array(vector, dtype=float) # Just to be sure
     if len(vector):
         if minval is None:
             minval = np.nanmin(vector)
         if maxval is None:
             maxval = np.nanmax(vector)
 
-        vector = vector-minval # Subtract minimum
-        vector = vector/float(maxval-minval) # Divide by maximum
+        diff = maxval - minval
+        vector = (vector - minval)/diff # Normalize vector
         if midpoint is not None:
-            norm = midpointnorm(vcenter=midpoint, vmin=0, vmax=1)
+            vcenter = (midpoint - minval)/diff
+            assert 0 <= vcenter <= 1, f'Values not in order: must be minval={minval:n} <= midpoint={midpoint:n} <= maxval={maxval:n}'
+            norm = midpointnorm(vcenter=vcenter, vmin=0, vmax=1)
             vector = np.array(norm(vector))
         nelements = len(vector) # Count number of elements
         colors = zeros((nelements,4))
         for i in range(nelements):
             point = vector[i]
             if np.isnan(point) and nancolor is not None:
                 color = sanitizecolor(nancolor, alpha=True) # If it's NaN
@@ -287,15 +290,15 @@
     """
     Map an N-dimensional array of values onto the current colormap. An extension
     of vectocolor() for multidimensional arrays; see that function for additional
     arguments.
 
     Args:
         arr (array): a multidimensional array to be converted to an array of colors
-        kwargs(dict): passed to ``sc.vectocolor()``
+        kwargs(dict): passed to :func:`sc.vectocolor() <vectocolor>`
 
     **Example**::
 
         n = 1000
         ncols = 5
         arr = pl.rand(n,ncols)
         for c in range(ncols):
@@ -421,15 +424,15 @@
     ## Wrap up -- turn color array into a list, or reverse
     if hueshift: colors = shifthue(colors, hueshift=hueshift) # Shift hue if requested
     output = _processcolors(colors=colors, asarray=asarray, ashex=ashex, reverse=reverse)
 
     ## For plotting -- optional
     if demo:
         from . import sc_plotting as scp # To avoid circular import
-        ax = scp.scatter3d(colors[:,0], colors[:,1], colors[:,2], c=output, s=200, depthshade=False, lw=0, figkwargs={'facecolor':'w'})
+        ax = scp.scatter3d(colors[:,0], colors[:,1], colors[:,2], c=output, s=200, depthshade=False, lw=0, fig=True, figkwargs={'facecolor':'w'})
         ax.set_xlabel('Red', fontweight='bold')
         ax.set_ylabel('Green', fontweight='bold')
         ax.set_zlabel('Blue', fontweight='bold')
         ax.set_xlim((0,1))
         ax.set_ylim((0,1))
         ax.set_zlim((0,1))
 
@@ -448,15 +451,15 @@
         vmax (float): the maximum of the colormap
 
     **Example**::
 
         data = pl.rand(10,10) - 0.2
         pl.pcolor(data, cmap='bi', norm=sc.midpointnorm())
 
-    New in version 1.2.0.
+    *New in version 1.2.0.*
     '''
     from matplotlib.colors import TwoSlopeNorm
     norm = TwoSlopeNorm(vcenter=vcenter, vmin=vmin, vmax=vmax)
     return norm
 
 
 
@@ -479,15 +482,15 @@
     # Set data
     if n         is None: n         = 100
     if smoothing is None: smoothing = 40
     if randseed  is None: randseed  = 8
     if cmap is None: cmap = 'parula' # For no particular reason
     maxheight = 1
     horizontalsize = 4
-    pl.seed(randseed)
+    np.random.seed(randseed)
     kernel = np.array([0.25,0.5,0.25])
     data = pl.randn(n,n)
     for s in range(smoothing): # Quick-and-dirty-and-slow smoothing
         for i in range(n): data[:,i] = np.convolve(data[:,i],kernel,mode='same')
         for i in range(n): data[i,:] = np.convolve(data[i,:],kernel,mode='same')
     data -= data.min()
     data /= data.max()
@@ -497,28 +500,28 @@
     fig1 = pl.figure(figsize=(10,8))
     X = np.linspace(0,horizontalsize,n)
     pcl = pl.pcolor(X, X, data, cmap=cmap, linewidth=0, antialiased=False, shading='auto')
     cb2 = fig1.colorbar(pcl)
     cb2.set_label('Height (km)',horizontalalignment='right', labelpad=50)
     pl.xlabel('Position (km)')
     pl.ylabel('Position (km)')
-    if doshow:
+    if doshow: # pragma: no cover
         pl.show()
 
     # Plot in 3D
-    fig2,ax2 = scp.fig3d(returnax=True, figsize=(18,8))
+    fig2,ax2 = scp.fig3d(returnax=True, figsize=(12,8))
     ax2.view_init(elev=45, azim=30)
     X = np.linspace(0,horizontalsize,n)
     X, Y = np.meshgrid(X, X)
     surf = ax2.plot_surface(X, Y, data, rstride=1, cstride=1, cmap=cmap, linewidth=0, antialiased=False)
     cb = fig2.colorbar(surf)
     cb.set_label('Height (km)', horizontalalignment='right', labelpad=50)
     pl.xlabel('Position (km)')
     pl.ylabel('Position (km)')
-    if doshow:
+    if doshow: # pragma: no cover
         pl.show()
 
     return {'2d':fig1, '3d':fig2}
 
 
 
 ##############################################################################
@@ -574,15 +577,15 @@
                      (breaks[2], forest1[2], forest1[2]),
                      (breaks[3], forest2[2], forest2[2]),
                      (breaks[4], rock[2], rock[2]),
                      (breaks[5], snow[2], snow[2]))}
 
     # Make map
     cmap = mplc.LinearSegmentedColormap('alpine', cdict, 256)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
     return cmap
 
 
 
 def bicolormap(gap=0.1, mingreen=0.2, redbluemix=0.5, epsilon=0.01, demo=False, apply=False):
     """
@@ -626,15 +629,15 @@
           'blue':   ((0.00000, 1.0, 1.0),
                      (0.5-eps, 1.0, omg),
                      (0.50000, omg, omg),
                      (0.5+eps, omg, mix),
                      (1.00000, 0.0, 0.0))}
 
     cmap = mplc.LinearSegmentedColormap('bi', cdict, 256)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
 
     def demoplot(): # pragma: no cover
 
         maps = []
         maps.append(bicolormap()) # Default ,should work for most things
         maps.append(bicolormap(gap=0,mingreen=0,redbluemix=1,epsilon=0)) # From pure red to pure blue with white in the middle
@@ -645,15 +648,15 @@
         pl.figure(figsize=(5*nexamples, 4))
         for m in range(nexamples):
             pl.subplot(1, nexamples, m+1)
             pl.imshow(np.random.rand(20,20), cmap=maps[m], interpolation='none')
             pl.colorbar()
         pl.show()
 
-    if demo:
+    if demo: # pragma: no cover
         demoplot()
 
     return cmap
 
 
 def parulacolormap(apply=False):
     '''
@@ -697,15 +700,15 @@
             [0.9971,0.7513,0.2309], [0.9972,0.7569,0.2267], [0.9971,0.7626,0.2224], [0.9969,0.7683,0.2181], [0.9966,0.7740,0.2138], [0.9962,0.7798,0.2095], [0.9957,0.7856,0.2053], [0.9949,0.7915,0.2012],
             [0.9938,0.7974,0.1974], [0.9923,0.8034,0.1939], [0.9906,0.8095,0.1906], [0.9885,0.8156,0.1875], [0.9861,0.8218,0.1846], [0.9835,0.8280,0.1817], [0.9807,0.8342,0.1787], [0.9778,0.8404,0.1757],
             [0.9748,0.8467,0.1726], [0.9720,0.8529,0.1695], [0.9694,0.8591,0.1665], [0.9671,0.8654,0.1636], [0.9651,0.8716,0.1608], [0.9634,0.8778,0.1582], [0.9619,0.8840,0.1557], [0.9608,0.8902,0.1532],
             [0.9601,0.8963,0.1507], [0.9596,0.9023,0.1480], [0.9595,0.9084,0.1450], [0.9597,0.9143,0.1418], [0.9601,0.9203,0.1382], [0.9608,0.9262,0.1344], [0.9618,0.9320,0.1304], [0.9629,0.9379,0.1261],
             [0.9642,0.9437,0.1216], [0.9657,0.9494,0.1168], [0.9674,0.9552,0.1116], [0.9692,0.9609,0.1061], [0.9711,0.9667,0.1001], [0.9730,0.9724,0.0938], [0.9749,0.9782,0.0872], [0.9769,0.9839,0.0805]]
 
     cmap = mplc.LinearSegmentedColormap.from_list('parula', data)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
     return cmap
 
 
 def turbocolormap(apply=False):
     '''
     NOTE: as of Matplotlib 3.4.0, this colormap is included by default, and will
@@ -759,15 +762,15 @@
             [0.87422,0.24526,0.03297],[0.86760,0.23730,0.03082],[0.86079,0.22945,0.02875],[0.85380,0.22170,0.02677],[0.84662,0.21407,0.02487],[0.83926,0.20654,0.02305],[0.83172,0.19912,0.02131],[0.82399,0.19182,0.01966],
             [0.81608,0.18462,0.01809],[0.80799,0.17753,0.01660],[0.79971,0.17055,0.01520],[0.79125,0.16368,0.01387],[0.78260,0.15693,0.01264],[0.77377,0.15028,0.01148],[0.76476,0.14374,0.01041],[0.75556,0.13731,0.00942],
             [0.74617,0.13098,0.00851],[0.73661,0.12477,0.00769],[0.72686,0.11867,0.00695],[0.71692,0.11268,0.00629],[0.70680,0.10680,0.00571],[0.69650,0.10102,0.00522],[0.68602,0.09536,0.00481],[0.67535,0.08980,0.00449],
             [0.66449,0.08436,0.00424],[0.65345,0.07902,0.00408],[0.64223,0.07380,0.00401],[0.63082,0.06868,0.00401],[0.61923,0.06367,0.00410],[0.60746,0.05878,0.00427],[0.59550,0.05399,0.00453],[0.58336,0.04931,0.00486],
             [0.57103,0.04474,0.00529],[0.55852,0.04028,0.00579],[0.54583,0.03593,0.00638],[0.53295,0.03169,0.00705],[0.51989,0.02756,0.00780],[0.50664,0.02354,0.00863],[0.49321,0.01963,0.00955],[0.47960,0.01583,0.01055]]
 
     cmap = mplc.LinearSegmentedColormap.from_list('turbo', data)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
     return cmap
 
 
 
 def bandedcolormap(minvalue=None, minsaturation=None, hueshift=None, saturationscale=None, npts=None, apply=False):
     '''
@@ -796,51 +799,51 @@
     hsv[:,2] = pl.sqrt(pl.linspace(minvalue,1,npts)) # Value: map linearly
     hsv[:,0] = pl.sin(x+hueshift)**2 # Hue: a big sine wave
     hsv[:,1] = minsaturation+(1-minsaturation)*pl.sin(saturationscale*x)**2 # Saturation: a small sine wave
     data = hsv2rgb(hsv)
 
     # Create and use
     cmap = mplc.LinearSegmentedColormap.from_list('banded', data)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
     return cmap
 
 
 def orangebluecolormap(apply=False):
     '''
     Create an orange-blue colormap; most like RdYlBu but more pleasing. Created
     by Prashanth Selvaraj.
 
     **Demo and example**::
 
         cmap = sc.orangebluecolormap()
         sc.colormapdemo(cmap=cmap)
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     '''
     bottom = pl.get_cmap('Oranges', 128)
-    top = pl.get_cmap('Blues_r', 128)
-    x = np.linspace(0, 1, 128)
-    data = np.vstack((top(x), bottom(x)))
+    top    = pl.get_cmap('Blues_r', 128)
+    x      = np.linspace(0, 1, 128)
+    data   = np.vstack((top(x), bottom(x)))
 
     # Create and use
     cmap = mplc.LinearSegmentedColormap.from_list('orangeblue', data)
-    if apply:
+    if apply: # pragma: no cover
         pl.set_cmap(cmap)
     return cmap
 
 
-# Register colormaps
+# Register colormaps -- under their original names as well as with the "sciris-" prefix
 existing = pl.colormaps()
 colormap_map = dict(
     alpine     = alpinecolormap(),
     parula     = parulacolormap(),
     banded     = bandedcolormap(),
     bi         = bicolormap(),
     orangeblue = orangebluecolormap(),
     turbo      = turbocolormap(),
 )
 for origname,cmap in colormap_map.items():
     newname = f'sciris-{origname}'
     for name in [origname, newname]:
         if name not in existing: # Avoid re-registering already registered colormaps
-            pl.register_cmap(name=name, cmap=cmap)
+            mplcm.register(cmap=cmap, name=name)
```

### Comparing `sciris-2.1.0/sciris/sc_dataframe.py` & `sciris-3.0.0/sciris/sc_settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,637 +1,743 @@
 '''
-Extension of the pandas dataframe to be more flexible, especially with filtering
-rows/columns and concatenating data.
+Define options for Sciris, mostly plotting options.
+
+All options should be set using ``set()`` or directly, e.g.::
+
+    sc.options(font_size=18)
+
+To reset default options, use::
+
+    sc.options('default')
+
+Note: "options" is used to refer to the choices available (e.g., DPI), while "settings"
+is used to refer to the choices made (e.g., ``dpi=150``).
 '''
 
-##############################################################################
-#%% Dataframe
-##############################################################################
-
-import numbers # For numeric type
-import numpy as np
-import pandas as pd
+import os
+import re
+import inspect
+import warnings
+import collections as co
+import pylab as pl
 from . import sc_utils as scu
-from . import sc_math as scm
 from . import sc_odict as sco
+from . import sc_printing as scp
 
 
-__all__ = ['dataframe']
+__all__ = ['ScirisOptions', 'options', 'parse_env', 'help']
 
-class dataframe(pd.DataFrame):
+#%% Define plotting options
+# See also simple.mplstyle and fancy.mplstyle files, which can be generated by:
+#   sc.saveyaml('simple.mplstyle', sc.sc_settings.rc_simple)
+#   sc.saveyaml('fancy.mplstyle',  sc.sc_settings.rc_fancy)
+
+# Define simple plotting options -- similar to Matplotlib default
+rc_simple = {
+    'axes.axisbelow':    True, # So grids show up behind
+    'axes.spines.right': False,
+    'axes.spines.top':   False,
+    'figure.facecolor':  'white',
+    'font.family':       'sans-serif', # Replaced with Mulish in load_fonts() if import succeeds
+    'legend.frameon':    False,
+}
+
+# Define default plotting options -- loosely inspired by Seaborn
+rc_fancy = scu.dcp(rc_simple)
+rc_fancy.update({
+    'axes.facecolor': '#f2f2ff',
+    'axes.grid':      True,
+    'grid.color':     'white',
+    'grid.linewidth':  1,
+    'lines.linewidth': 2,
+})
+
+
+def parse_env(var, default=None, which='str'):
     '''
-    An extension of the pandas dataframe with additional convenience methods for
-    accessing rows and columns and performing other operations.
-    
+    Simple function to parse environment variables
+
     Args:
-        data (dict/array/dataframe): the data to use
-        columns (list): column labels
-        nrows (int): the number of arrows to preallocate (default 0)
-        kwargs (dict): passed to ``pd.DataFrame()``
+        var (str): name of the environment variable to get
+        default (any): default value
+        which (str): what type to convert to (if None, don't convert)
 
-    **Examples**::
+    *New in version 2.0.0.*
+    '''
+    val = os.getenv(var, default)
+    if which is None:
+        return val
+    elif which in ['str', 'string']:
+        if val: out = str(val)
+        else:   out = ''
+    elif which == 'int':
+        if val: out = int(val)
+        else:   out = 0
+    elif which == 'float':
+        if val: out = float(val)
+        else:   out = 0.0
+    elif which == 'bool':
+        if val:
+            if isinstance(val, str):
+                if val.lower() in ['false', 'f', '0', '', 'none']:
+                    val = False
+                else:
+                    val = True
+            out = bool(val)
+        else:
+            out = False
+    else: # pragma: no cover
+        errormsg = f'Could not understand type "{which}": must be None, str, int, float, or bool'
+        raise ValueError(errormsg)
+    return out
 
-        a = sc.dataframe(cols=['x','y'],data=[[1238,2],[384,5],[666,7]]) # Create data frame
-        a['x'] # Print out a column
-        a[0] # Print out a row
-        a['x',0] # Print out an element
-        a[0] = [123,6]; print(a) # Set values for a whole row
-        a['y'] = [8,5,0]; print(a) # Set values for a whole column
-        a['z'] = [14,14,14]; print(a) # Add new column
-        a.addcol('z', [14,14,14]); print(a) # Alternate way to add new column
-        a.rmcol('z'); print(a) # Remove a column
-        a.pop(1); print(a) # Remove a row
-        a.append([555,2,14]); print(a) # Append a new row
-        a.insert(1,[555,2,14]); print(a) # Insert a new row
-        a.sort(); print(a) # Sort by the first column
-        a.sort('y'); print(a) # Sort by the second column
-        a.addrow([555,2,14]); print(a) # Replace the previous row and sort
-        a.getrow(1) # Return the row starting with value '1'
-        a.rmrow(); print(a) # Remove last row
-        a.rmrow(1238); print(a) # Remove the row starting with element '3'
 
-    The dataframe can be used for both numeric and non-numeric data.
+#%% Define the options class
 
-    | New in version 2.0.0: subclass pandas DataFrame
+class ScirisOptions(sco.objdict):
     '''
+    Set options for Sciris.
 
-    def __init__(self, data=None, columns=None, nrows=None, **kwargs):
+    Note: this class should not be invoked directly. An instance is created automatically,
+    which is the accessible via ``sc.options``.
 
-        # Handle inputs
-        if 'cols' in kwargs:
-            columns = kwargs.pop('cols')
-        if nrows and data is None:
-            ncols = len(columns)
-            data = np.zeros((nrows, ncols))
+    Use ``sc.options.set('defaults')`` to reset all values to default, or ``sc.options.set(dpi='default')``
+    to reset one parameter to default. See :meth:`sc.options.help(detailed=True) <ScirisOptions.help>` for
+    more information.
+
+    Options can also be saved and loaded using :meth:`sc.options.save() <ScirisOptions.save>` and :meth:`sc.options.load() <ScirisOptions.load>`.
+    See :meth:`sc.options.with_style() <ScirisOptions.with_style>` to set options temporarily.
+
+    Common options are (see also :meth:`sc.options.help(detailed=True) <ScirisOptions.help>`):
+
+        - dpi:            the overall DPI (i.e. size) of the figures
+        - font:           the font family/face used for the plots
+        - fontsize:       the font size used for the plots
+        - backend:        which Matplotlib backend to use
+        - interactive:    convenience method to set backend
+        - jupyter:        defaults for Jupyter (change backend)
+        - style:          the plotting style to use
+
+    Each setting can also be set with an environment variable, e.g. SCIRIS_DPI.
+    Note also the environment variable SCIRIS_LAZY, which imports Sciris lazily
+    (i.e. does not import submodules).
+
+    **Examples**::
+
+        sc.options(dpi=150) # Larger size
+        sc.options(style='simple', font='Rosario') # Change to the "simple" Sciris style with a custom font
+        sc.options.set(fontsize=18, show=False, backend='agg', precision=64) # Multiple changes
+        sc.options(interactive=False) # Turn off interactive plots
+        sc.options(jupyter=True) # Defaults for Jupyter
+        sc.options('defaults') # Reset to default options
+
+    | *New in version 1.3.0.*
+    | *New in version 2.0.0:* revamped with additional options ``interactive`` and ``jupyter``, plus styles
+    | *New in version 3.0.0:* renamed from Options to ScirisOptions to avoid potential confusion with ``sc.options``
+    '''
 
-        # Create the dataframe
-        super().__init__(data=data, columns=columns, **kwargs)
+    def __init__(self):
+        super().__init__()
+        optdesc, options = self.get_orig_options() # Get the options
+        self.update(options) # Update this object with them
+        self.optdesc = optdesc # Set the description as an attribute, not a dict entry
+        self.orig_options = scu.dcp(options) # Copy the default options
         return
 
 
-    @property
-    def cols(self):
-        ''' Get columns as a list '''
-        return self.columns.tolist()
+    def __call__(self, *args, **kwargs):
+        '''Allow ``sc.options(dpi=150)`` instead of ``sc.options.set(dpi=150)`` '''
+        return self.set(*args, **kwargs)
 
 
-    def _to_array(self, arr):
-        ''' Try to conver to the current data type, or else use an object '''
-        try: # Try to use current type
-            output = np.array(arr, dtype=self.values.dtype)
-        except: # This is to e.g. not force conversion to strings # pragma: no cover
-            output = np.array(arr, dtype=object)
+    def to_dict(self):
+        ''' Pull out only the settings from the options object '''
+        return {k:v for k,v in self.items()}
+
+
+    def __repr__(self):
+        ''' Brief representation '''
+        output = scp.objectid(self)
+        output += 'Sciris options (see also sc.options.disp()):\n'
+        output += scu.pp(self.to_dict(), output=True)
         return output
 
 
-    def _val2row(self, value=None, to2d=True):
-        ''' Convert a list, array, or dictionary to the right format for appending to a dataframe '''
-        if isinstance(value, dict):
-            output = np.zeros(self.ncols, dtype=object)
-            for c,col in enumerate(self.cols):
-                try:
-                    output[c] = value[col]
-                except:
-                    errormsg = f'Entry for column {col} not found; keys you supplied are: {scu.strjoin(value.keys())}'
-                    raise Exception(errormsg)
-        elif value is None:
-            output = np.empty(self.ncols)
-        else: # Not sure what it is, just make it an array
-            output = self._to_array(value)
-
-        # Validation
-        if output.ndim == 1: # Convert from 1D to 2D
-            shape = output.shape[0]
-            if to2d:
-                output = np.array([output])
-        else:
-            shape = output.shape[1]
-        if shape != self.ncols:
-            errormsg = f'Row has wrong length ({shape} supplied, {self.ncols} expected)'
-            raise IndexError(errormsg)
+    def __enter__(self):
+        ''' Allow to be used in a with block '''
+        return self
 
-        # Try to convert back to default type, but don't worry if not
-        try:
-            output = np.array(output, dtype=self.values.dtype)
-        except: # pragma: no cover
-            pass
 
-        return output
+    def __exit__(self, *args, **kwargs):
+        ''' Allow to be used in a with block '''
+        try:
+            reset = {}
+            for k,v in self.on_entry.items():
+                if self[k] != v: # Only reset settings that have changed
+                    reset[k] = v
+            self.set(**reset)
+            del self.on_entry
+        except AttributeError as E: # pragma: no cover
+            errormsg = 'Please use sc.options.context() if using a with block'
+            raise AttributeError(errormsg) from E
+        return
 
 
-    def _sanitizecol(self, col, die=True):
-        ''' Take None or a string and return the index of the column '''
-        if col is None:
-            output = 0 # If not supplied, assume first column is control
-        elif scu.isstring(col):
-            try:
-                output = self.cols.index(col) # Convert to index
-            except Exception as E: # pragma: no cover
-                errormsg = 'Could not get index of column "%s"; columns are:\n%s\n%s' % (col, '\n'.join(self.cols), str(E))
-                if die:
-                    raise scu.KeyNotFoundError(errormsg)
-                else:
-                    print(errormsg)
-                    output = None
-        elif scu.isnumber(col):
-            output = col
-        else: # pragma: no cover
-            errormsg = f'Unrecognized column/column type "{col}" {type(col)}'
-            if die:
-                raise ValueError(errormsg)
-            else:
-                print(errormsg)
-                output = None
-        return output
+    def disp(self):
+        ''' Detailed representation '''
+        output = 'Sciris options (see also sc.options.help()):\n'
+        keylen = 14 # Maximum key length  -- "numba_parallel"
+        for k,v in self.items():
+            keystr = scp.colorize(f'  {k:>{keylen}s}: ', fg='cyan', output=True)
+            reprstr = scu.pp(v, output=True)
+            reprstr = scp.indent(n=keylen+4, text=reprstr, width=None)
+            output += f'{keystr}{reprstr}'
+        print(output)
+        return
 
 
     @staticmethod
-    def _cast(arr):
-        ''' Attempt to cast an array to different data types, to avoid having completely numeric arrays of object type '''
-        output = arr
-        if isinstance(arr, np.ndarray) and np.can_cast(arr, numbers.Number, casting='same_kind'): # Check that everything is a number before trying to cast to an array
-            try: # If it is, try to cast the whole array to the type of the first element
-                output = np.array(arr, dtype=type(arr[0]))
-            except: # If anything goes wrong, do nothing # pragma: no cover
-                pass
-        return output
+    def get_orig_options():
+        '''
+        Set the default options for Sciris -- not to be called by the user, use
+        :meth:`sc.options.set('defaults') <ScirisOptions.set>` instead.
+        '''
 
+        # Options acts like a class, but is actually an objdict for simplicity
+        optdesc = sco.objdict() # Help for the options
+        options = sco.objdict() # The options
 
-    def __getitem__(self, key=None, die=True, cast=True):
-        ''' Simple method for returning; see self.flexget() for a version based on col and row '''
-        try:
-            output = super().__getitem__(key)
-        except:
-            if scu.isstring(key): # e.g. df['a'] -- usually handled by pandas # pragma: no cover
-                rowindex = slice(None)
-                try:
-                    colindex = self.cols.index(key)
-                except ValueError:
-                    errormsg = f'Key "{key}" is not a valid column; choices are: {scu.strjoin(self.cols)}'
-                    raise scu.KeyNotFoundError(errormsg)
-            elif isinstance(key, (numbers.Number, list, np.ndarray, slice)): # e.g. df[0], df[[0,2]], df[:4]
-                rowindex = key
-                colindex = slice(None)
-            elif isinstance(key, tuple):
-                rowindex = key[0]
-                colindex = key[1]
-                if scu.isstring(rowindex) and not scu.isstring(colindex): # Swap order if one's a string and the other isn't
-                    rowindex, colindex = colindex, rowindex
-                if scu.isstring(colindex): # e.g. df['a',0]
-                    colindex = self.cols.index(colindex)
-            else: # pragma: no cover
-                errormsg = f'Unrecognized dataframe key of {type(key)}: must be str, numeric, or tuple'
-                if die:
-                    raise scu.KeyNotFoundError(errormsg)
-                else:
-                    print(errormsg)
-                    output = None
-            output = self.iloc[rowindex,colindex]
+        optdesc.sep = 'Set thousands seperator'
+        options.sep = parse_env('SCIRIS_SEP', ',', 'str')
 
-        return output
+        optdesc.aspath = 'Set whether to return Path objects instead of strings by default'
+        options.aspath = parse_env('SCIRIS_ASPATH', False, 'bool')
 
+        optdesc.style = 'Set the default plotting style -- options are "default", "simple", and "fancy", plus those in pl.style.available; see also options.rc'
+        options.style = parse_env('SCIRIS_STYLE', 'default', 'str')
 
-    def set(self, key, value=None):
-        ''' Alias to pandas __setitem__ method '''
-        return super().__setitem__(key, value)
+        optdesc.dpi = 'Set the default DPI -- the larger this is, the larger the figures will be'
+        options.dpi = parse_env('SCIRIS_DPI', pl.rcParams['figure.dpi'], 'int')
 
+        optdesc.font = 'Set the default font family (e.g., sans-serif or Arial)'
+        options.font = parse_env('SCIRIS_FONT', pl.rcParams['font.family'], None) # Can be a string or list, so don't cast it to any object
 
-    def __setitem__(self, key, value=None):
-        try:
-            assert isinstance(key, str) or key in self.cols # Don't create new non-text columns, only set existing ones
-            super().__setitem__(key, value)
-        except:
-            if scu.isnumber(key):
-                newrow = self._val2row(value, to2d=False) # Make sure it's in the correct format
-                if len(newrow) != self.ncols:
-                    errormsg = f'Vector has incorrect length ({len(newrow)} vs. {self.ncols})'
-                    raise Exception(errormsg)
-                rowindex = int(key)
-                try:
-                    self.iloc[rowindex,:] = newrow
-                except:
-                    self.appendrow(value)
-            elif isinstance(key, tuple):
-                rowindex = key[0]
-                colindex = key[1]
-                if scu.isstring(rowindex) and not scu.isstring(colindex): # Swap order if one's a string and the other isn't
-                    rowindex, colindex = colindex, rowindex
-                if scu.isstring(colindex): # e.g. df['a',0]
-                    colindex = self.cols.index(colindex)
-                self.iloc[rowindex,colindex] = value
-        return
+        optdesc.fontsize = 'Set the default font size'
+        options.fontsize = parse_env('SCIRIS_FONT_SIZE', pl.rcParams['font.size'], 'str')
+
+        optdesc.interactive = 'Convenience method to set figure backend'
+        options.interactive = parse_env('SCIRIS_INTERACTIVE', True, 'bool')
 
+        optdesc.jupyter = 'Convenience method to set common settings for Jupyter notebooks: set to "auto" (which detects if Jupyter is running), "retina", "default" (or empty, which use regular PNG output), or "widget" to set backend'
+        options.jupyter = parse_env('SCIRIS_JUPYTER', 'auto', 'str')
 
-    def flexget(self, cols=None, rows=None, asarray=False, cast=True, default=None):
+        optdesc.backend = 'Set the Matplotlib backend (use "agg" for non-interactive)'
+        options.backend = parse_env('SCIRIS_BACKEND', pl.get_backend(), 'str')
+
+        optdesc.rc = 'Matplotlib rc (run control) style parameters used during plotting -- usually set automatically by "style" option'
+        options.rc = {}
+
+        return optdesc, options
+
+
+    def set(self, key=None, value=None, use=True, **kwargs):
         '''
-        More complicated way of getting data from a dataframe. While getting directly
-        by key usually returns the array data directly, this usually returns another
-        dataframe.
+        Actually change the style. See :meth:`sc.options.help() <ScirisOptions.help>` for more information.
 
         Args:
-            cols (str/list): the column(s) to get
-            rows (int/list): the row(s) to get
-            asarray (bool): whether to return an array (otherwise, return a dataframe)
-            cast (bool): attempt to cast to an all-numeric array
-            default (any): the value to return if the column(s)/row(s) can't be found
+            key    (str):    the parameter to modify, or 'defaults' to reset everything to default values
+            value  (varies): the value to specify; use None or 'default' to reset to default
+            use    (bool):   whether to immediately apply the change (to Matplotlib)
+            kwargs (dict):   if supplied, set multiple key-value pairs
 
         **Example**::
 
-            df = sc.dataframe(cols=['x','y','z'],data=[[1238,2,-1],[384,5,-2],[666,7,-3]]) # Create data frame
-            df.flexget(cols=['x','z'], rows=[0,2])
+            sc.options.set(dpi=50) # Equivalent to sc.options(dpi=50)
         '''
-        if cols is None:
-            colindices = Ellipsis
-        else:
-            colindices = []
-            for col in scu.tolist(cols):
-                colindices.append(self._sanitizecol(col))
-        if rows is None:
-            rowindices = Ellipsis
-        else:
-            rowindices = rows
 
-        output = self.iloc[rowindices,colindices] # Split up so can handle non-consecutive entries in either
-        if output.size == 1: output = output[0] # If it's a single element, return the value rather than the array
-        if asarray:
-            if cast:
-                output = self._cast(output)
-            return output
-        else:
-            output = dataframe(cols=np.array(self.cols)[colindices].tolist(), data=output)
+        # Reset to defaults
+        if key in ['default', 'defaults']:
+            kwargs = self.orig_options # Reset everything to default
+
+        # Handle other keys
+        elif key is not None:
+            kwargs.update({key:value})
+
+        # Handle Jupyter
+        self.set_jupyter(kwargs)
+
+        # Handle interactivity
+        if 'interactive' in kwargs.keys():
+            interactive = kwargs['interactive']
+            if interactive in [None, 'default']:
+                interactive = self.orig_options['interactive']
+            if interactive:
+                kwargs['backend'] = self.orig_options['backend']
+            else:
+                kwargs['backend'] = 'agg'
 
-        return output
+        # Reset options
+        for key,value in kwargs.items():
+
+            # Handle deprecations
+            rename = {'font_size': 'fontsize', 'font_family':'font'}
+            if key in rename.keys(): # pragma: no cover
+                oldkey = key
+                key = rename[oldkey]
+
+            if key not in self.keys(): # pragma: no cover
+                keylist = self.orig_options.keys()
+                keys = '\n'.join(keylist)
+                errormsg = f'Option "{key}" not recognized; options are "defaults" or:\n{keys}\n\nSee help(sc.options.set) for more information.'
+                raise ValueError(errormsg) from KeyError(key) # Can't use sc.KeyNotFoundError since would be a circular import
+            else:
+                if value in [None, 'default']:
+                    value = self.orig_options[key]
+                self[key] = value
+                matplotlib_keys = ['fontsize', 'font', 'dpi', 'backend']
+                if key in matplotlib_keys:
+                    self.set_matplotlib_global(key, value)
+
+        if use:
+            self.use_style()
+
+        return
 
 
-    def disp(self, nrows=None, ncols=None, width=999, precision=4, options=None):
+    def context(self, **kwargs):
         '''
-        Flexible display of a dataframe, showing all rows/columns by default.
+        Alias to set() for non-plotting options, for use in a "with" block.
+
+        Note: for plotting options, use :meth:`sc.options.with_style() <ScirisOptions.with_style>`, which is linked
+        to Matplotlib's context manager. If you set plotting options with this,
+        they won't have any effect.
+        '''
+        # Store current settings
+        self.on_entry = {k:self[k] for k in kwargs.keys()}
+
+        # Make changes
+        self.set(**kwargs)
+        return self
+
+
+    def set_matplotlib_global(self, key, value):
+        ''' Set a global option for Matplotlib -- not for users '''
+        if value: # Don't try to reset any of these to a None value
+            if   key == 'fontsize': pl.rcParams['font.size']   = value
+            elif key == 'font':     pl.rcParams['font.family'] = value
+            elif key == 'dpi':      pl.rcParams['figure.dpi']  = value
+            elif key == 'backend':  pl.switch_backend(value)
+            else: raise KeyError(f'Key {key} not found')
+        return
+
+
+    def set_jupyter(self, kwargs=None):
+        ''' Handle Jupyter settings '''
+        if kwargs is None: # Default setting
+            kwargs = dict(jupyter=self['jupyter'])
         
-        Args:
-            nrows (int): maximum number of rows to show (default: all)
-            ncols (int): maximum number of columns to show (default: all)
-            width (int): maximum screen width (default: 999)
-            precision (int): number of decimal places to show (default: 4)
-            kwargs (dict): passed to ``pd.option_context()``
+        if scu.isjupyter() and 'jupyter' in kwargs.keys(): # pragma: no cover
         
-        **Examples**::
-            
-            df = sc.dataframe(data=np.random.rand(100,10))
-            df.disp()
-            df.disp(precision=1, ncols=5, options={'display.colheader_justify': 'left'})
+            # Handle import
+            try:
+                from IPython import get_ipython
+                import matplotlib_inline
+                magic = get_ipython().run_line_magic
+            except Exception as E:
+                warnmsg = f'Could not import IPython and matplotlib_inline; not attempting to set Jupyter ({str(E)})'
+                warnings.warn(warnmsg, category=UserWarning, stacklevel=2)
+                magic = None
+                
+            # Import succeeded
+            if magic:
+
+                # Handle options
+                widget_opts  = ['widget', 'matplotlib', 'interactive']
+                retina_opts  = [True, 'True', 'auto', 'retina']
+                default_opts = [None, False, '', 'False', 'default']
+                format_opts  = ['retina', 'pdf','png','png2x','svg','jpg']
+    
+                jupyter = kwargs['jupyter']
+                if jupyter in widget_opts:
+                    jupyter = 'widget'
+                elif jupyter in retina_opts:
+                    jupyter = 'retina'
+                elif jupyter in default_opts:
+                    jupyter = 'png'
+    
+                if jupyter == 'widget':
+                    try: # First try interactive
+                        with scp.capture() as stderr: # Hack since this outputs text rather an actual warning
+                            magic('matplotlib', 'widget')
+                        assert 'Warning' not in stderr, stderr
+                    except Exception as E:
+                        warnmsg = f'Could not set backend to "widget" (error: "{E}"); try "pip install ipympl". Defaulting to "retina" instead'
+                        warnings.warn(warnmsg, category=UserWarning, stacklevel=2)
+                        jupyter = 'retina'
+                if jupyter in format_opts:
+                    magic('matplotlib', 'inline')
+                    matplotlib_inline.backend_inline.set_matplotlib_formats(jupyter)
+                else:
+                    errormsg = f'Could not understand Jupyter option "{jupyter}": options are widget, {scu.strjoin(format_opts)}'
+                    raise ValueError(errormsg)
         
-        New in version 2.0.1.
-        '''
-        opts = scu.mergedicts({
-            'display.max_rows': nrows,
-            'display.max_columns': ncols,
-            'display.width': width,
-            'display.precision': precision,
-            }, options
-        )
-        optslist = [item for pair in opts.items() for item in pair] # Convert from dict to list
-        with pd.option_context(*optslist):
-            print(self)
         return
 
 
-    def poprow(self, key, returnval=True):
-        ''' Remove a row from the data frame '''
-        rowindex = int(key)
-        thisrow = self.iloc[rowindex,:]
-        self.drop(rowindex, inplace=True)
-        if returnval: return thisrow
-        else:         return
+    def get_default(self, key):
+        ''' Helper function to get the original default options '''
+        return self.orig_options[key]
 
 
-    def replacedata(self, newdata=None, newdf=None, reset_index=True, inplace=True):
-        '''
-        Replace data in the dataframe with other data
-
-        Args:
-            newdata (array): replace the dataframe's data with these data
-            newdf (dataframe): substitute the current dataframe with this one
-            reset_index (bool): update the index
-            inplace (bool): whether to modify in-place
-        '''
-        if newdf is None:
-            newdf = dataframe(data=newdata, columns=self.columns)
-        if reset_index:
-            newdf.reset_index(drop=True, inplace=True)
-        if inplace:
-            self.__dict__ = newdf.__dict__ # Hack to copy in-place
-            return self
+    def changed(self, key):
+        ''' Check if current setting has been changed from default '''
+        if key in self.orig_options:
+            return self[key] != self.orig_options[key]
         else:
-            return newdf
+            return None
 
 
-    def appendrow(self, value, reset_index=True, inplace=True):
+    def help(self, detailed=False, output=False):
         '''
-        Add a row to the end of the dataframe. See also ``concat()`` and ``insertrow()``.
+        Print information about options.
 
         Args:
-            value (array): the row(s) to append
-            reset_index (bool): update the index
-            inplace (bool): whether to modify in-place
+            detailed (bool): whether to print out full help
+            output (bool): whether to return a list of the options
+
+        **Example**::
+
+            sc.options.help(detailed=True)
         '''
-        newrow = self._val2row(value) # Make sure it's in the correct format
-        newdata = np.vstack((self.values, newrow))
-        return self.replacedata(newdata=newdata, reset_index=reset_index, inplace=inplace)
+
+        # If not detailed, just print the docstring for sc.options
+        if not detailed:
+            print(self.__doc__)
+            return
+
+        n = 15 # Size of indent
+        optdict = sco.objdict()
+        for key in self.orig_options.keys():
+            entry = sco.objdict()
+            entry.key = key
+            entry.current = scp.indent(n=n, width=None, text=scu.pp(self[key], output=True)).rstrip()
+            entry.default = scp.indent(n=n, width=None, text=scu.pp(self.orig_options[key], output=True)).rstrip()
+            if not key.startswith('rc'):
+                entry.variable = f'SCIRIS_{key.upper()}' # NB, hard-coded above!
+            else:
+                entry.variable = 'No environment variable'
+            entry.desc = scp.indent(n=n, text=self.optdesc[key])
+            optdict[key] = entry
+
+        # Convert to a dataframe for nice printing
+        print('Sciris global options ("Environment" = name of corresponding environment variable):')
+        for k, key, entry in optdict.enumitems():
+            scp.heading(f'{k}. {key}', spaces=0, spacesafter=0)
+            changestr = '' if entry.current == entry.default else ' (modified)'
+            print(f'          Key: {key}')
+            print(f'      Current: {entry.current}{changestr}')
+            print(f'      Default: {entry.default}')
+            print(f'  Environment: {entry.variable}')
+            print(f'  Description: {entry.desc}')
+
+        scp.heading('Methods:', spacesafter=0)
+        print('''
+    sc.options(key=value) -- set key to value
+    sc.options[key] -- get or set key
+    sc.options.set() -- set option(s)
+    sc.options.get_default() -- get default setting(s)
+    sc.options.load() -- load settings from file
+    sc.options.save() -- save settings to file
+    sc.options.to_dict() -- convert to dictionary
+    sc.options.with_style() -- create style context for plotting
+''')
+
+        if output:
+            return optdict
+        else:
+            return
 
 
-    def insertrow(self, row=0, value=None, reset_index=True, inplace=True):
+    def load(self, filename, verbose=True, **kwargs):
         '''
-        Insert a row at the specified location. See also ``concat()`` and ``appendrow()``.
+        Load current settings from a JSON file.
 
         Args:
-            row (int): index at which to insert new row(s)
-            value (array): the row(s) to insert
-            reset_index (bool): update the index
-            inplace (bool): whether to modify in-place
+            filename (str): file to load
+            kwargs (dict): passed to :func:`sc.loadjson() <loadjson>`
         '''
-        rowindex = int(row)
-        newrow = self._val2row(value) # Make sure it's in the correct format
-        newdata = np.vstack((self.iloc[:rowindex,:], newrow, self.iloc[rowindex:,:]))
-        return self.replacedata(newdata=newdata, reset_index=reset_index, inplace=inplace)
+        from . import sc_fileio as scf # To avoid circular import
+        json = scf.loadjson(filename=filename, **kwargs)
+        current = self.to_dict()
+        new = {k:v for k,v in json.items() if v != current[k]} # Don't reset keys that haven't changed
+        self.set(**new)
+        if verbose: print(f'Settings loaded from {filename}')
+        return
 
 
-    def concat(self, data, *args, columns=None, reset_index=True, inplace=False, dfargs=None, **kwargs):
+    def save(self, filename, verbose=True, **kwargs):
         '''
-        Concatenate additional data onto the current dataframe. See also ```appendrow()``
-        and ``insertrow()``.
+        Save current settings as a JSON file.
 
         Args:
-            data (dataframe/array): the data to concatenate
-            *args (dataframe/array): additional data to concatenate
-            columns (list): if supplied, columns to go with the data
-            reset_index (bool): update the index
-            inplace (bool): whether to append in place
-            dfargs (dict): arguments passed to construct each dataframe
-            **kwargs (dict): passed to ``pd.concat()``
-        
-        | New in version 2.0.2: "inplace" defaults to False
+            filename (str): file to save to
+            kwargs (dict): passed to :func:`sc.savejson() <savejson>`
         '''
-        dfargs = scu.mergedicts(dfargs)
-        dfs = [self]
-        if columns is None:
-            columns = self.columns
-        for arg in scu.tolist(data, coerce='tuple') + list(args):
-            if isinstance(arg, pd.DataFrame):
-                df = arg
-            else:
-                arg = np.array(arg)
-                if arg.shape == (self.ncols,): # It's a single row: make 2D
-                    arg = np.array([arg])
-                df = dataframe(data=arg, columns=columns, **dfargs)
-            dfs.append(df)
-        newdf = pd.concat(dfs, **kwargs)
-        return self.replacedata(newdf=newdf, reset_index=reset_index, inplace=inplace)
+        from . import sc_fileio as scf # To avoid circular import
+        json = self.to_dict()
+        output = scf.savejson(filename=filename, obj=json, **kwargs)
+        if verbose: print(f'Settings saved to {filename}')
+        return output
 
 
-    @staticmethod
-    def cat(data, *args, dfargs=None, **kwargs):
-        '''
-        Convenience method for concatenating multiple dataframes.
+    def _handle_style(self, style=None, reset=False, copy=True):
+        ''' Helper function to handle logic for different styles '''
+        rc = self.rc # By default, use current
+        if isinstance(style, dict): # If an rc-like object is supplied directly # pragma: no cover
+            rc = scu.dcp(style)
+        elif style is not None: # Usual use case
+            stylestr = str(style).lower()
+            if stylestr in ['default', 'matplotlib', 'reset']:
+                pl.style.use('default') # Need special handling here since not in pl.style.library...ugh
+                rc = {}
+            elif stylestr in ['simple', 'sciris']:
+                rc = scu.dcp(rc_simple)
+            elif stylestr in ['fancy', 'covasim']:
+                rc = scu.dcp(rc_fancy)
+            elif style in pl.style.library:
+                rc = scu.dcp(pl.style.library[style])
+            else: # pragma: no cover
+                errormsg = f'Style "{style}"; not found; options are "default", "simple", "fancy", plus:\n{scu.newlinejoin(pl.style.available)}'
+                raise ValueError(errormsg)
+        if reset: # pragma: no cover
+            self.rc = rc
+        if copy:
+            rc = scu.dcp(rc)
+        return rc
+
+
+    def with_style(self, style=None, use=False, **kwargs):
+        '''
+        Combine all Matplotlib style information, and either apply it directly
+        or create a style context.
+
+        To set globally, use :meth:`sc.options.use_style() <ScirisOptions.use_style>`. Otherwise, use :meth:`sc.options.with_style() <ScirisOptions.with_style>`
+        as part of a ``with`` block to set the style just for that block (using
+        this function outsde of a with block and with ``use=False`` has no effect, so
+        don't do that!).
         
+        Note: you can also just use :func:`pl.style.context() <matplotlib.style.context>`.
+
         Args:
-            data (dataframe/array): the dataframe/data to use as the basis of the new dataframe
-            args (list): additional dataframes (or object that can be converted to dataframes) to concatenate
-            dfargs (dict): arguments passed to construct each dataframe
-            kwargs (dict): passed to ``sc.dataframe.concat()``
-        
-        **Example**::
-            
-            arr1 = np.random.rand(6,3)
-            df2 = pd.DataFrame(np.random.rand(4,3))
-            df3 = sc.dataframe.cat(arr1, df2)
-        
-        New in version 2.0.2.
-        '''
-        dfargs = scu.mergedicts(dfargs)
-        df = dataframe(data, **dfargs)
-        if len(args):
-            df = df.concat(*args, dfargs=dfargs, **kwargs)
-        return df
-            
-
-    @property
-    def ncols(self):
-        ''' Get the number of columns in the dataframe '''
-        return len(self.columns)
-
-
-    @property
-    def nrows(self):
-        ''' Get the number of rows in the dataframe '''
-        return len(self)
-
-
-    def addcol(self, key=None, value=None):
-        ''' Add a new column to the data frame -- for consistency only '''
-        self.__setitem__(key, value)
-
-
-    def rmcol(self, key, die=True):
-        ''' Remove a column or columns from the data frame '''
-        cols = scu.tolist(key)
-        for col in cols:
-            if col not in self.cols: # pragma: no cover
-                errormsg = 'sc.dataframe(): cannot remove column %s: columns are:\n%s' % (col, '\n'.join(self.cols))
-                if die: raise Exception(errormsg)
-                else:   print(errormsg)
-            else:
-                self.pop(col)
-        return self
+            style_args (dict): a dictionary of style arguments
+            use (bool): whether to set as the global style; else, treat as context for use with "with" (default)
+            kwargs (dict): additional style arguments
+
+        Valid style arguments are:
+
+            - ``dpi``:       the figure DPI
+            - ``font``:      font (typeface)
+            - ``fontsize``:  font size
+            - ``grid``:      whether or not to plot gridlines
+            - ``facecolor``: color of the axes behind the plot
+            - any of the entries in :class:`pl.rcParams <matplotlib.RcParams>`
 
+        **Examples**::
 
-    def _rowindex(self, value=None, col=None, die=False):
-        ''' Get the sanitized row index for a given value and column '''
-        col = self._sanitizecol(col)
-        coldata = self.iloc[:,col].values # Get data for this column
-        if value is None: value = coldata[-1] # If not supplied, pick the last element
-        try:
-            index = coldata.tolist().index(value) # Try to find duplicates
-        except: # pragma: no cover
-            if die:
-                errormsg = f'Item {value} not found; choices are: {coldata}'
-                raise IndexError(errormsg)
-            else:
-                return
-        return index
+            with sc.options.with_style(dpi=300): # Use default options, but higher DPI
+                pl.plot([1,3,6])
+        '''
 
+        # Handle inputs
+        rc = scu.dcp(self.rc) # Make a local copy of the currently used settings
+        if isinstance(style, dict): # pragma: no cover
+            style_args = style
+            style = None
+        else:
+            kwargs['style'] = style # Store here to be used just below
+            style_args = None
+        kwargs = scu.mergedicts(style_args, kwargs)
+
+        # Handle style, overwiting existing
+        style = kwargs.pop('style', self.style)
+        rc = self._handle_style(style, reset=False)
+
+        def pop_keywords(sourcekeys, rckey):
+            ''' Helper function to handle input arguments '''
+            sourcekeys = scu.tolist(sourcekeys)
+            key = sourcekeys[0] # Main key
+            value = None
+            changed = self.changed(key)
+            if changed:
+                value = self[key]
+            for k in sourcekeys:
+                kwvalue = kwargs.pop(k, None)
+                if kwvalue is not None:
+                    value = kwvalue
+            if value is not None:
+                rc[rckey] = value
+            return
+
+        # Handle special cases
+        pop_keywords('dpi', rckey='figure.dpi')
+        pop_keywords(['font', 'fontfamily', 'font_family'], rckey='font.family')
+        pop_keywords(['fontsize', 'font_size'], rckey='font.size')
+        pop_keywords('grid', rckey='axes.grid')
+        pop_keywords('facecolor', rckey='axes.facecolor')
+
+        # Handle other keywords
+        for key,value in kwargs.items():
+            if key not in pl.rcParams:
+                errormsg = f'Key "{key}" does not match any value in Sciris options or pl.rcParams'
+                raise KeyError(errormsg)
+            elif value is not None:
+                rc[key] = value
+
+        # Tidy up
+        if use:
+            return pl.style.use(scu.dcp(rc))
+        else:
+            return pl.style.context(scu.dcp(rc))
 
-    def rmrow(self, value=None, col=None, returnval=False, die=True):
-        ''' Like pop, but removes by matching the value in the given column instead of the index '''
-        index = self._rowindex(value=value, col=col, die=die)
-        if index is not None: self.poprow(index, returnval=returnval)
-        return self
 
+    def use_style(self, **kwargs):
+        '''
+        Shortcut to set Sciris's current style as the global default.
 
-    def _diffinds(self, inds=None):
-        ''' For a given set of indices, get the inverse, in set-speak '''
-        if inds is None: inds = []
-        ind_set = set(np.array(inds))
-        all_set = set(np.arange(self.nrows))
-        diff_set = np.array(list(all_set - ind_set))
-        return diff_set
-
-
-    def rmrows(self, inds=None, reset_index=True, inplace=True):
-        ''' Remove rows by index '''
-        keep_set = self._diffinds(inds)
-        keep_data = self.iloc[keep_set,:]
-        newdf = dataframe(data=keep_data, cols=self.cols)
-        return self.replacedata(newdf=newdf, reset_index=reset_index, inplace=inplace)
-
-
-    def replacecol(self, col=None, old=None, new=None):
-        ''' Replace all of one value in a column with a new value '''
-        col = self._sanitizecol(col)
-        coldata = self.iloc[:,col] # Get data for this column
-        inds = scm.findinds(arr=coldata, val=old)
-        self.iloc[inds,col] = new
-        return self
+        **Example**::
 
+            sc.options.use_style() # Set Sciris options as default
+            pl.figure()
+            pl.plot([1,3,7])
 
-    def to_odict(self, row=None):
+            pl.style.use('seaborn-whitegrid') # to something else
+            pl.figure()
+            pl.plot([3,1,4])
         '''
-        Convert dataframe to a dict of columns, optionally specifying certain rows.
+        return self.with_style(use=True, **kwargs)
 
-        Args:
-            row (int/list): the rows to include
-        '''
-        if row is None:
-            row = slice(None)
-        data = self.iloc[row,:].values
-        datadict = {col:data[:,c] for c,col in enumerate(self.cols)}
-        output = sco.odict(datadict)
-        return output
 
+# Create the options on module load
+options = ScirisOptions()
 
-    def findrow(self, value=None, col=None, default=None, closest=False, die=False, asdict=False):
-        '''
-        Return a row by searching for a matching value.
 
-        Args:
-            value: the value to look for
-            col: the column to look for this value in
-            default: the value to return if key is not found (overrides die)
-            closest: whether or not to return the closest row (overrides default and die)
-            die: whether to raise an exception if the value is not found
-            asdict: whether to return results as dict rather than list
+#%% Module help
 
-        **Example**::
+def help(pattern=None, source=False, ignorecase=True, flags=None, context=False, output=False, debug=False):
+    '''
+    Get help on Sciris in general, or search for a word/expression.
 
-            df = dataframe(cols=['year','val'],data=[[2016,0.3],[2017,0.5]])
-            df.findrow(2016) # returns array([2016, 0.3], dtype=object)
-            df.findrow(2013) # returns None, or exception if die is True
-            df.findrow(2013, closest=True) # returns array([2016, 0.3], dtype=object)
-            df.findrow(2016, asdict=True) # returns {'year':2016, 'val':0.3}
-        '''
-        if not closest: # Usual case, get
-            index = self._rowindex(value=value, col=col, die=(die and default is None))
-        else:
-            col = self._sanitizecol(col)
-            coldata = self.iloc[:,col] # Get data for this column
-            index = np.argmin(abs(coldata-value)) # Find the closest match to the key
-        if index is not None:
-            thisrow = self.iloc[index,:].values
-            if asdict:
-                thisrow = self.to_odict(thisrow)
-        else:
-            thisrow = default # If not found, return as default
-        return thisrow
+    Args:
+        pattern    (str):  the word, phrase, or regex to search for
+        source     (bool): whether to search source code instead of docstrings for matches
+        ignorecase (bool): whether to ignore case (equivalent to ``flags=re.I``)
+        flags      (list): additional flags to pass to :func:`re.findall()`
+        context    (bool): whether to show the line(s) of matches
+        output     (bool): whether to return the dictionary of matches
 
+    **Examples**::
 
-    def findinds(self, value=None, col=None):
-        ''' Return the indices of all rows matching the given key in a given column. '''
-        col = self._sanitizecol(col)
-        coldata = self.iloc[:,col].values # Get data for this column
-        inds = scm.findinds(arr=coldata, val=value)
-        return inds
-
-
-    def _filterrows(self, inds=None, value=None, col=None, keep=True, verbose=False, reset_index=True, inplace=False):
-        ''' Filter rows and either keep the ones matching, or discard them '''
-        if inds is None:
-            inds = self.findinds(value=value, col=col)
-        if keep: inds = self._diffinds(inds)
-        if verbose: print(f'Dataframe filtering: {len(inds)} rows removed based on key="{inds}", column="{col}"')
-        output = self.rmrows(inds=inds, reset_index=reset_index, inplace=inplace)
-        return output
+        sc.help()
+        sc.help('smooth')
+        sc.help('JSON', ignorecase=False, context=True)
+        sc.help('pickle', source=True, context=True)
 
+    | *New in version 1.3.0.*
+    | *New in version 1.3.1:* "source" argument
+    '''
+    defaultmsg = '''
+For general help using Sciris, the best place to start is the docs:
 
-    def filterin(self, inds=None, value=None, col=None, verbose=False, reset_index=True, inplace=False):
-        '''Keep only rows matching a criterion '''
-        return self._filterrows(inds=inds, value=value, col=col, keep=True, verbose=verbose, reset_index=reset_index, inplace=inplace)
-
-
-    def filterout(self, inds=None, value=None, col=None, verbose=False, reset_index=True, inplace=False):
-        '''Remove rows matching a criterion (in place) '''
-        return self._filterrows(inds=inds, value=value, col=col, keep=False, verbose=verbose, reset_index=reset_index, inplace=inplace)
-
-
-    def filtercols(self, cols=None, die=True, reset_index=True, inplace=False):
-        ''' Filter columns keeping only those specified -- note, by default, do not perform in place '''
-        if cols is None: cols = scu.dcp(self.cols) # By default, do nothing
-        cols = scu.tolist(cols)
-        order = []
-        notfound = []
-        for col in cols:
-            if col in self.cols:
-                order.append(self.cols.index(col))
-            else:
-                cols.remove(col)
-                notfound.append(col)
-        if len(notfound): # pragma: no cover
-            errormsg = 'sc.dataframe(): could not find the following column(s): %s\nChoices are: %s' % (notfound, self.cols)
-            if die: raise Exception(errormsg)
-            else:   print(errormsg)
-        ordered_data = self.iloc[:,order] # Resort and filter the data
-        newdf = dataframe(cols=cols, data=ordered_data)
-        return self.replacedata(newdf=newdf, reset_index=reset_index, inplace=inplace)
-
-
-    def sortrows(self, col=None, reverse=False, returninds=False):
-        ''' Sort the dataframe rows in place by the specified column(s)'''
-        if col is None:
-            col = 0 # Sort by first column by default
-        cols = scu.tolist(col)[::-1] # Ensure it's a list and reverse order
-        sortorder = [] # In case there are no columns
-        for col in cols:
-            col = self._sanitizecol(col)
-            sortorder = np.argsort(self.iloc[:,col], kind='mergesort') # To preserve order
-            if reverse:
-                sortorder = sortorder[::-1]
-            self.iloc[:,:] = self.iloc[sortorder,:]
-        if returninds:
-            return sortorder
-        else:
-            return self
+    http://docs.sciris.org
 
+To search for a keyword/phrase/regex in Sciris' docstrings, use e.g.:
 
-    def sortcols(self, sortorder=None, reverse=False, returninds=False):
-        ''' Like sortrows(), but change column order (in place) instead '''
-        if sortorder is None:
-            sortorder = np.argsort(self.cols, kind='mergesort')
-            if reverse:
-                sortorder = sortorder[::-1]
-        newcols = list(np.array(self.cols)[sortorder])
-        self.rename(columns={old:new for old,new in zip(self.cols, newcols)}, inplace=True)
-        self.iloc[:,:] = self.iloc[:,sortorder]
-        if returninds:
-            return sortorder
-        else:
-            return self
+    >>> sc.help('smooth')
 
+See help(sc.help) for more information.
+'''
+    # No pattern is provided, print out default help message
+    if pattern is None:
+        print(defaultmsg)
 
-    @staticmethod
-    def from_dict(*args, **kwargs):
-        return dataframe(super().from_dict(*args, **kwargs))
+    else:
 
-    @staticmethod
-    def from_records(*args, **kwargs):
-        return dataframe(super().from_records(*args, **kwargs))
+        import sciris as sc # Here to avoid circular import
 
-    def to_pandas(self, **kwargs):
-        ''' Convert to a plain pandas dataframe '''
-        return pd.DataFrame(data=self.values, columns=self.cols, **kwargs)
+        # Handle inputs
+        flags = sc.tolist(flags)
+        if ignorecase:
+            flags.append(re.I)
+
+        def func_ok(f):
+            ''' Skip certain functions '''
+            excludes = [
+                f.startswith('_'),
+                f.startswith('sc_'),
+                f in ['help', 'options', 'extras'],
+            ]
+            ok = not(any(excludes))
+            return ok
+
+        # Get available functions/classes
+        funcs = [f for f in dir(sc) if func_ok(f)] # Skip dunder methods and modules
+
+        # Get docstrings or full source code
+        docstrings = dict()
+        for funcname in funcs:
+            try:
+                f = getattr(sc, funcname)
+                if source: string = inspect.getsource(f)
+                else:      string = f.__doc__
+                docstrings[funcname] = string
+            except OSError as E: # Happens for built-ins, e.g. defaultdict
+                if debug:
+                    errormsg = f'sc.help(): Encountered an error on {funcname}: {E}'
+                    print(errormsg)
+                    
+
+        # Find matches
+        matches = co.defaultdict(list)
+        linenos = co.defaultdict(list)
+
+        for k,docstring in docstrings.items():
+            if docstring:
+                for l,line in enumerate(docstring.splitlines()):
+                    if re.findall(pattern, line, *flags):
+                        linenos[k].append(str(l))
+                        matches[k].append(line)
+            elif debug:
+                errormsg = f'sc.help(): No docstring for {k}'
+                print(errormsg)
+
+        # Assemble output
+        if not len(matches): # pragma: no cover
+            string = f'No matches for "{pattern}" found among {len(docstrings)} available functions.'
+        else:
+            string = f'Found {len(matches)} matches for "{pattern}" among {len(docstrings)} available functions:\n'
+            maxkeylen = 0
+            for k in matches.keys(): maxkeylen = max(len(k), maxkeylen)
+            for k,match in matches.items():
+                if not context:
+                    keystr = f'  {k:>{maxkeylen}s}'
+                else:
+                    keystr = k
+                matchstr = f'{keystr}: {len(match)} matches'
+                if context:
+                    matchstr = sc.heading(matchstr, output=True)
+                else:
+                    matchstr += '\n'
+                string += matchstr
+                if context:
+                    lineno = linenos[k]
+                    maxlnolen = max([len(l) for l in lineno])
+                    for l,m in zip(lineno, match):
+                        string += sc.colorize(string=f'  {l:>{maxlnolen}s}: ', fg='cyan', output=True)
+                        string += f'{m}\n'
+                    string += '—'*60 + '\n'
+
+        # Print result and return
+        print(string)
+        if output:
+            return string
+        else:
+            return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sciris-2.1.0/sciris/sc_datetime.py` & `sciris-3.0.0/sciris/sc_datetime.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Time/date utilities.
 
 Highlights:
-    - :func:`tic` / :func:`toc` / :func:`timer`: simple methods for timing durations
-    - :func:`readdate`: convert strings to dates using common formats
-    - :func:`daterange`: create a list of dates
-    - :func:`datedelta`: perform calculations on date strings
+    - :func:`:func:`sc.tic() <tic>` / :func:`sc.toc() <toc>` / :class:`sc.timer() <timer>`: simple methods for timing durations
+    - :func:`sc.readdate() <readdate>`: convert strings to dates using common formats
+    - :func:`sc.daterange() <daterange>`: create a list of dates
+    - :func:`sc.datedelta() <datedelta>`: perform calculations on date strings
 '''
 
-import time
+import time as pytime
 import warnings
 import numpy as np
 import pandas as pd
 import pylab as pl
 import datetime as dt
 import dateutil as du
 from . import sc_utils as scu
@@ -20,59 +20,71 @@
 from . import sc_printing as scp
 
 
 ###############################################################################
 #%% Date functions
 ###############################################################################
 
-__all__ = ['now', 'getdate', 'readdate', 'date', 'day', 'daydiff', 'daterange', 'datedelta', 'datetoyear']
+__all__ = ['time', 'now', 'getdate', 'readdate', 'date', 'day', 'daydiff', 'daterange', 'datedelta', 'datetoyear']
 
 
+def time():
+    '''
+    Get current time in seconds -- alias to time.time()
+    
+    See also :func:`sc.now() <now>` to return a datetime object, and :func:`sc.getdate() <getdate>` to
+    return a string.
+    
+    *New in version 3.0.0.*
+    '''
+    return pytime.time()
+    
+
 def now(astype='dateobj', timezone=None, utc=False, tostring=False, dateformat=None):
     '''
     Get the current time as a datetime object, optionally in UTC time.
 
-    ``sc.now()`` is similar to ``sc.getdate()``, but ``sc.now()`` returns a datetime
-    object by default, while ``sc.getdate()`` returns a string by default.
+    :func:`sc.now() <now>` is similar to :func:`sc.getdate() <getdate>`, but :func:`sc.now() <now>` returns a datetime
+    object by default, while :func:`sc.getdate() <getdate>` returns a string by default.
 
     Args:
-        astype     (str)  : what to return; choices are "dateobj", "str", "float"; see ``sc.getdate()`` for more
+        astype     (str)  : what to return; choices are "dateobj", "str", "float"; see :func:`sc.getdate() <getdate>` for more
         timezone   (str)  : the timezone to set the itme to
         utc        (bool) : whether the time is specified in UTC time
         dateformat (str)  : if ``astype`` is ``'str'``, use this output format
 
     **Examples**::
 
         sc.now() # Return current local time, e.g. 2019-03-14 15:09:26
         sc.now(timezone='US/Pacific') # Return the time now in a specific timezone
         sc.now(utc=True) # Return the time in UTC
         sc.now(astype='str') # Return the current time as a string instead of a date object; use 'int' for seconds
         sc.now(tostring=True) # Backwards-compatible alias for astype='str'
         sc.now(dateformat='%Y-%b-%d') # Return a different date format
 
-    New in version 1.3.0: made "astype" the first argument; removed "tostring" argument
+    *New in version 1.3.0:* made "astype" the first argument; removed "tostring" argument
     '''
     if isinstance(utc, str): timezone = utc # Assume it's a timezone
     if timezone is not None: tzinfo = du.tz.gettz(timezone) # Timezone is a string
     elif utc:                tzinfo = du.tz.tzutc() # UTC has been specified
     else:                    tzinfo = None # Otherwise, do nothing
-    if tostring:
-        warnmsg = 'sc.now() argument "tostring" will be deprecated soon'
+    if tostring: # pragma: no cover
+        warnmsg = 'sc.now() argument "tostring" is deprecated; use astype="str" instead'
         warnings.warn(warnmsg, category=FutureWarning, stacklevel=2)
         astype='str'
     timenow = dt.datetime.now(tzinfo)
     output = getdate(timenow, astype=astype, dateformat=dateformat)
     return output
 
 
 def getdate(obj=None, astype='str', dateformat=None):
         '''
         Alias for converting a date object to a formatted string.
 
-        See also ``sc.now()``.
+        See also :func:`sc.now() <now>`.
 
         Args:
             obj (datetime): the datetime object to convert
             astype (str): what to return; choices are "str" (default), "dateobj", "float" (full timestamp), "int" (timestamp to second precision)
             dateformat (str): if ``astype`` is ``'str'``, use this output format
 
         **Examples**::
@@ -85,27 +97,27 @@
 
         if dateformat is None:
             dateformat = '%Y-%b-%d %H:%M:%S'
         else:
             astype = 'str' # If dateformat is specified, assume type is a string
 
         try:
-            if scu.isstring(obj):
+            if scu.isstring(obj): # pragma: no cover
                 return obj # Return directly if it's a string
             obj.timetuple() # Try something that will only work if it's a date object
             dateobj = obj # Test passed: it's a date object
         except Exception as E: # pragma: no cover # It's not a date object
             errormsg = f'Getting date failed; date must be a string or a date object: {repr(E)}'
             raise TypeError(errormsg)
 
         timestamp = obj.timestamp()
         if   astype == 'str':     output = dateobj.strftime(dateformat)
         elif astype == 'int':     output = int(timestamp)
         elif astype == 'dateobj': output = dateobj
-        elif astype in  ['float', 'number', 'timestamp']:
+        elif astype in  ['float', 'number', 'timestamp']: # pragma: no cover
             output = timestamp
         else: # pragma: no cover
             errormsg = f'"astype={astype}" not understood; must be "str" or "int"'
             raise ValueError(errormsg)
         return output
 
 
@@ -198,15 +210,15 @@
     # Actually process the dates
     dateobjs = []
     for datestr in datestrs: # Iterate over them
         dateobj = None
         exceptions = {}
         if isinstance(datestr, dt.datetime):
             dateobj = datestr # Nothing to do
-        elif scu.isnumber(datestr):
+        elif scu.isnumber(datestr): # pragma: no cover
             if 'posix' in format_list or None in format_list:
                 dateobj = dt.datetime.fromtimestamp(datestr)
             elif 'ordinal' in format_list or 'matplotlib' in format_list:
                 dateobj = pl.num2date(datestr)
             else:
                 errormsg = f'Could not convert numeric date {datestr} using available formats {scu.strjoin(format_list)}; must be "posix" or "ordinal"'
                 raise ValueError(errormsg)
@@ -218,86 +230,92 @@
                 except Exception as E:
                     exceptions[key] = str(E)
             if dateobj is None:
                 formatstr = scu.newlinejoin([f'{item[1]}' for item in formats_to_try.items()])
                 errormsg = f'Was unable to convert "{datestr}" to a date using the formats:\n{formatstr}'
                 if dateformat not in ['dmy', 'mdy']:
                     errormsg += '\n\nNote: to read day-month-year or month-day-year dates, use dateformat="dmy" or "mdy" respectively.'
-                    if verbose:
+                    if verbose: # pragma: no cover
                         for key,val in exceptions.items():
                             errormsg += f'\n {key}: {val}'
                 raise ValueError(errormsg)
         dateobjs.append(dateobj)
 
     # If only a single date was supplied, return just that; else return the list/array
     output = scu._sanitize_output(dateobjs, is_list, is_array, dtype=object)
     return output
 
 
-def date(obj, *args, start_date=None, readformat=None, outformat=None, as_date=True, **kwargs):
+def date(obj=None, *args, start_date=None, readformat=None, to='date', as_date=None, outformat=None, **kwargs):
     '''
     Convert any reasonable object -- a string, integer, or datetime object, or
-    list/array of any of those -- to a date object. To convert an integer to a
-    date, you must supply a start date.
+    list/array of any of those -- to a date object (or string, pandas, or numpy
+    date). To convert an integer to a date, you must supply a start date.
 
-    Caution: while this function and ``sc.readdate()`` are similar, and indeed this function
-    calls ``sc.readdate()`` if the input is a string, in this function an integer is treated
-    as a number of days from start_date, while for ``sc.readdate()`` it is treated as a
+    Caution: while this function and :func:`sc.readdate() <readdate>` are similar, and indeed this function
+    calls :func:`sc.readdate() <readdate>` if the input is a string, in this function an integer is treated
+    as a number of days from start_date, while for :func:`sc.readdate() <readdate>` it is treated as a
     timestamp in seconds.
 
     Note: in this and other date functions, arguments work either with or without
     underscores (e.g. ``start_date`` or ``startdate``)
 
     Args:
-        obj (str/int/date/datetime/list/array): the object to convert
+        obj (str/int/date/datetime/list/array): the object to convert; if None, return current date
         args (str/int/date/datetime): additional objects to convert
         start_date (str/date/datetime): the starting date, if an integer is supplied
-        readformat (str/list): the format to read the date in; passed to ``sc.readdate()``
+        readformat (str/list): the format to read the date in; passed to :func:`sc.readdate() <readdate>` (NB: can also use "format" instead of "readformat")
+        to (str): the output format: 'date' (default), 'str' (or 'string'), 'pandas', or 'numpy'
+        as_date (bool): alternate method of choosing between  output format of 'date' (True) or 'str' (False); if None, use "to" instead
         outformat (str): the format to output the date in, if returning a string
-        as_date (bool): whether to return as a datetime date instead of a string
+        kwargs (dict): only used for deprecated argument aliases
 
     Returns:
         dates (date or list): either a single date object, or a list of them (matching input data type where possible)
 
     **Examples**::
 
         sc.date('2020-04-05') # Returns datetime.date(2020, 4, 5)
-        sc.date([35,36,37], start_date='2020-01-01', as_date=False) # Returns ['2020-02-05', '2020-02-06', '2020-02-07']
+        sc.date([35,36,37], start_date='2020-01-01', to='str') # Returns ['2020-02-05', '2020-02-06', '2020-02-07']
         sc.date(1923288822, readformat='posix') # Interpret as a POSIX timestamp
 
-    | New in version 1.0.0.
-    | New in version 1.2.2: "readformat" argument; renamed "dateformat" to "outformat"
-    | New in version 2.0.0: support for ``np.datetime64`` objects
+    | *New in version 1.0.0.*
+    | *New in version 1.2.2:* "readformat" argument; renamed "dateformat" to "outformat"
+    | *New in version 2.0.0:* support for :obj:`np.datetime64 <numpy.datetime64>` objects
+    | *New in version 3.0.0:* added "to" argument, and support for :obj:`pd.Timestamp <pandas.Timestamp>` and :obj:`np.datetime64 <numpy.datetime64>` output; allow None
     '''
 
     # Handle deprecation
     start_date = kwargs.pop('startdate', start_date) # Handle with or without underscore
     as_date    = kwargs.pop('asdate', as_date) # Handle with or without underscore
+    readformat = kwargs.pop('format', readformat) # Handle either name
     dateformat = kwargs.pop('dateformat', None)
     if dateformat is not None: # pragma: no cover
         outformat = dateformat
         warnmsg = 'sc.date() argument "dateformat" has been deprecated as of v1.2.2; use "outformat" instead'
         warnings.warn(warnmsg, category=FutureWarning, stacklevel=2)
+    if as_date is not None: # pragma: no cover
+        to = 'date' if as_date else 'str' # Legacy support for as_date boolean
 
     # Convert to list and handle other inputs
     if obj is None:
-        return
+        obj = dt.datetime.now().date()
     if outformat is None:
         outformat = '%Y-%m-%d'
     obj, is_list, is_array = scu._sanitize_iterables(obj, *args)
 
     dates = []
     for d in obj:
-        if d is None:
+        if d is None: # pragma: no cover
             dates.append(d)
             continue
         try:
             if type(d) == dt.date: # Do not use isinstance, since must be the exact type
                 pass
-            elif isinstance(d, dt.datetime):
+            elif isinstance(d, dt.datetime): # This includes pd.Timestamp
                 d = d.date()
             elif scu.isstring(d):
                 d = readdate(d, dateformat=readformat).date()
             elif isinstance(d, np.datetime64):
                 d = pd.Timestamp(d).date()
             elif scu.isnumber(d):
                 if readformat is not None:
@@ -306,31 +324,41 @@
                     if start_date is None:
                         errormsg = f'To convert the number {d} to a date, you must either specify "posix" or "ordinal" read format, or supply start_date'
                         raise ValueError(errormsg)
                     d = date(start_date) + dt.timedelta(days=int(d))
             else: # pragma: no cover
                 errormsg = f'Cannot interpret {type(d)} as a date, must be date, datetime, or string'
                 raise TypeError(errormsg)
-            if as_date:
-                dates.append(d)
+            
+            # Handle output
+            if to == 'date':
+                out = d
+            elif to in ['str', 'string']:
+                out = d.strftime(outformat)
+            elif to == 'pandas':
+                out = pd.Timestamp(d)
+            elif to == 'numpy':
+                out = np.datetime64(d)
             else:
-                dates.append(d.strftime(outformat))
+                errormsg = f'Could not understand to="{to}": must be "date", "str", "pandas", or "numpy"'
+                raise ValueError(errormsg)
+            dates.append(out)
         except Exception as E:
             errormsg = f'Conversion of "{d}" to a date failed'
             raise ValueError(errormsg) from E
 
-    # Return an integer rather than a list if only one provided
+    # Return a scalar rather than a list if only one provided
     output = scu._sanitize_output(dates, is_list, is_array, dtype=object)
     return output
 
 
 def day(obj, *args, start_date=None, **kwargs):
     '''
     Convert a string, date/datetime object, or int to a day (int), the number of
-    days since the start day. See also ``sc.date()`` and ``sc.daydiff()``. If a start day
+    days since the start day. See also :func:`sc.date() <date>` and :func:`sc.daydiff() <daydiff>``. If a start day
     is not supplied, it returns the number of days into the current year.
 
     Args:
         obj (str, date, int, list, array): convert any of these objects to a day relative to the start day
         args (list): additional days
         start_date (str or date): the start day; if none is supplied, return days since (supplied year)-01-01.
 
@@ -338,16 +366,16 @@
         days (int or list): the day(s) in simulation time (matching input data type where possible)
 
     **Examples**::
 
         sc.day(sc.now()) # Returns how many days into the year we are
         sc.day(['2021-01-21', '2024-04-04'], start_date='2022-02-22') # Days can be positive or negative
 
-    | New in version 1.0.0.
-    | New in version 1.2.2: renamed "start_day" to "start_date"
+    | *New in version 1.0.0.*
+    | *New in version 1.2.2:* renamed "start_day" to "start_date"
     '''
 
     # Handle deprecation
     start_date = kwargs.pop('startdate', start_date) # Handle with or without underscore
     start_day = kwargs.pop('start_day', None)
     if start_day is not None: # pragma: no cover
         start_date = start_day
@@ -385,72 +413,78 @@
     output = scu._sanitize_output(days, is_list, is_array)
     return output
 
 
 def daydiff(*args):
     '''
     Convenience function to find the difference between two or more days. With
-    only one argument, calculate days since 2020-01-01.
+    only one argument, calculate days since Jan. 1st.
 
     **Examples**::
 
         diff  = sc.daydiff('2020-03-20', '2020-04-05') # Returns 16
         diffs = sc.daydiff('2020-03-20', '2020-04-05', '2020-05-01') # Returns [16, 26]
+        
+        doy = sc.daydiff('2022-03-20') # Returns 79, the number of days since 2022-01-01
 
-    New in version 1.0.0.
+    | *New in version 1.0.0.*
+    | *New in version 3.0.0:* Calculated relative days with one argument
     '''
     days = [date(day) for day in args]
     if len(days) == 1:
-        days.insert(0, date(f'{now().year}-01-01')) # With one date, return days since Jan. 1st
+        days.insert(0, date(f'{days[0].year}-01-01')) # With one date, return days since Jan. 1st
 
     output = []
     for i in range(len(days)-1):
         diff = (days[i+1] - days[i]).days
         output.append(diff)
 
     if len(output) == 1:
         output = output[0]
 
     return output
 
 
-def daterange(start_date=None, end_date=None, interval=None, inclusive=True, as_date=False,
+def daterange(start_date=None, end_date=None, interval=None, inclusive=True, as_date=None,
               readformat=None, outformat=None, **kwargs):
     '''
     Return a list of dates from the start date to the end date. To convert a list
-    of days (as integers) to dates, use ``sc.date()`` instead.
+    of days (as integers) to dates, use :func:`sc.date() <date>` instead.
 
     Note: instead of an end date, can also pass one or more of days, months, weeks,
-    or years, which will be added on to the start date via ``sc.datedelta()``.
+    or years, which will be added on to the start date via :func:`sc.datedelta() <datedelta>`.
 
     Args:
         start_date (int/str/date) : the starting date, in any format
-        end_date   (int/str/date) : the end date, in any format
+        end_date   (int/str/date) : the end date, in any format (see also kwargs below)
         interval   (int/str/dict) : if an int, the number of days; if 'week', 'month', or 'year', one of those; if a dict, passed to ``dt.relativedelta()``
         inclusive  (bool)         : if True (default), return to end_date inclusive; otherwise, stop the day before
-        as_date    (bool)         : if True, return a list of datetime.date objects instead of strings (note: you can also use "asdate" instead of "as_date")
-        readformat (str)          : passed to date()
-        outformat  (str)          : passed to date()
-        days       (int)          : optional
+        as_date    (bool)         : if True, return a list of ``datetime.date`` objects; else, as input type (e.g. strings; note: you can also use "asdate" instead of "as_date")
+        readformat (str)          : passed to :func:`sc.date() <date>`
+        outformat  (str)          : passed to :func:`sc.date() <date>`
+        kwargs     (dict)         : optionally, use any valid argument to :func:`sc.datedelta() <datedelta>` to create the end_date
 
     **Examples**::
 
         dates1 = sc.daterange('2020-03-01', '2020-04-04')
         dates2 = sc.daterange('2020-03-01', '2022-05-01', interval=dict(months=2), asdate=True)
         dates3 = sc.daterange('2020-03-01', weeks=5)
 
-    | New in version 1.0.0.
-    | New in version 1.3.0: "interval" argument
-    | New in version 2.0.0: ``sc.datedelta()`` arguments
+    | *New in version 1.0.0.*
+    | *New in version 1.3.0:* "interval" argument
+    | *New in version 2.0.0:* :func:`sc.datedelta() <datedelta>` arguments
+    | *New in version 3.0.0:* preserve input type
     '''
 
     # Handle inputs
     start_date = kwargs.pop('startdate', start_date) # Handle with or without underscore
     end_date   = kwargs.pop('enddate',   end_date) # Handle with or without underscore
     as_date    = kwargs.pop('asdate', as_date) # Handle with or without underscore
+    if as_date is None: # Typical case, return the same format as the input
+        as_date = False if isinstance(start_date, str) else True
     if len(kwargs):
         end_date = datedelta(start_date, **kwargs)
     start_date = date(start_date, readformat=readformat)
     end_date = date(end_date, readformat=readformat)
 
     if   interval in [None, 'day']: interval = dict(days=1)
     elif interval == 'week':        interval = dict(weeks=1)
@@ -462,57 +496,65 @@
     # Calculate dates
     dates = []
     curr_date = start_date
     delta = datedelta(**interval)
     while curr_date < end_date:
         dates.append(curr_date)
         curr_date += delta
-
+    
     # Convert to final format
     dates = date(dates, start_date=start_date, as_date=as_date, outformat=outformat)
     return dates
 
 
 def datedelta(datestr=None, days=0, months=0, years=0, weeks=0, dt1=None, dt2=None, as_date=None, **kwargs):
     '''
     Perform calculations on a date string (or date object), returning a string (or a date).
     Wrapper to ``dateutil.relativedelta.relativedelta()``.
 
     If ``datestr`` is ``None``, then return the delta object rather than the new date.
 
     Args:
-        datestr (None/str/date): the starting date (typically a string); if None, return the relative delta
+        datestr (None/str/date/list): the starting date (typically a string); if None, return the relative delta
         days (int): the number of days (positive or negative) to increment
         months (int): as above
         years (int): as above
         weeks (int): as above
         dt1, dt2 (dates): if both provided, compute the difference between them
         as_date (bool): if True, return a date object; otherwise, return as input type
-        kwargs (dict): passed to ``sc.readdate()``
+        kwargs (dict): passed to :func:`sc.readdate() <readdate>`
 
     **Examples**::
 
         sc.datedelta('2021-07-07', 3) # Add 3 days
         sc.datedelta('2021-07-07', days=-4) # Subtract 4 days
         sc.datedelta('2021-07-07', weeks=4, months=-1, as_date=True) # Add 4 weeks but subtract a month, and return a dateobj
         sc.datedelta(days=3) # Alias to du.relativedelta.relativedelta(days=3)
+    
+    *New in version 3.0.0:* operate on list of dates
     '''
     as_date = kwargs.pop('asdate', as_date) # Handle with or without underscore
 
     # Calculate the time delta, and return immediately if no date is provided
     delta = du.relativedelta.relativedelta(days=days, months=months, years=years, weeks=weeks, dt1=dt1, dt2=dt2)
     if datestr is None:
         return delta
     else:
-        if as_date is None: # Typical case, return the same format as the input
-            as_date = False if isinstance(datestr, str) else True
-        dateobj = readdate(datestr, **kwargs)
-        newdate = dateobj + delta
-        newdate = date(newdate, as_date=as_date)
-        return newdate
+        datelist = scu.tolist(datestr)
+        newdates = []
+        for datestr in datelist:
+            if as_date is None: # Typical case, return the same format as the input
+                as_date = False if isinstance(datestr, str) else True
+            dateobj = readdate(datestr, **kwargs)
+            newdate = dateobj + delta
+            newdate = date(newdate, as_date=as_date)
+            newdates.append(newdate)
+        if not isinstance(datestr, list) and len(newdates) == 1: # Convert back to string/date
+            newdates = newdates[0]
+        return newdates
 
 
 def datetoyear(dateobj, dateformat=None):
     """
     Convert a DateTime instance to decimal year.
 
     Args:
@@ -524,15 +566,15 @@
 
     **Example**::
 
         sc.datetoyear('2010-07-01') # Returns approximately 2010.5
 
     By Luke Davis from https://stackoverflow.com/a/42424261, adapted by Romesh Abeysuriya.
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     """
     if scu.isstring(dateobj):
         dateobj = readdate(dateobj, dateformat=dateformat)
     year_part = dateobj - dt.datetime(year=dateobj.year, month=1, day=1)
     year_length = dt.datetime(year=dateobj.year + 1, month=1, day=1) - dt.datetime(year=dateobj.year, month=1, day=1)
     output = dateobj.year + year_part / year_length
     return output
@@ -543,154 +585,222 @@
 ###############################################################################
 
 __all__+= ['tic', 'toc', 'toctic', 'timer', 'Timer']
 
 
 def tic():
     '''
-    With ``sc.toc()``, a little pair of functions to calculate a time difference:
+    With :func:`sc.toc() <toc>`, a little pair of functions to calculate a time difference:
 
     **Examples**::
 
         sc.tic()
         slow_func()
         sc.toc()
 
         T = sc.tic()
         slow_func2()
         sc.toc(T, label='slow_func2')
 
-    See also ``sc.timer()``.
+    See also :class:`sc.timer() <timer>`.
     '''
     global _tictime  # The saved time is stored in this global
-    _tictime = time.time()  # Store the present time in the global
+    _tictime = pytime.time()  # Store the present time in the global
     return _tictime    # Return the same stored number
 
 
+def _convert_time_unit(unit, elapsed=None):
+    ''' Convert between different units of time; not for the user '''
+    
+    # Shortcut for speed
+    if unit == 's':
+        return 1, 's'
+
+    # Standard use case
+    else:
+    
+        # Define the mapping -- in order of expected usage frequency for speed
+        mapping = {
+            's'  : dict(factor=   1, aliases=[None, 'default', 's', 'sec', 'secs', 'second', 'seconds']),
+            'ms' : dict(factor=1e-3, aliases=['ms', 'milisecond', 'miliseconds']),
+            'μs' : dict(factor=1e-6, aliases=['us', 'μs', 'microsecond', 'microseconds']),
+            'ns' : dict(factor=1e-9, aliases=['ns', 'nanosecond', 'nanoseconds']),
+            'min': dict(factor=  60, aliases=['m', 'min', 'mins', 'minute', 'minutes']),
+            'hr' : dict(factor=3600, aliases=['h', 'hr', 'hrs', 'hour', 'hours']),
+        }
+        
+        # Handle 'auto'
+        if unit == 'auto':
+            if elapsed is None:  unit = 's'
+            elif elapsed < 1e-7: unit = 'ns'
+            elif elapsed < 1e-4: unit = 'μs'
+            elif elapsed < 1e-1: unit = 'ms'
+            else:                unit = 's'
+    
+        # Perform the mapping
+        factor = None
+        for label,entry in mapping.items():
+            if unit in [label, entry['factor']] + entry['aliases']:
+                factor = entry['factor']
+                break
+        if factor is None:
+            errormsg = f'Could not understand "{unit}"; all possible values are:\n{mapping}'
+            raise ValueError(errormsg)
+    
+    return factor, label
+
 
-def toc(start=None, label=None, baselabel=None, sigfigs=None, reset=False, output=False, doprint=None, elapsed=None):
+def toc(start=None, label=None, baselabel=None, sigfigs=None, reset=False, unit='s',
+        output=False, doprint=None, elapsed=None):
     '''
-    With ``sc.tic()``, a little pair of functions to calculate a time difference. See
-    also ``sc.timer()``.
+    With :func:`sc.tic() <tic>`, a little pair of functions to calculate a time difference. See
+    also :class:`sc.timer() <timer>`.
+    
+    By default, output is displayed in seconds. You can change this with the ``unit``
+    argument, which can be a string or a float:
+        
+        - 'hr' or 3600
+        - 'min' or 60
+        - 's' or 1 (default)
+        - 'ms' or 1e-3
+        - 'us' or 1e-6
+        - 'ns' or 1e-9
+        - 'auto' to choose an appropriate unit
 
     Args:
-        start     (float): the starting time, as returned by e.g. ``sc.tic()``
-        label     (str): optional label to add
-        baselabel (str): optional base label; default is "Elapsed time: "
-        sigfigs   (int): number of significant figures for time estimate
-        reset     (bool): reset the time; like calling ``sc.toctic()`` or ``sc.tic()`` again
+        start    (float): the starting time, as returned by e.g. :func:`sc.tic() <tic>`
+        label      (str): optional label to add
+        baselabel  (str): optional base label; default is "Elapsed time: "
+        sigfigs    (int): number of significant figures for time estimate
+        reset     (bool): reset the time; like calling :func:`sc.toctic() <toctic>` or :func:`sc.tic() <tic>` again
+        unit (str/float): the unit of time to display; see options above
         output    (bool): whether to return the output (otherwise print); if output='message', then return the message string; if output='both', then return both
         doprint   (bool): whether to print (true by default)
-        elapsed   (float): use a pre-calculated elapsed time instead of recalculating (not recommneded)
+        elapsed  (float): use a pre-calculated elapsed time instead of recalculating (not recommneded)
 
     **Examples**::
 
         sc.tic()
         slow_func()
         sc.toc()
 
         T = sc.tic()
         slow_func2()
         sc.toc(T, label='slow_func2')
 
-    New in version 1.3.0: new arguments.
+    *New in version 1.3.0:* new arguments
+    *New in version 3.0.0:* "unit" argument
     '''
-    now = time.time() # Get the time as quickly as possible
+    now = pytime.time() # Get the time as quickly as possible
 
     from . import sc_printing as scp # To avoid circular import
     global _tictime  # The saved time is stored in this global
 
     # Set defaults
     if sigfigs is None: sigfigs = 3
 
     # If no start value is passed in, try to grab the global _tictime
-    if isinstance(start, str): # Start and label are probably swapped
+    if isinstance(start, str): # Start and label are probably swapped # pragma: no cover
         start,label = label,start
     if start is None:
         try:    start = _tictime
         except: start = 0 # This doesn't exist, so just leave start at 0.
 
     # Calculate the elapsed time in seconds
     if elapsed is None:
         elapsed = now - start
 
     # Create the message giving the elapsed time
     if label is None:
         if baselabel is None:
             base = 'Elapsed time: '
-        else:
+        else: # pragma: no cover
             base = baselabel
     else:
         if baselabel is None:
             if label:
                 base = f'{label}: '
-            else: # Handles case toc(label='')
+            else: # Handles case toc(label='') # pragma: no cover
                 base = ''
         else:
             base = f'{baselabel}{label}: '
-    logmessage = f'{base}{scp.sigfig(elapsed, sigfigs=sigfigs)} s'
+    factor, unitlabel = _convert_time_unit(unit, elapsed=elapsed)
+    logmessage = f'{base}{scp.sigfig(elapsed/factor, sigfigs=sigfigs)} {unitlabel}'
 
     # Print if asked, or if no other output
     if doprint or ((doprint is None) and (not output)):
         print(logmessage)
 
     # Optionally reset the counter
     if reset:
-        _tictime = time.time()  # Store the present time in the global
+        _tictime = pytime.time()  # Store the present time in the global
 
     # Return elapsed if desired
-    if output:
+    if output: # pragma: no cover
         if output == 'message':
             return logmessage
         elif output == 'both':
             return (elapsed, logmessage)
         else:
             return elapsed
     else:
         return
 
 
 def toctic(returntic=False, returntoc=False, *args, **kwargs):
     '''
-    A convenience fu`ction for multiple timings. Can return the default output of
-    either ``sc.tic()`` or ``sc.toc()`` (default neither). Arguments are passed to ``sc.toc()``.
-    Equivalent to ``sc.toc(reset=True)``.
+    A convenience fuction for multiple timings. Can return the default output of
+    either :func:`sc.tic() <tic>` or :func:`sc.toc() <toc>` (default neither). Arguments are passed to :func:`sc.toc() <toc>`.
+    Equivalent to :func:`sc.toc(reset=True) <toc>`.
 
     **Example**::
 
         sc.tic()
         slow_operation_1()
         sc.toctic()
         slow_operation_2()
         sc.toc()
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     '''
     tocout = toc(*args, **kwargs)
     ticout = tic()
     if   returntic: return ticout
     elif returntoc: return tocout
     else:           return
 
 
 class timer:
     '''
-    Simple timer class. Note: ``sc.timer()`` and ``sc.Timer()`` are aliases.
+    Simple timer class. Note: :class:`sc.timer() <timer>` and :class:`sc.Timer() <Timer>` are aliases.
 
-    This wraps ``tic`` and ``toc`` with the formatting arguments and the start time
+    This wraps :func:`sc.tic() <tic>` and :func:`sc.toc() <toc>` with the formatting arguments and the start time
     (at construction).
 
     Use this in a ``with`` block to automatically print elapsed time when
     the block finishes.
+    
+    By default, output is displayed in seconds. You can change this with the ``unit``
+    argument, which can be a string or a float:
+        
+        - 'hr' or 3600
+        - 'min' or 60
+        - 's' or 1 (default)
+        - 'ms' or 1e-3
+        - 'us' or 1e-6
+        - 'ns' or 1e-9
+        - 'auto' to choose an appropriate unit
 
     Args:
         label (str): label identifying this timer
         auto (bool): whether to automatically increment the label
-        start (bool): whether to start timing from object creation (else, call ``timer.tic()`` explicitly)
-        kwargs (dict): passed to ``toc()`` when invoked
+        start (bool): whether to start timing from object creation (else, call :meth:`timer.tic()` explicitly)
+        unit (str/float): the unit of time to display; see options above
+        verbose (bool): whether to print output on each timing
+        kwargs (dict): passed to :func:`sc.toc() <toc>` when invoked
 
 
     Example making repeated calls to the same timer, using ``auto`` to keep track::
 
         >>> T = sc.timer(auto=True)
         >>> T.toc()
         (0): 2.63 s
@@ -698,35 +808,38 @@
         (1): 5.00 s
 
     Example wrapping code using with-as::
 
         >>> with sc.timer('mylabel'):
         >>>     sc.timedsleep(0.5)
 
-    Example using a timer to collect data, using ``tt()`` as an alias for ``toctic()``
+    Example using a timer to collect data, using :meth:`timer.tt() <timer.tt>` as an alias for :func:`sc.toctic() <toctic>`
     to reset the time::
 
         T = sc.timer(doprint=False)
         for key in 'abcde':
             sc.timedsleep(pl.rand())
             T.tt(key)
         print(T.timings)
 
     Implementation based on https://preshing.com/20110924/timing-your-code-using-pythons-with-statement/
 
-    | New in version 1.3.0: ``sc.timer()`` alias, and allowing the label as first argument.
-    | New in version 1.3.2: ``toc()`` passes label correctly; ``tt()`` method; ``auto`` argument
-    | New in version 2.0.0: ``plot()`` method; ``total()`` method; ``indivtimings`` and ``cumtimings`` properties
-    | New in version 2.1.0: ``total`` as property instead of method; updated repr; added disp() method
+    | *New in version 1.3.0:* :class:`sc.timer() <timer>` alias, and allowing the label as first argument.
+    | *New in version 1.3.2:* ``toc()`` passes label correctly; ``tt()`` method; ``auto`` argument
+    | *New in version 2.0.0:* ``plot()`` method; ``total()`` method; ``indivtimings`` and ``cumtimings`` properties
+    | *New in version 2.1.0:* ``total`` as property instead of method; updated repr; added disp() method
+    | *New in version 3.0.0:* ``unit`` argument; ``verbose`` argument; ``sum, min, max, mean, std`` methods; ``rawtimings`` property
     '''
-    def __init__(self, label=None, auto=False, start=True, **kwargs):
+    def __init__(self, label=None, auto=False, start=True, unit='auto', verbose=None, **kwargs):
         from . import sc_odict as sco # Here to avoid circular import
         self.kwargs = kwargs # Store kwargs to pass to toc() at the end of the block
         self.kwargs['label'] = label
         self.auto = auto
+        self.unit = unit
+        self.verbose = verbose
         self._start = None
         self._tics = []
         self._tocs = []
         self.elapsed = None
         self.message = None
         self.count = 0
         self.timings = sco.odict()
@@ -736,47 +849,49 @@
 
 
     def __enter__(self):
         ''' Reset start time when entering with-as block '''
         self.tic()
         return self
 
-
     def __exit__(self, *args):
         ''' Print elapsed time when leaving a with-as block '''
         self.toc()
         return
     
     def __repr__(self):
         string = scp.objectid(self)
         string += 'Timings:\n'
         string += str(self.timings)
         string += f'\nTotal time: {self.total:n} s'
         return string
     
+    def __len__(self):
+        return len(self._tocs)
+    
     
     def disp(self):
         ''' Display the full representation of the object '''
         return scp.pr(self)
 
 
     def tic(self):
         ''' Set start time '''
-        now = time.time()  # Store the present time locally
+        now = pytime.time()  # Store the present time locally
         self._start = now
         self._tics.append(now) # Store when this tic was invoked
         return
 
 
     def toc(self, label=None, **kwargs):
-        ''' Print elapsed time; see ``sc.toc()`` for keyword arguments '''
+        ''' Print elapsed time; see :func:`sc.toc() <toc>` for keyword arguments '''
 
         # Get the time
         self.elapsed, self.message = toc(start=self._start, output='both', doprint=False) # Get time as quickly as possible
-        self._tocs.append(time.time()) # Store when this toc was invoked
+        self._tocs.append(pytime.time()) # Store when this toc was invoked
 
         # Update the kwargs, including the label
         if label is not None:
             kwargs['label'] = label
         for k,v in self.kwargs.items():
             if k not in kwargs:
                 kwargs[k] = v
@@ -793,128 +908,178 @@
         timingslabel = countlabel if (self.auto or not(labelstr) or (labelstr in self.timings)) else labelstr # Use labelstr if it's a valid key, else include count information
         self.timings[timingslabel] = self.elapsed
         self.count += 1
         if self.auto:
             kwargs['label'] = countlabel
 
         # Call again to get the correct output
-        output = toc(elapsed=self.elapsed, **kwargs)
+        doprint = kwargs.pop('doprint', self.verbose)
+        output = toc(elapsed=self.elapsed, unit=self.unit, doprint=doprint, **kwargs)
 
         # If reset was used, apply it
         if kwargs.get('reset'):
             self.tic()
 
         return output
 
 
     @property
     def total(self):
         ''' Calculate total time '''
 
         # If the timer hasn't been started, return 0
-        if not len(self._tics):
+        if not len(self._tics): # pragma: no cover
             return 0
         else:
             start = self._tics[0]
 
         # If the timer hasn't been finished, use the current time; else the latest
-        if not len(self._tocs):
-            end = time.time()
+        if not len(self._tocs): # pragma: no cover
+            end = pytime.time()
         else:
             end = self._tocs[-1]
 
         elapsed = end - start
 
         return elapsed
 
 
     # Alias/shortcut methods
 
     def start(self):
-        ''' Alias for ``tic()`` '''
+        ''' Alias for :func:`sc.tic() <tic>` '''
         return self.tic()
 
     def stop(self, *args, **kwargs):
-        ''' Alias for ``toc()`` '''
+        ''' Alias for :func:`sc.toc() <toc>` '''
         return self.toc(*args, **kwargs)
 
     def tocout(self, label=None, output=True, **kwargs):
-        ''' Alias for ``toc()`` with output=True '''
+        ''' Alias for :func:`sc.toc() <toc>` with output=True '''
         return self.toc(label=label, output=output, **kwargs)
 
     def toctic(self, *args, reset=True, **kwargs):
         ''' Like toc, but reset time between timings '''
         return self.toc(*args, reset=reset, **kwargs)
 
     def tt(self, *args, **kwargs):
-        ''' Alias for ``toctic()`` '''
+        ''' Alias for :func:`sc.toctic() <toctic>` '''
         return self.toctic(*args, **kwargs)
 
     def tto(self, *args, output=True, **kwargs):
-        ''' Alias for ``toctic()`` with output=True '''
+        ''' Alias for :func:`sc.toctic() <toctic>` with output=True '''
         return self.toctic(*args, output=output, **kwargs)
+    
+    @property
+    def rawtimings(self):
+        ''' Return an array of timings '''
+        return self.timings[:]
 
     @property
     def indivtimings(self):
+        ''' Compute the individual time between each timing '''
         from . import sc_odict as sco # Here to avoid circular import
         vals = np.diff(scm.cat(self._tics[0], self._tocs))
         output = sco.odict(zip(self.timings.keys(), vals))
         return output
 
     @property
     def cumtimings(self):
+        ''' Compute the cumulative time for each timing '''
         from . import sc_odict as sco # Here to avoid circular import
         vals = np.array(self._tocs) - self._tics[0]
         output = sco.odict(zip(self.timings.keys(), vals))
         return output
 
+    def sum(self):
+        '''
+        Sum of timings; similar to :obj:`timer.total <timer.total>`
+        
+        *New in version 3.0.0.*
+        '''
+        return self.rawtimings.sum()
+    
+    def min(self):
+        '''
+        Minimum of timings
+        
+        *New in version 3.0.0.*
+        '''
+        return self.rawtimings.min()
+    
+    def max(self):
+        ''' 
+        Maximum of timings
+        
+        *New in version 3.0.0.*
+        '''
+        return self.rawtimings.max()
+    
+    def mean(self):
+        ''' 
+        Mean of timings
+        
+        *New in version 3.0.0.*
+        '''
+        return self.rawtimings.mean()
+    
+    def std(self):
+        ''' 
+        Standard deviation of timings
+        
+        *New in version 3.0.0.*
+        '''
+        return self.rawtimings.std()
+
 
     def plot(self, fig=None, figkwargs=None, grid=True, **kwargs):
         """
         Create a plot of Timer.timings
 
         Arguments:
             cumulative (bool): how the timings will be presented, individual or cumulative
             fig (fig): an existing figure to draw the plot in
-            figkwargs (dict): passed to ``pl.figure()``
+            figkwargs (dict): passed to :func:`pl.figure() <matplotlib.pyplot.figure>`
             grid (bool): whether to show a grid
-            kwargs (dict): passed to ``pl.bar()``
+            kwargs (dict): passed to :func:`pl.bar() <matplotlib.pyplot.bar>`
 
-        New in version 2.0.0.
+        *New in version 2.0.0.*
         """
         from . import sc_plotting as scp # Here to avoid circular import
 
         figkwargs = scu.mergedicts(figkwargs)
 
         # Handle the figure
         if fig is None:
             fig = pl.figure(**figkwargs)  # It's necessary to have an open figure or else the commands won't work
 
-        # plot times
+        # Plot times
         if len(self.timings) > 0:
             keys = self.timings.keys()
             vals = self.indivtimings[:]
+            
+            factor, label = _convert_time_unit(self.unit, elapsed=vals.sum())
+            vals /= factor
+            
             ax1 = pl.subplot(2,1,1)
             pl.barh(keys, vals, **kwargs)
             pl.title('Individual timings')
-            pl.ylabel('Label')
-            pl.xlabel('Elapsed time (s)')
+            pl.xlabel(f'Elapsed time ({label})')
 
             ax2 = pl.subplot(2,1,2)
             pl.barh(keys, np.cumsum(vals), **kwargs)
             pl.title('Cumulative timings')
-            pl.ylabel('Label')
-            pl.xlabel('Elapsed time (s)')
+            pl.xlabel(f'Elapsed time ({label})')
 
             for ax in [ax1, ax2]:
                 ax.invert_yaxis()
                 ax.grid(grid)
 
             scp.figlayout()
-        else:
+        else: # pragma: no cover
             errormsg = "Looks like nothing has been timed. Forgot to do T.start() and T.stop()??'"
             raise RuntimeWarning(errormsg)
 
         return fig
 
 
 Timer = timer # Alias
@@ -954,34 +1119,34 @@
         Prints a datetime object as a full date, stripping off any leading
         zeroes from the day (strftime() gives the day of the month as a zero-padded
         decimal number).
         """
         # %b/%B are the tokens for abbreviated/full names of months to strftime()
         if shortmonths:
             month_token = '%b'
-        else:
+        else: # pragma: no cover
             month_token = '%B'
 
         # Get a string from strftime()
         if includeyear:
             date_str = date.strftime('%d ' + month_token + ' %Y')
-        else:
+        else: # pragma: no cover
             date_str = date.strftime('%d ' + month_token)
 
         # There will only ever be at most one leading zero, so check for this and
         # remove if necessary
         if date_str[0] == '0':
             date_str = date_str[1:]
 
         return date_str
 
     now_time = dt.datetime.now()
 
     # If the user passes in a string, try to turn it into a datetime object before continuing
-    if isinstance(pasttime, str):
+    if isinstance(pasttime, str): # pragma: no cover
         try:
             pasttime = readdate(pasttime)
         except ValueError as E: # pragma: no cover
             errormsg = f"User supplied string {pasttime} is not in a readable format."
             raise ValueError(errormsg) from E
     elif isinstance(pasttime, dt.datetime):
         pass
@@ -991,15 +1156,15 @@
 
     # It doesn't make sense to measure time elapsed between now and a future date, so we'll just print the date
     if pasttime > now_time:
         includeyear = (pasttime.year != now_time.year)
         time_str = print_date(pasttime, includeyear=includeyear, shortmonths=shortmonths)
 
     # Otherwise, start by getting the elapsed time as a datetime object
-    else:
+    else: # pragma: no cover
         elapsed_time = now_time - pasttime
 
         # Check if the time is within the last minute
         if elapsed_time < dt.timedelta(seconds=60):
             if elapsed_time.seconds <= minseconds:
                 time_str = "just now"
             else:
@@ -1036,76 +1201,106 @@
         else:
             includeyear = (pasttime.year != now_time.year)
             time_str = print_date(pasttime, includeyear=includeyear, shortmonths=shortmonths)
 
     return time_str
 
 
-def timedsleep(delay=None, start=None, verbose=True):
+# Most robust results just from hard-coding this, despite variability between machines
+_sleep_overhead = 5e-5 # Amount of time taken for a "zero" delay
+
+def timedsleep(delay=None, start=None, verbose=False):
     '''
-    Delay for a certain amount of time, to ensure accurate timing.
+    Pause for the specified amount of time, taking into account how long other
+    operations take.
+    
+    This function is usually used in a loop; it works like ``time.sleep()``, but 
+    subtracts time taken by the other operations in the loop so that each loop
+    iteration takes exactly ``delay`` amount of time. Note: since ``time.sleep()`` 
+    has a minimum overhead (about 2e-4 seconds), below this duration, no pause
+    will occur.
 
     Args:
         delay (float): time, in seconds, to wait for
         start (float): if provided, the start time
-        verbose (bool): whether to print activity
+        verbose (bool): whether to print details
 
-    **Example**::
+    **Examples**::
 
+        # Example for a long(ish) computation
+        import numpy as np
         for i in range(10):
             sc.timedsleep('start') # Initialize
-            for j in range(int(1e6)):
-                tmp = pl.rand()
-            sc.timedsleep(1) # Wait for one second including computation time
+            n = int(2*np.random.rand()*1e6) # Variable computation time
+            for j in range(n):
+                tmp = np.random.rand()
+            sc.timedsleep(1, verbose=True) # Wait for one second per iteration including computation time
+        
+        
+        # Example illustrating more accurate timing
+        import time
+        n = 1000
+
+        with sc.timer():
+            for i in range(n):
+                sc.timedsleep(1/n)
+        # Elapsed time: 1.01 s
+
+        with sc.timer():
+            for i in range(n):
+                time.sleep(1/n)
+        # Elapsed time: 1.21 s
+    
+    *New in version 3.0.0:* "verbose" False by default; more accurate overhead calculation
     '''
-    self_time = 0.00012 # Roughly how long this function itself takes to run -- slightly underestimate
     global _delaytime
     if delay is None or delay=='start':
-        _delaytime = time.time()  # Store the present time in the global.
+        _delaytime = pytime.time()  # Store the present time in the global.
         return _delaytime         # Return the same stored number.
     else:
         if start is None:
             try:    start = _delaytime
-            except: start = time.time()
-        elapsed = time.time() - start
-        remaining = delay - elapsed
-        if remaining>0:
-            if verbose:
-                print(f'Pausing for {remaining:0.1f} s')
-            time.sleep(remaining - self_time)
-            try:    del _delaytime # After it's been used, we can't use it again
-            except: pass
-        else:
-            if verbose:
-                print(f'Warning, delay less than elapsed time ({delay:0.1f} vs. {elapsed:0.1f})')
+            except: start = pytime.time()
+        elapsed = pytime.time() - start
+        remaining = max(1e-12, delay - elapsed - _sleep_overhead)
+        pytime.sleep(remaining)
+        try:    del _delaytime # After it's been used, we can't use it again
+        except: pass
+        if remaining > 0 and verbose:
+            print(f'Pausing for {remaining:n} s')
+        elif verbose: # pragma: no cover
+            print(f'Warning, delay less than elapsed time ({delay:n} vs. {elapsed:n})')
     return
 
 
-def randsleep(delay=1.0, var=1.0, low=None, high=None):
+def randsleep(delay=1.0, var=1.0, low=None, high=None, seed=None):
     '''
     Sleep for a nondeterminate period of time (useful for desynchronizing tasks)
 
     Args:
         delay (float/list): average duration in seconds to sleep for; if a pair of values, treat as low and high
         var   (float):      how much variability to have (default, 1.0, i.e. from 0 to 2*interval)
         low   (float):      optionally define lower bound of sleep
         high  (float):      optionally define upper bound of sleep
+        seed  (int):        if provided, reset the random seed
 
     **Examples**::
         sc.randsleep(1) # Sleep for 0-2 s (average 1.0)
         sc.randsleep(2, 0.1) # Sleep for 1.8-2.2 s (average 2.0)
         sc.randsleep([0.5, 1.5]) # Sleep for 0.5-1.5 s
         sc.randsleeep(low=0.5, high=1.5) # Ditto
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
+    *New in version 3.0.0:* "seed" argument
     '''
     if low is None or high is None:
         if scu.isnumber(delay):
             low  = delay*(1-var)
             high = delay*(1+var)
         else:
             low, high = delay[0], delay[1]
 
-    dur = np.random.uniform(low, high)
-    time.sleep(dur)
+    rng = np.random.default_rng(seed)
+    dur = rng.uniform(low, high)
+    pytime.sleep(dur)
 
     return dur
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sciris-2.1.0/sciris/sc_fileio.py` & `sciris-3.0.0/sciris/sc_fileio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,225 +1,293 @@
 """
 Functions for reading/writing to files, including pickles, JSONs, and Excel.
 
 Highlights:
-    - :func:`save` / :func:`load`: efficiently save/load any Python object (via pickling)
-    - :func:`savetext` / :func:`loadtext`: likewise, for text
-    - :func:`savejson` / :func:`loadjson`: likewise, for JSONs
-    - :func:`saveyaml` / :func:`saveyaml`: likewise, for YAML
-    - :func:`thisdir`: get current folder
-    - :func:`getfilelist`: easy way to access glob
-    - :func:`rmpath`: remove files and folders
+    - :func:`sc.save() <save>` / :func:`sc.load() <load>`: efficiently save/load any Python object (via pickling)
+    - :func:`sc.savetext() <savetext>` / :func:`sc.loadtext() <loadtext>`: likewise, for text
+    - :func:`sc.savejson() <savejson>` / :func:`sc.loadjson() <loadjson>`: likewise, for JSONs
+    - :func:`sc.saveyaml() <saveyaml>` / :func:`sc.saveyaml() <saveyaml>`: likewise, for YAML
+    - :func:`sc.thisdir() <thisdir>`: get current folder
+    - :func:`sc.getfilelist() <getfilelist>`: easy way to access glob
+    - :func:`sc.rmpath() <rmpath>`: remove files and folders
 """
 
 ##############################################################################
 #%% Imports
 ##############################################################################
 
 # Basic imports
 import io
 import os
 import json
-import shutil
 import uuid
+import dill
+import shutil
 import string
 import inspect
 import importlib
-import traceback
 import warnings
 import numpy as np
 import pandas as pd
 import datetime as dt
 import gzip as gz
 import pickle as pkl
+import zstandard as zstd
 from zipfile import ZipFile
 from contextlib import closing
-from io import BytesIO as IO
 from pathlib import Path
-from glob import glob
+from glob import glob as pyglob
 import fnmatch as fnm
 from . import sc_settings as scs
 from . import sc_utils as scu
 from . import sc_printing as scp
 from . import sc_datetime as scd
 from . import sc_odict as sco
 from . import sc_dataframe as scdf
-zstd = scu.importbyname('zstandard', die=False, verbose=False) # Optional import
 
 
 ##############################################################################
 #%% Pickling functions
 ##############################################################################
 
-__all__ = ['load', 'save', 'loadobj', 'saveobj', 'zsave', 'loadstr', 'dumpstr', 'rmpath']
-
-
-def load(filename=None, folder=None, verbose=False, die=None, remapping=None, method='pickle', **kwargs):
-    '''
-    Load a file that has been saved as a gzipped pickle file, e.g. by :func:`save`.
-    Accepts either a filename (standard usage) or a file object as the first argument.
-    Note that `:func:`load`/:func:`loadobj` are aliases of each other.
-
-    Note: be careful when loading pickle files, since a malicious pickle can be
-    used to execute arbitrary code.
-
-    When a pickle file is loaded, Python imports any modules that are referenced
-    in it. This is a problem if module has been renamed. In this case, you can
-    use the ``remapping`` argument to point to the new modules or classes.
-
-    Args:
-        filename  (str/Path): the filename (or full path) to load
-        folder    (str/Path): the folder
-        verbose   (bool):     print details
-        die       (bool):     whether to raise an exception if errors are encountered (otherwise, load as much as possible)
-        remapping (dict):     way of mapping old/unavailable module names to new
-        method    (str):      method for loading (usually pickle or dill)
-        kwargs    (dict):     passed to ``pickle.loads()``/``dill.loads()``
-
-    **Examples**::
-
-        obj = sc.load('myfile.obj') # Standard usage
-        old = sc.load('my-old-file.obj', method='dill', ignore=True) # Load classes from saved files
-        old = sc.load('my-old-file.obj', remapping={'foo.Bar':cat.Mat}) # If loading a saved object containing a reference to foo.Bar that is now cat.Mat
-        old = sc.load('my-old-file.obj', remapping={'foo.Bar':('cat', 'Mat')}) # Equivalent to the above
+__all__ = ['load', 'save', 'loadobj', 'saveobj', 'zsave', 'loadstr', 'dumpstr']
 
-    | New in version 1.1.0: "remapping" argument
-    | New in version 1.2.2: ability to load non-gzipped pickles; support for dill; arguments passed to loader
-    '''
-
-    # Handle loading of either filename or file object
-    if isinstance(filename, Path):
-        filename = str(filename)
-    if scu.isstring(filename):
-        argtype = 'filename'
-        filename = makefilepath(filename=filename, folder=folder, makedirs=False) # If it is a file, validate the folder (but don't create one if it's missing)
-    elif isinstance(filename, io.BytesIO):
-        argtype = 'fileobj'
-    else: # pragma: no cover
-        errormsg = f'First argument to loadobj() must be a string or file object, not {type(filename)}'
-        raise TypeError(errormsg)
-    fileargs = {'mode': 'rb', argtype: filename}
 
-    # Define common error messages
-    gziperror = f'''
+# Define common error messages
+def _gziperror(filename):
+    ''' Base error message when a file couldn't be opened '''
+    return f'''
 Unable to load
     {filename}
 as either a gzipped, zstandard or regular pickle file. Ensure that it is actually a pickle file.
 '''
-    unpicklingerror = f'''
+
+def _unpicklingerror(filename):
+    ''' Base error message when a file couldn't be loaded '''
+    return f'''
 Unable to load file: "{filename}"
 as a gzipped pickle file. Loading pickles can fail if Python modules have changed
 since the object was saved. If you are loading a custom class that has failed,
-you can use the remapping argument; see the sc.loadobj() docstring for details.
+you can use the remapping argument; see the sc.load() docstring for details.
 Otherwise, you might need to revert to the previous version of that module (e.g.
 in a virtual environment), save in a format other than pickle, reload in a different
 environment with the new version of that module, and then re-save as a pickle.
 
 For general information on unpickling errors, see e.g.:
 https://wiki.python.org/moin/UsingPickle
 https://stackoverflow.com/questions/41554738/how-to-load-an-old-pickle-file
 '''
 
-    # Load the file
+
+def _load_filestr(filename, folder):
+    ''' Try different options for loading a file on disk into a string -- not for external use '''
+    
+    # Handle loading of either filename or file object
+    if isinstance(filename, Path):
+        filename = str(filename)
+    if scu.isstring(filename):
+        argtype = 'filename'
+        filename = makefilepath(filename=filename, folder=folder, makedirs=False) # If it is a file, validate the folder (but don't create one if it's missing)
+    elif isinstance(filename, io.BytesIO):
+        argtype = 'fileobj'
+    else: # pragma: no cover
+        errormsg = f'First argument to sc.load() must be a string or file object, not {type(filename)}; see also sc.loadstr()'
+        raise TypeError(errormsg)
+    fileargs = {'mode': 'rb', argtype: filename}
+    
     try:
         with gz.GzipFile(**fileargs) as fileobj:
             filestr = fileobj.read() # Convert it to a string
     except Exception as E: # pragma: no cover
         exc = type(E) # Figure out what kind of error it is
         if exc == FileNotFoundError: # This is simple, just raise directly
             raise E
         elif exc == gz.BadGzipFile:
             try: # If the gzip file failed, first try as a zstd compressed object
                 with open(filename, 'rb') as fh:
                     zdcompressor = zstd.ZstdDecompressor()
                     with zdcompressor.stream_reader(fh) as fileobj:
                         filestr = fileobj.read()
-            except Exception as E2: # If that fails
-                try: # Try as a regular object
+            except Exception as E2: # If that fails...
+                try: # Try as a regular binary object
                     with open(filename, 'rb') as fileobj:
                         filestr = fileobj.read() # Convert it to a string
                 except Exception as E3:
-                    gziperror += f'\nAdditional errors encountered:\n{str(E2)}\n{str(E3)}'
-                    raise exc(gziperror) from E
+                    try: # And finally as a regular object
+                        with open(filename, 'r') as fileobj:
+                            filestr = fileobj.read() # Convert it to a string
+                    except Exception as E4:
+                        gziperror = _gziperror(filename) + f'\nAdditional errors encountered:\n{str(E2)}\n{str(E3)}\n{str(E4)}'
+                        raise exc(gziperror) from E
+        else:
+            exc = type(E)
+            errormsg = 'sc.load(): Could not open the # pragma: no cover file string for an unknown reason; see error above for details'
+            raise exc(errormsg) from E
+    return filestr
+
+
+def load(filename=None, folder=None, verbose=False, die=None, remapping=None, 
+         method='pickle', auto_remap=True, **kwargs):
+    '''
+    Load a file that has been saved as a gzipped pickle file, e.g. by :func:`sc.save() <save>`.
+    Accepts either a filename (standard usage) or a file object as the first argument.
+    Note that :func:`sc.load() <load>`/:func:`sc.loadobj() <loadobj>` are aliases of each other.
+
+    **Note 1**: Since this function relies on pickle, it can potentially execute arbitrary
+    code, so you should only use it with sources you trust. For more information, see:
+    https://docs.python.org/3/library/pickle.html
+
+    **Note 2**: When a pickle file is loaded, Python imports any modules that are referenced
+    in it. This is a problem if module has been renamed. In this case, you can
+    use the ``remapping`` argument to point to the new modules or classes. For
+    more robustness, use the :func:`sc.savearchive() <savearchive>`/:func:`sc.loadarchive() <loadarchive>`
+    functions.
+
+
+    Args:
+        filename   (str/Path): the filename (or full path) to load
+        folder     (str/Path): the folder
+        verbose    (bool):     print details
+        die        (bool):     whether to raise an exception if errors are encountered (otherwise, load as much as possible)
+        remapping  (dict):     way of mapping old/unavailable module names to new
+        method     (str):      method for loading (usually pickle or dill)
+        auto_remap (bool):     whether to use known deprecations to load failed pickles
+        kwargs     (dict):     passed to ``pickle.loads()``/``dill.loads()``
+
+    **Examples**::
+
+        obj = sc.load('myfile.obj') # Standard usage
+        old = sc.load('my-old-file.obj', method='dill', ignore=True) # Load classes from saved files
+        old = sc.load('my-old-file.obj', remapping={'foo.Bar':cat.Mat}) # If loading a saved object containing a reference to foo.Bar that is now cat.Mat
+        old = sc.load('my-old-file.obj', remapping={'foo.Bar':('cat', 'Mat')}) # Equivalent to the above
+
+    | *New in version 1.1.0:* "remapping" argument
+    | *New in version 1.2.2:* ability to load non-gzipped pickles; support for dill; arguments passed to loader
+    '''
+    # Load the file
+    filestr = _load_filestr(filename, folder)
 
     # Unpickle it
     try:
-        obj = _unpickler(filestr, filename=filename, verbose=verbose, die=die, remapping=remapping, method=method, **kwargs) # Actually load it
+        kw = dict(filename=filename, verbose=verbose, die=die, remapping=remapping, method=method, auto_remap=auto_remap)
+        obj = _unpickler(filestr, **kw, **kwargs) # Unpickle the data
     except Exception as E: # pragma: no cover
         exc = type(E) # Figure out what kind of error it is
-        errormsg = unpicklingerror + '\n\nSee the stack trace above for more information on this specific error.'
+        errormsg = _unpicklingerror(filename) + '\n\nSee the stack trace above for more information on this specific error.'
         raise exc(errormsg) from E
 
     # If it loaded but with errors, print them here
     if isinstance(obj, Failed):
-        print(unpicklingerror)
-    elif verbose:
+        print(_unpicklingerror(filename))
+    elif verbose: # pragma: no cover
         print(f'Object loaded from "{filename}"')
 
     return obj
 
 
-def save(filename='default.obj', obj=None, folder=None, compression='gzip', compresslevel=5, 
-         verbose=0, method='pickle', sanitizepath=True, die=False, *args, **kwargs):
+def save(filename='default.obj', obj=None, folder=None, method='pickle', compression='gzip', 
+         compresslevel=5, verbose=0, sanitizepath=True, die=False, allow_empty=False, **kwargs):
     '''
-    Save an object to file as a gzipped pickle -- use compression 5 by default,
-    since more is much slower but not much smaller. Once saved, can be loaded
-    with :func:`load`. Note that :func:`save`/:func:`saveobj` are identical.
+    Save any object to disk
+    
+    This function is similar to :func:`pickle.dump()` in that it serializes the object
+    to a file. Key differences include:
+        
+        - It takes care of opening/closing the file for writing
+        - It compresses the data by default
+        - It supports different serialization methods (e.g. pickle or dill)
+    
+    Once an object is saved, it can be loaded with :func:`sc.load() <load>`. Note that 
+    :func:`sc.save() <save>`/:func:`sc.saveobj() <saveobj>` are identical.
+    
+    
+    **Note 1**: Since this function relies on pickle, it can potentially execute arbitrary
+    code, so you should only use it with sources you trust. For more information, see:
+    https://docs.python.org/3/library/pickle.html
+        
+    **Note 2**: When a pickle file is loaded, Python imports any modules that are referenced
+    in it. This is a problem if module has been renamed (in which case the pickle
+    usually can't be opened). For more robustness (e.g. to pickle custom classes), use 
+    ``method='dill'`` and/or the :func:`sc.savearchive() <savearchive>`/:func:`sc.loadarchive() <loadarchive>`
+    functions.
+    
+    If you do not need to save arbitrary Python and just need to save data, consider
+    saving the data in a standard format, e.g. JSON (:func:`sc.savejson() <savejson>`). For large
+    amounts of tabular data, also consider formats like HDF5 or PyArrow.
 
     Args:
-        filename      (str/Path) : the filename or path to save to; if None, return an io.BytesIO filestream instead of saving to disk
+        filename      (str/path) : the filename or path to save to; if None, return an io.BytesIO filestream instead of saving to disk
         obj           (anything) : the object to save
-        folder        (str)      : passed to :func:`makepath`
+        folder        (str)      : optional additional folder, passed to :func:`sc.makepath() <makepath>`
+        method        (str)      : whether to use 'pickle' (default) or 'dill'
         compression   (str)      : type of compression to use: 'gzip' (default), 'zstd' (zstandard), or 'none' (no compression)
         compresslevel (int)      : the level of gzip/zstd compression (1 to 9 for gzip, -7 to 22 for zstandard, default 5)
-        verbose       (int)      : detail to print
-        method        (str)      : whether to use 'pickle' (default) or 'dill'
-        die           (bool)     : whether to fail if the object can't be pickled (else, try dill)
+        verbose       (int)      : level of detail to print
         sanitizepath  (bool)     : whether to sanitize the path prior to saving
-        args          (list)     : passed to ``pickle.dumps()``
-        kwargs        (dict)     : passed to ``pickle.dumps()``
+        die           (bool)     : whether to fail if the object can't be pickled (else, try dill); if die is 'never'
+        allow_empty   (bool)     : whether or not to allow "None" to be saved (usually treated as an error)
+        kwargs        (dict)     : passed to :func:`pickle.dumps()` (or ``dill.dumps()``)
 
-    **Example**::
+    **Examples**::
 
-        myobj = ['this', 'is', 'a', 'weird', {'object':44}]
-        sc.save('myfile.obj', myobj)
-        sc.save('myfile.obj', myobj, method='dill') # Use dill instead, to save custom classes as well
+        # Standard usage
+        my_obj = ['this', 'is', 'my', 'custom', {'object':44}]
+        sc.save('myfile.obj', my_obj)
+        loaded = sc.load('myfile.obj')
+        assert loaded == my_obj
+        
+        # Use dill instead, to save custom classes as well
+        class MyClass:
+            def __init__(self, x):
+                self.data = np.random.rand(100) + x
+            def sum(self):
+                return self.data.sum()
+        my_class = MyClass(10)
+        
+        sc.save('my_class.obj', my_class, method='dill', compression='zstd')
+        loaded = sc.load('my_class.obj') # With dill, can be loaded anywhere, not just in the same script
+        assert loaded.sum() == my_class.sum()
+    
+    See also :func:`sc.zsave() <zsave>` (identical except defaults to zstandard compression).
 
-    | New in version 1.1.1: removed Python 2 support.
-    | New in version 1.2.2: automatic swapping of arguments if order is incorrect; correct passing of arguments
-    | New in version 2.0.4: "die" argument for saving as dill
-    | New in version 2.1.0: "zstandard" compression method
+    | *New in version 1.1.1:* removed Python 2 support.
+    | *New in version 1.2.2:* automatic swapping of arguments if order is incorrect; correct passing of arguments
+    | *New in version 2.0.4:* "die" argument for saving as dill
+    | *New in version 2.1.0:* "zstandard" compression method
+    | *New in version 3.0.0:* "allow_empty" argument; removed "args"
     '''
 
-    def serialize(fileobj, obj, success, *args, **kwargs):
+    def serialize(fileobj, obj, success, **kwargs):
         ''' Actually write a serial bytestream to disk '''
         # Try pickle first
         if method == 'pickle':
             try:
                 if verbose>=2: print('Saving as pickle...')
-                _savepickle(fileobj, obj, *args, **kwargs) # Use pickle
+                _savepickle(fileobj, obj, **kwargs) # Use pickle
                 success = True
             except Exception as E: # pragma: no cover
                 if die is True:
                     raise E
                 else:
                     if verbose>=2: print(f'Exception when saving as pickle ({repr(E)}), saving as dill...')
 
         # If dill is requested or pickle failed, use dill
         if not success: # pragma: no cover
             if verbose>=2: print('Saving as dill...')
-            _savedill(fileobj, obj, *args, **kwargs)
+            _savedill(fileobj, obj, **kwargs)
         
         return
     
     # Handle path
     if filename is None: # If the user explicitly specifies None as the file, create a byte stream instead
-        bytesobj = io.BytesIO()
+        tobytes = True
+        bytestream = io.BytesIO()
     else:
-        bytesobj = None
+        tobytes = False
+        bytestream = None
 
         # Process and sanitize the filename passed in by the user
         filetypes = (str, type(Path()), type(None))
         if isinstance(filename, Path): # If it's a path object, convert to string
             filename = str(filename)
 
         if not isinstance(filename, filetypes): # pragma: no cover
@@ -229,104 +297,123 @@
                 real_file = obj
                 filename = real_file
                 obj = real_obj
             else:
                 errormsg = f'Filename type {type(filename)} is not valid: must be one of {filetypes}'
                 raise Exception(errormsg)
 
-        filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath)
+        filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath, makedirs=True)
 
     # Handle object
     if obj is None: # pragma: no cover
         errormsg = "No object was supplied to saveobj(), or the object was empty; if this is intentional, set die='never'"
-        if die != 'never':
+        if not allow_empty and die != 'never': # die = 'never' is kept for backwards compatibility
             raise ValueError(errormsg)
 
     # Compress and actually save
     success = False
-    if compression in ['gz', 'gzip']:
+    
+    if compression in ['gz', 'gzip']:  # Main use case
         # File extension is .gz
-        with gz.GzipFile(filename=filename, fileobj=bytesobj, mode='wb', compresslevel=compresslevel) as fileobj:
-            serialize(fileobj, obj, success, *args, **kwargs)
-    elif compression in ['zst', 'zstd', 'zstandard']:
-        # File extension is .zst
-        with open(filename, 'wb') as fh:
-            zcompressor = zstd.ZstdCompressor(level=compresslevel)
-            with zcompressor.stream_writer(fh) as fileobj:
-                serialize(fileobj, obj, success, *args, **kwargs)
-    elif compression in ['none']:
-        with open(filename, 'wb') as fileobj:
-            serialize(fileobj, obj, success, *args, **kwargs)
+        with gz.GzipFile(filename=filename, fileobj=bytestream, mode='wb', compresslevel=compresslevel) as fileobj:
+            serialize(fileobj, obj, success, **kwargs)
+    
     else:
-        errormsg = f"Invalid compression format '{compression}': must be 'gzip', 'zstd', or 'none'"
-        raise ValueError(errormsg)
+        if tobytes: # pragma: no cover
+            filecontext = closing(bytestream)
+        else:
+            filecontext = open(filename, 'wb')
+        
+        if compression in ['zst', 'zstd', 'zstandard']:
+            # File extension is .zst
+            with filecontext as fh:
+                zcompressor = zstd.ZstdCompressor(level=compresslevel)
+                with zcompressor.stream_writer(fh) as fileobj:
+                    serialize(fileobj, obj, success, **kwargs)
+        elif compression in ['none']:
+            # File extension can be anything
+            with filecontext as fileobj:
+                serialize(fileobj, obj, success, **kwargs)
+        else: # pragma: no cover
+            errormsg = f"Invalid compression format '{compression}': must be 'gzip', 'zstd', or 'none'"
+            raise ValueError(errormsg)
 
-    if verbose and filename:
+    if verbose and filename: # pragma: no cover
         print(f'Object saved to "{filename}"')
 
     if filename:
         return filename
     else: # pragma: no cover
-        bytesobj.seek(0)
-        return bytesobj
+        bytestream.seek(0)
+        return bytestream
 
 
 # Backwards compatibility for core functions
 loadobj = load
 saveobj = save
 
 
-def loadstr(string, verbose=False, die=None, remapping=None):
+def zsave(*args, compression='zstd', **kwargs):
+    '''
+    Save a file using zstandard (instead of gzip) compression. This is an alias
+    for ``sc.save(..., compression='zstd')``; see :func:`sc.save() <save>` for details.
+    
+    Note: there is no matching function ``sc.zload()`` since :func:`sc.load() <load>` will
+    automatically try loading zstandard.
+    
+    *New in version 2.1.0.*
+    '''
+    return save(*args, compression=compression, **kwargs)
+
+
+def loadstr(string, **kwargs):
     '''
-    Like :func:`load()`, but for a bytes-like string (rarely used).
+    Like :func:`sc.load() <load>`, but for a bytes-like string (rarely used).
+    
+    Args:
+        string (str): the bytes-like string to load
+        kwargs (dict): passed to :func:`sc.load() <load>`
 
     **Example**::
 
         obj = sc.objdict(a=1, b=2)
-        string1 = sc.dumpstr(obj)
-        string2 = sc.loadstr(string1)
-        assert string1 == string2
-    '''
-    with closing(IO(string)) as output: # Open a "fake file" with the Gzip string pickle in it
-        with gz.GzipFile(fileobj=output, mode='rb') as fileobj: # Set a Gzip reader to pull from the "file"
-            picklestring = fileobj.read() # Read the string pickle from the "file" (applying Gzip decompression).
-    obj = _unpickler(picklestring, filestring=string, verbose=verbose, die=die, remapping=remapping) # Return the object gotten from the string pickle.
+        bytestring = sc.dumpstr(obj)
+        obj2 = sc.loadstr(bytestring)
+        assert obj == obj2
+    
+    | *New in version 3.0.0:* uses :func:`sc.load() <load>` for more robustness
+    '''
+    with closing(io.BytesIO(string)) as bytestream: # Open a "fake file" with the Gzip string pickle in it
+        obj = load(bytestream, **kwargs)
     return obj
 
 
-def dumpstr(obj=None):
-    ''' Dump an object as a bytes-like string (rarely used); see :func:`loadstr()` '''
-    with closing(IO()) as output: # Open a "fake file"
-        with gz.GzipFile(fileobj=output, mode='wb') as fileobj:  # Open a Gzip-compressing way to write to this "file"
-            try:    _savepickle(fileobj, obj) # Use pickle
-            except: _savedill(fileobj, obj) # ...but use Dill if that fails
-        output.seek(0) # Move the mark to the beginning of the "file."
-        result = output.read() # Read all of the content into result.
-    return result
-
-
-def zsave(*args, compression='zstd', **kwargs):
+def dumpstr(obj=None, **kwargs):
     '''
-    Save a file using zstandard (instead of gzip) compression. This is an alias
-    for ``sc.save(..., compression='zstd')``; see :func:`save()` for details.
+    Dump an object to a bytes-like string (rarely used by the user); see :func:`sc.save() <save>`
+    instead.
     
-    Note: there is no matching function ``sc.zload()`` since :func:`load()` will
-    automatically try loading
+    Args:
+        obj (any): the object to convert
+        kwargs (dict): passed to :func:`sc.save() <save>`
     
-    New in version 2.1.0.    
+    *New in version 3.0.0:* uses :func:`sc.save() <save>` for more robustness
     '''
-    return save(*args, compression=compression, **kwargs)
+    bytesobj = save(filename=None, obj=obj, **kwargs)
+    result = bytesobj.read() # Read all of the content into result
+    return result
 
 
 ##############################################################################
 #%% Other file functions
 ##############################################################################
 
-__all__ += ['loadtext', 'savetext', 'loadzip', 'savezip', 'path', 'ispath', 'thisfile', 'thisdir', 'thispath',
-            'getfilelist', 'getfilepaths', 'sanitizefilename', 'sanitizepath', 'makefilepath', 'makepath', 'rmpath']
+__all__ += ['loadtext', 'savetext', 'loadzip', 'unzip', 'savezip', 'path', 'ispath', 
+            'thisfile', 'thisdir', 'thispath', 'getfilelist', 'glob', 'getfilepaths', 
+            'sanitizefilename', 'sanitizepath', 'makefilepath', 'makepath', 'rmpath']
 
 
 def loadtext(filename=None, folder=None, splitlines=False):
     '''
     Convenience function for reading a text file
 
     **Example**::
@@ -345,126 +432,188 @@
     '''
     Convenience function for saving a text file -- accepts a string or list of strings;
     can also save an arbitrary object, in which case it will first convert to a string.
     
     Args:
         filename (str): the filename to save to
         string (str): the string (or object) to save
-        kwargs (dict): passed to ``np.savetxt()`` if saving an array
+        kwargs (dict): passed to :func:`np.savetxt() <numpy.savetxt>` if saving an array
 
     **Example**::
 
         text = ['Here', 'is', 'a', 'poem']
         sc.savetext('my-poem.txt', text)
     '''
     is_array = scu.isarray(string)
     if isinstance(string, list):
-        string = '\n'.join(string) # Convert from list to string)
+        string = '\n'.join(str(string)) # Convert from list to string)
     elif not is_array and not scu.isstring(string):
         string = str(string)
-    filename = makefilepath(filename=filename)
+    filename = makefilepath(filename=filename, makedirs=True)
     if is_array: # Shortcut to Numpy for saving arrays -- basic CSV
         kw = scu.mergedicts(dict(fmt='%s', delimiter=', '), kwargs)
         np.savetxt(filename, string, **kw)
     else: # Main use case: save text
         with open(filename, 'w') as f:
             f.write(string)
     return
 
 
-def loadzip(filename=None, outfolder='.', folder=None, extract=True):
+def loadzip(filename=None, folder=None, **kwargs):
+    '''
+    Load the contents of a zip file into a variable
+
+    Args:
+        filename (str/path): the name of the zip file to write to
+        folder (str): optional additional folder for the filename
+        kwargs (dict): passed to :func:`sc.load() <load>`
+    
+    Returns:
+        dict with each file loaded as a key
+
+    **Example**::
+
+        data = sc.loadzip('my-files.zip')
+
+    | *New in version 2.0.0.*
+    | *New in version 3.0.0:* load into memory instead of extracting to disk; see :func:`sc.unzip() <unzip>` for extracting
+    '''
+    filename = makefilepath(filename=filename, folder=folder)
+    output = dict()
+    with ZipFile(filename, 'r') as zf: # Create the zip file
+        names = zf.namelist()
+        for name in names:
+            val = zf.read(name)
+            try:
+                val = loadstr(val, **kwargs) # Try to load as a pickle or some kind of valid file
+            except:
+                pass # Otherwise, just return the raw value
+            output[name] = val
+    return output
+
+
+def unzip(filename=None, outfolder='.', folder=None, members=None):
     '''
     Convenience function for reading a zip file
 
     Args:
         filename (str/path): the name of the zip file to write to
         outfolder (str/path): the path location to extract the files to (default: current folder)
         folder (str): optional additional folder for the filename
-        extract (bool): whether to extract the compressed files; otherwise, load data
+        members (list): optional list of members
+    
+    Returns:
+        list of the names of the unzipped files
 
-    **Examples**::
+    **Example**::
 
-        sc.loadzip('my-files.zip')
-        data = sc.loadzip('mydata.zip', extract=False)
+        sc.unzip('my-files.zip', outfolder='my_data') # extracts all files 
 
-    New in version 2.0.0.
+    | *New in version 3.0.0* (equivalent to sc.loadzip(..., extract=True) previously)
     '''
     filename = makefilepath(filename=filename, folder=folder)
-    output = None
-    with ZipFile(filename, 'r') as zf: # Create the zip file
-        if extract:
-            zf.extractall(outfolder)
-        else:
-            output = dict()
-            names = zf.namelist()
-            for name in names:
-                val = zf.read(name)
-                try:
-                    val = loadstr(val)
-                except:
-                    pass
-                output[name] = val
+    with ZipFile(filename, 'r') as zf: # Load the zip file
+        names = zf.namelist()
+        zf.extractall(outfolder, members=members)
+    
+    output = [makefilepath(filename=name, folder=outfolder, makedirs=True) for name in names]
     return output
 
 
-def savezip(filename=None, filelist=None, data=None, folder=None, basename=True, sanitizepath=True, verbose=True):
+def savezip(filename=None, files=None, data=None, folder=None, sanitizepath=True, 
+            basename=False, tobytes=True, verbose=True, **kwargs):
     '''
     Create a zip file from the supplied list of files (or less commonly, supplied data)
 
     Args:
         filename (str/path): the name of the zip file to write to
-        filelist (list): the list of files to compress
-        data (dict): if supplied, instead of files, write this data instead (must be a dictionary of filename keys and data values)
+        files (list): file(s) and/or folder(s) to compress
+        data (dict): if supplied, write this data as well or instead (must be a dictionary of filename keys and data values)
         folder (str): optional additional folder for the filename
-        basename (bool): whether to use only the file's basename as the name inside the zip file
         sanitizepath (bool): whether to sanitize the path prior to saving
+        basename (bool): whether to use only the file's basename as the name inside the zip file (otherwise, store folder info)
+        tobytes (bool): if data is provided, convert it automatically to bytes (otherwise, up to the user)
         verbose (bool): whether to print progress
+        kwargs (dict): passed to :func:`sc.save() <save>`
 
     **Examples**::
 
         scripts = sc.getfilelist('./code/*.py')
         sc.savezip('scripts.zip', scripts)
 
         sc.savezip('mydata.zip', data=dict(var1='test', var2=np.random.rand(3)))
 
-    New in version 2.0.0: saving data
+    | *New in version 2.0.0:* saving data
+    | *New in version 3.0.0:* "tobytes" argument and kwargs; "filelist" renamed "files"
     '''
 
-    # Handle inpus
-    fullpath = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath)
-    filelist = scu.tolist(filelist)
+    # Handle inputs
+    fullpath = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath, makedirs=True)
+    
+    
+    # If data is provided, do simple validation
     if data is not None:
-        if not isinstance(data, dict):
+        if not isinstance(data, dict): # pragma: no cover
             errormsg = 'Data has invalid format: must be a dictionary of filename keys and data values'
             raise ValueError(errormsg)
-
+    else:
+        data = {}
+    
+    # Typical use case: data is not provided, handle files
+    if files:
+        origfilelist = [path(file) for file in scu.tolist(files)]
+        
+        # Handle subfolders
+        extfilelist = scu.dcp(origfilelist) # An extended file list, including recursion into subfolders
+        for orig in origfilelist:
+            if orig.is_dir():
+                contents = getfilelist(orig, abspath=False, recursive=True, aspath=True)
+                extfilelist.extend(contents[1:]) # Skip the first entry since it's the folder that's already in the list
+        
+        # Remove duplicates to create the final file list
+        filelist = []
+        for efile in extfilelist:
+            if efile not in filelist:
+                filelist.append(efile)
+            
     # Write zip file
     with ZipFile(fullpath, 'w') as zf: # Create the zip file
-        if data is not None:
+        if data: # Optionally also save data
             for key,val in data.items():
-                zf.writestr(key, dumpstr(val))
-        else: # Main use case
+                if tobytes:
+                    val = dumpstr(val, **kwargs)
+                zf.writestr(key, val)
+        if files: # Main use case, save files
             for thisfile in filelist:
-                thispath = makefilepath(filename=thisfile, abspath=False)
-                if basename: thisname = os.path.basename(thispath)
-                else:        thisname = thispath
-                zf.write(thispath, thisname)
+                thispath = makefilepath(filename=thisfile, abspath=False, makedirs=False)
+                thisname = os.path.basename(thisfile) if basename else thisfile
+                zf.write(thispath, thisname) # Actually save
+        if not data and not files:
+            errormsg = 'No data and no files provided: nothing to save!'
+            raise FileNotFoundError(errormsg)
+        
     if verbose: print(f'Zip file saved to "{fullpath}"')
     return fullpath
 
 
 def path(*args, **kwargs):
     '''
     Alias to ``pathlib.Path()`` with some additional input sanitization:
 
         - ``None`` entries are removed
         - a list of arguments is converted to separate arguments
+        
+    **Examples**::
+        
+        sc.path('thisfile.py') # Returns PosixPath('thisfile.py')
+        
+        sc.path('/a/folder', None, 'a_file.txt') # Returns PosixPath('/a/folder/a_file.txt')
 
-    | New in version 1.2.2.
-    | New in version 2.0.0: handle None or list arguments
+    | *New in version 1.2.2.*
+    | *New in version 2.0.0:* handle None or list arguments
     '''
 
     # Handle inputs
     new_args = []
     for arg in args:
         if isinstance(arg, list):
             new_args.extend(arg)
@@ -480,15 +629,15 @@
 path.__doc__ += '\n\n' + Path.__doc__
 
 
 def ispath(obj):
     '''
     Alias to isinstance(obj, Path).
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     '''
     return isinstance(obj, Path)
 
 
 def thisfile(frame=1, aspath=None):
     '''
     Return the full path of the current file.
@@ -498,15 +647,15 @@
         aspath (bool): whether to return a Path object
     
     **Examples**::
         
         my_script_name = sc.thisfile() # Get the name of the current file
         calling_script = sc.thisfile(frame=2) # Get the name of the script that called this script
 
-    New in verison 2.1.0.
+    *New in verison 2.1.0.*
     '''
     if aspath is None: aspath = scs.options.aspath
     file = inspect.stack()[frame][1] # Adopted from Atomica
     if aspath:
         file = Path(file)
     return file
 
@@ -532,101 +681,111 @@
         thisdir = sc.thisdir() # Get folder of calling file
         thisdir = sc.thisdir('.') # Ditto (usually)
         thisdir = sc.thisdir(__file__) # Ditto (usually)
         file_in_same_dir = sc.thisdir(path='new_file.txt')
         file_in_sub_dir = sc.thisdir('..', 'tests', 'mytests.py') # Merge parent folder with sufolders and a file
         np_dir = sc.thisdir(np) # Get the folder that Numpy is loaded from (assuming "import numpy as np")
 
-    | New in version 1.1.0: "as_path" argument renamed "aspath"
-    | New in version 1.2.2: "path" argument
-    | New in version 1.3.0: allow modules
-    | New in version 2.1.0: frame argument
+    | *New in version 1.1.0:* "as_path" argument renamed "aspath"
+    | *New in version 1.2.2:* "path" argument
+    | *New in version 1.3.0:* allow modules
+    | *New in version 2.1.0:* frame argument
     '''
     if file is None: # No file: use the current folder
-         file = thisfile(frame=frame+1) # Need +1 since want the calling script
+        if scu.isjupyter():
+            file = os.path.abspath(os.path.expanduser('file_placeholder')) # This is as best we can do on Jupyter
+        else:
+            file = thisfile(frame=frame+1) # Need +1 since want the calling script
     elif hasattr(file, '__file__'): # It's actually a module
         file = file.__file__
     if aspath is None: aspath = scs.options.aspath
     folder = os.path.abspath(os.path.dirname(file))
     path = scu.mergelists(path, *args)
     filepath = os.path.join(folder, *path)
     if aspath:
         filepath = Path(filepath, **kwargs)
     return filepath
 
 
 def thispath(*args, frame=1, aspath=True, **kwargs):
     '''
-    Alias for :func:`thisdir` that returns a path by default instead of a string.
+    Alias for :func:`sc.thisdir() <thisdir>` that returns a path by default instead of a string.
     
-    New in version 2.1.0.
+    *New in version 2.1.0.*
     '''
     return thisdir(*args, frame=frame+1, aspath=aspath, **kwargs)
 
 thispath.__doc__ += '\n\n' + thisdir.__doc__
 
 
 def getfilelist(folder=None, pattern=None, fnmatch=None, abspath=False, nopath=False, 
                 filesonly=False, foldersonly=False, recursive=True, aspath=None):
     '''
-    A shortcut for using glob.
+    A shortcut for using :func:`glob.glob()`.
+    
+    Note that :func:`sc.getfilelist() <getfilelist>` and :func:`sc.glob() <glob>` 
+    are aliases of each other.
 
     Args:
         folder      (str):  the folder to find files in (default, current)
         pattern     (str):  the pattern to match (default, wildcard); can be excluded if part of the folder
         fnmatch     (str):  optional additional string to filter results by
         abspath     (bool): whether to return the full path
         nopath      (bool): whether to return no path
         filesonly   (bool): whether to only return files (not folders)
         foldersonly (bool): whether to only return folders (not files)
-        recursive   (bool): passed to glob() (note: ** is required as the pattern to match all subfolders)
+        recursive   (bool): passed to :func:`glob.glob()` (note: ** is required as the pattern to match all subfolders)
         aspath      (bool): whether to return Path objects
         
     Returns:
         List of files/folders
 
     **Examples**::
 
         sc.getfilelist() # return all files and folders in current folder
         sc.getfilelist('~/temp', '*.py', abspath=True) # return absolute paths of all Python files in ~/temp folder
         sc.getfilelist('~/temp/*.py') # Like above
         sc.getfilelist(fnmatch='*.py') # Recursively find all files ending in .py
 
-    New in version 1.1.0: "aspath" argument
-    New in version 2.1.0: default pattern of "**"; "fnmatch" argument; default recursive=True
+    | *New in version 1.1.0:* "aspath" argument
+    | *New in version 2.1.0:* default pattern of "**"; "fnmatch" argument; default recursive=True
     '''
     if folder is None:
         folder = '.'
     folder = os.path.expanduser(folder)
     if abspath:
         folder = os.path.abspath(folder)
     if os.path.isdir(folder) and pattern is None:
         pattern = '**'
     if aspath is None: 
         aspath = scs.options.aspath
     globstr = os.path.join(folder, pattern) if pattern else folder
-    filelist = sorted(glob(globstr, recursive=recursive))
+    filelist = sorted(pyglob(globstr, recursive=recursive))
     if filesonly:
         filelist = [f for f in filelist if os.path.isfile(f)]
     elif foldersonly:
         filelist = [f for f in filelist if os.path.isdir(f)]
     if nopath:
         filelist = [os.path.basename(f) for f in filelist]
     if fnmatch:
         filelist = [f for f in filelist if fnm.fnmatch(f, fnmatch)]
     if aspath:
         filelist = [Path(f) for f in filelist]
     return filelist
 
 
+# Define as an alias
+glob = getfilelist
+
+
 def getfilepaths(*args, aspath=True, **kwargs):
     '''
-    Alias for :func:`getfilelist` that returns paths by default instead of strings.
+    Alias for :func:`sc.getfilelist() <getfilelist>` that returns paths by default instead of strings.
     
-    New in version 2.1.0.
+    *New version 2.1.0.*
     '''
     return getfilelist(*args, aspath=True, **kwargs)
 
 getfilepaths.__doc__ += '\n\n' + getfilelist.__doc__
 
 
 def sanitizefilename(filename, sub='_', allowspaces=False, asciify=True, strict=False, disallowed=None, aspath=False):
@@ -644,15 +803,15 @@
         aspath (bool): whether to return a Path object
 
     **Example**::
 
         bad = 'Nöt*a   file&name?!.doc'
         good = sc.sanitizefilename(bad)
         
-    New in version 2.0.1: arguments "sub", "allowspaces", "asciify", "strict", and "disallowed"
+    *New version 2.0.1:* arguments "sub", "allowspaces", "asciify", "strict", and "disallowed"
     '''
     
     # Handle options
     if asciify:
         filename = scu.asciify(filename) # Ensure it's ASCII compatible
     if disallowed is None:
         if strict:
@@ -677,42 +836,42 @@
         sanitized = Path(sanitized)
 
     return sanitized # Return the sanitized file name.
 
 
 def sanitizepath(*args, aspath=True, **kwargs):
     '''
-    Alias for :func:`sanitizefilename` that returns a path by default instead of a string.
+    Alias for :func:`sc.sanitizefilename() <sanitizefilename>` that returns a path by default instead of a string.
     
-    New in version 2.1.0.
+    *New version 2.1.0.*
     '''
     return sanitizefilename(*args, aspath=True, **kwargs)
 
 sanitizepath.__doc__ += '\n\n' + sanitizefilename.__doc__
 
 
 
-def makefilepath(filename=None, folder=None, ext=None, default=None, split=False, aspath=None, abspath=True, makedirs=True, checkexists=None, sanitize=False, die=True, verbose=False):
+def makefilepath(filename=None, folder=None, ext=None, default=None, split=False, aspath=None, abspath=True, makedirs=False, checkexists=None, sanitize=False, die=True, verbose=False):
     '''
     Utility for taking a filename and folder -- or not -- and generating a
     valid path from them. By default, this function will combine a filename and
     folder using os.path.join, create the folder(s) if needed with os.makedirs,
     and return the absolute path.
 
     Args:
         filename    (str or Path)   : the filename, or full file path, to save to -- in which case this utility does nothing
-        folder      (str/Path/list) : the name of the folder to be prepended to the filename; if a list, fed to ``os.path.join()``
+        folder      (str/Path/list) : the name of the folder to be prepended to the filename; if a list, fed to :func:`os.path.join()`
         ext         (str)           : the extension to ensure the file has
         default     (str or list)   : a name or list of names to use if filename is None
         split       (bool)          : whether to return the path and filename separately
-        aspath      (bool)          : whether to return a Path object
+        aspath      (bool)          : whether to return a Path object (default: set by ``sc.options.aspath``)
         abspath     (bool)          : whether to conver to absolute path
         makedirs    (bool)          : whether or not to make the folders to save into if they don't exist
         checkexists (bool)          : if False/True, raises an exception if the path does/doesn't exist
-        sanitize    (bool)          : whether or not to remove special characters from the path; see :func:`sanitizepath` for details
+        sanitize    (bool)          : whether or not to remove special characters from the path; see :func:`sc.sanitizepath() <sanitizepath>` for details
         die         (bool)          : whether or not to raise an exception if cannot create directory failed (otherwise, return a string)
         verbose     (bool)          : how much detail to print
 
     Returns:
         filepath (str or Path): the validated path (or the folder and filename if split=True)
 
     **Simple example**::
@@ -722,43 +881,44 @@
     **Complex example**::
 
         filepath = makefilepath(filename=None, folder='./congee', ext='prj', default=[project.filename, project.name], split=True, abspath=True, makedirs=True)
 
     Assuming project.filename is None and project.name is "recipe" and ./congee
     doesn't exist, this will makes folder ./congee and returns e.g. ('/home/myname/congee', 'recipe.prj')
 
-    New in version 1.1.0: "aspath" argument
+    | *New in version 1.1.0:* "aspath" argument
+    | *New in version 3.0.0:* "makedirs" defaults to False
     '''
 
     # Initialize
     filefolder = '' # The folder the file will be located in
     filebasename = '' # The filename
     if aspath is None: aspath = scs.options.aspath
 
     if isinstance(filename, Path):
         filename = str(filename)
     if isinstance(folder, Path): # If it's a path object, convert to string
         folder = str(folder)
-    if isinstance(folder, list): # It's a list, join together
+    if isinstance(folder, list): # It's a list, join together # pragma: no cover
         folder = os.path.join(*folder)
 
     # Process filename
     if filename is None: # pragma: no cover
         defaultnames = scu.tolist(default) # Loop over list of default names
         for defaultname in defaultnames:
             if not filename and defaultname: filename = defaultname # Replace empty name with default name
     if filename is not None: # If filename exists by now, use it
         filebasename = os.path.basename(filename)
         filefolder = os.path.dirname(filename)
     if not filebasename: filebasename = 'default' # If all else fails
 
     # Add extension if it's defined but missing from the filebasename
-    if ext and not filebasename.endswith(ext):
+    if ext and not filebasename.endswith(ext): # pragma: no cover
         filebasename += '.'+ext
-    if verbose:
+    if verbose: # pragma: no cover
         print(f'From filename="{filename}", default="{default}", extension="{ext}", made basename "{filebasename}"')
 
     # Sanitize base filename
     if sanitize: filebasename = sanitizefilename(filebasename)
 
     # Process folder
     if folder is not None: # Replace with specified folder, if defined
@@ -791,75 +951,75 @@
             errormsg = f'File {filepath} should exist, but it does not'
             if die:
                 raise FileNotFoundError(errormsg)
         if errormsg:
             print(errormsg)
 
     # Decide on output
-    if verbose:
+    if verbose: # pragma: no cover
         print(f'From filename="{filename}", folder="{folder}", made path name "{filepath}"')
-    if split:
+    if split: # pragma: no cover
         output = filefolder, filebasename
     elif aspath:
         output = Path(filepath)
     else:
         output = filepath
 
     return output
 
 
 def makepath(*args, aspath=True, **kwargs):
     '''
-    Alias for :func:`makefilepath` that returns a path by default instead of a string
+    Alias for :func:`sc.makefilepath() <makefilepath>` that returns a path by default instead of a string
     (with apologies for the confusing terminology, kept for backwards compatibility).
     
-    New in version 2.1.0.
+    *New version 2.1.0.*
     '''
     return makefilepath(*args, **kwargs, aspath=True)
 
 makepath.__doc__ += '\n\n' + makefilepath.__doc__
 
 
 def rmpath(path=None, *args, die=True, verbose=True, interactive=False, **kwargs):
     """
-    Remove file(s) and folder(s). Alias to ``os.remove()`` (for files) and ``shutil.rmtree()``
+    Remove file(s) and folder(s). Alias to :func:`os.remove()` (for files) and :func:`shutil.rmtree()`
     (for folders).
 
     Arguments:
         path (str/Path/list): file, folder, or list to remove
         args (list): additional paths to remove
         die (bool): whether or not to raise an exception if cannot remove
         verbose (bool): how much detail to print
         interactive (bool): whether to confirm prior to each deletion
-        kwargs (dict): passed to ``os.remove()``/``shutil.rmtree()``
+        kwargs (dict): passed to :func:`os.remove()`/:func:`shutil.rmtree()`
 
     **Examples**::
 
         sc.rmpath('myobj.obj') # Remove a single file
         sc.rmpath('myobj1.obj', 'myobj2.obj', 'myobj3.obj') # Remove multiple files
         sc.rmpath(['myobj.obj', 'tests']) # Remove a file and a folder interactively
         sc.rmpath(sc.getfilelist('tests/*.obj')) # Example of removing multiple files
 
-    New in version 2.0.0.
+    *New version 2.0.0.*
     """
 
     paths = scu.mergelists(path, *args)
     for path in paths:
-        if not os.path.exists(path):
+        if not os.path.exists(path): # pragma: no cover
             errormsg = f'Path "{path}" does not exist'
             if die:
                 raise FileNotFoundError(errormsg)
             elif verbose:
                 print(errormsg)
         else:
             if os.path.isfile(path):
                 rm_func = os.remove
-            elif os.path.isdir(path):
+            elif os.path.isdir(path): # pragma: no cover
                 rm_func = shutil.rmtree
-            else:
+            else: # pragma: no cover
                 errormsg = f'Path "{path}" exists, but is neither a file nor a folder: unable to remove'
                 if die:
                     raise FileNotFoundError(errormsg)
                 elif verbose:
                     print(errormsg)
 
         if interactive: # pragma: no cover
@@ -882,168 +1042,251 @@
     return
 
 
 ##############################################################################
 #%% JSON functions
 ##############################################################################
 
-__all__ += ['sanitizejson', 'jsonify', 'loadjson', 'savejson', 'loadyaml', 'saveyaml', 'jsonpickle', 'jsonunpickle']
+__all__ += ['sanitizejson', 'jsonify', 'printjson', 'readjson', 'loadjson', 'savejson', 
+            'readyaml', 'loadyaml', 'saveyaml', 'jsonpickle', 'jsonunpickle']
 
 
-def sanitizejson(obj, verbose=True, die=False, tostring=False, **kwargs):
+def jsonify(obj, verbose=True, die=False, tostring=False, **kwargs):
     """
     This is the main conversion function for Python data-structures into JSON-compatible
-    data structures (note: :func:`sanitizejson`/:func:`jsonify` are identical).
+    data structures (note: :func:`sc.sanitizejson() <sanitizejson>`/:func:`sc.jsonify() <jsonify>` are identical).
 
     Args:
-        obj      (any):  almost any kind of data structure that is a combination of list, numpy.ndarray, odicts, etc.
+        obj      (any):  almost any kind of data structure that is a combination of list, :obj:`numpy.ndarray`, odicts, etc.
         verbose  (bool): level of detail to print
         die      (bool): whether or not to raise an exception if conversion failed (otherwise, return a string)
         tostring (bool): whether to return a string representation of the sanitized object instead of the object itself
         kwargs   (dict): passed to json.dumps() if tostring=True
 
     Returns:
         object (any or str): the converted object that should be JSON compatible, or its representation as a string if tostring=True
 
-    Version: 2020apr11
+    **Example**::
+        
+        data = dict(a=np.random.rand(3), b=dict(foo='cat', bar='dog'))
+        json = sc.jsonify(data)
+        jsonstr = sc.jsonify(data, tostring=True, indent=2)
     """
     if obj is None: # Return None unchanged
         output = None
 
     elif isinstance(obj, (bool, np.bool_)): # It's true/false
         output = bool(obj)
 
     elif scu.isnumber(obj): # It's a number
-        if np.isnan(obj): # It's nan, so return None
+        if np.isnan(obj): # It's nan, so return None # pragma: no cover
             output = None
         else:
             if isinstance(obj, (int, np.int64)):
                 output = int(obj) # It's an integer
             else:
                 output = float(obj)# It's something else, treat it as a float
 
     elif scu.isstring(obj): # It's a string of some kind
         try:    string = str(obj) # Try to convert it to ascii
         except: string = obj # Give up and use original
         output = string
 
     elif isinstance(obj, np.ndarray): # It's an array, iterate recursively
         if obj.shape: output = [sanitizejson(p) for p in list(obj)] # Handle most cases, incluing e.g. array([5])
-        else:         output = [sanitizejson(p) for p in list(np.array([obj]))] # Handle the special case of e.g. array(5)
+        else:         output = [sanitizejson(p) for p in list(np.array([obj]))] # Handle the special case of e.g. array(5) # pragma: no cover
 
     elif isinstance(obj, (list, set, tuple)): # It's another kind of interable, so iterate recurisevly
         output = [sanitizejson(p) for p in list(obj)]
 
     elif isinstance(obj, dict): # It's a dictionary, so iterate over the items
         output = {str(key):sanitizejson(val) for key,val in obj.items()}
 
-    elif isinstance(obj, (dt.time, dt.date, dt.datetime)):
+    elif isinstance(obj, (dt.time, dt.date, dt.datetime)): # pragma: no cover
         output = str(obj)
 
-    elif isinstance(obj, uuid.UUID):
+    elif isinstance(obj, uuid.UUID): # pragma: no cover
         output = str(obj)
 
-    elif callable(getattr(obj, 'to_dict', None)): # Handle e.g. pandas, where we want to return the object, not the string
+    elif callable(getattr(obj, 'to_dict', None)): # Handle e.g. pandas, where we want to return the object, not the string # pragma: no cover
         output = obj.to_dict()
 
-    elif callable(getattr(obj, 'to_json', None)):
+    elif callable(getattr(obj, 'to_json', None)): # pragma: no cover
         output = obj.to_json()
 
-    elif callable(getattr(obj, 'toJSON', None)):
+    elif callable(getattr(obj, 'toJSON', None)): # pragma: no cover
         output = obj.toJSON()
 
     else: # None of the above
         try:
-            output = jsonpickle(obj)
-        except Exception as E: # pragma: no cover
-            errormsg = f'Could not sanitize "{obj}" {type(obj)} ({str(E)}), converting to string instead'
-            if die:       raise TypeError(errormsg)
-            elif verbose: print(errormsg)
-            output = str(obj)
+            output = jsonify(obj.__dict__) # Try converting the contents to JSON
+            output = scu.mergedicts({'python_class': str(type(obj))}, output)
+        except:
+            try:
+                output = jsonpickle(obj)
+            except Exception as E: # pragma: no cover
+                errormsg = f'Could not sanitize "{obj}" {type(obj)} ({E}), converting to string instead'
+                if die:       raise TypeError(errormsg)
+                elif verbose: print(errormsg)
+                output = str(obj)
 
     # Convert to string if desired
     if tostring:
         output = json.dumps(output, **kwargs)
 
     return output
 
 # Define alias
-jsonify = sanitizejson
+sanitizejson = jsonify
+
+
+def printjson(obj, indent=2, **kwargs):
+    '''
+    Print an object as a JSON
+    
+    Acts as an alias to :func:`print(sc.jsonify(..., tostring=True)) <jsonify>`.
+    
+    Args:
+        obj (any): the object to print
+        indent (int): the level of indent to use 
+        kwargs (dict): passed to :func:`sc.jsonify() <jsonify>`
+    
+    **Example**::
+        
+        data = dict(a=dict(x=[1,2,3], y=[4,5,6]), b=dict(foo='string', bar='other_string'))
+        sc.printjson(data)
+    
+    *New in version 3.0.0.*
+    '''
+    json = jsonify(obj, tostring=True, indent=indent, **kwargs)
+    print(json)
+    return
+
+
+def readjson(string, **kwargs):
+    '''
+    Read JSON from a string
+    
+    Alias to :func:`json.loads()`.
+
+    Args:
+        string (str): a string representation of the JSON
+        kwargs (dict): passed to :func:`json.loads()`
+    
+    See also :func:`sc.loadjson() <loadjson>` for loading a JSON from
+    a file.
+    
+    **Example**::
+        
+        string = '{"this":1, "is":2, "a":3, "JSON":4}'
+        json = sc.readjson(string)
+        
+    *New in version 3.0.0.*
+    '''
+    return json.loads(string, **kwargs)
 
 
 def loadjson(filename=None, folder=None, string=None, fromfile=True, **kwargs):
     '''
     Convenience function for reading a JSON file (or string).
 
     Args:
         filename (str): the file to load, or the JSON object if using positional arguments
         folder (str): folder if not part of the filename
         string (str): if not loading from a file, a string representation of the JSON
         fromfile (bool): whether or not to load from file
-        kwargs (dict): passed to json.load()
+        kwargs (dict): passed to :func:`json.load()`
 
     Returns:
         output (dict): the JSON object
 
     **Examples**::
 
         json = sc.loadjson('my-file.json')
         json = sc.loadjson(string='{"a":null, "b":[1,2,3]}')
+    
+    See also :func:`sc.readjson() <readjson>` for loading a JSON from
+    a string.
     '''
     if string is not None or not fromfile:
-        if string is None and filename is not None:
+        if string is None and filename is not None: # pragma: no cover
             string = filename # Swap arguments
         output = json.loads(string, **kwargs)
     else:
         filepath = makefilepath(filename=filename, folder=folder)
         try:
             with open(filepath) as f:
                 output = json.load(f, **kwargs)
         except FileNotFoundError as E: # pragma: no cover
-            errormsg = f'No such file "{filename}". Use fromfile=False if loading a JSON string rather than a file.'
+            errormsg = f'No such file "{filename}". Use "string" argument or "fromfile=False" if loading a JSON string rather than a file.'
             raise FileNotFoundError(errormsg) from E
     return output
 
 
 def savejson(filename=None, obj=None, folder=None, die=True, indent=2, keepnone=False, sanitizepath=True, **kwargs):
     '''
     Convenience function for saving to a JSON file.
 
     Args:
         filename (str): the file to save
         obj (anything): the object to save; if not already in JSON format, conversion will be attempted
         folder (str): folder if not part of the filename
         die (bool): whether or not to raise an exception if saving an empty object
         indent (int): indentation to use for saved JSON
-        keepnone (bool): allow ``sc.savejson(None)`` to return 'null' rather than raising an exception
+        keepnone (bool): allow :func:`sc.savejson(None) <savejson(None>` to return 'null' rather than raising an exception
         sanitizepath (bool): whether to sanitize the path prior to saving
-        kwargs (dict): passed to ``json.dump()``
+        kwargs (dict): passed to :func:`json.dump()`
 
     Returns:
         The filename saved to
 
     **Example**::
 
         json = {'foo':'bar', 'data':[1,2,3]}
         sc.savejson('my-file.json', json)
+    
+    See also :func:`sc.jsonify() <jsonify>`.
     '''
 
-    filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath)
+    filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath, makedirs=True)
 
     if obj is None and not keepnone: # pragma: no cover
         errormsg = 'No object was supplied to savejson(), or the object was empty'
         if die: raise ValueError(errormsg)
         else:   print(errormsg)
 
     with open(filename, 'w') as f:
         json.dump(sanitizejson(obj), f, indent=indent, **kwargs)
 
     return filename
 
 
+def readyaml(string, **kwargs):
+    '''
+    Read YAML from a string
+    
+    Alias to :func:`sc.loadyaml(string=...) <loadyaml>`.
+
+    Args:
+        string (str): a string representation of the YAML
+        kwargs (dict): passed to :func:`sc.loadyaml() <loadyaml>`
+    
+    See also :func:`sc.loadyaml() <loadyaml>` for loading a YAML from
+    a file.
+    
+    **Example**::
+    
+        string = '{"this":1, "is":2, "a":3, "YAML":4} # YAML allows comments!'
+        yaml = sc.readyaml(string)
+    
+    *New in version 3.0.0.*
+    '''
+    return loadyaml(string=string, **kwargs)
+
+
 def loadyaml(filename=None, folder=None, string=None, fromfile=True, safe=False, loader=None):
     '''
     Convenience function for reading a YAML file (or string).
 
     Args:
         filename (str): the file to load, or the YAML object if using positional arguments
         folder (str): folder if not part of the filename
@@ -1062,15 +1305,15 @@
     '''
     import yaml # Optional import
 
     if loader is None:
         if safe: loader = yaml.loader.SafeLoader
         else:    loader = yaml.loader.UnsafeLoader
 
-    if string is not None or not fromfile:
+    if string is not None or not fromfile: # pragma: no cover
         if string is None and filename is not None:
             string = filename # Swap arguments
         output = yaml.load_all(string, loader)
         output = list(output)
     else:
         filepath = makefilepath(filename=filename, folder=folder)
         try:
@@ -1094,15 +1337,15 @@
 
     Args:
         filename (str): the file to save (if empty, return string representation of the YAML instead)
         obj (anything): the object to save
         folder (str): folder if not part of the filename
         die (bool): whether or not to raise an exception if saving an empty object
         indent (int): indentation to use for saved YAML
-        keepnone (bool): allow ``sc.saveyaml(None)`` to return 'null' rather than raising an exception
+        keepnone (bool): allow :func:`sc.saveyaml(None) <saveyaml>` to return 'null' rather than raising an exception
         dumpall (bool): if True, treat a list input as separate YAML pages
         sanitizepath (bool): whether to sanitize the path prior to saving
         kwargs (dict): passed to ``yaml.dump()``
 
     Returns:
         The filename saved to
 
@@ -1121,21 +1364,21 @@
     if obj is None and not keepnone: # pragma: no cover
         errormsg = 'No object was supplied to saveyaml(), or the object was empty'
         if die: raise ValueError(errormsg)
         else:   print(errormsg)
 
     # Standard usage: dump to file
     if filename is not None:
-        filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath)
+        filename = makefilepath(filename=filename, folder=folder, sanitize=sanitizepath, makedirs=True)
         output = filename
         with open(filename, 'w') as f:
             dump_func(obj, f, **kwargs)
 
     # Alternate usage:
-    else:
+    else: # pragma: no cover
         output = dump_func(obj, **kwargs)
 
     return output
 
 
 def jsonpickle(obj, tostring=False):
     '''
@@ -1248,35 +1491,35 @@
         if isinstance(source, Path):  # If it's a path object, convert to string
             source = str(source)
 
         if source is None:
             if self.bytes is not None:
                 self.blob = read_bin(self.bytes)
                 self.bytes = None # Once read in, delete
-            else:
+            else: # pragma: no cover
                 if self.filename is not None:
                     self.blob = read_file(self.filename)
                 else:
                     print('Nothing to load: no source or filename supplied and self.bytes is empty.')
         else:
             if isinstance(source,io.BytesIO):
                 self.blob = read_bin(source)
             elif scu.isstring(source):
                 self.blob = read_file(source)
-            else:
+            else: # pragma: no cover
                 errormsg = f'Input source must be type string (for a filename) or BytesIO, not {type(source)}'
                 raise TypeError(errormsg)
 
         self.modified = scd.now()
         return
 
 
     def save(self, filename=None):
         ''' This function writes the spreadsheet to a file on disk. '''
-        filepath = makefilepath(filename=filename)
+        filepath = makefilepath(filename=filename, makedirs=True)
         with open(filepath, mode='wb') as f:
             f.write(self.blob)
         self.filename = filename
         print(f'Object saved to {filepath}.')
         return filepath
 
 
@@ -1305,29 +1548,29 @@
 
 
 class Spreadsheet(Blobject):
     '''
     A class for reading and writing Excel files in binary format. No disk IO needs
     to happen to manipulate the spreadsheets with openpyxl (or xlrd or pandas).
 
-    New in version 1.3.0: Changed default from xlrd to openpyxl and added self.wb
+    *New version 1.3.0:* Changed default from xlrd to openpyxl and added self.wb
     attribute to avoid the need to reload workbooks.
 
     **Examples**::
 
 
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.wb = None
         return
 
 
-    def __getstate__(self):
+    def __getstate__(self): # pragma: no cover
         d = self.__dict__.copy() # Shallow copy
         d['wb'] = None
         return d
 
 
     def _reload_wb(self, reload=None):
         ''' Helper function to check if workbook is already loaded '''
@@ -1371,15 +1614,15 @@
             wb = self.wb
 
         if store:
             self.wb = wb
         return wb
 
 
-    def openpyexcel(self, *args, **kwargs):
+    def openpyexcel(self, *args, **kwargs): # pragma: no cover
         ''' Legacy name for openpyxl() '''
         warnmsg = '''
 Spreadsheet() no longer supports openpyexcel as of v1.3.1. To load using it anyway, you can manually do:
 
     %pip install openpyexcel
     import openpyexcel
     spreadsheet = sc.Spreadsheet()
@@ -1458,15 +1701,15 @@
         if cells is None:  # If no cells specified, return the whole sheet.
             return sheetoutput
         else:
             results = []
             for cell in cells:  # Loop over all cells
                 rownum = cell[0]
                 colnum = cell[1]
-                if method in ['xlrd']:  # If we're using xlrd/pandas, reduce the row number by 1.
+                if method in ['xlrd']:  # If we're using xlrd/pandas, reduce the row number by 1 # pragma: no cover
                     rownum -= 1
                 results.append(sheetoutput[rownum][colnum])  # Grab and append the result at the cell.
             return results
 
 
     def writecells(self, cells=None, startrow=None, startcol=None, vals=None, sheetname=None, sheetnum=None, verbose=False, wbargs=None):
         '''
@@ -1504,23 +1747,23 @@
                         cellobj = ws[cell]
                     elif scu.checktype(cell, 'arraylike','number') and len(cell)==2: # Handles e.g. cell=(0,0)
                         cellobj = ws.cell(row=cell[0], column=cell[1])
                     else: # pragma: no cover
                         errormsg = f'Cell must be formatted as a label or row-column pair, e.g. "A1" or (3,5); not "{cell}"'
                         raise TypeError(errormsg)
                     if verbose: print(f'  Cell {cell} = {val}')
-                    if isinstance(val,tuple):
+                    if isinstance(val, tuple): # pragma: no cover
                         cellobj.value = val[0]
                         cellobj.cached_value = val[1]
                     else:
                         cellobj.value = val
                 except Exception as E: # pragma: no cover
                     errormsg = f'Could not write "{val}" to cell "{cell}": {repr(E)}'
                     raise RuntimeError(errormsg)
-        else:# Cells aren't supplied, assume a matrix
+        else: # Cells aren't supplied, assume a matrix
             if startrow is None: startrow = 1 # Excel uses 1-based indexing
             if startcol is None: startcol = 1
             valarray = np.atleast_2d(np.array(vals, dtype=object))
             for i,rowvals in enumerate(valarray):
                 row = startrow + i
                 for j,val in enumerate(rowvals):
                     col = startcol + j
@@ -1536,24 +1779,24 @@
         wb.save(self.freshbytes())
         self.load()
 
         return
 
 
     def save(self, filename='spreadsheet.xlsx'):
-        filepath = makefilepath(filename=filename, ext='xlsx')
+        filepath = makefilepath(filename=filename, ext='xlsx', makedirs=True)
         Blobject.save(self, filepath)
 
 
 
 def loadspreadsheet(filename=None, folder=None, fileobj=None, sheet=0, header=1, asdataframe=None, method='pandas', **kwargs):
     '''
     Load a spreadsheet as a dataframe or a list of lists.
 
-    By default, an alias to ``pandas.read_excel()`` with a header, but also supports loading
+    By default, an alias to :func:`pandas.read_excel()` with a header, but also supports loading
     via openpyxl or xlrd. Read from either a filename or a file object.
 
     Args:
         filename (str): filename or path to read
         folder (str): optional folder to use with the filename
         fileobj (obj): load from file object rather than path
         sheet (str/int/list): name or number of sheet(s) to use (default 0)
@@ -1564,15 +1807,15 @@
 
     **Examples**::
 
         df = sc.loadspreadsheet('myfile.xlsx') # Alias to pd.read_excel(header=1)
         wb = sc.loadspreadsheet('myfile.xlsx', method='openpyxl') # Returns workbook
         data = sc.loadspreadsheet('myfile.xlsx', method='xlrd', asdataframe=False) # Returns raw data; requires xlrd
 
-    New in version 1.3.0: change default from xlrd to pandas; renamed sheetname and sheetnum arguments to sheet.
+    *New version 1.3.0:* change default from xlrd to pandas; renamed sheetname and sheetnum arguments to sheet.
     '''
 
     # Handle path and sheet name/number
     fullpath = makefilepath(filename=filename, folder=folder)
     for key in ['sheetname', 'sheetnum', 'sheet_name']:
         sheet = kwargs.pop('sheetname', sheet)
 
@@ -1716,55 +1959,55 @@
         testdata5[0,:] = ['A', 'B', 'C'] # Create header
         testdata5[1:,:] = np.random.rand(nrows,ncols) # Create data
         formatdata[1:,:] = 'plain' # Format data
         formatdata[testdata5>0.7] = 'big' # Find "big" numbers and format them differently
         formatdata[0,:] = 'header' # Format header
         sc.savespreadsheet(filename='test5.xlsx', data=testdata5, formats=formats, formatdata=formatdata)
 
-    New in version 2.0.0: allow arguments to be passed to the ``Workbook``.
+    *New version 2.0.0:* allow arguments to be passed to the ``Workbook``.
     '''
     workbook_args = scu.mergedicts({'nan_inf_to_errors': True}, workbook_args)
     try:
         import xlsxwriter # Optional import
     except ModuleNotFoundError as e: # pragma: no cover
         raise ModuleNotFoundError('The "xlsxwriter" Python package is not available; please install manually') from e
-    fullpath = makefilepath(filename=filename, folder=folder, default='default.xlsx')
+    fullpath = makefilepath(filename=filename, folder=folder, default='default.xlsx', makedirs=True)
     datadict   = sco.odict()
     formatdict = sco.odict()
     hasformats = (formats is not None) and (formatdata is not None)
 
     # Handle input arguments
-    if isinstance(data, dict) and sheetnames is None:
+    if isinstance(data, dict) and sheetnames is None: # pragma: no cover
         if verbose: print('Data is a dict, taking sheetnames from keys')
         sheetnames = data.keys()
         datadict   = sco.odict(data) # Use directly, converting to odict first
         if hasformats: formatdict = sco.odict(formatdata) #  NB, might be None but should be ok
-    elif isinstance(data, dict) and sheetnames is not None:
+    elif isinstance(data, dict) and sheetnames is not None: # pragma: no cover
         if verbose: print('Data is a dict, taking sheetnames from input')
         if len(sheetnames) != len(data):
             errormsg = f'If supplying data as a dict as well as sheetnames, length must match ({len(data)} vs {len(sheetnames)})'
             raise ValueError(errormsg)
         datadict   = sco.odict(data) # Use directly, but keep original sheet names
         if hasformats: formatdict = sco.odict(formatdata)
     elif not isinstance(data, dict):
         if sheetnames is None:
             if verbose: print('Data is a simple array')
             sheetnames = ['Sheet1']
             datadict[sheetnames[0]]   = data # Set it explicitly
             formatdict[sheetnames[0]] = formatdata # Set it explicitly -- NB, might be None but should be ok
-        else:
+        else: # pragma: no cover
             if verbose: print('Data is a list, taking matching sheetnames from inputs')
             if len(sheetnames) == len(data):
                 for s,sheetname in enumerate(sheetnames):
                     datadict[sheetname] = data[s] # Assume there's a 1-to-1 mapping
                     if hasformats: formatdict[sheetname] = formatdata[s]
             else:
                 errormsg = f'Unable to figure out how to match {len(sheetnames)} sheet names with data of length {len(data)}'
                 raise ValueError(errormsg)
-    else:
+    else: # pragma: no cover
         errormsg = f'Cannot figure out how to handle data of type: {type(data)}'
         raise TypeError(errormsg) # This shouldn't happen!
 
     # Create workbook
     if verbose: print(f'Creating file {fullpath}')
     workbook = xlsxwriter.Workbook(fullpath, workbook_args)
 
@@ -1798,15 +2041,15 @@
                     raise RuntimeError(errormsg)
 
     # Either close the workbook and write to file, or return it for further working
     if close:
         if verbose: print(f'Saving file {filename} and closing')
         workbook.close()
         return fullpath
-    else:
+    else: # pragma: no cover
         if verbose: print('Returning workbook')
         return workbook
 
 
 
 ##############################################################################
 #%% Pickling support methods
@@ -1818,38 +2061,38 @@
 class Failed(object):
     ''' An empty class to represent a failed object loading '''
     failure_info = sco.odict()
 
     def __init__(self, *args, **kwargs):
         pass
 
-    def __repr__(self):
+    def __repr__(self): # pragma: no cover
         output = scp.objrepr(self) # This does not include failure_info since it's a class attribute
         output += self.showfailures(verbose=False, tostring=True)
         return output
 
     def showfailures(self, verbose=True, tostring=False):
         output = ''
         for f,failure in self.failure_info.enumvals():
             output += f'\nFailure {f+1} of {len(self.failure_info)}:\n'
             output += f'Module: {failure["module"]}\n'
             output += f'Class: {failure["class"]}\n'
             output += f'Error: {failure["error"]}\n'
-            if verbose:
+            if verbose: # pragma: no cover
                 output += '\nTraceback:\n'
-                output += failure['exception']
+                output += f"\n{failure['exception']}"
                 output += '\n\n'
-        if tostring:
+        if tostring: # pragma: no cover
             return output
         else:
             print(output)
             return
 
 
-class Empty(object):
+class Empty(object): # pragma: no cover
     ''' Another empty class to represent a failed object loading, but do not proceed with setstate '''
 
     def __init__(self, *args, **kwargs):
         pass
 
     def __setstate__(self, state):
         pass
@@ -1874,117 +2117,150 @@
         return
 
     def __repr__(self):
         output = scp.objrepr(self) # This does not include failure_info since it's a class attribute
         return output
 
     def __setstate__(self, state):
-        self.__set_empty()
-        self.state = state
+        try:
+            self.__dict__.update(state) # NB, does not support slots
+        except:
+            self.__set_empty()
+            self.state = state
         return
 
     def __len__(self):
         return len(self.dict)
 
     def __getitem__(self, key):
         return self.dict[key]
 
     def __setitem__(self, key, value):
         self.dict[key] = value
         return
 
     def disp(self, *args, **kwargs):
-        return scu.pr(self, *args, **kwargs)
+        return scp.pr(self, *args, **kwargs)
 
 
 def makefailed(module_name=None, name=None, error=None, exception=None, universal=False):
     ''' Create a class -- not an object! -- that contains the failure info for a pickle that failed to load '''
     base = UniversalFailed if universal else Failed
     key = f'Failure {len(base.failure_info)+1}'
     base.failure_info[key] = sco.odict()
     base.failure_info[key]['module']    = module_name
     base.failure_info[key]['class']     = name
     base.failure_info[key]['error']     = error
     base.failure_info[key]['exception'] = exception
     return base
 
 
-class _RobustUnpickler(pkl.Unpickler):
+def _remap_module(remapping, module_name, name):
+    ''' Use a remapping dictionary to try to load a module from a different location ''' 
+    key = f'{module_name}.{name}'
+    obj = remapping.get(key) # If the user has supplied the module directly
+    if isinstance(obj, str): # Split a string into a tuple, e.g. 'foo.bar.Cat' to ('foo.bar', 'Cat')
+        obj = tuple(obj.rsplit('.', 1))
+    if obj is None or (isinstance(obj, tuple) and len(obj)==2): # Either it's not in the remapping, or it's a tuple
+        if obj is None: # Key not in remapping, just use regular
+            load_module = module_name
+            load_name = name
+        else: # It's a tuple of names, process # pragma: no cover
+            load_module = obj[0]
+            load_name = obj[1]
+        module = importlib.import_module(load_module)
+        obj = getattr(module, load_name) # pragma: no cover
+    return obj
+
+
+class _RobustUnpickler(dill.Unpickler):
     ''' Try to import an object, and if that fails, return a Failed object rather than crashing '''
 
     def __init__(self, bytesio, fix_imports=True, encoding="latin1", errors="ignore", remapping=None):
-        pkl.Unpickler.__init__(self, bytesio, fix_imports=fix_imports, encoding=encoding, errors=errors)
-        self.remapping = remapping if remapping is not None else {}
+        super().__init__(bytesio, fix_imports=fix_imports, encoding=encoding, errors=errors)
+        self.remapping = scu.mergedicts(remapping)
         return
 
     def find_class(self, module_name, name, verbose=True):
-        key = f'{module_name}.{name}'
-        obj = self.remapping.get(key) # If the user has supplied the module directly
-        if obj is None or (isinstance(obj, tuple) and len(obj)==2): # Either it's not in the remapping, or it's a tuple
-            try:
-                if obj is None: # Key not in remapping
-                    load_module = module_name
-                    load_name = name
-                else: # It's a tuple of names, process
-                    load_module = obj[0]
-                    load_name = obj[1]
-                module = importlib.import_module(load_module)
-                obj = getattr(module, load_name)
-            except Exception as E:
-                if verbose: print(f'Unpickling warning: could not import {load_module}.{load_name}: {str(E)}')
-                exception = traceback.format_exc() # Grab the trackback stack
-                obj = makefailed(module_name=module_name, name=name, error=E, exception=exception)
+        obj = _remap_module(self.remapping, module_name, name)
         return obj
 
 
-class _UltraRobustUnpickler(pkl.Unpickler): # pragma: no cover
+class _UltraRobustUnpickler(dill.Unpickler): # pragma: no cover
     ''' If all else fails, just make a default object '''
 
-    def __init__(self, bytesio, *args, unpicklingerrors=None, **kwargs):
-        pkl.Unpickler.__init__(self, bytesio, *args, **kwargs)
+    def __init__(self, bytesio, *args, fix_imports=True, encoding="latin1", errors="ignore", 
+                 remapping=None, unpicklingerrors=None):
+        super().__init__(bytesio, fix_imports=fix_imports, encoding=encoding, errors=errors)
+        self.remapping = scu.mergedicts(remapping)
         self.unpicklingerrors = unpicklingerrors if unpicklingerrors is not None else []
         return
 
     def find_class(self, module_name, name):
         ''' Ignore all attempts to use the actual class and always make a UniversalFailed class '''
-        error = scu.strjoin(self.unpicklingerrors)
-        exception = self.unpicklingerrors
-        obj = makefailed(module_name=module_name, name=name, error=error, exception=exception, universal=True)
+        try:
+            obj = _remap_module(self.remapping, module_name, name)
+        except:
+            error = scu.strjoin(self.unpicklingerrors)
+            exception = self.unpicklingerrors
+            obj = makefailed(module_name=module_name, name=name, error=error, exception=exception, universal=True)
         return obj
 
 
-def _unpickler(string=None, filename=None, filestring=None, die=None, verbose=False, remapping=None, method='pickle', **kwargs):
+def _unpickler(string=None, filename=None, filestring=None, die=None, verbose=False, remapping=None, method='pickle', auto_remap=True, **kwargs):
     ''' Not invoked directly; used as a helper function for saveobj/loadobj '''
+    
+    # Sanitize kwargs, since wrapped in try-except statements otherwise
+    if kwargs: # pragma: no cover
+        valid_kwargs = ['fix_imports', 'encoding', 'errors', 'buffers', 'ignore']
+        for k in kwargs:
+            if k not in valid_kwargs:
+                errormsg = f'Keyword "{k}" is not a valid keyword: {scu.strjoin(valid_kwargs)}'
+                raise ValueError(errormsg)
 
     if die is None: die = False
     try: # Try pickle first
         if method == 'pickle':
             obj = pkl.loads(string, **kwargs) # Actually load it -- main usage case
         elif method == 'dill':
-            import dill # Optional Sciris dependency
             obj = dill.loads(string, **kwargs) # Actually load it, with dill
-        else:
+        else: # pragma: no cover
             errormsg = f'Method "{method}" not recognized, must be pickle or dill'
             raise ValueError(errormsg)
     except Exception as E1:
-        if die:
+        if die: # pragma: no cover
             raise E1
         else:
             try:
                 if verbose: print(f'Standard unpickling failed ({str(E1)}), trying encoding...')
                 obj = pkl.loads(string, encoding='latin1', **kwargs) # Try loading it again with different encoding
             except Exception as E2:
                 try:
                     if verbose: print(f'Encoded unpickling failed ({str(E2)}), trying dill...')
                     import dill # Optional Sciris dependency
                     obj = dill.loads(string, **kwargs) # If that fails, try dill
                 except Exception as E3:
                     try:
-                        if verbose: print(f'Dill failed ({str(E3)}), trying robust unpickler...')
-                        obj = _RobustUnpickler(io.BytesIO(string), remapping=remapping).load() # And if that fails, throw everything at it
+                        if verbose: print(f'Dill failed ({str(E3)}), trying robust unpickler with remapping...')
+                        loaded = False
+                        while not loaded:
+                            try:
+                                obj = _RobustUnpickler(io.BytesIO(string), remapping=remapping).load() # And if that fails, throw everything at it
+                                loaded = True
+                            except Exception as E3b:
+                                from . import sc_versioning as scv # Here to avoid circular import
+                                remapping = scu.mergedicts(remapping)
+                                known = scv.known_deprecations()
+                                errstr = str(E3b)
+                                if errstr in known and auto_remap: # pragma: no cover
+                                    remapping.update(known[errstr]['fix'])
+                                    warnmsg = f'Fixing known unpickling deprecation "{errstr}"'
+                                    warnings.warn(warnmsg, category=UserWarning, stacklevel=2)
+                                else:
+                                    raise E3b
                     except Exception as E4:
                         try:
                             if verbose: print(f'Robust failed ({str(E4)}), trying ultrarobust unpickler...')
                             obj = _UltraRobustUnpickler(io.BytesIO(string), unpicklingerrors=[E1, E2, E3, E4]).load() # And if that fails, really throw everything at it
                         except Exception as E5: # pragma: no cover
                             errormsg = f'''
 All available unpickling methods failed:
@@ -1998,23 +2274,19 @@
     if isinstance(obj, Failed):
         print('Warning, the following errors were encountered during unpickling:')
         obj.showfailures(verbose=False)
 
     return obj
 
 
-def _savepickle(fileobj=None, obj=None, protocol=None, *args, **kwargs):
+def _savepickle(fileobj=None, obj=None, protocol=None, **kwargs):
         ''' Use pickle to do the salty work. '''
         if protocol is None:
             protocol = 4 # Use protocol 4 for backwards compatibility
-        fileobj.write(pkl.dumps(obj, protocol=protocol, *args, **kwargs))
+        fileobj.write(pkl.dumps(obj, protocol=protocol, **kwargs))
         return
 
 
-def _savedill(fileobj=None, obj=None, *args, **kwargs): # pragma: no cover
+def _savedill(fileobj=None, obj=None, **kwargs): # pragma: no cover
     ''' Use dill to do the sour work (note: this function is not actively maintained) '''
-    try:
-        import dill # Optional Sciris dependency
-    except ModuleNotFoundError as e:
-        raise ModuleNotFoundError('The "dill" Python package is not available; please install manually') from e
-    fileobj.write(dill.dumps(obj, protocol=-1, *args, **kwargs))
+    fileobj.write(dill.dumps(obj, protocol=-1, **kwargs))
     return
```

### Comparing `sciris-2.1.0/sciris/sc_legacy.py` & `sciris-3.0.0/sciris/_extras/legacy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 '''
-Legacy methods for handling old pickles (eg Python 2 pickles). Included for backwards
-compatibility, but not imported into Sciris by default.
+This is the graveyard for old Sciris functions that are no longer used. It is preserved
+for backwards compatibility, but is not imported into Sciris by default.
 '''
 
 import types
+import warnings
+import textwrap
 import traceback
 import gzip as gz
 import numpy as np
 import pickle as pkl
 import datetime as dt
 import copyreg as cpreg
+import multiprocess as mp
 from io import BytesIO as IO
+from functools import partial
 from contextlib import closing
-from . import sc_fileio as scf
-from . import sc_utils as scu
-from . import sc_odict as sco
+from .. import sc_utils as scu
+from .. import sc_odict as sco
+from .. import sc_fileio as scf
+from .. import sc_profiling as scp
 
 
 ##############################################################################
 #%% Python 2 legacy support
 ##############################################################################
 
 not_string_pickleable = ['datetime', 'BytesIO']
@@ -240,15 +245,15 @@
 class legacy_dataframe(object): # pragma: no cover
     '''
     This legacy dataframe is maintained solely to allow loading old files.
 
     **Example**::
 
         import sciris as sc
-        from sciris import sc_legacy as scl
+        from sciris.extras import legacy as scl
         remapping = {'sciris.sc_dataframe.dataframe':scl.legacy_dataframe}
         old = sc.load('my-old-file.obj', remapping=remapping)
 
     | Version: 2020nov29
     | Migrated to ``sc_legacy`` in version 2.0.0.
     '''
 
@@ -387,8 +392,174 @@
         else:
             errormsg = 'Number of columns (%s) does not match array shape (%s)' % (len(cols), data.shape)
             raise Exception(errormsg)
 
         # Store it
         self.cols = list(cols)
         self.data = data
-        return
+        return
+    
+
+
+##############################################################################
+#%% Parallelization
+##############################################################################
+
+
+def parallelcmd(cmd=None, parfor=None, returnval=None, maxcpu=None, maxmem=None, interval=None, die=True, **kwargs):
+    '''
+    A function to parallelize any block of code. Note: this is intended for quick
+    prototyping only; since it uses exec(), it is not recommended for use in production
+    code.
+
+    Args:
+        cmd       (str):   a string representation of the code to be run in parallel
+        parfor    (dict):  a dictionary of lists of the variables to loop over
+        returnval (str):   the name of the output variable
+        maxcpu    (float): maximum CPU load; used by ``sc.loadbalancer()``
+        maxmem    (float): maximum fraction of virtual memory (RAM); used by ``sc.loadbalancer()``
+        interval  (float): the time delay to poll to see if load is OK,  used in ``sc.loadbalancer()``
+        die       (bool):  whether to stop immediately if an exception is encountered (otherwise, store the exception as the result)
+        kwargs    (dict):  variables to pass into the code
+
+    **Example**::
+
+        const = 4
+        parfor = {'val':[3,5,9]}
+        returnval = 'result'
+        cmd = """
+        newval = val+const
+        result = newval**2
+        """
+        results = sc.parallelcmd(cmd=cmd, parfor=parfor, returnval=returnval, const=const)
+
+    | New in version 2.0.0: replaced ``maxload`` with ``maxcpu``/``maxmem``; automatically de-indent the command
+    | Migrated to ``sc_legacy`` in version 2.2.0.
+    '''
+
+    # Handle maxload
+    maxload = kwargs.pop('maxload', None)
+    if maxload is not None: # pragma: no cover
+        maxcpu = maxload
+        warnmsg = 'sc.loadbalancer() argument "maxload" has been renamed "maxcpu" as of v2.0.0'
+        warnings.warn(warnmsg, category=FutureWarning, stacklevel=2)
+
+    # Deindent the command
+    cmd = textwrap.dedent(cmd)
+
+    # Create queue
+    nfor = len(list(parfor.values())[0])
+    outputqueue = mp.Queue()
+    outputlist = np.empty(nfor, dtype=object)
+    processes = []
+    for i in range(nfor):
+        args = (cmd, parfor, returnval, i, outputqueue, maxcpu, maxmem, interval, die, kwargs)
+        prc = mp.Process(target=_parallelcmd_task, args=args)
+        prc.start()
+        processes.append(prc)
+    for i in range(nfor):
+        _i,returnval = outputqueue.get()
+        outputlist[_i] = returnval
+    for prc in processes:
+        prc.join() # Wait for them to finish
+
+    outputlist = outputlist.tolist()
+
+    return outputlist
+
+
+def parallel_progress(fcn, inputs, num_workers=None, show_progress=True, initializer=None): # pragma: no cover
+    """
+    Run a function in parallel with a optional single progress bar
+
+    The result is essentially equivalent to::
+
+        >>> list(map(fcn, inputs))
+
+    But with execution in parallel and with a single progress bar being shown.
+
+    Args:
+        fcn (function): Function object to call, accepting one argument, OR a function with zero arguments in which case inputs should be an integer
+        inputs (list): A collection of inputs that will each be passed to the function OR a number, if the fcn() has no input arguments
+        num_workers (int): Number of processes, defaults to the number of CPUs
+        show_progress (bool): Whether to show a progress bar
+        initializer (func): A function that each worker process will call when it starts
+
+    Returns:
+        A list of outputs
+
+    | New in version 1.0.0.
+    | Migrated to ``sc_legacy`` in version 2.2.0.
+    """
+    try:
+        from tqdm import tqdm
+    except ModuleNotFoundError as E:
+        errormsg = 'Module tqdm not found; please install with "pip install tqdm"'
+        raise ModuleNotFoundError(errormsg) from E
+
+    pool = mp.Pool(num_workers, initializer=initializer)
+
+    results = [None]
+    if scu.isnumber(inputs):
+        results *= inputs
+        pbar = tqdm(total=inputs) if show_progress else None
+    else:
+        results *= len(inputs)
+        pbar = tqdm(total=len(inputs)) if show_progress else None
+
+    def callback(result, idx):
+        results[idx] = result
+        if show_progress:
+            pbar.update(1)
+
+    if scu.isnumber(inputs):
+        for i in range(inputs):
+            pool.apply_async(fcn, callback=partial(callback, idx=i))
+    else:
+        for i, x in enumerate(inputs):
+            pool.apply_async(fcn, args=(x,), callback=partial(callback, idx=i))
+
+    pool.close()
+    pool.join()
+
+    if show_progress:
+        pbar.close()
+
+    return results
+
+
+def _parallelcmd_task(_cmd, _parfor, _returnval, _i, _outputqueue, _maxcpu, _maxmem, _interval, _die, _kwargs): # pragma: no cover # No coverage since pickled
+    '''
+    The task to be executed by ``sc.parallelcmd()``. All internal variables start with
+    underscores to avoid possible collisions in the ``exec()`` statements. Not to be called
+    directly.
+    
+    Migrated to ``sc_legacy`` in version 2.2.0.
+    '''
+    if _maxcpu or _maxmem:
+        scp.loadbalancer(maxcpu=_maxcpu, maxmem=_maxmem, index=_i, interval=_interval)
+
+    # Set the loop variables
+    for _key in _parfor.keys():
+        _thisval = _parfor[_key][_i] # analysis:ignore
+        exec(f'{_key} = _thisval') # Set the value of this variable
+
+    # Set the keyword arguments
+    for _key in _kwargs.keys():
+        _thisval = _kwargs[_key] # analysis:ignore
+        exec(f'{_key} = _thisval') # Set the value of this variable
+
+    # Run the command
+    try:
+        exec(_cmd) # The meat of the matter!
+    except Exception:
+        if _die:
+            raise Exception
+        else:
+            warnmsg = f'sc.parallelcmd(): Task {_i} failed, but die=False so continuing.\n{scu.traceback()}'
+            warnings.warn(warnmsg, category=RuntimeWarning, stacklevel=2)
+            exec(f'{_returnval} = None')
+
+    # Append results
+    _outputqueue.put((_i,eval(_returnval)))
+
+    return
```

### Comparing `sciris-2.1.0/sciris/sc_math.py` & `sciris-3.0.0/sciris/sc_math.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 '''
 Extensions to Numpy, including finding array elements and smoothing data.
 
 Highlights:
-    - :func:`findinds`: find indices of an array matching a condition
-    - :func:`findnearest`: find nearest matching value
-    - :func:`rolling`: calculate rolling average
-    - :func:`smooth`: simple smoothing of 1D or 2D arrays
+    - :func:`sc.findinds() <findinds>`: find indices of an array matching a condition
+    - :func:`sc.findnearest() <findnearest>`: find nearest matching value
+    - :func:`sc.rolling() <rolling>`: calculate rolling average
+    - :func:`sc.smooth() <smooth>`: simple smoothing of 1D or 2D arrays
 '''
 
 import numpy as np
 import pandas as pd
 import warnings
 from . import sc_utils as scu
 from . import sc_odict as sco
 
 
 ##############################################################################
 #%% Find and approximation functions
 ##############################################################################
 
 __all__ = ['approx', 'safedivide', 'findinds', 'findfirst', 'findlast', 'findnearest', 'count',
-           'dataindex', 'getvalidinds', 'sanitize', 'rmnans','fillnans', 'getvaliddata', 'isprime', 'numdigits']
+           'dataindex', 'getvalidinds', 'sanitize', 'rmnans','fillnans', 'findnans', 'getvaliddata',
+           'isprime', 'numdigits']
 
 
 def approx(val1=None, val2=None, eps=None, **kwargs):
     '''
     Determine whether two scalars (or an array and a scalar) approximately match.
     Alias for np.isclose() and may be removed in future versions.
 
@@ -65,15 +66,15 @@
     if isinstance(denominator, list): denominator = np.array(denominator)
 
     # Handle the logic
     invalid = approx(denominator, 0.0, eps=eps)
     if scu.isnumber(denominator): # The denominator is a scalar
         if invalid:
             output = default
-        else:
+        else: # pragma: no cover
             output = numerator/denominator
     elif scu.checktype(denominator, 'array'):
         if not warn:
             denominator[invalid] = 1.0 # Replace invalid values with 1
         output = numerator/denominator
         output[invalid] = default
     else: # pragma: no cover # Unclear input, raise exception
@@ -86,38 +87,39 @@
 def findinds(arr=None, val=None, *args, eps=1e-6, first=False, last=False, ind=None, die=True, **kwargs):
     '''
     Find matches even if two things aren't eactly equal (e.g. floats vs. ints).
 
     If one argument, find nonzero values. With two arguments, check for equality
     using eps (by default 1e-6, to handle single-precision floating point). Returns 
     a tuple of arrays if val1 is multidimensional, else returns an array. Similar 
-    to calling ``np.nonzero(np.isclose(arr, val))[0]``.
+    to calling :func:`np.nonzero(np.isclose(arr, val))[0] <numpy.nonzero>`.
 
     Args:
         arr    (array): the array to find values in
         val    (float): if provided, the value to match
         args   (list):  if provided, additional boolean arrays
-        eps    (float): the precision for matching (default 1e-6, equivalent to ``np.isclose()``'s atol)
+        eps    (float): the precision for matching (default 1e-6, equivalent to :func:`numpy.isclose`'s atol)
         first  (bool):  whether to return the first matching value (equivalent to ind=0)
         last   (bool):  whether to return the last matching value (equivalent to ind=-1)
         ind    (int):   index of match to retrieve
         die    (bool):  whether to raise an exception if first or last is true and no matches were found
-        kwargs (dict):  passed to ``np.isclose()``
+        kwargs (dict):  passed to :func:`numpy.isclose()`
 
     **Examples**::
 
         data = np.random.rand(10)
         sc.findinds(data<0.5) # Standard usage; returns e.g. array([2, 4, 5, 9])
         sc.findinds(data>0.1, data<0.5) # Multiple arguments
 
         sc.findinds([2,3,6,3], 3) # Returs array([1,3])
         sc.findinds([2,3,6,3], 3, first=True) # Returns 1
 
-    | New in version 1.2.3: "die" argument
-    | New in version 2.0.0: fix string matching; allow multiple arguments
+    | *New in version 1.2.3:* "die" argument
+    | *New in version 2.0.0:* fix string matching; allow multiple arguments
+    | *New in version 3.0.0:* multidimensional arrays now return a list of tuples
     '''
 
     # Handle first or last
     if first and last: raise ValueError('Can use first or last but not both')
     elif first: ind = 0
     elif last:  ind = -1
 
@@ -161,49 +163,51 @@
     try:
         if arr.ndim == 1: # Uni-dimensional
             output = output[0] # Return an array rather than a tuple of arrays if one-dimensional
             if ind is not None:
                 output = output[ind] # And get the first element
         else:
             if ind is not None:
-                output = [output[i][ind] for i in range(arr.ndim)]
+                output = tuple([output[i][ind] for i in range(arr.ndim)])
     except IndexError as E:
         if die:
             errormsg = 'No matching values found; use die=False to return None instead of raising an exception'
             raise IndexError(errormsg) from E
         else:
             output = None
 
     return output
 
 
 def findfirst(*args, **kwargs):
-    ''' Alias for findinds(..., first=True). New in version 1.0.0. '''
+    ''' Alias for findinds(..., first=True). *New in version 1.0.0.* '''
     return findinds(*args, **kwargs, first=True)
 
 
 def findlast(*args, **kwargs):
-    ''' Alias for findinds(..., last=True). New in version 1.0.0. '''
+    ''' Alias for findinds(..., last=True). *New in version 1.0.0.* '''
     return findinds(*args, **kwargs, last=True)
 
 
 def findnearest(series=None, value=None):
     '''
     Return the index of the nearest match in series to value -- like findinds, but
     always returns an object with the same type as value (i.e. findnearest with
     a number returns a number, findnearest with an array returns an array).
+    
+    Args:
+        series (array): the array of numbers to look for nearest matches in
+        value (scalar or array): the number or numbers to compare against
 
     **Examples**::
 
-        findnearest(rand(10), 0.5) # returns whichever index is closest to 0.5
-        findnearest([2,3,6,3], 6) # returns 2
-        findnearest([2,3,6,3], 6) # returns 2
-        findnearest([0,2,4,6,8,10], [3, 4, 5]) # returns array([1, 2, 2])
-
-    Version: 2017jan07
+        sc.findnearest(rand(10), 0.5) # returns whichever index is closest to 0.5
+        sc.findnearest([2,3,6,3], 6) # returns 2
+        sc.findnearest([2,3,6,3], 6) # returns 2
+        sc.findnearest([0,2,4,6,8,10], [3, 4, 5]) # returns array([1, 2, 2])
     '''
     series = scu.toarray(series)
     if scu.isnumber(value):
         output = np.argmin(abs(series-value))
     else:
         output = []
         for val in value: output.append(findnearest(series, val))
@@ -211,29 +215,29 @@
     return output
 
 
 def count(arr=None, val=None, eps=1e-6, **kwargs):
     '''
     Count the number of matching elements.
 
-    Similar to ``np.count_nonzero()``, but allows for slight mismatches (e.g.,
+    Similar to :func:`numpy.count_nonzero()`, but allows for slight mismatches (e.g.,
     floats vs. ints). Equivalent to ``len(sc.findinds())``.
 
     Args:
         arr (array): the array to find values in
         val (float): if provided, the value to match
-        eps (float): the precision for matching (default 1e-6, equivalent to np.isclose's atol)
-        kwargs (dict): passed to ``np.isclose()``
+        eps (float): the precision for matching (default 1e-6, equivalent to :func:`numpy.isclose`'s atol)
+        kwargs (dict): passed to :func:`numpy.isclose()` 
 
     **Examples**::
 
         sc.count(rand(10)<0.5) # returns e.g. 4
-        sc.count([2,3,6,3], 3) # returs 2
+        sc.count([2,3,6,3], 3) # returns 2
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     '''
     output = len(findinds(arr=arr, val=val, eps=eps, **kwargs))
     return output
 
 
 
 def dataindex(dataarray, index): # pragma: no cover
@@ -298,15 +302,15 @@
     else:
         validdata = np.array([]) # No valid data, return an empty array
     return validdata
 
 
 def sanitize(data=None, returninds=False, replacenans=None, defaultval=None, die=True, verbose=False, label=None):
         '''
-        Sanitize input to remove NaNs. (NB: ``sc.sanitize()`` and ``sc.rmnans()`` are aliases.)
+        Sanitize input to remove NaNs. (NB: :func:`sc.sanitize() <sanitize>` and :func:`sc.rmnans() <rmnans>` are aliases.)
 
         Returns an array with the sanitized data. If ``replacenans=True``, the sanitized
         array is of the same length/size as data. If ``replacenans=False``, the sanitized
         array may be shorter than data.
 
         Args:
             data        (arr/list)   : array or list with numbers to be sanitized
@@ -322,18 +326,19 @@
             data = [3, 4, np.nan, 8, 2, np.nan, np.nan, 8]
             sanitized1, inds = sc.sanitize(data, returninds=True) # Remove NaNs
             sanitized2 = sc.sanitize(data, replacenans=True) # Replace NaNs using nearest neighbor interpolation
             sanitized3 = sc.sanitize(data, replacenans='nearest') # Eequivalent to replacenans=True
             sanitized4 = sc.sanitize(data, replacenans='linear') # Replace NaNs using linear interpolation
             sanitized5 = sc.sanitize(data, replacenans=0) # Replace NaNs with 0
 
-        New in version 2.0.0: handle multidimensional arrays
+        | *New in version 2.0.0:* handle multidimensional arrays
+        | *New in version 3.0.0:* return zero-length arrays if all NaN
         '''
         try:
-            data = np.array(data, dtype=float) # Make sure it's an array of float type
+            data = np.array(data, dtype=float) # Make sure it's an array of float type, otherwise nan operations fail
             is_multidim = data.ndim > 1
             if is_multidim:
                 if not replacenans:
                     errormsg = 'For multidimensional data, NaNs cannot be removed. Set replacenans=<value>, or flatten data before use.'
                     raise ValueError(errormsg)
             inds = np.nonzero(~np.isnan(data))
             if not is_multidim:
@@ -346,53 +351,69 @@
                 if scu.isstring(replacenans):
                     if replacenans in ['nearest','linear']:
                         if is_multidim:
                             errormsg = 'Cannot perform interpolation on multidimensional data; use replacenans=<value> instead'
                             raise NotImplementedError(errormsg)
                         newx = range(len(data)) # Create a new x array the size of the original array
                         sanitized = smoothinterp(newx, inds, sanitized, method=replacenans, smoothness=0) # Replace nans with interpolated values
-                    else:
+                    else: # pragma: no cover
                         errormsg = f'Interpolation method "{replacenans}" not found: must be "nearest" or "linear"'
                         raise ValueError(errormsg)
                 else:
                     naninds = np.nonzero(np.isnan(data))
                     sanitized = data.copy() # To avoid overwriting original array
                     sanitized[naninds] = replacenans
 
             if len(sanitized)==0:
                 if defaultval is not None:
                     sanitized = defaultval
                 else:
-                    sanitized = data
                     inds = []
 
                     if verbose: # pragma: no cover
                         if label is None: label = 'these input data'
                         print(f'sc.sanitize(): no valid values found for {label}. Returning 0.')
         except Exception as E: # pragma: no cover
             if die:
                 raise E
             else:
-                sanitized = data # Give up and just return an empty array
+                sanitized = data # Give up and just return original array
                 inds = []
         if returninds: return sanitized, inds
         else:          return sanitized
 
 
+# Define as an alias
+rmnans = sanitize
+
 def fillnans(data=None, replacenans=True, **kwargs):
     """
-    Alias for ``sc.sanitize(..., replacenans=True)`` with nearest interpolation (or a specified value).
+    Alias for :func:`sc.sanitize(..., replacenans=True) <sanitize>` with nearest interpolation
+    (or a specified value).
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     """
     return sanitize(data=data, replacenans=replacenans, **kwargs)
-fillnans.__doc__ += '\n\n' + sanitize.__doc__
 
-# Define as an alias
-rmnans = sanitize
+
+def findnans(data=None, **kwargs):
+    """
+    Alias for :func:`sc.findinds(np.isnan(data)) <findinds>`.
+    
+    **Examples**::
+        
+        data = [0, 1, 2, np.nan, 4, np.nan, 6, np.nan, np.nan, np.nan, 10]
+        sc.findnans(data) # Returns array([3, 5, 7, 8, 9])
+
+    *New in version 3.0.0.*
+    """
+    data  = np.array(data, dtype=float)
+    isnan = np.isnan(data)
+    inds  = findinds(arr=isnan, **kwargs)
+    return inds
 
 
 def isprime(n, verbose=False):
     '''
     Determine if a number is prime.
 
     From https://stackoverflow.com/questions/15285534/isprime-function-for-python-language
@@ -457,26 +478,26 @@
         sc.numdigits(0) # Returns 1
         sc.numdigits(-12345) # Returns 5
         sc.numdigits(-12345, count_minus=True) # Returns 6
         sc.numdigits(12, 123, 12345) # Returns [2, 3, 5]
         sc.numdigits(0.01) # Returns -2
         sc.numdigits(0.01, count_decimal=True) # Returns -4
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     """
     is_scalar = True if scu.isnumber(n) and len(args) == 0 else False
 
     vals = cat(n, *args)
 
     output = []
     for n in vals:
         abs_n = abs(n)
         is_decimal = 0 < abs_n < 1
         n_digits = 1
-        if n < 0 and count_minus:
+        if n < 0 and count_minus: # pragma: no cover
             n_digits += 1
         if is_decimal:
             if count_decimal:
                 n_digits += 1
             else:
                 n_digits -= 1
 
@@ -509,28 +530,29 @@
         span (float): width of distribution on either side of 1
         randseed (int): seed passed to the reseed numpy's legacy MT19937 BitGenerator
         normal (bool):  whether to use a normal distribution instead of uniform
 
     **Example**::
 
         sc.perturb(5, 0.3) # Returns e.g. array([0.73852362, 0.7088094 , 0.93713658, 1.13150755, 0.87183371])
+    
+    *New in version 3.0.0:* Uses a separate random number stream
     '''
-    if randseed is not None:
-        np.random.seed(int(randseed)) # Optionally reset random seed
+    rng = np.random.default_rng(randseed)
     if normal:
-        output = 1.0 + span*np.random.randn(n)
+        output = 1.0 + rng.normal(0, span, size=n)
     else:
-        output = 1.0 + 2*span*(np.random.rand(n)-0.5)
+        output = 1.0 + rng.uniform(-span, span, size=n)
     return output
 
 
 def normsum(arr, total=None):
     '''
     Multiply a list or array by some normalizing factor so that its sum is equal
-    to the total. Formerly called ``sc.scaleratio()``.
+    to the total. Formerly called :func:`sc.scaleratio() <scaleratio>`.
 
     Args:
         arr (array): array (or list) to normalize
         total (float): amount to sum to (default 1)
 
     **Example**::
 
@@ -566,24 +588,24 @@
     out += minval
     if isinstance(arr, list): out = out.tolist() # Preserve type
     return out
 
 
 def inclusiverange(*args, **kwargs):
     '''
-    Like ``np.arange()``/``np.linspace()``, but includes the start and stop points.
+    Like :func:`numpy.arange`/`numpy.linspace`, but includes the start and stop points.
     Accepts 0-3 args, or the kwargs start, stop, step.
 
     In most cases, equivalent to ``np.linspace(start, stop, int((stop-start)/step)+1)``.
 
     Args:
         start (float): value to start at
         stop (float): value to stop at
         step (float): step size
-        kwargs (dict): passed to ``np.linspace()``
+        kwargs (dict): passed to :func:`numpy.linspace`
 
     **Examples**::
 
         x = sc.inclusiverange(10)        # Like np.arange(11)
         x = sc.inclusiverange(3,5,0.2)   # Like np.linspace(3, 5, int((5-3)/0.2+1))
         x = sc.inclusiverange(stop=5)    # Like np.arange(6)
         x = sc.inclusiverange(6, step=2) # Like np.arange(0, 7, 2)
@@ -634,62 +656,65 @@
     Returns:
         Array of integers
 
     **Example**::
 
         sc.randround(np.random.randn(8)) # Returns e.g. array([-1,  0,  1, -2,  2,  0,  0,  0])
 
-    New in version 1.0.0.
+    | *New in version 1.0.0.*
+    | *New in version 3.0.0:* allow arrays of arbitrary shape
     '''
     if isinstance(x, np.ndarray):
-        output = np.array(np.floor(x+np.random.random(x.size)), dtype=int)
+        output = np.array(np.floor(x+np.random.random(x.shape)), dtype=int)
     elif isinstance(x, list):
         output = [randround(i) for i in x]
     else:
         output = int(np.floor(x+np.random.random()))
     return output
 
 
 def cat(*args, copy=False, **kwargs):
     '''
     Like np.concatenate(), but takes anything and returns an array. Useful for
     e.g. appending a single number onto the beginning or end of an array.
 
     Args:
         args   (any):  items to concatenate into an array
-        kwargs (dict): passed to ``np.concatenate()``
+        kwargs (dict): passed to :func:`numpy.concatenate`
 
     **Examples**::
 
         arr = sc.cat(4, np.ones(3))
         arr = sc.cat(np.array([1,2,3]), [4,5], 6)
         arr = sc.cat(np.random.rand(2,4), np.random.rand(2,6), axis=1)
 
-    | New in version 1.0.0.
-    | New in version 1.1.0: "copy" and keyword arguments.
-    | New in version 2.0.2: removed "copy" argument; changed default axis of 0; arguments passed to ``np.concatenate()``
+    | *New in version 1.0.0.*
+    | *New in version 1.1.0:* "copy" and keyword arguments.
+    | *New in version 2.0.2:* removed "copy" argument; changed default axis of 0; arguments passed to ``np.concatenate()``
     '''
     
     if not len(args):
         return np.array([])
     arrs = [scu.toarray(arg) for arg in args] # Key step: convert everything to an array
+    if arrs[0].ndim == 2: # Convert to 2D if first array is
+        arrs = [np.atleast_2d(arr) for arr in arrs]
     output = np.concatenate(arrs, **kwargs)
     return output
 
 
 def linregress(x, y, full=False, **kwargs):
     '''
     Simple linear regression returning the line of best fit and R value. Similar
-    to ``scipy.stats.linregress`` but simpler.
+    to :func:`scipy.stats.linregress`` but simpler.
     
     Args:
         x (array): the x coordinates
         y (array): the y coordinates
         full (bool): whether to return a full data structure
-        kwargs (dict): passed to ``np.polyfit()``
+        kwargs (dict): passed to :func:`numpy.polyfit`
     
     **Examples**::
         
         x = range(10)
         y = sorted(2*np.random.rand(10) + 1)
         m,b = sc.linregress(x, y) # Simple usage
         out = sc.linregress(x, y, full=True) # Has out.m, out.b, out.x, out.y, out.corr, etc.
@@ -697,15 +722,15 @@
         pl.plot(x, m*x+b)
         pl.bar(x, out.residuals)
         pl.title(f'R² = {out.r2}')
     '''
     x = scu.toarray(x)
     y = scu.toarray(y)
     fit = np.polyfit(x, y, deg=1, **kwargs) # Do the fit
-    if not full:
+    if not full: # pragma: no cover
         return fit
     else:
         out = sco.objdict()
         out.m = fit[0] # Slope
         out.b = fit[-1] # Intercept
         out.coeffs = fit
         out.corr = np.corrcoef(x, y)[0,1]
@@ -721,28 +746,29 @@
 #%% Smoothing functions
 ##############################################################################
 
 
 __all__ += ['rolling', 'convolve', 'smooth', 'smoothinterp', 'gauss1d', 'gauss2d']
 
 
-def rolling(data, window=7, operation='mean', **kwargs):
+def rolling(data, window=7, operation='mean', replacenans=None, **kwargs):
     '''
     Alias to pandas' rolling() (window) method to smooth a series.
 
     Args:
         data (list/arr): the 1D or 2D data to be smoothed
         window (int): the length of the window
         operation (str): the operation to perform: 'mean' (default), 'median', 'sum', or 'none'
+        replacenans (bool/float): if None, leave NaNs; if False, remove them; if a value, replace with that value; if the string 'nearest' or 'linear', do interpolation (see :func:`sc.rmnans() <rmnans>` for details)
         kwargs (dict): passed to pd.Series.rolling()
 
     **Example**::
 
         data = [5,5,5,0,0,0,0,7,7,7,7,0,0,3,3,3]
-        rolled = sc.rolling(data)
+        rolled = sc.rolling(data, replacenans='nearest')
     '''
     # Handle the data
     data = np.array(data)
     data = pd.Series(data) if data.ndim == 1 else pd.DataFrame(data)
 
     # Perform the roll
     roll = data.rolling(window=window, **kwargs)
@@ -751,37 +777,42 @@
     if   operation in [None, 'none']: output = roll
     elif operation == 'mean':         output = roll.mean().values
     elif operation == 'median':       output = roll.median().values
     elif operation == 'sum':          output = roll.sum().values
     else:
         errormsg = f'Operation "{operation}" not recognized; must be mean, median, sum, or none'
         raise ValueError(errormsg)
+    
+    if replacenans is None:
+        pass
+    else:
+        output = sanitize(data=output, replacenans=replacenans)
 
     return output
 
 
 def convolve(a, v):
     '''
-    Like ``np.convolve()``, but always returns an array the size of the first array
-    (equivalent to mode='same'), and solves the boundary problem present in ``np.convolve()``
+    Like :func:`numpy.convolve`, but always returns an array the size of the first array
+    (equivalent to mode='same'), and solves the boundary problem present in :func:`numpy.convolve`
     by adjusting the edges by the weight of the convolution kernel.
 
     Args:
         a (arr): the input array
         v (arr): the convolution kernel
 
     **Example**::
 
         a = np.ones(5)
         v = np.array([0.3, 0.5, 0.2])
         c1 = np.convolve(a, v, mode='same') # Returns array([0.8, 1.  , 1.  , 1.  , 0.7])
         c2 = sc.convolve(a, v)              # Returns array([1., 1., 1., 1., 1.])
 
-    | New in version 1.3.0.
-    | New in version 1.3.1: handling the case where len(a) < len(v)
+    | *New in version 1.3.0.*
+    | *New in version 1.3.1:* handling the case where len(a) < len(v)
     '''
 
     # Handle types
     a = np.array(a)
     v = np.array(v)
 
     # Perform standard Numpy convolution
@@ -801,54 +832,54 @@
     if len_rhs:
         w_rhs = (np.cumsum(v[::-1])[::-1]/vtot) # Ditto, reversed for RHS
         w_rhs = w_rhs[1:len_rhs+1] # Ditto
         out[-len_rhs:] = out[-len_rhs:]/w_rhs # Ditto
 
     # Handle the case where len(v) > len(a)
     len_diff = max(0, len_v - len_a)
-    if len_diff:
+    if len_diff: # pragma: no cover
         lhs_trim = len_diff // 2
         out = out[lhs_trim:lhs_trim+len_a]
 
     return out
 
 
 def smooth(data, repeats=None, kernel=None, legacy=False):
     '''
     Very simple function to smooth a 1D or 2D array.
 
-    See also ``sc.gauss1d()`` for simple Gaussian smoothing.
+    See also :func:`sc.gauss1d() <gauss1d>` for simple Gaussian smoothing.
 
     Args:
         data (arr): 1D or 2D array to smooth
         repeats (int): number of times to apply smoothing (by default, scale to be 1/5th the length of data)
         kernel (arr): the smoothing kernel to use (default: ``[0.25, 0.5, 0.25]``)
         legacy (bool): if True, use the old (pre-1.3.0) method of calculation that doesn't correct for edge effects
 
     **Example**::
 
         data = pl.randn(5,5)
         smoothdata = sc.smooth(data)
 
-    New in version 1.3.0: Fix edge effects.
+    *New in version 1.3.0:* Fix edge effects.
     '''
     if repeats is None:
         repeats = int(np.floor(len(data)/5))
     if kernel is None:
         kernel = [0.25,0.5,0.25]
     kernel = np.array(kernel)
     output = np.array(data).copy()
 
     # Only convolve the kernel with itself -- equivalent to doing the full convolution multiple times
     v = kernel.copy()
     for r in range(repeats-1):
         v = np.convolve(v, kernel, mode='full')
 
     # Support legacy method of not correcting for edge effects
-    if legacy:
+    if legacy: # pragma: no cover
         conv = np.convolve
         kw = {'mode':'same'}
     else:
         conv = convolve
         kw = {}
 
     # Perform the convolution
@@ -860,52 +891,66 @@
     else: # pragma: no cover
         errormsg = 'Simple smoothing only implemented for 1D and 2D arrays'
         raise ValueError(errormsg)
 
     return output
 
 
-def smoothinterp(newx=None, origx=None, origy=None, smoothness=None, growth=None, ensurefinite=False, keepends=True, method='linear'):
+def smoothinterp(newx=None, origx=None, origy=None, smoothness=None, growth=None, 
+                 ensurefinite=True, keepends=True, method='linear'):
     '''
-    Smoothly interpolate over values and keep end points. Same format as numpy.interp().
+    Smoothly interpolate over values
+    
+    Unlike :func:`np.interp() <numpy.interp>`, this function does exactly pass 
+    through each data point: 
 
     Args:
         newx (arr): the points at which to interpolate
         origx (arr): the original x coordinates
         origy (arr): the original y coordinates
         smoothness (float): how much to smooth
-        growth (float): the growth rate to apply past the ends of the data [deprecated]
-        ensurefinite (bool):  ensure all values are finite
-        keepends (bool): whether to keep the ends [deprecated]
+        growth (float): the growth rate to apply past the ends of the data
+        ensurefinite (bool):  ensure all values are finite (including skipping NaNs)
         method (str): the type of interpolation to use (options are 'linear' or 'nearest')
 
     Returns:
         newy (arr): the new y coordinates
 
     **Example**::
 
-        origy = np.array([0,0.1,0.3,0.8,0.7,0.9,0.95,1])
+        import sciris as sc
+        import numpy as np
+        from scipy import interpolate
+        
+        origy = np.array([0,0.2,0.1,0.9,0.7,0.8,0.95,1])
         origx = np.linspace(0,1,len(origy))
         newx = np.linspace(0,1,5*len(origy))
-        newy = sc.smoothinterp(newx, origx, origy, smoothness=5)
-        pl.plot(newx,newy)
-        pl.scatter(origx,origy)
+        sc_y = sc.smoothinterp(newx, origx, origy, smoothness=5)
+        np_y = np.interp(newx, origx, origy)
+        si_y = interpolate.interp1d(origx, origy, 'cubic')(newx)
+        kw = dict(lw=3, alpha=0.7)
+        pl.plot(newx, np_y, '--', label='NumPy', **kw)
+        pl.plot(newx, si_y, ':',  label='SciPy', **kw)
+        pl.plot(newx, sc_y, '-',  label='Sciris', **kw)
+        pl.scatter(origx, origy, s=50, c='k', label='Data')
+        pl.legend()
+        pl.show()
 
-    Version: 2018jan24
+    | *New in verison 3.0.0:* "ensurefinite" now defaults to True; removed "skipnans" argument
     '''
     # Ensure arrays and remove NaNs
     if scu.isnumber(newx):  newx = [newx] # Make sure it has dimension
     if scu.isnumber(origx): origx = [origx] # Make sure it has dimension
     if scu.isnumber(origy): origy = [origy] # Make sure it has dimension
     newx  = np.array(newx, dtype=float)
     origx = np.array(origx, dtype=float)
     origy = np.array(origy, dtype=float)
 
     # If only a single element, just return it, without checking everything else
-    if len(origy)==1:
+    if len(origy)==1: # pragma: no cover
         newy = np.zeros(newx.shape)+origy[0]
         return newy
 
     if not(newx.shape):  raise ValueError('To interpolate, must have at least one new x value to interpolate to') # pragma: no cover
     if not(origx.shape): raise ValueError('To interpolate, must have at least one original x value to interpolate to') # pragma: no cover
     if not(origy.shape): raise ValueError('To interpolate, must have at least one original y value to interpolate to') # pragma: no cover
     if not(origx.shape==origy.shape): # pragma: no cover
@@ -917,21 +962,21 @@
     origx = origx[correctorder]
     origy = origy[correctorder]
     neworder = np.argsort(newx)
     newx = newx[neworder] # And sort newx just in case
 
     # Only keep finite elements
     finitey = np.isfinite(origy) # Boolean for whether it's finite
-    if finitey.any() and not finitey.all(): # If some but not all is finite, pull out indices that are
+    if finitey.any() and not finitey.all(): # If some but not all is finite, pull out indices that are 
         finiteorigy = origy[finitey]
         finiteorigx = origx[finitey]
     else: # Otherwise, just copy the original
         finiteorigy = origy.copy()
         finiteorigx = origx.copy()
-
+        
     # Perform actual interpolation
     if method=='linear':
         newy = np.interp(newx, finiteorigx, finiteorigy) # Perform standard interpolation without infinities
     elif method=='nearest':
         newy = np.zeros(newx.shape) # Create the new array of the right size
         for i,x in enumerate(newx): # Iterate over each point
             xind = np.argmin(abs(finiteorigx-x)) # Find the nearest neighbor
@@ -1039,29 +1084,29 @@
         pl.scatter(x, yi2,   label='More smoothing')
         pl.scatter(xi3, yi3, label='Uniform spacing')
         pl.show()
 
         # Simple usage
         sc.gauss1d(y)
 
-    New in version 1.3.0.
+    *New in version 1.3.0.*
     '''
 
     # Swap inputs if x is provided but not y
-    if y is None and x is not None:
+    if y is None and x is not None: # pragma: no cover
         y,x = x,y
-    if x is None:
+    if x is None: # pragma: no cover
         x = np.arange(len(y))
     if xi is None:
         xi = x
 
     # Convert to arrays
     try:
         orig_dtype = y.dtype
-    except:
+    except: # pragma: no cover
         orig_dtype = np.float64
     if use32:
         x, y, xi, = _arr32(x), _arr32(y), _arr32(xi)
 
     # Handle scale
     if scale is None:
         minmax = np.ptp(x) # Calculate the range of x
@@ -1131,30 +1176,30 @@
 
         # Plot oiginal and interpolated versions
         sc.scatter3d(x, y, z, c=z)
         sc.surf3d(zi)
         sc.scatter3d(xi2, yi2, zi2, c=zi2)
         pl.show()
 
-    | New in version 1.3.0.
-    | New in version 1.3.1: default arguments; support for 2D inputs
+    | *New in version 1.3.0.*
+    | *New in version 1.3.1:* default arguments; support for 2D inputs
     '''
     # Swap variables if needed
-    if z is None and x is not None:
+    if z is None and x is not None: # pragma: no cover
         z,x = x,z
-    if x is None or y is None:
+    if x is None or y is None: # pragma: no cover
         if z.ndim != 2:
             errormsg = f'If the x and y axes are not provided, then z must be 2D, not {z.ndim}D'
             raise ValueError(errormsg)
         else:
             x = np.arange(z.shape[1]) # It's counterintuitive, but x is the 1st dimension, not the 0th
             y = np.arange(z.shape[0])
 
     # Handle shapes
-    if z.ndim == 2 and (x.ndim == 1) and (y.ndim == 1):
+    if z.ndim == 2 and (x.ndim == 1) and (y.ndim == 1): # pragma: no cover
         if (z.shape[0] != z.shape[1]) and (len(x) == z.shape[0]) and (len(y) == z.shape[1]):
             print(f'sc.gauss2d() warning: the length of x (={len(x)}) and y (={len(y)}) match the wrong dimensions of z; transposing')
             z = z.transpose()
         if len(x) != z.shape[1] or len(y) != z.shape[0]:
             errormsg = f'Shape mismatch: (y, x) = {(len(y), len(x))}, but z = {z.shape}'
             raise ValueError(errormsg)
 
@@ -1170,30 +1215,30 @@
         scale, xscale, yscale = _f32(scale), _f32(xscale), _f32(yscale)
     xsc = xscale*scale
     ysc = yscale*scale
 
     # Now that we have xi and yi, handle more 1D vs 2D logic
     if xi.ndim == 1 and yi.ndim == 1 and grid:
         xi, yi = np.meshgrid(xi, yi)
-    if xi.shape != yi.shape:
+    if xi.shape != yi.shape: # pragma: no cover
         errormsg = f'Output arrays must have same shape, but xi = {xi.shape} and yi = {yi.shape}'
         raise ValueError(errormsg)
 
     # Flatten everything and check sizes
     orig_shape = xi.shape
     x  = x.flatten()
     y  = y.flatten()
     z  = z.flatten()
     xi = xi.flatten()
     yi = yi.flatten()
     ni = len(xi)
-    if len(x) != len(y) != len(z):
+    if len(x) != len(y) != len(z): # pragma: no cover
         errormsg = f'Input arrays do not have the same number of elements: x = {len(x)}, y = {len(y)}, z = {len(z)}'
         raise ValueError(errormsg)
-    if len(xi) != len(yi):
+    if len(xi) != len(yi): # pragma: no cover
         errormsg = f'Output arrays do not have the same number of elements: xi = {len(xi)}, yi = {len(yi)}'
         raise ValueError(errormsg)
 
     def calc(xi, yi):
         ''' Calculate the calculation '''
         dist = ((x - xi)/xsc)**2 + ((y - yi)/ysc)**2
         weights = np.exp(-dist)
@@ -1206,8 +1251,8 @@
     if use32: zi = _arr32(zi)
     for i in range(ni):
         zi[i] = calc(xi[i], yi[i])
 
     # Convert back to original size and dtype
     zi = np.array(zi.reshape(orig_shape), dtype=orig_dtype)
 
-    return zi
+    return zi
```

### Comparing `sciris-2.1.0/sciris/sc_odict.py` & `sciris-3.0.0/sciris/sc_odict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 '''
-The 'odict' class, combining features from an OrderedDict and a list/array.
+The "odict" class, combining features from an OrderedDict and a list/array.
 
 Highlights:
-    - :class:`odict`: flexible container representing the best-of-all-worlds across lists, dicts, and arrays
+    - :class:`sc.odict() <odict>`: flexible container representing the best-of-all-worlds across dicts, lists, and arrays
     - :class:`objdict`: like an odict, but allows get/set via e.g. ``foo.bar`` instead of ``foo['bar']``
 '''
 
 ##############################################################################
 #%% odict class
 ##############################################################################
 
 import re
+import json
 import numpy as np
-from collections import OrderedDict as OD, defaultdict as ddict
+import collections as co
 from . import sc_utils as scu
 from . import sc_printing as scp
 from . import sc_nested as scn
 
 # Restrict imports to user-facing modules
 __all__ = ['ddict', 'odict', 'objdict', 'dictobj', 'asobj']
 
+ddict = co.defaultdict # Define alias
+OD = dict # Base class; was OrderedDict before v3.0.0
 
 class odict(OD):
     '''
     Ordered dictionary with integer indexing
 
-
     An ordered dictionary, like the OrderedDict class, but supports list methods like integer
     indexing, key slicing, and item inserting. It can also replicate defaultdict behavior
     via the ``defaultdict`` argument.
+    
+    Args:
+        args (dict): convert an existing dict, e.g. ``sc.odict({'a':1})``
+        defaultdict (class): if provided, create as a defaultdict as well
+        kwargs (dict): additional keyword arguments, e.g. ``sc.odict(a=1)``
 
     **Examples**::
 
         # Simple example
         mydict = sc.odict(foo=[1,2,3], bar=[4,5,6]) # Assignment is the same as ordinary dictionaries
         mydict['foo'] == mydict[0] # Access by key or by index
         mydict[:].sum() == 21 # Slices are returned as numpy arrays by default
@@ -59,38 +66,50 @@
         dd = sc.odict(a=[1,2,3], defaultdict=list)
         dd['c'].append(4)
 
         nested = sc.odict(a=0, defaultdict='nested') # Create a infinitely nested dictionary (NB: may behave strangely on IPython)
         nested['b']['c']['d'] = 2
 
     Note: by default, integers are used as an alias to string keys, so cannot be used
-    as keys directly. However, you can force regular-dict behavior using ``setitem()``,
-    and you can convert a dictionary with integer keys to an odict using ``sc.odict.makefrom()``.
+    as keys directly. However, you can force regular-dict behavior using :meth:`setitem() <odict.setitem>`,
+    and you can convert a dictionary with integer keys to an odict using :meth:`sc.odict.makefrom() <odict.makefrom>`.
     If an odict has integer keys and the keys do not match the key positions, then the
     key itself will take precedence (e.g., ``od[3]`` is equivalent to ``dict(od)[3]``,
     not ``dict(od)[od.keys()[3]]``). This usage is discouraged.
 
-    | New in version 1.1.0: "defaultdict" argument
-    | New in version 1.3.1: allow integer keys via ``makefrom()``; removed ``to_OD``; performance improvements
-    | New in version 2.0.1: allow deletion by index
+    | *New in version 1.1.0:* "defaultdict" argument
+    | *New in version 1.3.1:* allow integer keys via ``makefrom()``; removed ``to_OD``; performance improvements
+    | *New in version 2.0.1:* allow deletion by index
+    | *New in version 3.0.0:* allow numeric indices; inherit from dict rather than OrderedDict
     '''
 
     def __init__(self, *args, defaultdict=None, **kwargs):
         ''' Combine the init properties of both OrderedDict and defaultdict '''
-        if len(args)==1 and args[0] is None: args = [] # Remove a None argument
-        OD.__init__(self, *args, **kwargs) # Standard init
+        
+        # Standard init
+        mapping = dict(*args, **kwargs)
+        dict.update(self, mapping)
+        
+        # Handle defaultdict
         if defaultdict is not None:
             if defaultdict != 'nested' and not callable(defaultdict): # pragma: no cover
                 errormsg = f'The defaultdict argument must be either "nested" or callable, not {type(defaultdict)}'
                 raise TypeError(errormsg)
             self._setattr('_defaultdict', defaultdict) # Use OD.__setattr__() since setattr() is overridden by sc.objdict()
+        
         self._cache_keys()
         return
 
 
+    @classmethod
+    def _new(cls, *args, **kwargs):
+        ''' Constructor for a new instance -- used in place of self.__class__() '''
+        return cls(*args, **kwargs)
+
+
     def _cache_keys(self):
         ''' Store a copy of the keys as a list so integer lookup doesn't have to regenerate it each time '''
         self._setattr('_cached_keys', self.keys())
         self._setattr('_stale', False)
         return
 
 
@@ -117,15 +136,15 @@
                 if isinstance(E, KeyError): # We already encountered an exception, usually a KeyError
                     try: # Handle defaultdict behavior by first checking if it exists
                         _defaultdict = OD.__getattribute__(self, '_defaultdict')
                     except:
                         _defaultdict = None
                     if _defaultdict is not None and allow_default: # If it does, use it, then get the key again
                         if _defaultdict == 'nested':
-                            _defaultdict = lambda: self.__class__(defaultdict=_defaultdict) # Make recursive
+                            _defaultdict = lambda: self._new(defaultdict=_defaultdict) # Make recursive
                         dd = _defaultdict() # Create the new object
                         self._setitem(key, dd) # Add it to the dictionary
                         self._setattr('_stale', True) # Flag to refresh the cached keys
                         return dd # Return
                     else:
                         keys = self.keys()
                         if len(keys): errormsg = f'odict key "{key}" not found; available keys are:\n{scu.newlinejoin(keys)}'
@@ -213,15 +232,17 @@
     def setitem(self, key, value):
         ''' Use regular dictionary ``setitem``, rather than odict's '''
         self._setattr('_stale', True) # Flag to refresh the cached keys
         self._setitem(key, value)
         return
 
 
-    def __repr__(self, maxlen=None, showmultilines=True, divider=False, dividerthresh=10, numindents=0, recursionlevel=0, sigfigs=None, numformat=None, maxitems=200, classname='odict()', quote='', numleft='#', numsep=':', keysep=':', dividerchar='—'):
+    def __repr__(self, maxlen=None, showmultilines=True, divider=False, dividerthresh=10, 
+                 numindents=0, recursionlevel=0, sigfigs=None, numformat=None, maxitems=200, 
+                 classname='odict', quote='', numleft='#', numsep=':', keysep=':', dividerchar='—'):
         ''' Print a meaningful representation of the odict '''
 
         # Set non-customizable primitives for display
         toolong      = ' [...]'    # String to display at end of line when maximum value character length is overrun.
         dividerstr   = dividerchar*40+'\n' # String to use as an inter-item divider.
         indentstr    = '    '      # Create string to use to indent.
         maxrecursion = 5           # It's a repr, no one could want more than that
@@ -234,15 +255,15 @@
 
         # If the odict is empty, make the string just indicate it's an odict.
         allkeys = self.keys()
         nkeys = len(allkeys)
         halfmax = int(maxitems/2)
         extraitems = 0
         if nkeys == 0:
-            output = classname
+            output = classname + '()'
         else:
             output = ''
             keystrs = [] # Start with an empty list which we'll save key strings in.
             valstrs = [] # Start with an empty list which we'll save value strings in.
             vallinecounts = [] # Start with an empty list which we'll save line counts in.
             extraitems = nkeys - maxitems
             if extraitems <= 0:
@@ -307,18 +328,18 @@
                 # Create the the text to add, apply the indent, and add to the output
                 spacer = ' '*(maxkeylen-len(keystr))
                 if vallinecount == 1 or not showmultilines:
                     rawoutput = f'{numleft}{ind:d}{numsep} {quote}{keystr}{quote}{keysep}{spacer} {valstr}\n'
                 else:
                     rawoutput = f'{numleft}{ind:d}{numsep} {quote}{keystr}{quote}{keysep}{spacer} \n{valstr}\n'
 
-                # Perform the indentation.
+                # Perform the indentation
                 newoutput = scp.indent(prefix=theprefix, text=rawoutput, width=80)
 
-                # Strip ot any terminal newline.
+                # Strip out any terminal newline
                 if newoutput[-1] == '\n':
                     newoutput = newoutput[:-1]
 
                 # Add the new output to the full output
                 if extraitems>0 and i == halfmax:
                     output += f'\n[{extraitems} additional odict items not shown]\n\n'
                 output += newoutput
@@ -360,15 +381,15 @@
 
 
     def __delitem__(self, key):
         ''' Default delitem, except set stale to true and allow numeric values; slices etc are not supported '''
         self._setattr('_stale', True) # Flag to refresh the cached keys
         try:
             return OD.__delitem__(self, key)
-        except Exception as E:
+        except Exception as E: # pragma: no cover
             if isinstance(key, scu._numtype): # If it's a number, use that
                 thiskey = self._ikey(key)
                 return OD.__delitem__(self, thiskey) # Note that defaultdict behavior isn't supported for non-string lookup
             else:
                 raise E
 
 
@@ -389,15 +410,15 @@
 
     def _ikey(self, key):
         ''' Handle an integer key '''
         if self._stale:
             self._cache_keys()
         try:
             return self._cached_keys[key]
-        except IndexError:
+        except IndexError: # pragma: no cover
             errormsg = f'index {key} out of range for dict of length {len(self)}'
             raise IndexError(errormsg) from None # Don't show the traceback
 
 
     def _slicekey(self, key, slice_end):
         ''' Validate a key supplied as a slice object '''
         if slice_end == 'stop':
@@ -427,15 +448,15 @@
         ''' Helper function for findkeys '''
         match = False
         if isinstance(key, tuple):
             for item in key:
                 if odict._matchkey(item, pattern, method):
                     return True
         else: # For everything except a tuple, treat it as a string
-            if not scu.isstring(key):
+            if not scu.isstring(key): # pragma: no cover
                 try:
                     key = str(key) # Try to cast it to a string
                 except Exception as E: # pragma: no cover
                     errormsg = f'Could not convert odict key of type {type(key)} to a string: {str(E)}'
                     raise TypeError(E)
             if   method == 're':         match = bool(re.search(pattern, key))
             elif method == 'in':         match = pattern in key
@@ -444,15 +465,15 @@
             else: # pragma: no cover
                 errormsg = f'Method "{method}" not found; must be "re", "in", "startswith", or "endswith"'
                 raise ValueError(errormsg)
         return match
 
 
     def _is_odict_iterable(self, key):
-        ''' Check to see whether the "key" is actually an iterable '''
+        ''' Check to see whether the "key" is actually an iterable: a list or array '''
         output = isinstance(key, (list, np.ndarray))
         return output
 
 
     def _sanitize_items(self, items):
         ''' Try to convert the output of a slice to an array, but give up easily and return a list '''
         try:
@@ -460,17 +481,17 @@
             if 'S' in str(output.dtype) or 'U' in str(output.dtype): # ...but instead of converting to string, convert to object array for Python 2 or 3 -- WARNING, fragile!
                 output = np.array(items, dtype=object)
         except: # pragma: no cover
             output = items # If that fails, just give up and return the list
         return output
 
 
-    def export(self, doprint=True):
+    def export(self, doprint=True, classname='odict'):
         ''' Export the odict in a form that is valid Python code '''
-        start = 'odict(['
+        start = classname + '(['
         end = '])'
         output = start
 
         for key in self.keys():
             output += '('+repr(key)
             output += ', '
             child = self.get(key)
@@ -578,17 +599,17 @@
     def findbyval(self, value, first=True, strict=False):
         '''
         Returns the key(s) that match a given value -- reverse of findbykey, except here
         uses exact matches to the value or values provided.
 
         **Example**::
 
-            z = odict({'dog':[2,3], 'cat':[4,6], 'mongoose':[4,6]})
-            z.findvals([4,6]) # returns 'cat'
-            z.findvals([4,6], first=False) # returns ['cat', 'mongoose']
+            z = sc.odict({'dog':[2,3], 'cat':[4,6], 'mongoose':[4,6]})
+            z.findbyval([4,6]) # returns 'cat'
+            z.findbyval([4,6], first=False) # returns ['cat', 'mongoose']
         '''
         keys = []
         for key,val in self.items():
             if val == value:  # Exact match, return a match
                 match = True
             elif not strict and isinstance(value, list) and val in value: # "value" is a list and it's contained
                 match = True
@@ -598,22 +619,32 @@
                 if first: return key
                 else:     keys.append(key)
         return keys
 
 
     def filter(self, keys=None, pattern=None, method=None, exclude=False):
         '''
+        Find matching keys in the odict, and return a new odict
+        
         Filter the odict keys and return a new odict which is a subset. If keys is a list,
         then uses that for matching. If the first argument is a string, then treats as a pattern
-        for matching using findkeys(). If exclude=True, then will exclude rather than include matches.
+        for matching using :meth:`findkeys() <odict.findkeys`.
+        
+        Args:
+            keys (list): the list of keys to keep (or exclude)
+            pattern (str): the pattern by which to match keys; see :meth:`findkeys() <odict.findkeys` for details
+            method (str): the method by which to match keys; see :meth:`findkeys() <odict.findkeys` for details
+            exclude (bool): if exclude=True, then exclude rather than include matches
+            
+        See also :meth:`sort() <odict.sort>`, which includes filtering by position.
         '''
         if scu.isstring(keys) and pattern is None: # Assume first argument, transfer
             pattern = keys
             keys = None
-        filtered = odict()
+        filtered = self._new() # Create a new instance of the same class
         if keys is None:
             keys = self.findkeys(pattern=pattern, method=method, first=False)
         if not exclude:
             for key in keys:
                 filtered[key] = self.__getitem__(key)
         else:
             for key in self.keys():
@@ -632,31 +663,31 @@
         ''' Support an append method, like a list '''
         needkey = False
         if value is None: # Assume called with a single argument
             value = key
             needkey = True
         if key is None or needkey:
             keyname = 'key'+scu.flexstr(len(self))  # Define the key just to be the current index
-        else:
+        else: # pragma: no cover
             keyname = key
         self.__setitem__(keyname, value)
         return
 
 
     def insert(self, pos=None, key=None, value=None):
         '''
         Function to do insert a key -- note, computationally inefficient.
 
         **Example**::
 
-            z = odict()
+            z = sc.odict()
             z['foo'] = 1492
             z.insert(1604)
             z.insert(0, 'ganges', 1444)
-            z.insert(2, 'meikang', 1234)
+            z.insert(2, 'mekong', 1234)
         '''
 
         # Handle inputs
         realpos, realkey, realvalue = pos, key, value
         if key is None and value is None: # Assume it's called like odict.insert(666)
             realvalue = pos
             realkey = 'key'+scu.flexstr(len(self))
@@ -668,19 +699,19 @@
         if pos is None:
             realpos = 0
         if realpos>len(self): # pragma: no cover
             errormsg = f'Cannot insert {key} at position {pos} since length of odict is {len(self)}'
             raise ValueError(errormsg)
 
         # Create a temporary dictionary to hold all of the items after the insertion point
-        tmpdict = odict()
+        tmpdict = self._new()
         origkeys = self.keys()
         originds = range(len(origkeys))
         if not len(originds) or realpos==len(originds): # It's empty or in the final position, just append
-            self.__setitem__(realkey, realvalue)
+            self.__setitem__(realkey, realvalue) # pragma: no cover
         else: # Main usage case, it's not empty
             try:
                 insertind = originds.index(realpos) # Figure out which index we're inseting at
             except Exception as E: # pragma: no cover
                 errormsg = f'Could not insert item at position {realpos} in odict with {len(originds)} items'
                 raise ValueError(errormsg) from E
             keystopop = origkeys[insertind:] # Pop these keys until we get far enough back
@@ -699,73 +730,83 @@
         self.__setitem__(newkey, newval)
         return
 
 
     def rename(self, oldkey, newkey):
         ''' Change a key name (note: not optimized for speed) '''
         nkeys = len(self)
-        if isinstance(oldkey, scu._numtype):
+        if isinstance(oldkey, scu._numtype): # pragma: no cover
             index = oldkey
             keystr = self.keys()[index]
         else: # Forge ahead for strings and anything else!
             index = self.keys().index(oldkey)
             keystr = oldkey
         self.__setitem__(newkey, self.pop(keystr))
         if index<nkeys-1:
             for i in range(index+1, nkeys):
                 key = self.keys()[index]
                 value = self.pop(key)
                 self.__setitem__(key, value)
         return
 
 
-    def sort(self, sortby=None, reverse=False, copy=False, verbose=True):
+    def sort(self, sortby=None, reverse=False, copy=False):
         '''
-        Create a sorted version of the odict. Sorts by order of sortby, if provided, otherwise alphabetical.
-        If copy is True, then returns a copy (like sorted()).
-
-        Note that you can also use this to do filtering.
+        Create a sorted version of the odict. 
+        
+        By default, this method sorts alphabetically by key, but many other options 
+        are possible:
+            
+            - 'keys' sorts alphabetically by key
+            - 'values' sorts in ascending order by value
+            - if a list of keys is provided, sort by that order (any keys not provided will be omitted from the sorted dict!)
+            - if a list of numbers is provided, treat these as indices and sort by that order
+            - if a list of boolean values is provided, then omit False entries
+        
+        Args:
+            sortby (str or list): what to sort by; see above for options
+            reverse (bool): whether to return results in reverse order
+            copy (bool): whether to return a copy (same as :meth:`sorted() <odict.sorted>`)
+        
+        For filtering by string matching on keys, see :meth:`filter() <odict.filter>`.
+        
+        | *New in version 3.0.0:* removed "verbose" argument
         '''
         origkeys = self.keys()
         if sortby is None or sortby == 'keys':
             allkeys = sorted(origkeys)
         else:
             if sortby == 'values':
                 origvals = self.values()
                 sortby = sorted(range(len(origvals)), key=origvals.__getitem__) # Reset sortby based on https://stackoverflow.com/questions/3382352/equivalent-of-numpy-argsort-in-basic-python
             if not scu.isiterable(sortby): # pragma: no cover
                 raise Exception('Please provide a list to determine the sort order.')
             if all([isinstance(x, scu._stringtypes) for x in sortby]): # Going to sort by keys
                 allkeys = sortby # Assume the user knows what s/he is doing
             elif all([isinstance(x,bool) for x in sortby]): # Using Boolean values to filter
-                allkeys = []
-                for i,x in enumerate(sortby):
-                     if x: allkeys.append(origkeys[i])
+                allkeys = [origkeys[i] for i,tf in enumerate(sortby) if tf]
             elif all([isinstance(x, scu._numtype) for x in sortby]): # Going to sort by numbers
-                if not set(sortby)==set(range(len(self))): # pragma: no cover
-                    warningmsg = f'Warning: list to sort by "{sortby}" has different length than odict "{len(self)}"'
-                    if verbose: print(warningmsg)
                 allkeys = [origkeys[ind] for ind in sortby]
             else: # pragma: no cover
                 errormsg = f'Cannot figure out how to sort by "{sortby}"'
                 raise TypeError(errormsg)
-        tmpdict = odict()
+        tmpdict = self._new()
         if reverse:
             allkeys.reverse() # If requested, reverse order
         if copy:
             for key in allkeys: tmpdict[key] = self[key]
             return tmpdict
         else:
             for key in allkeys: tmpdict.__setitem__(key, self.pop(key))
             for key in allkeys: self.__setitem__(key, tmpdict.pop(key))
             return
 
 
     def sorted(self, sortby=None, reverse=False):
-        ''' Shortcut for making a copy of the sorted odict -- see sort() for options '''
+        ''' Shortcut for making a copy of the sorted odict -- see :meth:`sort() <odict.sort>` for options '''
         return self.sort(sortby=sortby, copy=True, reverse=reverse)
 
 
     def reverse(self, copy=False):
         ''' Reverse the order of an odict '''
         reversedkeys = self.keys()
         reversedkeys.reverse()
@@ -796,21 +837,21 @@
             c = sc.odict().make(['a','b']) # Make an odict with keys 'a' and 'b'
             d = sc.odict().make(['a','b'], 0) # Make an odict with keys 'a' and 'b', initialized to 0
             e = sc.odict().make(keys=['a','b'], vals=[1,2]) # Make an odict with 'a':1 and 'b':2
             f = sc.odict().make(keys=['a','b'], vals=np.array([1,2])) # As above, since arrays are coerced into lists
             g = sc.odict({'a':34, 'b':58}).make(['c','d'],[99,45]) # Add extra keys to an exising odict
             h = sc.odict().make(keys=['a','b','c'], keys2=['A','B','C'], keys3=['x','y','z'], vals=0) # Make a triply nested odict
 
-        New in version 1.2.2: "coerce" argument
+        *New in version 1.2.2:* "coerce" argument
         '''
         # Handle keys
         keylist = []
-        if keys is None and vals is None:
+        if keys is None and vals is None: # pragma: no cover
             return self # Nothing to do if nothing supplied
-        if keys is None and vals is not None:
+        if keys is None and vals is not None: # pragma: no cover
             keys = len(scu.tolist(vals)) # Values are supplied but keys aren't: use default keys
         if isinstance(keys, scu._numtype): # It's a single number: pre-generate
             keylist = ['%i'%i for i in range(keys)] # Generate keylist
         elif isinstance(keys, scu._stringtypes): # It's a single string
             keylist = [scu.flexstr(keys)]
         elif isinstance(keys, list): # It's a list: use directly
             keylist = keys
@@ -830,26 +871,26 @@
             vallist = vals
         else: # pragma: no cover
             errormsg = f'Must supply either a single value or a list of same length as the keys ({nkeys} keys, {nvals} values supplied)'
             raise ValueError(errormsg)
 
         # Handle nested keys -- warning, would be better to not hard-code this, but does the brain in as it is!
         if keys2 is not None and keys3 is not None: # Doubly nested
-            self.make(keys=keys, vals=odict().make(keys=keys2, vals=odict().make(keys=keys3, vals=vals)))
-        elif keys2 is not None: # Singly nested
-            self.make(keys=keys, vals=odict().make(keys=keys2, vals=vals))
+            self.make(keys=keys, vals=self._new().make(keys=keys2, vals=self._new().make(keys=keys3, vals=vals)))
+        elif keys2 is not None: # Singly nested # pragma: no cover
+            self.make(keys=keys, vals=self._new().make(keys=keys2, vals=vals))
         else: # Not nested -- normal case of making an odict
             for key,val in zip(keylist,vallist): # Update odict
                 self.__setitem__(key, val)
 
         return self # Return the odict
 
 
-    @staticmethod
-    def makefrom(source=None, include=None, keynames=None, force=True, *args, **kwargs):
+    @classmethod
+    def makefrom(cls, source=None, include=None, keynames=None, force=True, *args, **kwargs):
         '''
         Create an odict from entries in another dictionary. If keys is None, then
         use all keys from the current dictionary.
 
         Args:
             source (dict/list/etc): the item(s) to convert to an odict
             include (list): list of keys to include from the source dict in the odict (default: all)
@@ -859,26 +900,26 @@
         **Examples**::
 
             a = 'cat'
             b = 'dog'
             o = sc.odict.makefrom(source=locals(), include=['a','b']) # Make use of fact that variables are stored in a dictionary
 
             d = {'a':'cat', 'b':'dog'}
-            o = sc.odict.makefrom(d) # Same as odict(d)
+            o = sc.odict.makefrom(d) # Same as sc.odict(d)
             l = ['cat', 'monkey', 'dog']
             o = sc.odict.makefrom(source=l, include=[0,2], keynames=['a','b'])
 
             d = {12:'monkeys', 3:'musketeers'}
             o = sc.odict.makefrom(d)
         '''
         # Initialize new odict
-        out = odict()
+        out = cls()
 
         # Make sure it's iterable
-        if source is not None: # Don't do anything if there's nothing there
+        if source is not None: # Don't do anything if there's nothing there # pragma: no cover
             if not(scu.isiterable(source)): # Make sure it's iterable
                 source = scu.tolist(source)
             elif isinstance(source, scu._stringtypes):
                 source = [source] # Special case -- strings are iterable, but we don't want to
 
             if len(source)==0:
                 return out # Nothing to do here
@@ -910,51 +951,51 @@
     def map(self, func=None):
         '''
         Apply a function to each element of the odict, returning
         a new odict with the same keys.
 
         **Example**::
 
-            cat = odict({'a':[1,2], 'b':[3,4]})
+            cat = sc.odict({'a':[1,2], 'b':[3,4]})
             def myfunc(mylist): return [i**2 for i in mylist]
             dog = cat.map(myfunc) # Returns odict({'a':[1,4], 'b':[9,16]})
         '''
-        output = odict()
+        output = self._new()
         for key in self.keys():
             output[key] = func(self.__getitem__(key))
         return output
 
 
     def fromeach(self, ind=None, asdict=True):
         '''
         Take a "slice" across all the keys of an odict, applying the same
         operation to entry. The simplest usage is just to pick an index.
         However, you can also use it to apply a function to each key.
 
         **Example**::
 
-            z = odict({'a':array([1,2,3,4]), 'b':array([5,6,7,8])})
+            z = sc.odict({'a':array([1,2,3,4]), 'b':array([5,6,7,8])})
             z.fromeach(2) # Returns array([3,7])
             z.fromeach(ind=[1,3], asdict=True) # Returns odict({'a':array([2,4]), 'b':array([6,8])})
         '''
-        output = odict()
+        output = self._new()
         for key in self.keys():
             output[key] = self.__getitem__(key)[ind]
         if asdict: return output # Output as a slimmed-down odict
         else:      return output[:] # Output as just the entries
 
 
     def toeach(self, ind=None, val=None):
         '''
         The inverse of fromeach: partially reset elements within
         each odict key.
 
         **Example**::
 
-            z = odict({'a':[1,2,3,4], 'b':[5,6,7,8]})
+            z = sc.odict({'a':[1,2,3,4], 'b':[5,6,7,8]})
             z.toeach(2, [10,20])    # z is now odict({'a':[1,2,10,4], 'b':[5,6,20,8]})
             z.toeach(ind=3,val=666) #  z is now odict({'a':[1,2,10,666], 'b':[5,6,20,666]})
         '''
         nkeys = len(self.keys())
         if not(scu.isiterable(val)): # Assume it's meant to be populated in each
             val = [val]*nkeys # Duplicated
         if len(val)!=nkeys: # pragma: no cover
@@ -983,16 +1024,16 @@
         If transpose=True, return a tuple of lists rather than a list of tuples.
         '''
         iterator = list(enumerate(self.values()))
         if transpose: iterator = tuple(scu.transposelist(iterator))
         return iterator
 
 
-    def enumvalues(self, transpose=False):
-        ''' Alias for enumvals(). New in version 1.2.0. '''
+    def enumvalues(self, transpose=False): # pragma: no cover
+        ''' Alias for enumvals(). *New in version 1.2.0.* '''
         return self.enumvals(transpose=transpose)
 
 
     def enumitems(self, transpose=False):
         '''
         Returns tuple of 3 things: index, key, value.
 
@@ -1001,36 +1042,37 @@
         iterator = []
         for ind,item in enumerate(self.items()):
             thistuple = (ind,)+item # Combine into one tuple
             iterator.append(thistuple)
         if transpose: iterator = tuple(scu.transposelist(iterator))
         return iterator
 
-    @staticmethod
-    def promote(obj=None):
+
+    @classmethod
+    def promote(cls, obj=None):
         '''
         Like promotetolist, but for odicts.
 
         **Example**::
 
             od = sc.odict.promote(['There','are',4,'keys'])
 
         Note, in most cases sc.odict(obj) or sc.odict().make(obj) can be used instead.
         '''
         if isinstance(obj, odict):
             return obj # Don't need to do anything
         elif isinstance(obj, dict):
-            return odict(obj)
+            return cls._new(obj)
         elif isinstance(obj, list):
-            newobj = odict()
+            newobj = cls._new()
             for i,val in enumerate(obj):
                 newobj['Key %i'%i] = val
             return newobj
         else:
-            return odict({'Key':obj})
+            return cls._new({'Key':obj})
 
     def keys(self):
         """ Return a list of keys (as in Python 2), not a dict_keys object. """
         return list(OD.keys(self))
 
     def values(self):
         """ Return a list of values (as in Python 2). """
@@ -1040,64 +1082,74 @@
         """ Return a list of items (as in Python 2). """
         iterator = list(OD.items(self))
         if transpose: iterator = tuple(scu.transposelist(iterator))
         return iterator
 
     def dict_keys(self):
         """ Return an iterator (not a list) over keys (as in Python 2). """
-        return OD.keys(self)
+        return dict.keys(self)
 
     def dict_values(self):
         """ Return an iterator (not a list) over values (as in Python 2). """
-        return OD.values(self)
+        return dict.values(self)
 
     def dict_items(self):
         """ Return an iterator (not a list) over items (as in Python 2). """
-        return OD.items(self)
+        return dict.items(self)
 
     def iteritems(self, transpose=False):
         """ Alias to items() """
         return self.items(transpose=transpose)
 
     def makenested(self, *args, **kwargs):
-        ''' Alias to sc.makenested(odict); see sc.makenested() for full documentation. New in version 1.2.0. '''
+        ''' Alias to sc.makenested(odict); see sc.makenested() for full documentation. *New in version 1.2.0.* '''
         return scn.makenested(self, *args, **kwargs)
 
     def getnested(self, *args, **kwargs):
-        ''' Alias to sc.getnested(odict); see sc.makenested() for full documentation. New in version 1.2.0. '''
+        ''' Alias to sc.getnested(odict); see sc.makenested() for full documentation. *New in version 1.2.0.* '''
         return scn.getnested(self, *args, **kwargs)
 
     def setnested(self, *args, **kwargs):
-        ''' Alias to sc.setnested(odict); see sc.makenested() for full documentation. New in version 1.2.0. '''
+        ''' Alias to sc.setnested(odict); see sc.makenested() for full documentation. *New in version 1.2.0.* '''
         return scn.setnested(self, *args, **kwargs)
 
     def iternested(self, *args, **kwargs):
-        ''' Alias to sc.iternested(odict); see sc.makenested() for full documentation. New in version 1.2.0. '''
+        ''' Alias to sc.iternested(odict); see sc.makenested() for full documentation. *New in version 1.2.0.* '''
         return scn.iternested(self, *args, **kwargs)
 
 
 class objdict(odict):
     '''
     An ``odict`` that acts like an object -- allow keys to be set/retrieved by object
     notation.
-
-    For a lighter-weight example, see ``sc.dictobj()``.
-
-    Example
-    -------
-    >>> import sciris as sc
-    >>> od = sc.objdict({'height':1.65, 'mass':59})
-    >>> od.bmi = od.mass/od.height**2
-    >>> od['bmi'] = od['mass']/od['height']**2 # Vanilla syntax still works
-    >>> od.keys = 3 # This raises an exception (you can't overwrite the keys() method)
-
+    
+    In general, operations that would normally act on attributes (e.g. ``obj.x = 3``)
+    instead act on dict keys (e.g. ``obj['x'] = 3``). If you want to actually get/set
+    an attribute, use ``obj.getattribute()``/``obj.setattribute()``.
+    
+    For a lighter-weight example (an object that acts like a dict), see :func:`sc.dictobj() <dictobj>`.
+    
+    **Examples**::
+        
+        import sciris as sc
+        
+        obj = sc.objdict(foo=3, bar=2)
+        obj.foo + obj.bar # Gives 5
+        for key in obj.keys(): # It's still a dict
+            obj[key] = 10
+        
+        od = sc.objdict({'height':1.65, 'mass':59})
+        od.bmi = od.mass/od.height**2
+        od['bmi'] = od['mass']/od['height']**2 # Vanilla syntax still works
+        od.keys = 3 # This raises an exception (you can't overwrite the keys() method)
+    
     Nested logic based in part on addict: https://github.com/mewwts/addict
-
-    For a lighter-weight equivalent (based on ``dict`` instead of ``odict``), see
-    ``sc.dictobj()``.
+    
+    For a lighter-weight equivalent (based on ``dict`` instead of :class:`odict`), see
+    :func:`sc.dictobj() <dictobj>`.
     '''
 
     def __init__(self, *args, **kwargs):
         nested_parent = kwargs.pop('_nested_parent', None)
         nested_attr  = kwargs.pop('_nested_attr', None)
         if nested_parent is not None:
             odict.__setattr__(self, '_nested_parent', nested_parent)
@@ -1139,15 +1191,15 @@
         except Exception as E2: # If that fails, raise the original exception
             try: # Handle defaultdict behavior by first checking if it exists
                 _defaultdict = odict.__getattribute__(self, '_defaultdict')
             except:
                 _defaultdict = None
             if _defaultdict is not None: # If it does, use it, then get the key again
                 if _defaultdict == 'nested':
-                    return self.__class__(defaultdict='nested', _nested_parent=self, _nested_attr=attr) # Create a recursive object with links back to the ultimate parent
+                    return self._new(defaultdict='nested', _nested_parent=self, _nested_attr=attr) # Create a recursive object with links back to the ultimate parent
                 else:
                     dd = _defaultdict() # Create the new object
                     self[attr] = dd # Since we don't know what this object is, we can't be clever about recursion
                     return dd
             else:
                 if exception:
                     raise exception
@@ -1171,15 +1223,15 @@
         return
 
 
     def __delattr__(self, name):
         ''' Delete dict key before deleting actual attribute '''
         try:
             del self[name]
-        except:
+        except: # pragma: no cover
             odict.__delattr__(self, name)
         return
 
 
     def getattribute(self, name):
         ''' Get attribute if truly desired '''
         return odict.__getattribute__(self, name)
@@ -1205,76 +1257,89 @@
     **Example**::
 
         obj = sc.dictobj()
         obj.a = 5
         obj['b'] = 10
         print(obj.items())
 
-    For a more powerful alternative, see ``sc.objdict()``.
-
-    | New in version 1.3.0.
-    | New in version 1.3.1: inherit from dict
-    | New in version 2.0.0: allow positional arguments
+    For a more powerful alternative, see :class:`sc.objdict() <objdict>`.
+    
+    **Note**: because ``dictobj`` is halfway between a dict and an object, it can't 
+    be automatically converted to a JSON (but will fail silently). Use :meth:`to_json() <dictobj.to_json>`
+    instead.
+
+    | *New in version 1.3.0.*
+    | *New in version 1.3.1:* inherit from dict
+    | *New in version 2.0.0:* allow positional arguments
+    | *New in version 3.0.0:* "fromkeys" now a class method; ``to_json()`` method
     '''
 
     def __init__(self, *args, **kwargs):
         kwargs = scu.mergedicts(*args, kwargs)
         for k,v in kwargs.items():
             self.__dict__[k] = v
         return
 
     def __repr__(self):
         output = 'dictobj(' + self.__dict__.__repr__() + ')'
         return output
 
-    def fromkeys(self, *args, **kwargs):
-        return dictobj(self.__dict__.fromkeys(*args, **kwargs))
+    def to_json(self):
+        ''' Export the dictobj to JSON (NB: regular :func:`json.dumps()` does not work) '''
+        return json.dumps(self.__dict__)
+
+    @classmethod
+    def fromkeys(cls, *args, **kwargs):
+        ''' Create a new dictobj from keys '''
+        return cls(dict.fromkeys(*args, **kwargs))
 
     # Copy default dictionary methods
     def __getitem__( self, *args, **kwargs): return self.__dict__.__getitem__( *args, **kwargs)
     def __setitem__( self, *args, **kwargs): return self.__dict__.__setitem__( *args, **kwargs)
     def __contains__(self, *args, **kwargs): return self.__dict__.__contains__(*args, **kwargs)
     def __len__(     self, *args, **kwargs): return self.__dict__.__len__(     *args, **kwargs)
+    def __iter__(    self, *args, **kwargs): return self.__dict__.__iter__(    *args, **kwargs)
     def clear(       self, *args, **kwargs): return self.__dict__.clear(       *args, **kwargs)
     def copy(        self, *args, **kwargs): return self.__dict__.copy(        *args, **kwargs)
     def get(         self, *args, **kwargs): return self.__dict__.get(         *args, **kwargs)
     def items(       self, *args, **kwargs): return self.__dict__.items(       *args, **kwargs)
     def keys(        self, *args, **kwargs): return self.__dict__.keys(        *args, **kwargs)
     def pop(         self, *args, **kwargs): return self.__dict__.pop(         *args, **kwargs)
     def popitem(     self, *args, **kwargs): return self.__dict__.popitem(     *args, **kwargs)
     def setdefault(  self, *args, **kwargs): return self.__dict__.setdefault(  *args, **kwargs)
     def update(      self, *args, **kwargs): return self.__dict__.update(      *args, **kwargs)
     def values(      self, *args, **kwargs): return self.__dict__.values(      *args, **kwargs)
 
 
 def asobj(obj, strict=True):
     '''
-    Convert any object for which you would normally do a['b'] to one where you
-    can do a.b.
+    Convert any object for which you would normally do ``a['b']`` to one where you
+    can do ``a.b``.
 
     Note: this may lead to unexpected behavior in some cases. Use at your own risk.
     At minimum, objects created using this function have an extremely odd type -- namely
-    "sciris.sc_odict.asobj.<locals>.objobj".
+    ``sciris.sc_odict.asobj.<locals>.objobj``.
 
     Args:
         obj (anything): the object you want to convert
         strict (bool): whether to raise an exception if an attribute is being set (instead of a key)
 
     **Example**::
 
         d = dict(foo=1, bar=2)
         d_obj = sc.asobj(d)
         d_obj.foo = 10
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     '''
 
     objtype = type(obj)
 
     class objobj(objtype):
+        ''' Define the "objobj" "type": convert any object to, well, an object. '''
 
         def __getattribute__(self, attr):
             try: # First, try to get the attribute as an attribute
                 output = objtype.__getattribute__(self, attr)
                 return output
             except Exception as E: # pragma: no cover # If that fails, try to get it as a dict item
                 try:
@@ -1286,24 +1351,23 @@
         def __setattr__(self, name, value):
             ''' Set key in dict, not attribute! '''
             try:
                 objtype.__getattribute__(self, name) # Try retrieving this as an attribute, expect AttributeError...
             except AttributeError:
                 return objtype.__setitem__(self, name, value) # If so, simply return
 
-            if not strict: # Let the attribute be set anyway
-                objtype.__setattr__(self, name, value)
+            if not strict: # Let the attribute be set anyway # pragma: no cover
+                return objtype.__setattr__(self, name, value)
             else: # pragma: no cover # Otherwise, raise an exception
                 errormsg = f'"{name}" exists as an attribute, so cannot be set as key; use setattribute() instead'
                 raise ValueError(errormsg)
 
-            return
-
         def getattribute(self, name):
             ''' Get attribute if truly desired '''
             return objtype.__getattribute__(self, name)
 
         def setattribute(self, name, value):
             ''' Set attribute if truly desired '''
             return objtype.__setattr__(self, name, value)
 
-    return objobj(obj)
+
+    return objobj(obj)
```

### Comparing `sciris-2.1.0/sciris/sc_plotting.py` & `sciris-3.0.0/sciris/sc_plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,136 @@
 
 '''
 Extensions to Matplotlib, including 3D plotting and plot customization.
 
 Highlights:
-    - :func:`plot3d`: easy way to render 3D plots
-    - :func:`boxoff`: turn off top and right parts of the axes box
-    - :func:`commaticks`: convert labels from "10000" and "1e6" to "10,000" and "1,000,0000"
-    - :func:`SIticks`: convert labels from "10000" and "1e6" to "10k" and "1m"
-    - :func:`maximize`: make the figure fill the whole screen
-    - :func:`savemovie`: save a sequence of figures as an MP4 or other movie
-    - :func:`fonts`: list available fonts or add new ones
+    - :func:`sc.plot3d() <plot3d>`: easy way to render 3D plots
+    - :func:`sc.boxoff() <boxoff>`: turn off top and right parts of the axes box
+    - :func:`sc.commaticks() <commaticks>`: convert labels from "10000" and "1e6" to "10,000" and "1,000,0000"
+    - :func:`sc.SIticks() <SIticks>`: convert labels from "10000" and "1e6" to "10k" and "1m"
+    - :func:`sc.maximize() <maximize>`: make the figure fill the whole screen
+    - :func:`sc.savemovie() <savemovie>`: save a sequence of figures as an MP4 or other movie
+    - :func:`sc.fonts() <fonts>`: list available fonts or add new ones
 '''
 
 ##############################################################################
 #%% Imports
 ##############################################################################
 
 import os
-import sys
 import tempfile
 import datetime as dt
 import pylab as pl
 import numpy as np
 import matplotlib as mpl
 from . import sc_settings as scs
 from . import sc_odict as sco
 from . import sc_utils as scu
 from . import sc_fileio as scf
 from . import sc_printing as scp
 from . import sc_datetime as scd
+from . import sc_versioning as scv
 
 
 ##############################################################################
 #%% 3D plotting functions
 ##############################################################################
 
 __all__ = ['fig3d', 'ax3d', 'plot3d', 'scatter3d', 'surf3d', 'bar3d']
 
 
-def fig3d(num=None, returnax=False, figkwargs=None, axkwargs=None, **kwargs):
+def fig3d(num=None, nrows=1, ncols=1, index=1, returnax=False, figkwargs=None, axkwargs=None, **kwargs):
     '''
     Shortcut for creating a figure with 3D axes.
 
-    Usually not invoked directly; kwargs are passed to ``pl.figure()``
+    Usually not invoked directly; kwargs are passed to :func:`pl.figure() <matplotlib.pyplot.figure>`
     '''
     figkwargs = scu.mergedicts(figkwargs, kwargs, num=num)
     axkwargs = scu.mergedicts(axkwargs)
 
-    fig,ax = ax3d(returnfig=True, figkwargs=figkwargs, **axkwargs)
-    if returnax:
+    fig = pl.figure(**figkwargs)
+    ax = ax3d(nrows=nrows, ncols=ncols, index=index, returnfig=False, figkwargs=figkwargs, **axkwargs)
+    if returnax: # pragma: no cover
         return fig,ax
     else:
         return fig
 
 
-def ax3d(fig=None, ax=None, returnfig=False, silent=False, elev=None, azim=None, figkwargs=None, axkwargs=None, **kwargs):
+def ax3d(nrows=None, ncols=None, index=None, fig=None, ax=None, returnfig=False, silent=False, 
+         elev=None, azim=None, figkwargs=None, axkwargs=None, **kwargs):
     '''
     Create a 3D axis to plot in.
 
     Usually not invoked directly; kwags are passed to add_subplot()
+    
+    *New in version 3.0.0:* nrows, ncols, and index arguments first
     '''
     from mpl_toolkits.mplot3d import Axes3D # analysis:ignore
 
     figkwargs = scu.mergedicts(figkwargs)
-    axkwargs = scu.mergedicts(axkwargs, kwargs)
-    nrows = axkwargs.pop('nrows', 1) # Since fig.add_subplot() can't handle kwargs...
-    ncols = axkwargs.pop('ncols', 1)
-    index = axkwargs.pop('index', 1)
+    axkwargs = scu.mergedicts(axkwargs, kwargs, nrows=nrows, ncols=ncols, index=index)
+    nrows = axkwargs.pop('nrows', nrows) # Since fig.add_subplot() can't handle kwargs...
+    ncols = axkwargs.pop('ncols', ncols)
+    index = axkwargs.pop('index', index)
+    
+    # Handle the "111" format of subplots
+    try:
+        if ncols is None and index is None:
+            nrows, ncols, index = map(int, str(nrows))
+    except:
+        pass # This is fine, just a different format
 
     # Handle the figure
-    if fig is None:
+    if fig in [True, False] or (fig is None and figkwargs): # Any of these things indicate that we want a new figure
+        fig = pl.figure(**figkwargs)
+    elif fig is None:
         if ax is None:
-            fig = pl.figure(**figkwargs) # It's necessary to have an open figure or else the commands won't work
-        else:
+            if not pl.get_fignums():
+                fig = pl.figure(**figkwargs)
+            else:
+                fig = pl.gcf()
+        else: # pragma: no cover
             fig = ax.figure
             silent = False
     else:
         silent = False # Never close an already open figure
 
     # Create and initialize the axis
     if ax is None:
-        ax = fig.add_subplot(nrows, ncols, index, projection='3d', **axkwargs)
-    if elev is not None or azim is not None:
+        if fig.axes and index is None:
+            ax = pl.gca()
+            if not isinstance(ax, Axes3D):
+                errormsg = f'''Cannot create 3D plot into axes {ax}: ensure "projection='3d'" was used when making it'''
+                raise ValueError(errormsg)
+        else:
+            if nrows is None: nrows = 1
+            if ncols is None: ncols = 1
+            if index is None: index = 1
+            ax = fig.add_subplot(nrows, ncols, index, projection='3d', **axkwargs)
+    
+    if elev is not None or azim is not None: # pragma: no cover
         ax.view_init(elev=elev, azim=azim)
-    if silent:
+    if silent: # pragma: no cover
         pl.close(fig)
     if returnfig:
         return fig,ax
-    else:
+    else: # pragma: no cover
         return ax
 
 
 def plot3d(x, y, z, c=None, fig=None, ax=None, returnfig=False, figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
     '''
     Plot 3D data as a line
 
     Args:
         x (arr): x coordinate data
         y (arr): y coordinate data
         z (arr): z coordinate data
         c (str/tuple): color, can be any of the types accepted by matplotlib's plot()
-        fig (fig): an existing figure to draw the plot in
+        fig (fig): an existing figure to draw the plot in (or set to True to create a new figure)
         ax (axes): an existing axes to draw the plot in
         returnfig (bool): whether to return the figure, or just the axes
         figkwargs (dict): passed to figure()
         axkwargs (dict): passed to axes()
         plotkwargs (dict): passed to plot()
         kwargs (dict): also passed to plot()
 
@@ -118,66 +144,95 @@
     axkwargs = scu.mergedicts(axkwargs)
 
     # Create axis
     fig,ax = ax3d(returnfig=True, fig=fig, ax=ax, figkwargs=figkwargs, **axkwargs)
 
     ax.plot(x, y, z, **plotkwargs)
 
-    if returnfig:
+    if returnfig: # pragma: no cover
         return fig,ax
     else:
         return ax
 
 
-def scatter3d(x, y, z, c=None, fig=None, returnfig=False, figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
+def scatter3d(x, y=None, z=None, c='z', fig=None, ax=None, returnfig=False, figkwargs=None, 
+              axkwargs=None, plotkwargs=None, **kwargs):
     '''
     Plot 3D data as a scatter
+    
+    Typically, ``x``, ``y``, and ``z``, are all vectors. However, if a single 2D
+    array is provided, then this will be treated as ``z`` values and ``x`` and ``y``
+    will be inferred on a grid.
 
     Args:
-        x (arr): x coordinate data
+        x (arr): x coordinate data (or z-coordinate data if 2D and ``z`` is ``None``)
         y (arr): y coordinate data
         z (arr): z coordinate data
-        c (arr): color data
-        fig (fig): an existing figure to draw the plot in
+        c (arr): color data; defaults to match z, explicitly pass ``c=None`` to use default colors
+        fig (fig): an existing figure to draw the plot in (or set to True to create a new figure)
         ax (axes): an existing axes to draw the plot in
         returnfig (bool): whether to return the figure, or just the axes
         figkwargs (dict): passed to figure()
         axkwargs (dict): passed to axes()
         plotkwargs (dict): passed to plot()
         kwargs (dict): also passed to plot()
 
-    **Example**::
+    **Examples**::
 
-        x,y,z = pl.rand(3,10)
-        sc.scatter3d(x, y, z, c=z)
+        # Explicit coordinates
+        x,y,z = np.random.rand(3,50)
+        sc.scatter3d(x, y, z)
+        
+        # Implicit coordinates
+        data = np.random.randn(10, 10)
+        sc.scatter3d(data)
+    
+    *New in version 3.0.0:* allow 2D input.
     '''
     # Set default arguments
     plotkwargs = scu.mergedicts({'s':200, 'depthshade':False, 'linewidth':0}, plotkwargs, kwargs)
     axkwargs = scu.mergedicts(axkwargs)
 
     # Create figure
-    fig,ax = ax3d(returnfig=True, fig=fig, figkwargs=figkwargs, **axkwargs)
+    fig,ax = ax3d(returnfig=True, fig=fig, ax=ax, figkwargs=figkwargs, **axkwargs)
+    
+    # Process data
+    if z is None and x is not None:
+        z,x = x,z # Swap variables so z always exists
+    z = np.array(z)
+    if z.ndim == 2:
+        ny,nx = z.shape
+        if x is None:
+            x = np.arange(nx)
+        if y is None:
+            y = np.arange(ny)
+        if x.ndim == 1 or y.ndim == 1:
+            X,Y = np.meshgrid(x, y)
+        x,y,z = X.flatten(), Y.flatten(), z.flatten() # Flatten everything to 1D
+    if isinstance(c, str) and c == 'z': # Handle automatic color scaling
+        c = z
 
+    # Actually plot
     ax.scatter(x, y, z, c=c, **plotkwargs)
 
-    if returnfig:
+    if returnfig: # pragma: no cover
         return fig,ax
     else:
         return ax
 
 
-def surf3d(data, x=None, y=None, fig=None, returnfig=False, colorbar=True, figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
+def surf3d(data, x=None, y=None, fig=None, ax=None, returnfig=False, colorbar=True, figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
     '''
     Plot 2D data as a 3D surface
 
     Args:
         data (arr): 2D data
         x (arr): 1D vector or 2D grid of x coordinates (optional)
         y (arr): 1D vector or 2D grid of y coordinates (optional)
-        fig (fig): an existing figure to draw the plot in
+        fig (fig): an existing figure to draw the plot in (or set to True to create a new figure)
         ax (axes): an existing axes to draw the plot in
         returnfig (bool): whether to return the figure, or just the axes
         colorbar (bool): whether to plot a colorbar
         figkwargs (dict): passed to figure()
         axkwargs (dict): passed to axes()
         plotkwargs (dict): passed to plot()
         kwargs (dict): also passed to plot()
@@ -189,45 +244,45 @@
     '''
 
     # Set default arguments
     plotkwargs = scu.mergedicts({'cmap':'viridis'}, plotkwargs, kwargs)
     axkwargs = scu.mergedicts(axkwargs)
 
     # Create figure
-    fig,ax = ax3d(returnfig=True, fig=fig, figkwargs=figkwargs, **axkwargs)
+    fig,ax = ax3d(returnfig=True, fig=fig, ax=ax, figkwargs=figkwargs, **axkwargs)
     ny,nx = np.array(data).shape
 
     if x is None:
         x = np.arange(nx)
     if y is None:
         y = np.arange(ny)
 
     if x.ndim == 1 or y.ndim == 1:
         X,Y = np.meshgrid(x, y)
-    else:
+    else: # pragma: no cover
         X,Y = x,y
 
     surf = ax.plot_surface(X, Y, data, **plotkwargs)
     if colorbar:
         fig.colorbar(surf)
 
-    if returnfig:
+    if returnfig: # pragma: no cover
         return fig,ax
     else:
         return ax
 
 
 
-def bar3d(data, fig=None, returnfig=False, cmap='viridis', figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
+def bar3d(data, fig=None, ax=None, returnfig=False, cmap='viridis', figkwargs=None, axkwargs=None, plotkwargs=None, **kwargs):
     '''
     Plot 2D data as 3D bars
 
     Args:
         data (arr): 2D data
-        fig (fig): an existing figure to draw the plot in
+        fig (fig): an existing figure to draw the plot in (or set to True to create a new figure)
         cmap (str): colormap name
         ax (axes): an existing axes to draw the plot in
         returnfig (bool): whether to return the figure, or just the axes
         colorbar (bool): whether to plot a colorbar
         figkwargs (dict): passed to figure()
         axkwargs (dict): passed to axes()
         plotkwargs (dict): passed to plot()
@@ -240,15 +295,15 @@
     '''
 
     # Set default arguments
     plotkwargs = scu.mergedicts({'dx':0.8, 'dy':0.8, 'shade':True}, plotkwargs, kwargs)
     axkwargs = scu.mergedicts(axkwargs)
 
     # Create figure
-    fig,ax = ax3d(returnfig=True, fig=fig, figkwargs=figkwargs, **axkwargs)
+    fig,ax = ax3d(returnfig=True, fig=fig, ax=ax, figkwargs=figkwargs, **axkwargs)
 
     x, y, z = [], [], []
     dz = []
     if 'color' not in plotkwargs:
         try:
             from . import sc_colors as scc # To avoid circular import
             plotkwargs['color'] = scc.vectocolor(data.flatten(), cmap=cmap)
@@ -258,15 +313,15 @@
         for j in range(data.shape[1]):
             x.append(i)
             y.append(j)
             z.append(0)
             dz.append(data[i,j])
     ax.bar3d(x=x, y=y, z=z, dz=dz, **plotkwargs)
 
-    if returnfig:
+    if returnfig: # pragma: no cover
         return fig,ax
     else:
         return ax
 
 
 
 ##############################################################################
@@ -287,84 +342,84 @@
         values    (array)    : the 2D array of values to plot as stacked bars
         colors    (list/arr) : the color of each set of bars
         labels    (list)     : the label for each set of bars
         transpose (bool)     : whether to transpose the array prior to plotting
         flipud    (bool)     : whether to flip the array upside down prior to plotting
         cum       (bool)     : whether the array is already a cumulative sum
         barh      (bool)     : whether to plot as a horizontal instead of vertical bar
-        kwargs    (dict)     : passed to ``pl.bar()``
+        kwargs    (dict)     : passed to :func:`pl.bar() <matplotlib.pyplot.bar>`
     
     **Example**::
         
         values = pl.rand(3,5)
         sc.stackedbar(values, labels=['bottom','middle','top'])
         pl.legend()
     
-    New in version 2.0.4.
+    *New in version 2.0.4.*
     '''
     from . import sc_colors as scc # To avoid circular import
     
     # Handle inputs
     if x is not None and values is None:
         values = x
         x = None
     
-    if values is None: # pragma: nocover
+    if values is None: # pragma: no cover
         errormsg = 'Must supply values to plot, typically as a 2D array'
         raise ValueError(errormsg)
     
     values = scu.toarray(values)
-    if values.ndim == 1: # pragma: nocover
+    if values.ndim == 1: # pragma: no cover
         values = values[None,:] # Convert to a 2D array
     
-    if transpose: # pragma: nocover
+    if transpose: # pragma: no cover
         values = values.T
     
-    if flipud: # pragma: nocover
+    if flipud: # pragma: no cover
         values = values[::-1,:]
     
     nstack = values.shape[0]
     npts = values.shape[1]
     
     if x is None:
         x = np.arange(npts)
         
-    if not cum: # pragma: nocover
+    if not cum: # pragma: no cover
         values = values.cumsum(axis=0)
     values = np.concatenate([np.zeros((1,npts)), values])
 
     # Handle labels and colors
-    if labels is not None: # pragma: nocover
+    if labels is not None: # pragma: no cover
         nlabels = len(labels)
         if nlabels != nstack:
             errormsg = f'Expected {nstack} labels, got {nlabels}'
             raise ValueError(errormsg)
     
-    if colors is not None: # pragma: nocover
+    if colors is not None: # pragma: no cover
         ncolors = len(colors)
         if ncolors != nstack:
             errormsg = f'Expected {nstack} colors, got {ncolors}'
             raise ValueError(errormsg)
     else:
         colors = scc.gridcolors(nstack)
         
     # Actually plot
     artists = []
     for i in range(nstack):
         if labels is not None:
             label = labels[i]
-        else:
+        else: # pragma: no cover
             label = None
         
         h = values[i+1,:]
         b = values[i,:]
         kw = dict(facecolor=colors[i], label=label, **kwargs)
         if not barh:
             artist = pl.bar(x=x, height=h, bottom=b, **kw)
-        else:
+        else: # pragma: no cover
             artist = pl.barh(y=x, width=h, left=b, **kw)
         artists.append(artist)
     
     return artists
 
 
 def boxoff(ax=None, which=None, removeticks=True):
@@ -390,26 +445,26 @@
         pl.plot([1,4,1,4])
         sc.boxoff(ax=ax, which='all')
 
         fig = pl.figure()
         pl.scatter(np.arange(100), pl.rand(100))
         sc.boxoff('top, bottom')
 
-    New in version 1.3.3: ability to turn off multiple spines; removed "flipticks" arguments
+    *New in version 1.3.3:* ability to turn off multiple spines; removed "flipticks" arguments
     '''
     # Handle axes
-    if isinstance(ax, (str, list)): # Swap input arguments
+    if isinstance(ax, (str, list)): # Swap input arguments # pragma: no cover
         ax,which = which,ax
     if ax is None: ax = pl.gca()
 
     # Handle which
     if not isinstance(which, list):
         if which is None:
             which = 'top, right'
-        if which == 'all':
+        if which == 'all': # pragma: no cover
             which = 'top, bottom, right, left'
         if isinstance(which, str):
             which = which.split(',')
             which = [w.rstrip().lstrip() for w in which]
 
     for spine in which: # E.g. ['top', 'right']
         ax.spines[spine].set_visible(False)
@@ -434,20 +489,20 @@
     Note, if you just want to set the lower limit, you can do that
     with this function via::
 
         sc.setaxislim()
     '''
 
     # Handle which axis
-    if which is None:
+    if which is None: # pragma: no cover
         which = 'both'
-    if which not in ['x','y','both']:
+    if which not in ['x','y','both']: # pragma: no cover
         errormsg = f'Setting axis limit for axis {which} is not supported'
         raise ValueError(errormsg)
-    if which == 'both':
+    if which == 'both': # pragma: no cover
         setaxislim(which='x', ax=ax, data=data)
         setaxislim(which='y', ax=ax, data=data)
         return
 
     # Ensure axis exists
     if ax is None:
         ax = pl.gca()
@@ -455,15 +510,15 @@
     # Get current limits
     if   which == 'x': currlower, currupper = ax.get_xlim()
     elif which == 'y': currlower, currupper = ax.get_ylim()
 
     # Calculate the lower limit based on all the data
     lowerlim = 0
     upperlim = 0
-    if scu.checktype(data, 'arraylike'): # Ensure it's numeric data (probably just None)
+    if scu.checktype(data, 'arraylike'): # Ensure it's numeric data (probably just None) # pragma: no cover
         flatdata = scu.toarray(data).flatten() # Make sure it's iterable
         lowerlim = min(lowerlim, flatdata.min())
         upperlim = max(upperlim, flatdata.max())
 
     # Set the new y limits
     if lowerlim<0: lowerlim = currlower # If and only if the data lower limit is negative, use the plotting lower limit
     upperlim = max(upperlim, currupper) # Shouldn't be an issue, but just in case...
@@ -471,31 +526,31 @@
     # Specify the new limits and return
     if   which == 'x': ax.set_xlim((lowerlim, upperlim))
     elif which == 'y': ax.set_ylim((lowerlim, upperlim))
     return lowerlim,upperlim
 
 
 def setxlim(data=None, ax=None):
-    ''' Alias for ``sc.setaxislim(which='x')`` '''
+    ''' Alias for :func:`sc.setaxislim(which='x') <setaxislim>` '''
     return setaxislim(data=data, ax=ax, which='x')
 
 
 def setylim(data=None, ax=None):
     '''
-    Alias for ``sc.setaxislim(which='y')``.
+    Alias for :func:`sc.setaxislim(which='y') <setaxislim>`.
 
     **Example**::
 
         pl.plot([124,146,127])
         sc.setylim() # Equivalent to pl.ylim(bottom=0)
     '''
     return setaxislim(data=data, ax=ax, which='y')
 
 
-def _get_axlist(ax):
+def _get_axlist(ax): # pragma: no cover
     ''' Helper function to turn either a figure, an axes, or a list of axes into a list of axes '''
 
     if ax is None: # If not supplied, get current axes
         axlist = [pl.gca()]
     elif isinstance(ax, pl.Axes): # If it's an axes, turn to a list
         axlist = [ax]
     elif isinstance(ax, pl.Figure): # If it's a figure, pull all axes
@@ -509,15 +564,15 @@
     return axlist
 
 
 def commaticks(ax=None, axis='y', precision=2, cursor_precision=0):
     '''
     Use commas in formatting the y axis of a figure (e.g., 34,000 instead of 34000).
 
-    To use something other than a comma, set the default separator via e.g. ``sc.options(sep='.')``.
+    To use something other than a comma, set the default separator via e.g. :class:`sc.options(sep='.') <ScirisOptions>`.
 
     Args:
         ax (any): axes to modify; if None, use current; else can be a single axes object, a figure, or a list of axes
         axis (str/list): which axis to change (default 'y'; can accept a list)
         precision (int): shift how many decimal places to show for small numbers (+ve = more, -ve = fewer)
         cursor_precision (int): ditto, for cursor
 
@@ -525,17 +580,17 @@
 
         data = pl.rand(10)*1e4
         pl.plot(data)
         sc.commaticks()
 
     See http://stackoverflow.com/questions/25973581/how-to-format-axis-number-format-to-thousands-with-a-comma-in-matplotlib
 
-    | New in version 1.3.0: ability to use non-comma thousands separator
-    | New in version 1.3.1: added "precision" argument
-    | New in version 2.0.0: ability to set x and y axes simultaneously
+    | *New in version 1.3.0:* ability to use non-comma thousands separator
+    | *New in version 1.3.1:* added "precision" argument
+    | *New in version 2.0.0:* ability to set x and y axes simultaneously
     '''
     def commaformatter(x, pos=None): # pragma: no cover
         interval = thisaxis.get_view_interval()
         prec = precision + cursor_precision if pos is None else precision # Use higher precision for cursor
         decimals = int(max(0, prec-np.floor(np.log10(np.ptp(interval)))))
         string = f'{x:0,.{decimals}f}' # Do the formatting
         if pos is not None and '.' in string: # Remove trailing decimal zeros from axis labels
@@ -549,16 +604,16 @@
     sep = scs.options.sep
     axlist = _get_axlist(ax)
     axislist = scu.tolist(axis)
     for ax in axlist:
         for axis in axislist:
             if   axis=='x': thisaxis = ax.xaxis
             elif axis=='y': thisaxis = ax.yaxis
-            elif axis=='z': thisaxis = ax.zaxis
-            else: raise ValueError('Axis must be x, y, or z')
+            elif axis=='z': thisaxis = ax.zaxis # pragma: no cover
+            else: raise ValueError('Axis must be x, y, or z') # pragma: no cover
             thisaxis.set_major_formatter(mpl.ticker.FuncFormatter(commaformatter))
     return
 
 
 
 def SIticks(ax=None, axis='y', fixed=False):
     '''
@@ -571,25 +626,25 @@
 
     **Example**::
 
         data = pl.rand(10)*1e4
         pl.plot(data)
         sc.SIticks()
     '''
-    def SItickformatter(x, pos=None, sigfigs=2, SI=True, *args, **kwargs):  # formatter function takes tick label and tick position
+    def SItickformatter(x, pos=None, sigfigs=2, SI=True, *args, **kwargs):  # formatter function takes tick label and tick position # pragma: no cover
         ''' Formats axis ticks so that e.g. 34000 becomes 34k -- usually not invoked directly '''
         output = scp.sigfig(x, sigfigs=sigfigs, SI=SI) # Pretty simple since scp.sigfig() does all the work
         return output
 
     axlist = _get_axlist(ax)
     for ax in axlist:
         if   axis=='x': thisaxis = ax.xaxis
         elif axis=='y': thisaxis = ax.yaxis
-        elif axis=='z': thisaxis = ax.zaxis
-        else: raise ValueError('Axis must be x, y, or z')
+        elif axis=='z': thisaxis = ax.zaxis # pragma: no cover
+        else: raise ValueError('Axis must be x, y, or z') # pragma: no cover
         if fixed: # pragma: no cover
             ticklocs = thisaxis.get_ticklocs()
             ticklabels = []
             for tickloc in ticklocs:
                 ticklabels.append(SItickformatter(tickloc))
             thisaxis.set_major_formatter(mpl.ticker.FixedFormatter(ticklabels))
         else:
@@ -603,15 +658,15 @@
 
     If you have 37 plots, then how many rows and columns of axes do you know? This
     function convert a number (i.e. of plots) to a number of required rows and columns.
     If nrows or ncols is provided, the other will be calculated. Ties are broken
     in favor of more rows (i.e. 7x6 is preferred to 6x7). It can also generate
     the plots, if ``make=True``.
 
-    Note: ``sc.getrowscols()`` and ``sc.get_rows_cols()`` are aliases.
+    Note: :func:`sc.getrowscols() <getrowscols>` and :func:`sc.get_rows_cols() <get_rows_cols>` are aliases.
 
     Args:
         n (int): the number (of plots) to accommodate
         nrows (int): if supplied, keep this fixed and calculate the columns
         ncols (int): if supplied, keep this fixed and calculate the rows
         ratio (float): sets the number of rows relative to the number of columns (i.e. for 100 plots, 1 will give 10x10, 4 will give 20x5, etc.).
         make (bool): if True, generate subplots
@@ -626,23 +681,23 @@
 
         nrows,ncols = sc.get_rows_cols(36) # Returns 6,6
         nrows,ncols = sc.get_rows_cols(37) # Returns 7,6
         nrows,ncols = sc.get_rows_cols(100, ratio=2) # Returns 15,7
         nrows,ncols = sc.get_rows_cols(100, ratio=0.5) # Returns 8,13 since rows are prioritized
         fig,axs     = sc.getrowscols(37, make=True) # Create 7x6 subplots, using the alias
 
-    | New in version 1.0.0.
-    | New in version 1.2.0: "make", "tight", and "remove_extra" arguments
-    | New in version 1.3.0: alias without underscores
+    | *New in version 1.0.0.*
+    | *New in version 1.2.0:* "make", "tight", and "remove_extra" arguments
+    | *New in version 1.3.0:* alias without underscores
     '''
 
     # Simple cases -- calculate the one missing
-    if nrows is not None:
+    if nrows is not None: # pragma: no cover
         ncols = int(np.ceil(n/nrows))
-    elif ncols is not None:
+    elif ncols is not None: # pragma: no cover
         nrows = int(np.ceil(n/ncols))
 
     # Standard case -- calculate both
     else:
         guess = np.sqrt(n)
         nrows = int(np.ceil(guess*np.sqrt(ratio)))
         ncols = int(np.ceil(n/nrows)) # Could also call recursively!
@@ -673,33 +728,33 @@
         kwargs (dict): passed to fig.subplots_adjust()
 
     **Example**::
 
         fig,axs = sc.get_rows_cols(37, make=True, tight=False) # Create 7x6 subplots, squished together
         sc.figlayout(bottom=0.3)
 
-    New in version 1.2.0.
+    *New in version 1.2.0.*
     '''
-    if isinstance(fig, bool):
+    if isinstance(fig, bool): # pragma: no cover
         fig = None
         tight = fig # To allow e.g. sc.figlayout(False)
     if fig is None:
         fig = pl.gcf()
     layout = ['none', 'tight'][tight]
     try: # Matplotlib >=3.6
         fig.set_layout_engine(layout)
-    except: # Earlier versions
+    except: # Earlier versions # pragma: no cover
         fig.set_tight_layout(tight)
-    if not keep:
-        pl.pause(0.01) # Force refresh
+    if (not keep) and (not pl.get_backend() == 'agg'):
+        pl.pause(0.01) # Force refresh if using an interactive backend
         try:
             fig.set_layout_engine('none')
-        except:
+        except: # pragma: no cover
             fig.set_tight_layout(False)
-    if len(kwargs):
+    if len(kwargs): # pragma: no cover
         fig.subplots_adjust(**kwargs)
     return
 
 
 def maximize(fig=None, die=False):  # pragma: no cover
     '''
     Maximize the current (or supplied) figure. Note: not guaranteed to work for
@@ -710,15 +765,15 @@
         die (bool): whether to propagate an exception if encountered (default no)
 
     **Example**::
 
         pl.plot([2,3,5])
         sc.maximize()
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     '''
     backend = pl.get_backend().lower()
     if fig is not None:
         pl.figure(fig.number) # Set the current figure
     try:
         mgr = pl.get_current_fig_manager()
         if   'qt'  in backend: mgr.window.showMaximized()
@@ -786,48 +841,48 @@
 
         # Handle output
         order = np.argsort(f.names) # Order by name
         for key in keys:
             f[key] = [f[key][o] for o in order]
         if 'name' in output:
             out = f.names
-        elif 'path' in output:
+        elif 'path' in output: # pragma: no cover
             out = dict(zip(f.names, f.paths))
-        elif 'font' in output:
+        elif 'font' in output: # pragma: no cover
             out = dict(zip(f.names, f.objs))
-        else:
+        else: # pragma: no cover
             errormsg = f'Output type not recognized: must be "name", "path", or "font", not "{output}"'
             raise ValueError(errormsg)
         return out
 
     # Or, add new fonts
     else:
 
         # Try, but by default don't crash if they can't be added
         try:
             fontname = None
             fontpaths = []
             paths = scu.tolist(add)
             for path in paths:
                 path = str(path)
-                if os.path.isdir(path):
+                if os.path.isdir(path): # pragma: no cover
                     fps = fm.findSystemFonts(path, **kwargs)
                     fontpaths.extend(fps)
                 else:
                     fontpaths.append(scf.makefilepath(path))
 
-            if dryrun:
+            if dryrun: # pragma: no cover
                 print(fontpaths)
             else:
                 for path in fontpaths:
                     fm.fontManager.addfont(path)
                     fontname = fm.get_font(path).family_name
                     if verbose:
                         print(f'Added "{fontname}"')
-                if verbose and fontname is None:
+                if verbose and fontname is None: # pragma: no cover
                     print('Warning: no fonts were added')
                 if use and fontname: # Set as default font
                     pl.rc('font', family=fontname)
 
             if rebuild: # pragma: no cover
                 print('Rebuilding font cache, please be patient...')
                 try:
@@ -865,21 +920,21 @@
     An adaptation of Matplotlib's ConciseDateFormatter with a slightly different
     approach to formatting dates. Specifically:
 
         - Years are shown below dates, rather than on the RHS
         - The day and month are always shown.
         - The cursor shows only the date, not the time
 
-    This formatter is not intended to be called directly -- use :func:`dateformatter`
+    This formatter is not intended to be called directly -- use :func:`sc.dateformatter() <dateformatter>`
     instead. It is also optimized for plotting dates, rather than times -- for those,
     ConciseDateFormatter is better.
 
-    See :func:`dateformatter` for explanation of arguments.
+    See :func:`sc.dateformatter() <dateformatter>` for explanation of arguments.
 
-    New in version 1.3.0.
+    *New in version 1.3.0.*
     '''
 
     def __init__(self, locator, formats=None, zero_formats=None, show_offset=False, show_year=True, **kwargs):
 
         # Handle inputs
         self.show_year = show_year
         if formats is None:
@@ -903,15 +958,17 @@
 
         # Initialize the ConciseDateFormatter with the corrected input
         super().__init__(locator, formats=formats, zero_formats=zero_formats, show_offset=show_offset, **kwargs)
 
         return
 
     def format_data_short(self, value): # pragma: no cover
-        ''' Show year-month-day, not with hours and seconds '''
+        '''
+        Show year-month-day, not with hours and seconds
+        '''
         return pl.num2date(value, tz=self._tz).strftime('%Y-%b-%d')
 
     def format_ticks(self, values): # pragma: no cover
         '''
         Append the year to the tick label for the first label, or if the year changes.
         This avoids the need to use offset_text, which is difficult to control.
         '''
@@ -942,26 +999,26 @@
     '''
     Format the x-axis to use a given date formatter.
 
     By default, this will apply the Sciris date formatter to the current x-axis.
     This formatter is a combination of Matplotlib's Concise date formatter, and
     Plotly's date formatter.
 
-    See also ``sc.datenumformatter()`` to convert a numeric axis to date labels.
+    See also :func:`sc.datenumformatter() <datenumformatter>` to convert a numeric axis to date labels.
 
     Args:
         ax         (axes)     : if supplied, use these axes instead of the current one
         style      (str)      : the style to use if the axis already uses dates; options are "sciris", "auto", "concise", or a Formatter object
         dateformat (str)      : the date format (default ``'%Y-%b-%d'``; not needed if x-axis already uses dates)
         start      (str/int)  : if supplied, the lower limit of the axis
         end        (str/int)  : if supplied, the upper limit of the axis
         rotation   (float)    : rotation of the labels, in degrees
         locator    (Locator)  : if supplied, use this instead of the default ``AutoDateLocator`` locator
         axis       (str)      : which axis to apply to the formatter to (default 'x')
-        kwargs     (dict)     : passed to the date formatter (e.g., ``ScirisDateFormatter``)
+        kwargs     (dict)     : passed to the date formatter (e.g., :class:`ScirisDateFormatter`)
 
     **Examples**::
 
         # Reformat date data
         pl.figure()
         x = sc.daterange('2021-04-04', '2022-05-05', asdate=True)
         y = sc.smooth(pl.rand(len(x)))
@@ -969,26 +1026,26 @@
         sc.dateformatter()
 
         # Configure with Matplotlib's Concise formatter
         fig,ax = pl.subplots()
         pl.plot(sc.date(np.arange(365), start_date='2022-01-01'), pl.randn(365))
         sc.dateformatter(ax=ax, style='concise')
 
-    | New in version 1.2.0.
-    | New in version 1.2.2: "rotation" argument; renamed "start_day" to "start_date"
-    | New in version 1.3.0: refactored to use built-in Matplotlib date formatting
-    | New in version 1.3.2: "axis" argument
-    | New in version 1.3.3: split ``sc.dateformatter()`` from ``sc.datenumformatter()``
+    | *New in version 1.2.0.*
+    | *New in version 1.2.2:* "rotation" argument; renamed "start_day" to "start_date"
+    | *New in version 1.3.0:* refactored to use built-in Matplotlib date formatting
+    | *New in version 1.3.2:* "axis" argument
+    | *New in version 1.3.3:* split ``sc.dateformatter()`` from ``sc.datenumformatter()``
     '''
 
     # Handle deprecation
     style = kwargs.pop('dateformatter', style) # Allow this as an alias
 
     # Handle axis
-    if isinstance(ax, str): # Swap style and axes -- allows sc.dateformatter(ax) or sc.dateformatter('auto')
+    if isinstance(ax, str): # Swap style and axes -- allows sc.dateformatter(ax) or sc.dateformatter('auto') # pragma: no cover
         style = ax
         ax = None
     if ax is None:
         ax = pl.gca()
 
     # Handle dateformat, if provided
     if dateformat is not None: # pragma: no cover
@@ -1007,24 +1064,24 @@
     style = str(style).lower()
     if style in ['none', 'sciris', 'house', 'default']:
         formatter = ScirisDateFormatter(locator, **kwargs)
     elif style in ['auto', 'matplotlib']:
         formatter = mpl.dates.AutoDateFormatter(locator, **kwargs)
     elif style in ['concise', 'brief']:
         formatter = mpl.dates.ConciseDateFormatter(locator, **kwargs)
-    elif isinstance(style, mpl.ticker.Formatter): # If a formatter is provided, use directly
+    elif isinstance(style, mpl.ticker.Formatter): # If a formatter is provided, use directly # pragma: no cover
         formatter = style
-    else:
+    else: # pragma: no cover
         errormsg = f'Style "{style}" not recognized; must be one of "sciris", "auto", or "concise"'
         raise ValueError(errormsg)
 
     # Handle axis and set the locator and formatter
     if axis == 'x':
         axis = ax.xaxis
-    elif axis == 'y': # If it's not x or y (!), assume it's an axis object
+    elif axis == 'y': # If it's not x or y (!), assume it's an axis object # pragma: no cover
         axis = ax.yaxis
     axis.set_major_locator(locator)
     axis.set_major_formatter(formatter)
 
     # Handle limits
     xmin, xmax = ax.get_xlim()
     if start: xmin = scd.date(start)
@@ -1042,15 +1099,15 @@
 
 
 def datenumformatter(ax=None, start_date=None, dateformat=None, interval=None, start=None,
                      end=None, rotation=None):
     '''
     Format a numeric x-axis to use dates.
 
-    See also ``sc.dateformatter()``, which is intended for use when the axis already
+    See also :func:`sc.dateformatter() <dateformatter>`, which is intended for use when the axis already
     has date data.
 
     Args:
         ax         (axes)     : if supplied, use these axes instead of the current one
         start_date (str/date) : the start day, either as a string or date object (not needed if x-axis already uses dates)
         dateformat (str)      : the date format (default ``'%Y-%b-%d'``; not needed if x-axis already uses dates)
         interval   (int)      : if supplied, the interval between ticks (not needed if x-axis already uses dates)
@@ -1065,148 +1122,139 @@
         sc.datenumformatter(start_date='2021-01-01')
 
         # Manually configure
         fig,ax = pl.subplots()
         ax.plot(np.arange(60), np.random.random(60))
         formatter = sc.datenumformatter(start_date='2020-04-04', interval=7, start='2020-05-01', end=50, dateformat='%m-%d', ax=ax)
 
-    | New in version 1.2.0.
-    | New in version 1.2.2: "rotation" argument; renamed "start_day" to "start_date"
-    | New in version 1.3.3: renamed from ``sc.dateformatter()`` to  ``sc.datenumformatter()``
+    | *New in version 1.2.0.*
+    | *New in version 1.2.2:* "rotation" argument; renamed "start_day" to "start_date"
+    | *New in version 1.3.3:* renamed from ``sc.dateformatter()`` to  ``sc.datenumformatter()``
     '''
 
     # Handle axis
-    if isinstance(ax, str): # Swap inputs
+    if isinstance(ax, str): # Swap inputs # pragma: no cover
         ax, start_date = start_date, ax
     if ax is None:
         ax = pl.gca()
 
     # Set the default format -- "2021-01-01"
     if dateformat is None:
         dateformat = '%Y-%b-%d'
 
     # Convert to a date object
-    if start_date is None:
+    if start_date is None: # pragma: no cover
         start_date = pl.num2date(ax.dataLim.x0)
     start_date = scd.date(start_date)
 
     @mpl.ticker.FuncFormatter
-    def formatter(x, pos):
+    def formatter(x, pos): # pragma: no cover
         return (start_date + dt.timedelta(days=int(x))).strftime(dateformat)
 
     # Handle limits
     xmin, xmax = ax.get_xlim()
     if start: xmin = scd.day(start, start_date=start_date)
     if end:   xmax = scd.day(end,   start_date=start_date)
     ax.set_xlim((xmin, xmax))
 
     # Set the x-axis intervals
-    if interval:
+    if interval: # pragma: no cover
         ax.set_xticks(np.arange(xmin, xmax+1, interval))
 
     # Set the rotation
-    if rotation:
+    if rotation: # pragma: no cover
         ax.tick_params(axis='x', labelrotation=rotation)
 
     # Set the formatter
     ax.xaxis.set_major_formatter(formatter)
 
     return formatter
 
 
 ##############################################################################
 #%% Figure saving
 ##############################################################################
 
-__all__ += ['savefig', 'loadmetadata', 'savefigs', 'loadfig', 'emptyfig', 'separatelegend', 'orderlegend']
+__all__ += ['savefig', 'savefigs', 'loadfig', 'emptyfig', 'separatelegend', 'orderlegend']
 
 
-_metadataflag = 'sciris_metadata' # Key name used to identify metadata saved in a figure
-
 
 def _get_dpi(dpi=None, min_dpi=200):
     ''' Helper function to choose DPI for saving figures '''
     if dpi is None:
         mpl_dpi = pl.rcParams['savefig.dpi']
         if mpl_dpi == 'figure':
             mpl_dpi = pl.rcParams['figure.dpi']
         dpi = max(mpl_dpi, min_dpi) # Don't downgrade DPI
     return dpi
 
 
-def savefig(filename, fig=None, dpi=None, comments=None, freeze=False, frame=2, folder=None, makedirs=True, die=True, verbose=True, **kwargs):
+def savefig(filename, fig=None, dpi=None, comments=None, pipfreeze=False, relframe=0, 
+            folder=None, makedirs=True, die=True, verbose=True, **kwargs):
     '''
     Save a figure, including metadata
 
-    Wrapper for Matplotlib's ``savefig()`` function which automatically stores
+    Wrapper for Matplotlib's :func:`pl.savefig() <matplotlib.pyplot.savefig>` function which automatically stores
     metadata in the figure. By default, it saves (git) information from the calling
     function. Additional comments can be added to the saved file as well. These
-    can be retrieved via ``sc.loadmetadata()``.
+    can be retrieved via :func:`sc.loadmetadata() <loadmetadata>`.
 
     Metadata can be stored and retrieved for PNG or SVG. Metadata
     can be stored for PDF, but cannot be automatically retrieved.
 
     Args:
-        filename (str/Path) : name of the file to save to
-        fig      (Figure)   : the figure to save (if None, use current)
-        dpi      (int)      : resolution of the figure to save (default 200 or current default, whichever is higher)
-        comments (str)      : additional metadata to save to the figure
-        freeze   (bool)     : whether to store the contents of ``pip freeze`` in the metadata (warning, slow)
-        frame    (int)      : which calling file to try to store information from (default, the file calling ``sc.savefig()``)
-        folder   (str/Path) : optional folder to save to (can also be provided as part of the filename)
-        makedirs (bool)     : whether to create folders if they don't already exist
-        die      (bool)     : whether to raise an exception if metadata can't be saved
-        verbose  (bool)     : if die is False, print a warning if metadata can't be saved
-        kwargs   (dict)     : passed to ``fig.save()``
+        filename  (str/Path) : name of the file to save to
+        fig       (Figure)   : the figure to save (if None, use current)
+        dpi       (int)      : resolution of the figure to save (default 200 or current default, whichever is higher)
+        comments  (str)      : additional metadata to save to the figure
+        pipfreeze (bool)     : whether to store the contents of ``pip freeze`` in the metadata
+        relframe  (int)      : which calling file to try to store information from (default 0, the file calling :func:`sc.savefig() <savefig>`)
+        folder    (str/Path) : optional folder to save to (can also be provided as part of the filename)
+        makedirs  (bool)     : whether to create folders if they don't already exist
+        die       (bool)     : whether to raise an exception if metadata can't be saved
+        verbose   (bool)     : if die is False, print a warning if metadata can't be saved
+        kwargs    (dict)     : passed to ``fig.save()``
 
     **Examples**::
 
         pl.plot([1,3,7])
 
         sc.savefig('example1.png')
         print(sc.loadmetadata('example1.png'))
 
         sc.savefig('example2.png', comments='My figure', freeze=True)
         sc.pp(sc.loadmetadata('example2.png'))
-
-    New in version 1.3.3.
+    
+    | *New in version 1.3.3.*
+    | *New in version 3.0.0:* "freeze" renamed "pipfreeze"; "frame" replaced with "relframe"; replaced metadata with ``sc.metadata()``
     '''
-
+    # Handle deprecation
+    orig_metadata = kwargs.pop('metadata', {}) # In case metadata is supplied, as it can be for fig.save()
+    pipfreeze     = kwargs.pop('freeze', pipfreeze) 
+    frame         = kwargs.pop('frame', None)
+    if frame is not None: # pragma: no cover
+        relframe = frame - 2
+    
     # Handle figure
     if fig is None:
         fig = pl.gcf()
 
     # Handle DPI
     dpi = _get_dpi(dpi)
 
     # Get caller and git info
-    caller = scu.getcaller(frame=frame, tostring=False)
-    gitinfo = scu.gitinfo(caller['filename'], die=False, verbose=False) # Don't print any git errors
-
-    # Construct metadata
-    metadata = kwargs.pop('metadata', {})
-    metadata['timestamp'] = scd.getdate()
-    metadata['calling_file'] = caller
-    metadata['git_info'] = gitinfo
-    if comments:
-        metadata['comments'] = comments
-    if freeze:
-        metadata['python'] = dict(platform=sys.platform, executable=sys.executable, version=sys.version)
-        metadata['modules'] = scu.freeze()
-
-    # Convert to a string
-    jsonstr = scf.jsonify(metadata, tostring=True) # PDF and SVG doesn't support storing a dict
+    jsonstr = scv.metadata(relframe=relframe+1, pipfreeze=pipfreeze, comments=comments, tostring=True, **orig_metadata)
 
     # Handle different formats
     filename = str(filename)
     lcfn = filename.lower() # Lowercase filename
     if lcfn.endswith('png'):
-        metadata = {_metadataflag:jsonstr}
-    elif lcfn.endswith('svg') or lcfn.endswith('pdf'):
-        metadata = dict(Keywords=f'{_metadataflag}={jsonstr}')
+        metadata = {scv._metadataflag:jsonstr}
+    elif lcfn.endswith('svg') or lcfn.endswith('pdf'): # pragma: no cover
+        metadata = dict(Keywords=f'{scv._metadataflag}={jsonstr}')
     else:
         errormsg = f'Warning: filename "{filename}" has unsupported type for metadata: must be PNG, SVG, or PDF. For JPG, use the separate exif library. To silence this message, set die=False and verbose=False.'
         if die:
             raise ValueError(errormsg)
         else:
             metadata = None
             if verbose:
@@ -1218,113 +1266,14 @@
 
     # Allow savefig to make directories
     filepath = scf.makefilepath(filename=filename, folder=folder, makedirs=makedirs)
     fig.savefig(filepath, dpi=dpi, **kwargs)
     return filename
 
 
-def loadmetadata(filename, load_all=False, die=True):
-    '''
-    Read metadata from a saved image; currently only PNG and SVG are supported.
-
-    Only for use with images saved with ``sc.savefig()``. Metadata retrieval for PDF
-    is not currently supported.
-
-    Args:
-        filename (str): the name of the file to load the data from
-        load_all (bool): whether to load all metadata available in an image (else, just load what was saved by Sciris)
-        die (bool): whether to raise an exception if the metadata can't be found
-
-    **Example**::
-
-        pl.plot([1,2,3], [4,2,6])
-        sc.savefig('example.png')
-        sc.loadmetadata('example.png')
-    '''
-
-    # Initialize
-    metadata = {}
-    lcfn = str(filename).lower() # Lowercase filename
-
-    # Handle bitmaps
-    is_png = lcfn.endswith('png')
-    is_jpg = lcfn.endswith('jpg') or lcfn.endswith('jpeg')
-    if is_png or is_jpg:
-        try:
-            import PIL
-        except ImportError as E: # pragma: no cover
-            errormsg = f'Pillow import failed ({str(E)}), please install first (pip install pillow)'
-            raise ImportError(errormsg) from E
-        im = PIL.Image.open(filename)
-        keys = im.info.keys()
-
-        # Usual case, can find metadata and is PNG
-        if is_png and (load_all or _metadataflag in keys):
-            if load_all:
-                metadata = im.info
-            else:
-                jsonstr = im.info[_metadataflag]
-                metadata = scf.loadjson(string=jsonstr)
-
-        # JPG -- from https://www.thepythoncode.com/article/extracting-image-metadata-in-python
-        elif is_jpg: # pragma: no cover
-            from PIL.ExifTags import TAGS # Must be imported directly
-            exifdata = im.getexif()
-            for tag_id in exifdata:
-                tag = TAGS.get(tag_id, tag_id)
-                data = exifdata.get(tag_id)
-                if isinstance(data, bytes):
-                    data = data.decode()
-                metadata[tag] = data
-
-        # Can't find metadata
-        else: # pragma: no cover
-            errormsg = f'Could not find "{_metadataflag}": metadata can only be extracted from figures saved with sc.savefig().\nAvailable keys are: {scu.strjoin(keys)}'
-            if die:
-                raise ValueError(errormsg)
-            else:
-                print(errormsg)
-                metadata = im.info
-
-
-    # Handle SVG
-    elif lcfn.endswith('svg'): # pragma: no cover
-
-        # Load SVG as text and parse it
-        svg = scf.loadtext(filename).splitlines()
-        flag = _metadataflag + '=' # Start of the line
-        end = '</'
-
-        found = False
-        for line in svg:
-            if flag in line:
-                found = True
-                break
-
-        # Usual case, can find metadata
-        if found:
-            jsonstr = line[line.find(flag)+len(flag):line.find(end)]
-            metadata = scf.loadjson(string=jsonstr)
-
-        # Can't find metadata
-        else:
-            errormsg = f'Could not find the string "{_metadataflag}" anywhere in "{filename}": metadata can only be extracted from figures saved with sc.savefig()'
-            if die:
-                raise ValueError(errormsg)
-            else:
-                print(errormsg)
-
-    # Other formats not supported
-    else: # pragma: no cover
-        errormsg = f'Filename "{filename}" has unsupported type: must be PNG, JPG, or SVG (PDF is not supported)'
-        raise ValueError(errormsg)
-
-    return metadata
-
-
 def savefigs(figs=None, filetype=None, filename=None, folder=None, savefigargs=None, aslist=False, verbose=False, **kwargs):
     '''
     Save the requested plots to disk.
 
     Args:
         figs        (list) : the figure objects to save
         filetype    (str)  : the file type; can be 'fig', 'singlepdf' (default), or anything supported by savefig()
@@ -1360,27 +1309,27 @@
     nfigs = len(figs)
 
     # Handle file types
     filenames = []
     if filetype=='singlepdf': # See http://matplotlib.org/examples/pylab_examples/multipage_pdf.html  # pragma: no cover
         from matplotlib.backends.backend_pdf import PdfPages
         defaultname = 'figures.pdf'
-        fullpath = scf.makefilepath(filename=filename, folder=folder, default=defaultname, ext='pdf')
+        fullpath = scf.makefilepath(filename=filename, folder=folder, default=defaultname, ext='pdf', makedirs=True)
         pdf = PdfPages(fullpath)
         filenames.append(fullpath)
         if verbose: print(f'PDF saved to {fullpath}')
     for p,item in enumerate(figs.items()):
         key,plt = item
         # Handle filename
         if filename and nfigs==1: # Single plot, filename supplied -- use it
-            fullpath = scf.makefilepath(filename=filename, folder=folder, default='Figure', ext=filetype) # NB, this filename not used for singlepdf filetype, so it's OK
+            fullpath = scf.makefilepath(filename=filename, folder=folder, default='Figure', ext=filetype, makedirs=True) # NB, this filename not used for singlepdf filetype, so it's OK
         else: # Any other case, generate a filename # pragma: no cover
             keyforfilename = filter(str.isalnum, str(key)) # Strip out non-alphanumeric stuff for key
             defaultname = keyforfilename
-            fullpath = scf.makefilepath(filename=filename, folder=folder, default=defaultname, ext=filetype)
+            fullpath = scf.makefilepath(filename=filename, folder=folder, default=defaultname, ext=filetype, makedirs=True)
 
         # Do the saving
         if savefigargs is None: savefigargs = {}
         defaultsavefigargs = {'dpi':200, 'bbox_inches':'tight'} # Specify a higher default DPI and save the figure tightly
         defaultsavefigargs.update(savefigargs) # Update the default arguments with the user-supplied arguments
         if filetype == 'fig':
             scf.save(fullpath, plt)
@@ -1395,15 +1344,15 @@
                 filenames.append(fullpath)
                 if verbose: print(f'{filetype.upper()} plot saved to {fullpath}')
             pl.close(plt)
 
     # Do final tidying
     if filetype=='singlepdf': pdf.close()
     if wasinteractive: pl.ion()
-    if aslist or len(filenames)>1:
+    if aslist or len(filenames)>1: # pragma: no cover
         return filenames
     else:
         return filenames[0]
 
 
 def loadfig(filename=None):
     '''
@@ -1419,15 +1368,15 @@
     **Later**::
 
         example = sc.loadfig('example.fig')
     '''
     pl.ion() # Without this, it doesn't show up
     try:
         fig = scf.loadobj(filename)
-    except Exception as E:
+    except Exception as E: # pragma: no cover
         errormsg = f'Unable to open file "{filename}": are you sure it was saved as a .fig file (not an image)?'
         raise type(E)(errormsg) from E
     
     reanimateplots(fig)
     
     return fig
 
@@ -1438,15 +1387,15 @@
         from matplotlib.backends.backend_agg import new_figure_manager_given_figure as nfmgf # Warning -- assumes user has agg on their system, but should be ok. Use agg since doesn't require an X server
     except Exception as E: # pragma: no cover
         errormsg = f'To reanimate plots requires the "agg" backend, which could not be imported: {repr(E)}'
         raise ImportError(errormsg) from E
     
     if len(pl.get_fignums()):
         fignum = pl.gcf().number # This is the number of the current active figure, if it exists
-    else:
+    else: # pragma: no cover
         fignum = 1
         
     plots = scu.mergelists(plots) # Convert to an odict
     for plot in plots:
         nfmgf(fignum, plot) # Make sure each figure object is associated with the figure manager -- WARNING, is it correct to associate the plot with an existing figure?
     
     return
@@ -1466,15 +1415,15 @@
          - A list of handles, where each handle contains the label
          - An axis object, containing the objects that should appear in the legend
          - A figure object, from which the first axis will be used
     '''
     if handles is None:
         if ax is None:
             ax = pl.gca()
-        elif isinstance(ax, pl.Figure): # Allows an argument of a figure instead of an axes
+        elif isinstance(ax, pl.Figure): # Allows an argument of a figure instead of an axes # pragma: no cover
             ax = ax.axes[-1]
         handles, labels = ax.get_legend_handles_labels()
     else: # pragma: no cover
         if labels is None:
             labels = [h.get_label() for h in handles]
         else:
             assert len(handles) == len(labels), f"Number of handles ({len(handles)}) and labels ({len(labels)}) must match"
@@ -1564,18 +1513,18 @@
 __all__ += ['animation', 'savemovie']
 
 
 class animation(scu.prettyobj):
     '''
     A class for storing and saving a Matplotlib animation.
 
-    See also ``sc.savemovie()``, which works directly with Matplotlib artists rather
+    See also :func:`sc.savemovie() <savemovie>`, which works directly with Matplotlib artists rather
     than an entire figure. Depending on your use case, one is likely easier to use
-    than the other. Use ``sc.animation()`` if you want to animate a complex figure
-    including non-artist objects (e.g., titles and legends); use ``sc.savemovie()``
+    than the other. Use :func:`sc.animation() <animation>` if you want to animate a complex figure
+    including non-artist objects (e.g., titles and legends); use :func:`sc.savemovie() <savemovie>`
     if you just want to animate a set of artists (e.g., lines).
 
     This class works by saving snapshots of the figure to disk as image files, then
     reloading them either via ``ffmpeg`` or as a Matplotlib animation. While (slightly)
     slower than working with artists directly, it means that anything that can be
     rendered to a figure can be animated.
 
@@ -1586,26 +1535,25 @@
         filename     (str):  the name of the output animation (default: animation.mp4)
         dpi          (int):  the resolution to save the animation at
         fps          (int):  frames per second for the animation
         imageformat  (str):  file type for temporary image files, e.g. 'jpg'
         basename     (str):  name for temporary image files, e.g. 'myanimation'
         nametemplate (str):  as an alternative to imageformat and basename, specify the full name template, e.g. 'myanimation%004d.jpg'
         imagefolder  (str):  location to store temporary image files; default current folder, or use 'tempfile' to create a temporary folder
-        anim_args    (dict): passed to ``matplotlib.animation.ArtistAnimation()`` or ``ffmpeg.input()``
-        save_args    (dict): passed to ``matplotlib.animation.save()`` or ``ffmpeg.run()``
+        anim_args    (dict): passed to :obj:`matplotlib.animation.ArtistAnimation` or ``ffmpeg.input()``
+        save_args    (dict): passed to :meth:`animation.save() <matplotlib.animation.Animation.save>` or ``ffmpeg.run()``
         tidy         (bool): whether to delete temporary files
         verbose      (bool): whether to print progress
-        kwargs       (dict): also passed to ``matplotlib.animation.save()``
+        kwargs       (dict): also passed to :meth:`animation.save() <matplotlib.animation.Animation.save>`
 
     **Example**::
 
         anim = sc.animation()
 
         pl.figure()
-        pl.seed(1)
         repeats = 21
         colors = sc.vectocolor(repeats, cmap='turbo')
         for i in range(repeats):
             scale = 1/np.sqrt(i+1)
             x = scale*pl.randn(10)
             y = scale*pl.randn(10)
             label = str(i) if not(i%5) else None
@@ -1613,16 +1561,16 @@
             pl.title(f'Scale = 1/√{i}')
             pl.legend()
             sc.boxoff('all')
             anim.addframe()
 
         anim.save('dots.mp4')
 
-    | New in version 1.3.3.
-    | New in version 2.0.0: ``ffmpeg`` option.
+    | *New in version 1.3.3.*
+    | *New in version 2.0.0:* ``ffmpeg`` option.
     '''
     def __init__(self, fig=None, filename=None, dpi=200, fps=10, imageformat='png', basename='animation', nametemplate=None,
                  imagefolder=None, anim_args=None, save_args=None, frames=None, tidy=True, verbose=True, **kwargs):
         self.fig          = fig
         self.filename     = filename
         self.dpi          = dpi
         self.fps          = fps
@@ -1643,15 +1591,15 @@
         return
 
 
     def initialize(self):
         ''' Handle additional initialization of variables '''
 
         # Handle folder
-        if self.imagefolder == 'tempfile':
+        if self.imagefolder == 'tempfile': # pragma: no cover
             self.imagefolder = tempfile.gettempdir()
         if self.imagefolder is None:
             self.imagefolder = os.getcwd()
         self.imagefolder = scf.path(self.imagefolder)
 
         # Handle name template
         if self.nametemplate is None:
@@ -1682,42 +1630,42 @@
             errormsg = f'Name template "{self.nametemplate}" does not seem valid for inserting current file number {self.n_files} into: should contain the string "%04d" or similar'
             raise TypeError(errormsg) from E
         if path:
             name = self.imagefolder / name
         return name
 
 
-    def __add__(self, *args, **kwargs):
+    def __add__(self, *args, **kwargs): # pragma: no cover
         ''' Allow anim += fig '''
         self.addframe(*args, **kwargs)
         return self
 
-    def __radd__(self, *args, **kwargs):
+    def __radd__(self, *args, **kwargs): # pragma: no cover
         ''' Allow anim += fig '''
         self.addframe(self, *args, **kwargs)
         return self
 
     @property
     def n_files(self):
         return len(self.filenames)
 
     @property
     def n_frames(self):
         return len(self.frames)
 
-    def __len__(self):
+    def __len__(self): # pragma: no cover
         ''' Since we can have either files or frames, need to check both  '''
         return max(self.n_files, self.n_frames)
 
 
     def addframe(self, fig=None, *args, **kwargs):
         ''' Add a frame to the animation -- typically a figure object, but can also be an artist or list of artists '''
 
         # If a figure is supplied but it's not a figure, add it to the frames directly
-        if fig is not None and isinstance(fig, (list, mpl.artist.Artist)):
+        if fig is not None and isinstance(fig, (list, mpl.artist.Artist)): # pragma: no cover
             self.frames.append(fig)
 
         # Typical case: add a figure
         else:
             if self.verbose and self.n_files == 0: # First frame
                 print('Adding frames...')
 
@@ -1730,22 +1678,22 @@
             # Check figure properties
             fig_size = fig.get_size_inches()
             fig_dpi = fig.get_dpi()
 
             if self.fig_size is None:
                 self.fig_size = fig_size
             else:
-                if not np.allclose(self.fig_size, fig_size):
+                if not np.allclose(self.fig_size, fig_size): # pragma: no cover
                     warnmsg = f'Note: current figure size {fig_size} does not match saved {self.fig_size}, unexpected results may occur!'
                     print(warnmsg)
 
             if self.fig_dpi is None:
                 self.fig_dpi = fig_dpi
             else:
-                if self.fig_dpi != fig_dpi:
+                if self.fig_dpi != fig_dpi: # pragma: no cover
                     warnmsg = f'Note: current figure DPI {fig_dpi} does not match saved {self.fig_dpi}, unexpected results may occur!'
                     print(warnmsg)
 
             if self.verbose:
                 print(f'  Added frame {self.n_files}: {self._getfilename(path=False)}')
 
         return
@@ -1762,65 +1710,65 @@
                 scp.progressbar(f+1, self.filenames)
             im = pl.imread(filename)
             self.frames.append(ax.imshow(im))
         pl.close(animfig)
         return
 
 
-    def __enter__(self, *args, **kwargs):
+    def __enter__(self, *args, **kwargs): # pragma: no cover
         ''' To allow with...as '''
         return self
 
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args, **kwargs): # pragma: no cover
         ''' Save on exist from a with...as block '''
         return self.save()
 
 
     def rmfiles(self):
         ''' Remove temporary image files '''
         succeeded = 0
         failed = scu.autolist()
         for filename in self.filenames:
             if os.path.exists(filename):
                 try:
                     os.remove(filename)
                     succeeded += 1
-                except Exception as E:
+                except Exception as E: # pragma: no cover
                     failed += f'{filename} ({E})'
         if self.verbose:
             if succeeded:
                 print(f'Removed {succeeded} temporary files')
-        if failed:
+        if failed: # pragma: no cover
             print(f'Failed to remove the following temporary files:\n{scu.newlinejoin(failed)}')
 
 
     def save(self, filename=None, fps=None, dpi=None, engine='ffmpeg', anim_args=None,
              save_args=None, frames=None, tidy=None, verbose=True, **kwargs):
-        ''' Save the animation -- arguments the same as ``sc.animation()`` and ``sc.savemovie()``, and are described there '''
+        ''' Save the animation -- arguments the same as :func:`sc.animation() <animation>` and :func:`sc.savemovie() <savemovie>`, and are described there '''
 
         # Handle engine
         if engine == 'ffmpeg':
             try:
                 import ffmpeg
             except:
                 print('Warning: engine ffmpeg not available; falling back to Matplotlib. Run "pip install ffmpeg-python" to use in future.')
                 engine = 'matplotlib'
         engines = ['ffmpeg', 'matplotlib']
-        if engine not in engines:
+        if engine not in engines: # pragma: no cover
             errormsg = f'Could not understand engine "{engine}": must be one of {scu.strjoin(engines)}'
             raise ValueError(errormsg)
 
         # Handle dictionary args
         anim_args = scu.mergedicts(self.anim_args, anim_args)
         save_args = scu.mergedicts(self.save_args, save_args)
 
         # Handle filename
         if filename is None:
-            if self.filename is None:
+            if self.filename is None: # pragma: no cover
                 self.filename = f'{self.basename}.mp4'
             filename = self.filename
 
         # Set parameters
         if fps  is None: fps  = save_args.pop('fps', self.fps)
         if dpi  is None: dpi  = save_args.pop('dpi', self.dpi)
         if tidy is None: tidy = self.tidy
@@ -1869,43 +1817,43 @@
             self.rmfiles()
 
         if verbose:
             print(f'Done; movie saved to "{filename}"')
             try: # Not essential, so don't try too hard if this doesn't work
                 filesize = os.path.getsize(filename)
                 if filesize<1e6: print(f'File size: {filesize/1e3:0.0f} KB')
-                else:            print(f'File size: {filesize/1e6:0.1f} MB')
-            except:
+                else:            print(f'File size: {filesize/1e6:0.1f} MB') # pragma: no cover
+            except: # pragma: no cover
                 pass
             T.toc(label='Time saving movie')
 
         return
 
 
 def savemovie(frames, filename=None, fps=None, quality=None, dpi=None, writer=None, bitrate=None,
               interval=None, repeat=False, repeat_delay=None, blit=False, verbose=True, **kwargs):
     '''
     Save a set of Matplotlib artists as a movie.
 
-    Note: in most cases, it is preferable to use ``sc.animation()``.
+    Note: in most cases, it is preferable to use :func:`sc.animation() <animation>`.
 
     Args:
         frames (list): The list of frames to animate
         filename (str): The name (or full path) of the file; expected to end with mp4 or gif (default movie.mp4)
         fps (int): The number of frames per second (default 10)
         quality (string): The quality of the movie, in terms of dpi (default "high" = 300 dpi)
         dpi (int): Instead of using quality, set an exact dpi
-        writer (str or object): Specify the writer to be passed to matplotlib.animation.save() (default "ffmpeg")
+        writer (str or object): Specify the writer to be passed to :meth:`animation.save() <matplotlib.animation.Animation.save>` (default "ffmpeg")
         bitrate (int): The bitrate. Note, may be ignored; best to specify in a writer and to pass in the writer as an argument
         interval (int): The interval between frames; alternative to using fps
         repeat (bool): Whether or not to loop the animation (default False)
         repeat_delay (bool): Delay between repeats, if repeat=True (default None)
         blit (bool): Whether or not to "blit" the frames (default False, since otherwise does not detect changes )
         verbose (bool): Whether to print statistics on finishing.
-        kwargs (dict): Passed to ``matplotlib.animation.save()``
+        kwargs (dict): Passed to :meth:`animation.save() <matplotlib.animation.Animation.save>`
 
     Returns:
         A Matplotlib animation object
 
     **Examples**::
 
         import pylab as pl
@@ -1941,53 +1889,53 @@
             old_dots = pl.vstack([old_dots, dots]) # Store the new dots as old dots
         sc.savemovie(frames, 'fleeing_dots.mp4', fps=20, quality='high') # Save movie as a high-quality mp4
 
     Version: 2019aug21
     '''
     from matplotlib import animation as mpl_anim # Place here since specific only to this function
 
-    if not isinstance(frames, list):
+    if not isinstance(frames, list): # pragma: no cover
         errormsg = f'sc.savemovie(): argument "frames" must be a list, not "{type(frames)}"'
         raise TypeError(errormsg)
     for f in range(len(frames)):
-        if not scu.isiterable(frames[f]):
+        if not scu.isiterable(frames[f]): # pragma: no cover
             frames[f] = (frames[f],) # This must be either a tuple or a list to work with ArtistAnimation
 
     # Try to get the figure from the frames, else use the current one
     try:    fig = frames[0][0].get_figure()
     except: fig = pl.gcf()
 
     # Set parameters
-    if filename is None:
+    if filename is None: # pragma: no cover
         filename = 'movie.mp4'
     if writer is None:
         if   filename.endswith('mp4'): writer = 'ffmpeg'
         elif filename.endswith('gif'): writer = 'imagemagick'
-        else:
+        else: # pragma: no cover
             errormsg = f'sc.savemovie(): unknown movie extension for file {filename}'
             raise ValueError(errormsg)
     if fps is None:
         fps = 10
     if interval is None:
         interval = 1000./fps
         fps = 1000./interval # To ensure it's correct
 
     # Handle dpi/quality
     if dpi is None and quality is None:
         quality = 'medium' # Make it medium quailty by default
-    if isinstance(dpi, str):
+    if isinstance(dpi, str): # pragma: no cover
         quality = dpi # Interpret dpi arg as a quality command
         dpi = None
     if dpi is not None and quality is not None:
         print(f'sc.savemovie() warning: quality is simply a shortcut for dpi; please specify one or the other, not both (dpi={dpi}, quality={quality})')
     if quality is not None:
         if   quality == 'low':    dpi =  50
         elif quality == 'medium': dpi = 150
-        elif quality == 'high':   dpi = 300
-        else:
+        elif quality == 'high':   dpi = 300 # pragma: no cover
+        else: # pragma: no cover
             errormsg = f'Quality must be high, medium, or low, not "{quality}"'
             raise ValueError(errormsg)
 
     # Optionally print progress
     if verbose:
         start = scd.tic()
         print(f'Saving {len(frames)} frames at {fps} fps and {dpi} dpi to "{filename}" using {writer}...')
@@ -1997,13 +1945,13 @@
     anim.save(filename, writer=writer, fps=fps, dpi=dpi, bitrate=bitrate, **kwargs)
 
     if verbose:
         print(f'Done; movie saved to "{filename}"')
         try: # Not essential, so don't try too hard if this doesn't work
             filesize = os.path.getsize(filename)
             if filesize<1e6: print(f'File size: {filesize/1e3:0.0f} KB')
-            else:            print(f'File size: {filesize/1e6:0.2f} MB')
-        except:
+            else:            print(f'File size: {filesize/1e6:0.2f} MB') # pragma: no cover
+        except: # pragma: no cover
             pass
         scd.toc(start)
 
     return anim
```

### Comparing `sciris-2.1.0/sciris/sc_printing.py` & `sciris-3.0.0/sciris/sc_printing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 '''
 Printing/notification functions.
 
 Highlights:
-    - :func:`heading`: print text as a 'large' heading
-    - :func:`colorize`: print text in a certain color
-    - :func:`pr`: print full representation of an object, including methods and each attribute
-    - :func:`sigfigs`: truncate a number to a certain number of significant figures
-    - :func:`progressbar`: show a (text-based) progress bar
-    - :func:`capture`: capture text output (e.g., stdout) as a variable
+    - :func:`sc.heading() <heading>`: print text as a 'large' heading
+    - :func:`sc.colorize() <colorize>`: print text in a certain color
+    - :func:`sc.pr() <pr>`: print full representation of an object, including methods and each attribute
+    - :func:`sc.sigfig() <sigfig>`: truncate a number to a certain number of significant figures
+    - :func:`sc.progressbar() <progressbar>`: show a (text-based) progress bar
+    - :func:`sc.capture() <capture>`: capture text output (e.g., stdout) as a variable
 '''
 
 import io
 import os
 import sys
 import time
+import tqdm
 import pprint
 import numpy as np
 import collections as co
 from textwrap import fill
 from collections import UserString
 from contextlib import redirect_stdout
+from ._extras import ansicolors as ac
 from . import sc_utils as scu
-from . import ansicolors as ac
 
 
 # Add Windows support for colors (do this at the module level so that colorama.init() only gets called once)
 if scu.iswindows(): # pragma: no cover # NB: can't use startswith() because of 'cygwin'
     try:
         import colorama
         colorama.init()
@@ -68,17 +69,17 @@
     return output
 
 
 def objatt(obj, strlen=18, ncol=3):
     ''' Return a sorted string of object attributes for the Python __repr__ method '''
     if   hasattr(obj, '__dict__'):  oldkeys = sorted(obj.__dict__.keys())
     elif hasattr(obj, '__slots__'): oldkeys = sorted(obj.__slots__)
-    else:                           oldkeys = []
+    else:                           oldkeys = [] # pragma: no cover
     if len(oldkeys): output = createcollist(oldkeys, 'Attributes', strlen = 18, ncol = 3)
-    else:            output = ''
+    else:            output = '' # pragma: no cover
     return output
 
 
 def objmeth(obj, strlen=18, ncol=3):
     ''' Return a sorted string of object methods for the Python __repr__ method '''
     try:
         oldkeys = sorted([method + '()' for method in dir(obj) if callable(getattr(obj, method)) and not method.startswith('__')])
@@ -121,31 +122,35 @@
         attrs = objatt(obj)
         if attrs:
             output += attrs
             output += divider
     return output
 
 
-def prepr(obj, maxlen=None, maxitems=None, skip=None, dividerchar='—', dividerlen=60, use_repr=True, maxtime=3, die=False):
+def prepr(obj, maxlen=None, maxitems=None, skip=None, dividerchar='—', dividerlen=60, 
+          use_repr=True, maxtime=3, die=False, debug=False):
     '''
     Akin to "pretty print", returns a pretty representation of an object --
     all attributes (except any that are skipped), plust methods and ID. Usually
-    used via the interactive sc.pr() (which prints), rather than this (which returns
+    used via the interactive :func:`sc.pr() <pr>` (which prints), rather than this (which returns
     a string).
 
     Args:
         obj (anything): the object to be represented
         maxlen (int): maximum number of characters to show for each item
         maxitems (int): maximum number of items to show in the object
         skip (list): any properties to skip
         dividerchar (str): divider for methods, attributes, etc.
         dividerlen (int): number of divider characters
         use_repr (bool): whether to use repr() or str() to parse the object
         maxtime (float): maximum amount of time to spend on trying to print the object
         die (bool): whether to raise an exception if an error is encountered
+        debug (bool): print out detail during string construction
+    
+    *New in version 3.0.0:* "debug" argument
     '''
 
     # Decide how to handle representation function -- repr is dangerous since can lead to recursion
     repr_fn = repr if use_repr else str
     T = time.time() # Start the timer
     time_exceeded = False
 
@@ -158,56 +163,47 @@
 
     # Initialize things to print out
     labels = []
     values = []
 
     # Wrap entire process in a try-except in case it fails
     try:
-        if not (hasattr(obj, '__dict__') or hasattr(obj, '__slots__')):
+        if not (hasattr(obj, '__dict__') or hasattr(obj, '__slots__')): # pragma: no cover
             # It's a plain object
             labels = [f'{type(obj)}']
             values = [repr_fn(obj)]
         else:
             if hasattr(obj, '__dict__'):
                 labels = sorted(set(obj.__dict__.keys()) - set(skip))  # Get the dict attribute keys
             else:
                 labels = sorted(set(obj.__slots__) - set(skip))  # Get the slots attribute keys
+            if debug: # pragma: no cover
+                print(f'Working on {len(labels)} entries...')
 
             if len(labels):
-                extraitems = len(labels) - maxitems
-                if extraitems>0:
+                extraitems = max(0, len(labels) - maxitems)
+                if extraitems > 0:
                     labels = labels[:maxitems]
                 values = []
                 for a,attr in enumerate(labels):
+                    if debug: # pragma: no cover
+                        print(f'  Working on attribute {a}: {attr}...')
                     if (time.time() - T) < maxtime:
                         try: value = repr_fn(getattr(obj, attr))
-                        except: value = 'N/A'
+                        except: value = 'N/A' # pragma: no cover
                         values.append(value)
                     else:
                         labels = labels[:a]
                         labels.append('etc. (time exceeded)')
                         values.append(f'{len(labels)-a} entries not shown')
                         time_exceeded = True
                         break
             else:
-                items = dir(obj)
-                extraitems = len(items) - maxitems
-                if extraitems > 0:
-                    items = items[:maxitems]
-                for a,attr in enumerate(items):
-                    if not attr.startswith('__'):
-                        if (time.time() - T) < maxtime:
-                            try:    value = repr_fn(getattr(obj, attr))
-                            except: value = 'N/A'
-                            labels.append(attr)
-                            values.append(value)
-                        else:
-                            labels.append('etc. (time exceeded)')
-                            values.append(f'{len(labels)-a} entries not shown')
-                            time_exceeded = True
+                extraitems = 0
+                
             if extraitems > 0:
                 labels.append('etc. (too many items)')
                 values.append(f'{extraitems} entries not shown')
 
         # Decide how to print them
         maxkeylen = 0
         if len(labels):
@@ -216,14 +212,16 @@
             maxlen = maxlen - maxkeylen # Shorten the amount of data shown if the keys are long
         formatstr = '%'+ '%i'%maxkeylen + 's' # Assemble the format string for the keys, e.g. '%21s'
         output  = objrepr(obj, showatt=False, dividerchar=dividerchar, dividerlen=dividerlen) # Get the methods
         for label,value in zip(labels,values): # Loop over each attribute
             if len(value)>maxlen: value = value[:maxlen] + ' [...]' # Shorten it
             prefix = formatstr%label + ': ' # The format key
             output += indent(prefix, value)
+        if not len(labels):
+            output += 'No attributes\n'
         output += divider
         if time_exceeded:
             timestr = f'\nNote: the object did not finish printing within maxtime={maxtime} s.\n'
             timestr += 'To see the full object, call prepr() with increased maxtime.'
             output += timestr
 
     # If that failed, try progressively simpler approaches
@@ -232,22 +230,27 @@
             errormsg = 'Failed to create pretty representation of object'
             raise RuntimeError(errormsg) from E
         else:
             try: # Next try the objrepr, which is the same except doesn't print attribute values
                 output = objrepr(obj, dividerchar=dividerchar, dividerlen=dividerlen)
                 output += f'\nWarning: showing simplified output since full repr failed {str(E)}'
             except: # If that fails, try just the string representation
-                output = str(obj)
+                try:
+                    output = str(obj)
+                except: # And if that fails, try the most basic object representation
+                    output = object.__repr__(obj)
 
     return output
 
 
 def pr(obj, *args, **kwargs):
     '''
-    Shortcut for printing the pretty repr for an object -- similar to prettyprint
+    Pretty-print the detailed representation of an object.
+
+    See :func:`sc.prepr() <prepr>` for options.
 
     **Example**::
 
         import pandas as pd
         df = pd.DataFrame({'a':[1,2,3], 'b':[4,5,6]})
         print(df) # See just the data
         sc.pr(df) # See all the methods too
@@ -273,28 +276,28 @@
     Args:
         prefix (str): text to begin with (optional)
         text (str): text to wrap
         suffix (str): what to put on the end (by default, a newline)
         n (int): if prefix is not specified, the size of the indent
         pretty (bool): whether to use pprint to format the text
         width (int): maximum width before wrapping (if None, don't wrap)
-        kwargs (dict): passed to ``textwrap.fill()``
+        kwargs (dict): passed to :func:`textwrap.fill()`
 
     **Examples**::
 
         prefix = 'and then they said: '
         text = 'blah '*100
         print(sc.indent(prefix, text))
 
         print('my fave is: ' + sc.indent(text=rand(100), n=12))
 
-    New in version 1.3.1: more flexibility in arguments
+    *New in version 1.3.1:* more flexibility in arguments
     '''
     # If "prefix" is given but text isn't, swap them
-    if text is None and prefix is not None:
+    if text is None and prefix is not None: # pragma: no cover
         text, prefix = prefix, text
 
     # Handle prefix and width
     if prefix is None: prefix = ' '*n
     if width  is None: width = 999_999
 
     # Get text in the right format -- i.e. a string
@@ -318,62 +321,63 @@
     if n: output = output[n:] # Need to remove the fake prefix
     return output
 
 
 
 #%% Data representation functions
 
-__all__ += ['sigfig', 'printarr', 'printdata', 'printvars']
+__all__ += ['sigfig', 'sigfigs', 'arraymean', 'arraymedian', 'printmean', 'printmedian', 
+            'humanize_bytes', 'printarr', 'printdata', 'printvars']
 
 
-def sigfig(x, sigfigs=5, SI=False, sep=False, keepints=False):
+def sigfig(x, sigfigs=4, SI=False, sep=False, keepints=False):
     '''
     Return a string representation of variable x with sigfigs number of significant figures
 
+    Note: :func:`sc.sigfig() <sigfig>` and :func:`sc.sigfigs() <sigfigs>` are aliases.
+
     Args:
-        x (int/float/arr): the number(s) to round
+        x (int/float/list/arr): the number(s) to round
         sigfigs (int): number of significant figures to round to
-        SI (bool): whether to use SI notation
+        SI (bool): whether to use SI notation (only for numbers >1)
         sep (bool/str): if provided, use as thousands separator
         keepints (bool): never round ints
 
-    **Examples**::
+    **Examples**:
 
-        x = 32433.3842
-        sc.sigfig(x, SI=True) # Returns 32.433k
-        sc.sigfig(x, sep=True) # Returns 32,433
+        x = 3432.3842
+        sc.sigfig(x, SI=True) # Returns 3.432k
+        sc.sigfig(x, sep=True) # Returns 3,432
+        
+        vals = np.random.rand(5)
+        sc.sigfig(vals, sigfigs=3)
+    
+    *New in version 3.0.0:* changed default number of significant figures from 5 to 4; return list rather than tuple; changed SI suffixes to uppercase
     '''
     output = []
 
-    try:
-        n=len(x)
-        X = x
-        islist = True
-    except:
-        X = [x]
-        n = 1
-        islist = False
-    for i in range(n):
-        x = X[i]
-
+    islist = scu.isiterable(x)
+    istuple = isinstance(x, tuple)
+    xlist = x if islist else scu.tolist(x)
+    for x in xlist:
         suffix = ''
-        formats = [(1e18,'e18'), (1e15,'e15'), (1e12,'t'), (1e9,'b'), (1e6,'m'), (1e3,'k')]
+        formats = [(1e18,'e18'), (1e15,'e15'), (1e12,'T'), (1e9,'B'), (1e6,'M'), (1e3,'K')]
         if SI:
             for val,suff in formats:
-                if abs(x)>=val:
+                if abs(x) >= val:
                     x = x/val
                     suffix = suff
                     break # Find at most one match
 
         try:
-            if x==0:
+            if x == 0:
                 output.append('0')
             elif sigfigs is None:
                 output.append(scu.flexstr(x)+suffix)
-            elif x>(10**sigfigs) and not SI and keepints: # e.g. x = 23432.23, sigfigs=3, output is 23432
+            elif x > (10**sigfigs) and not SI and keepints: # e.g. x = 23432.23, sigfigs=3, output is 23432
                 roundnumber = int(round(x))
                 if sep: string = format(roundnumber, ',')
                 else:   string = f'{x:0.0f}'
                 output.append(string)
             else:
                 magnitude = np.floor(np.log10(abs(x)))
                 factor = 10**(sigfigs-magnitude-1)
@@ -387,71 +391,246 @@
                     else:           roundnumber = int(string)
                     string = format(roundnumber, ',') # Allow comma separator
                 string += suffix
                 output.append(string)
         except: # pragma: no cover
             output.append(scu.flexstr(x))
     if islist:
-        return tuple(output)
+        if istuple:
+            output = tuple(output)
+        return output
     else:
         return output[0]
 
+# Alias to avoid confusion
+sigfigs = sigfig
+
+
+def arraymean(data, stds=2, mean_sf=None, err_sf=None, doprint=False, **kwargs):
+    '''
+    Quickly calculate the mean and standard deviation of an array.
+    
+    By default, will calculate the correct number of significant figures based on
+    the deviation.
+    
+    Args:
+        data (array): the data to summarize
+        stds (int): the number of multiples of the standard deviation to show (default 2; can also use 1)
+        mean_sf (int): if provided, use this number of significant figures for the mean rather than the auto-calculated
+        err_sf (int): ditto, but for the error (standard deviation)
+        doprint (bool): whether to print (else, return the string)
+        kwargs (dict): passed to :func:`sc.sigfig() <sigfig>`
+    
+    **Example**::
+        
+        data = [1210, 1072, 1722, 1229, 1902]
+        sc.printmean(data) # Returns 1430 ± 320
+    
+    *New in version 3.0.0.*
+    '''
+    vsf = mean_sf # vsf = "value significant figures"
+    esf = err_sf if err_sf is not None else 2
+    data = scu.toarray(data)
+    val = data.mean()
+    err = data.std()*stds
+    
+    relsize = np.floor(np.log10(abs(val))) - np.floor(np.log10(abs(err)))
+    if vsf is None:
+        vsf = esf + relsize
+    elif vsf is not None and err_sf is None:
+        esf = min(vsf, vsf - relsize)
+        
+    valstr = sigfig(val, vsf, **kwargs)
+    errstr = sigfig(err, esf, **kwargs)
+    string = f'{valstr} ± {errstr}'
+    
+    if doprint:
+        print(string)
+    else:
+        return string
+
 
-def printarr(arr, fmt=None, colsep='  ', vsep='—', decimals=2, dtype=None):
+def arraymedian(data, ci=95, sf=3, doprint=False, **kwargs):
+    '''
+    Quickly calculate the median and confidence interval of an array.
+    
+    The confidence interval defaults to 95%. If an integer is supplied, this is
+    treated as a percentile (e.g. 95=95% CI). If a float is supplied, it's treated
+    as a quantile (e.g. 0.95=95% CI). If a pair of ints or floats is provided, these are
+    treated as upper and lower percentiles/quantiles. If 'iqr' is provided, then
+    print the interquartile range (equivalent to 50% CI). If 'range' is provided
+    then print the full range (equivalent to 100% CI).
+    
+    Args:
+        data (array): the data to summarize
+        ci (int/float/list/str): the confidence interval to use to use (see above for details)
+        sf (int): number of significant figures to use
+        doprint (bool): whether to print (else, return the string)
+        kwargs (dict): passed to :func:`sc.sigfig() <sigfig>`
+    
+    **Examples**::
+        
+        data = [1210, 1072, 1722, 1229, 1902]
+        sc.printmedian(data, 80) # Returns '1230 (80.0% CI: 1130, 1830)'
+    
+    *New in version 3.0.0.*
+    '''
+    # Handle quantiles
+    if ci is None: # pragma: no cover
+        ci = 95
+    elif str(ci).lower() == 'iqr':
+        ci = 50
+    elif str(ci).lower() in ['range', 'minmax']:
+        ci = 100
+        
+    if scu.isnumber(ci):
+        if isinstance(ci, int):
+            x = ci/100/2
+        elif isinstance(ci, float):
+            x = ci/2
+        quantiles = [0.5-x, 0.5+x]
+        if x == 0.25:
+            cistr = 'IQR'
+        elif x == 0.5:
+            cistr = 'min, max'
+        else:
+            cistr = f'{x*100*2:n}% CI'
+    elif scu.isiterable(ci):
+        if len(ci) != 2: # pragma: no cover
+            errormsg = f'If providing a list of quantiles, must provide 2, not {len(ci)}'
+            raise ValueError(errormsg)
+        quantiles = ci
+        for i,q in enumerate(quantiles):
+            if isinstance(q, int):
+                quantiles[i] = q/100
+        cistr = f'{quantiles[0]*100:n}%, {quantiles[1]*100:n}%'
+    else: # pragma: no cover
+        errormsg = f'Could not understand confidence interval "{ci}"'
+        raise ValueError(errormsg)
+    
+    # Do calculations
+    data    = scu.toarray(data)
+    median  = np.quantile(data, 0.5)
+    bounds  = np.quantile(data, quantiles)
+    relsize = np.floor(np.log10(abs(median))) - np.floor(np.log10(np.abs(bounds)))
+        
+    # Assemble string
+    valstr  = sigfig(median, sf, **kwargs)
+    lowstr  = sigfig(bounds[0], sf-relsize[0], **kwargs)
+    highstr = sigfig(bounds[1], sf-relsize[1], **kwargs)
+    string = f'{valstr} ({cistr}: {lowstr}, {highstr})'
+    
+    if doprint:
+        print(string)
+    else:
+        return string
+
+
+def printmean(*args, doprint=True, **kwargs):
+    ''' Alias to :func:`sc.arraymean() <arraymean>` with doprint=True '''
+    return arraymean(*args, doprint=doprint, **kwargs)
+
+
+def printmedian(*args, doprint=True, **kwargs):
+    ''' Alias to :func:`sc.arraymedian() <arraymedian>` with doprint=True '''
+    return arraymedian(*args, doprint=doprint, **kwargs)
+
+
+def humanize_bytes(bytesize, decimals=3):
+    '''
+    Convert a number of bytes into a human-readable total.
+    
+    Args:
+        bytesize (int): the number of bytes
+        decimals (int): the number of decimal places to show
+    
+    **Example**::
+        
+        sc.humansize(2.3423887e6, decimals=2) # Returns '2.34 MB'
+        
+    See the humansize library for more flexibility.
+    
+    *New in version 3.0.0.*
+    '''
+    # Convert to string
+    factor = 1
+    label = 'B'
+    labels = ['KB','MB','GB']
+    for i,f in enumerate([3,6,9]):
+        if bytesize >= 10**f:
+            factor = 10**f
+            label = labels[i]
+    if factor == 1:
+        decimals = 0 # Do not show decimals for bytes
+    humansize = float(bytesize/float(factor))
+    string = f'{humansize:0.{decimals}f} {label}'
+    return string
+
+
+
+def printarr(arr, fmt=None, colsep='  ', vsep='—', decimals=2, doprint=True, dtype=None):
     '''
     Print a numpy array nicely.
     
     Args:
         arr (array): the array to print
         fmt (str): the formatting string to use
         colsep (str): the separator between columns of values
         vsep (str): the vertical separator between 2D slices
+        decimals (int): number of decimal places to print
+        doprint (bool): whether to print (else, return the string)
 
     **Examples**::
 
         numeric = pl.randn(3,7,4)**10
         mixed = np.array([['cat', 'nudibranch'], [23, 2423482]], dtype=object)
         sc.printarr(numeric)
         sc.printarr(mixed)
 
-    New in version 2.0.3: "fmt", "colsep", "vsep", "decimals", and "dtype" arguments
+    *New in version 2.0.3:* "fmt", "colsep", "vsep", "decimals", and "dtype" arguments
+    *New in version 3.0.0:* "doprint" argument
     '''
     from . import sc_math as scm # To avoid circular import
+    
+    string = ''
     arr = scu.toarray(arr, dtype=dtype)
     if fmt is None:
-        if arr.dtype == object:
+        if arr.dtype == object: # pragma: no cover
             maxdigits = max([len(str(v)) for v in arr.flatten()])
             fmt = f'%{maxdigits}s'
         else:
             maxdigits = scm.numdigits(arr.max())
             if arr.dtype == float:
                 fmt = f'%{maxdigits+decimals+1}.{decimals}f'
-            else:
+            else: # pragma: no cover
                 fmt = f'%{maxdigits}.0f'
     if np.ndim(arr)==1:
-        string = ''
         for i in range(len(arr)):
             string += fmt % arr[i] + colsep
-        print(string)
+        string += '\n'
     elif np.ndim(arr)==2:
         for i in range(len(arr)):
-            printarr(arr[i], fmt, colsep)
+            string += printarr(arr[i], fmt, colsep, doprint=False) + '\n'
     elif np.ndim(arr)==3:
         for i in range(len(arr)):
             ncols  = len(arr[i][0])
             vlen   = len(fmt % arr.flatten()[0])
             seplen = len(colsep)
             n = ncols*(vlen + seplen) - seplen
-            print(vsep*n)
+            string += vsep*n + '\n'
             for j in range(len(arr[i])):
-                printarr(arr[i][j], fmt, colsep)
+                string += printarr(arr[i][j], fmt, colsep, doprint=False)
     else: # pragma: no cover
         print('Dimensions higher than 3 are not supported')
-        print(arr) # Give up
-    return
+        string = str(arr) # Give up
+    
+    if doprint:
+        print(string)
+    else:
+        return string
 
 
 
 def printdata(data, name='Variable', depth=1, maxlen=40, indent='', level=0, showcontents=False): # pragma: no cover
     '''
     Nicely print a complicated data structure, a la Matlab.
 
@@ -537,15 +716,15 @@
     if label:  print(f'Variables for {label}:')
     if divider: print(dividerstr)
     for varnum,varname in enumerate(varlist):
         controlstr = f'{varnum}. "{varname}": ' # Basis for the control string -- variable number and name
         if color: controlstr = colorize(color, output=True) + controlstr + colorize('reset', output=True) # Optionally add color
         if spaces>1: controlstr += '\n' # Add a newline if the variables are going to be on different lines
         try:    controlstr += f'{localvars[varname]}' # The variable to be printed
-        except: controlstr += 'WARNING, could not be printed' # In case something goes wrong
+        except: controlstr += 'Warning, could not be printed' # In case something goes wrong # pragma: no cover
         controlstr += '\n' * spaces # The number of spaces to add between variables
         print(controlstr), # Print it out
     if divider: print(dividerstr) # If necessary, print the divider again
     return
 
 
 
@@ -560,32 +739,32 @@
     Colorize output text.
 
     Args:
         color (str): the color you want (use 'bg' with background colors, e.g. 'bgblue'); alternatively, use fg, bg, and style
         string (str): the text to be colored
         doprint (bool): whether to print the string (default true unless output)
         output (bool): whether to return the modified version of the string (default false)
-        enable (bool): switch to allow ``sc.colorize()`` to be easily turned off without converting to a ``print()`` statement
+        enable (bool): switch to allow :func:`sc.colorize() <colorize>` to be easily turned off without converting to a :func:`print()` statement
         showhelp (bool): show help rather than changing colors
         fg (str): foreground colour
         bg (str): background colour
         style (str): font style (eg, italic, underline, bold)
 
     **Examples**::
 
         sc.colorize('green', 'hi') # Simple example
         sc.colorize(['yellow', 'bgblack']); print('Hello world'); print('Goodbye world'); colorize() # Colorize all output in between
         bluearray = sc.colorize(color='blue', string=str(range(5)), output=True); print("c'est bleu: " + bluearray)
         sc.colorize('magenta') # Now type in magenta for a while
         sc.colorize() # Stop typing in magenta
         sc.colorize('cat in the hat', fg='#ffa044', bg='blue', style='italic+underline') # Alternate usage example
 
-    To get available colors, type ``sc.colorize(showhelp=True)``.
+    To get available colors, type :func:`sc.colorize(showhelp=True) <colorize>`.
 
-    | New in version 1.3.1: "doprint" argument; ansicolors shortcut
+    | *New in version 1.3.1:* "doprint" argument; ansicolors shortcut
     '''
 
     # Handle short-circuit case
     if not enable: # pragma: no cover
         if output:
             return string
         else:
@@ -596,20 +775,20 @@
     ansistring = ''
     alt_usage = (fg is not None) or (bg is not None) or (style is not None)
 
     # Handle alternate usage pattern -- string as first argument rather than color, so swap
     if alt_usage:
         if string is None and color is not None:
             string, color = color, string
-        if color is not None:
+        if color is not None: # pragma: no cover
             errormsg = 'You can supply either color or fg, but not both'
             raise ValueError(errormsg)
 
         if ansi_support: ansistring = ac.color(s=string, fg=fg, bg=bg, style=style) # Actually apply color
-        else:            ansistring = str(string) # Otherwise, just return the string
+        else:            ansistring = str(string) # Otherwise, just return the string # pragma: no cover
 
     # Original use case
     else:
 
         # Define ANSI colors
         ansicolors = co.OrderedDict([
             ('black', '30'),
@@ -642,15 +821,15 @@
         ansicolor = ''
         for color in colorlist:
             ansicolor += ansicolors[color]
 
         # Modify string, if supplied
         if string is None: ansistring = ansicolor # Just return the color
         else:              ansistring = ansicolor + str(string) + ansicolors['reset'] # Add to start and end of the string
-        if not ansi_support:
+        if not ansi_support: # pragma: no cover
             ansistring = str(string) # To avoid garbling output on unsupported systems
 
     if showhelp:
         print('Available colors are:')
         for key in ansicolors.keys():
             if key[:2] == 'bg':
                 darks = ['bgblack', 'bgred', 'bgblue', 'bgmagenta']
@@ -686,52 +865,46 @@
     return print(ac.yellow(s, **kwargs))
 
 def printmagenta(s, **kwargs):
     ''' Alias to print(colors.magenta(s)) '''
     return print(ac.magenta(s, **kwargs))
 
 
-def heading(string=None, *args, color=None, divider=None, spaces=None, spacesafter=None, minlength=None, maxlength=None, sep=' ', doprint=None, output=False, **kwargs):
+def heading(string='', *args, color='cyan', divider='—', spaces=2, spacesafter=1, 
+            minlength=10, maxlength=200, sep=' ', doprint=None, output=False, **kwargs):
     '''
     Create a colorful heading. If just supplied with a string (or list of inputs like print()),
     create blue text with horizontal lines above and below and 3 spaces above. You
     can customize the color, the divider character, how many spaces appear before
     the heading, and the minimum length of the divider (otherwise will expand to
     match the length of the string, up to a maximum length).
 
     Args:
         string      (str):  the string to print as the heading (or object to convert to a string)
         args        (list): additional strings to print
         color       (str):  color to use for the heading (default cyan)
         divider     (str):  symbol to use for the divider (default '—')
-        spaces      (int):  number of spaces to put before the heading (default 3)
+        spaces      (int):  number of spaces to put before the heading (default 2)
         spacesafter (int):  number of spaces to put after the heading (default 1)
-        minlength   (int):  minimum length of the divider (default 30)
-        maxlength   (int):  maximum length of the divider (default 120)
+        minlength   (int):  minimum length of the divider (default 10)
+        maxlength   (int):  maximum length of the divider (default 200)
         sep         (str):  if multiple arguments are supplied, use this separator to join them
         doprint     (bool): whether to print the string (default true if no output)
         output      (bool): whether to return the string as output (else, print)
-        kwargs      (dict): passed to ``sc.colorize()``
+        kwargs      (dict): passed to :func:`sc.colorize() <colorize>`
 
     Returns:
         Formatted string if ``output=True``
 
     **Examples**::
         sc.heading('This is a heading')
         sc.heading(string='This is also a heading', color='red', divider='*', spaces=0, minlength=50)
 
-    | New in version 1.3.1.: "spacesafter"
+    | *New in version 1.3.1.*: "spacesafter"
     '''
-    if string      is None: string      = ''
-    if color       is None: color       = 'cyan' # Reasonable default for light and dark consoles
-    if divider     is None: divider     = '—' # Em dash for a continuous line
-    if spaces      is None: spaces      = 3
-    if spacesafter is None: spacesafter = 1
-    if minlength   is None: minlength   = 30
-    if maxlength   is None: maxlength   = 120
 
     # Convert to single string
     args = scu.mergelists(string, list(args))
     string = sep.join([str(item) for item in args])
 
     # Add header and footer
     length      = int(np.median([minlength, len(string), maxlength]))
@@ -745,18 +918,19 @@
     # Create output
     return colorize(color=color, string=fullstring, doprint=doprint, output=output, **kwargs)
 
 
 
 #%% Other
 
-__all__ += ['printv', 'slacknotification', 'printtologfile', 'percentcomplete', 'progressbar', 'capture']
+__all__ += ['printv', 'slacknotification', 'printtologfile', 'percentcomplete', 
+            'progressbar', 'progressbars', 'capture']
 
 
-def printv(string, thisverbose=1, verbose=2, newline=True, indent=True):
+def printv(string, thisverbose=1, verbose=2, indent=2, **kwargs):
     '''
     Optionally print a message and automatically indent. The idea is that
     a global or shared "verbose" variable is defined, which is passed to
     subfunctions, determining how much detail to print out.
 
     The general idea is that verbose is an integer from 0-4 as follows:
 
@@ -769,32 +943,30 @@
     Thus a very important statement might be e.g.
 
     >>> sc.printv('WARNING, everything is wrong', 1, verbose)
 
     whereas a much less important message might be
 
     >>> sc.printv(f'This is timestep {i}', 4, verbose)
-
-    Version: 2016jan30
-    '''
-    if thisverbose>4 or verbose>4: print(f'Warning, verbosity should be from 0-4 (this message: {thisverbose}; current: {verbose})')
-    if verbose>=thisverbose: # Only print if sufficiently verbose
-        indents = '  '*thisverbose*bool(indent) # Create automatic indenting
-        if newline: print(indents+scu.flexstr(string)) # Actually print
-        else: print(indents+scu.flexstr(string)), # Actually print
+    
+    Args:
+        string (str): string to print
+        thisverbose (int): level of verbosity at which to print this message
+        verbose (int): global verbose variable
+        indent (int): amount by which to indent based on verbosity level
+        kwargs (dict): passed to :func:`print()`
+        
+    *New in version 3.0.0:* "kwargs" argument; removed "newline" argument
+    '''
+    if verbose >= thisverbose: # Only print if sufficiently verbose
+        indents = ' '*thisverbose*indent # Create automatic indenting
+        print(indents+scu.flexstr(string), **kwargs) # Actually print
     return
 
 
-
-
-
-
-
-
-
 def slacknotification(message=None, webhook=None, to=None, fromuser=None, verbose=2, die=False):  # pragma: no cover
     '''
     Send a Slack notification when something is finished.
 
     The webhook is either a string containing the webhook itself, or a plain text file containing
     a single line which is the Slack webhook. By default it will look for the file
     ".slackurl" in the user's home folder. The webhook needs to look something like
@@ -868,15 +1040,15 @@
     Append a message string to a file specified by a filename name/path.
 
     Note: in almost all cases, you are better off using Python's built-in logging
     system rather than this function.
     '''
 
     # Set defaults
-    if message is None:
+    if message is None: # pragma: no cover
         return # Return immediately if nothing to append
     if filename is None:
         import tempfile
         tempdir = tempfile.gettempdir()
         filename = os.path.join(tempdir, 'logfile') # Some generic filename that should work on *nix systems
 
     # Try writing to file
@@ -885,104 +1057,244 @@
             f.write('\n'+message+'\n') # Add a newline to the message.
     except Exception as E: # pragma: no cover # Fail gracefully
         print(f'Warning, could not write to logfile {filename}: {str(E)}')
 
     return
 
 
-
-
-
 def percentcomplete(step=None, maxsteps=None, stepsize=1, prefix=None):
     '''
-    Display progress.
+    Display progress as a percentage.
 
-    **Example**::
+    **Examples**::
 
         maxiters = 500
+        
+        # Will print on every 5th iteration
         for i in range(maxiters):
-            sc.percentcomplete(i, maxiters) # will print on every 5th iteration
-            sc.percentcomplete(i, maxiters, stepsize=10) # will print on every 50th iteration
-            sc.percentcomplete(i, maxiters, prefix='Completeness: ') # will print e.g. 'Completeness: 1%'
+            sc.percentcomplete(i, maxiters) 
+        
+        # Will print on every 50th iteration
+        for i in range(maxiters):
+            sc.percentcomplete(i, maxiters, stepsize=10)
+        
+        # Will print e.g. 'Completeness: 1%'
+        for i in range(maxiters):
+            sc.percentcomplete(i, maxiters, prefix='Completeness: ') 
+    
+    See also :func:`sc.progressbar() <progressbar>` for a progress bar.
     '''
     if prefix is None:
         prefix = ' '
-    elif scu.isnumber(prefix):
+    elif scu.isnumber(prefix): # pragma: no cover
         prefix = ' '*prefix
     onepercent = max(stepsize,round(maxsteps/100*stepsize)) # Calculate how big a single step is -- not smaller than 1
     if not step%onepercent: # Does this value lie on a percent
         thispercent = round(step/maxsteps*100) # Calculate what percent it is
         print(prefix + '%i%%'% thispercent) # Display the output
     return
 
 
-def progressbar(i, maxiters, label='', every=1, length=30, empty='—', full='•', newline=False):
+def progressbar(i=None, maxiters=None, label='', every=1, length=30, empty='—', full='•', 
+                newline=False, flush=False, **kwargs):
     '''
-    Call in a loop to create terminal progress bar.
+    Show a progress bar for a for loop.
+    
+    It can be called manually inside each iteration of the loop, or it can be used 
+    to wrap the object being iterated. In the latter case, it acts as an alias 
+    for the ``tqdm.tqdm()`` progress bar.
 
     Args:
-        i        (int): current iteration
+        i        (int/iterable): current iteration (for text output), or iterable object (for tqdm)
         maxiters (int): maximum number of iterations (can also use an object with length)
         label    (str): initial label to print
         every    (int/float): if int, print every "every"th iteration (if 1, print all); if float and <1, print every maxiters*every iteration
         length   (int): length of progress bar
         empty    (str): character for not-yet-completed steps
         full     (str): character for completed steps
-        newline  (str): character to print at the end of the line (default none)
+        newline  (bool): whether to print each iteration on a new line
+        flush    (bool): whether to force-flush the buffer
+        kwargs   (dict): passed to ``tqdm.tqdm()``; see its documentation for full options
 
     **Examples**::
 
+        # Direct usage inside a loop
         for i in range(20):
             sc.progressbar(i+1, 20)
-            pl.pause(0.05)
+            sc.timedsleep(0.05)
+        
+        # Direct usage inside a loop with custom formatting
+        for i in range(1000):
+            sc.progressbar(i+1, 1000, every=100, length=10, empty=' ', full='✓', newline=True)
+            sc.timedsleep(0.001)
 
+        # Used to wrap an iterable, using tqdm
         x = np.arange(100)
-        for i in x:
-            sc.progressbar(i+1, x, every=0.1)
+        for i in sc.progressbar(x):
             pl.pause(0.01)
 
     Adapted from example by Greenstick (https://stackoverflow.com/questions/3173320/text-progress-bar-in-the-console)
 
-    New in version 1.3.3: "every" argument
+    | *New in version 1.3.3:* "every" argument
+    | *New in version 3.0.0:* wrapper for tqdm
     '''
+    if i is None or scu.isiterable(i):
+        desc = kwargs.pop('desc', label)
+        return tqdm.tqdm(i, desc=desc, **kwargs)
+    
     # Handle inputs
     if hasattr(maxiters, '__len__'):
         maxiters = len(maxiters)
     ending = None if newline else '\r'
-    if every < 1:
+    if every < 1: # pragma: no cover
         every = max(1, int(every*maxiters)) # Don't let it go below 1
 
     # Calculate percent and handle zero case
     if maxiters > 0:
         pct = i/maxiters*100
-    else:
+    else: # pragma: no cover
         i = 1
         maxiters = 1
         pct = 100
     percent = f'{pct:0.0f}%'
 
     # Assemble string
     filled = int(length*i//maxiters)
     bar = full*filled + empty*(length-filled)
 
     # Print
     lastiter = (i == maxiters)
     if not(i%every) or lastiter:
-        print(f'\r{label} {bar} {percent}', end=ending)
+        print(f'\r{label} {bar} {percent}', end=ending, flush=flush)
         if lastiter:
             print() # Newline at the end
 
     return
 
 
+class tqdm_pickle(tqdm.tqdm):
+    '''
+    Simple subclass of tqdm that allows pickling
+    
+    Usually not used directly by the user; used via :func:`sc.progressbars() <progressbars>` instead.
+    Pickling is required for passing ``tqdm`` instances between processes.
+    
+    Based on ``tqdm`` 4.65.0; may become deprecated in future ``tqdm`` releases.
+    
+    *New in version 3.0.0.*
+    '''
+    
+    def __getstate__(self):
+        ''' Overwrite default __getstate__ '''
+        d = {k:v for k,v in self.__dict__.items() if k not in ['sp', 'fp']}
+        return d
+     
+    def __setstate__(self, d): # pragma: no cover
+        ''' Overwrite default __getstate__ '''
+        self.__dict__ = d
+        self.__dict__['fp'] = tqdm.utils.DisableOnWriteError(sys.stderr, tqdm_instance=self)
+        self.__dict__['sp'] = self.status_printer(self.fp)
+        return
+
+
+class progressbars(scu.prettyobj):
+    '''
+    Create multiple progress bars
+    
+    Useful for tracking the progress of multiple long-running tasks. Unlike regular
+    ``tqdm`` instances, this uses a pickable version so it can be used directly
+    in multiprocessing instances.
+    
+    Args:
+        n (int): number of progress bars to create
+        total (float): length of the progress bars
+        label (str/list): an optional prefix for the progress bar, or list of all labels
+        leave (bool): whether to remove the progress bars when they're done
+        kwargs (dict): passed to ``tqdm.tqdm()``
+    
+    **Note**: bars are supposed to update in-place, but may appear on separate lines
+    instead if not run in the terminal (e.g. if run in IPython environments like 
+    Spyder or Jupyter).
+    
+    **Example**::
+        
+        import sciris as sc
+        import random
+
+        def run_sim(index, ndays, pbs):
+            for i in range(ndays):
+                val = random.random()
+                sc.timedsleep(val*5/ndays)
+                pbs.update(index) # Update this progress bar based on the index
+            return
+
+        nsims = 5
+        ndays = 365
+
+        # Create progress bars
+        pbs = sc.progressbars(nsims, total=ndays, label='Sim')
+
+        # Run tasks
+        sc.parallelize(run_sim, iterarg=range(nsims), ndays=ndays, pbs=pbs)
+        
+        # Produces output like:
+        # Sim 0:  39%|███████████████████████████▊           | 143/365 [00:01<00:01, 137.17it/s]
+        # Sim 1:  42%|████████████████████████████▉          | 154/365 [00:01<00:01, 148.70it/s]
+        # Sim 2:  45%|████████████████████████████████       | 165/365 [00:01<00:01, 144.19it/s]
+        # Sim 3:  44%|███████████████████████████████        | 160/365 [00:01<00:01, 151.22it/s]
+        # Sim 4:  42%|████████████████████████████▏          | 145/365 [00:01<00:01, 136.75it/s]
+
+    *New in version 3.0.0.*
+    '''
+    
+    def __init__(self, n=1, total=1, label=None, leave=False, **kwargs):
+        self.n      = n
+        self.total  = total
+        self.leave  = leave
+        self.desc   = kwargs.pop('desc', label)
+        self.kwargs = kwargs
+        self.bars   = []
+        self.make()
+        return
+
+    def make(self):
+        for i in range(self.n):
+            total = self.total
+            if scu.isiterable(total):
+                total = total[i]
+            desc = self.desc
+            if scu.isiterable(desc, exclude=str):
+                desc = desc[i]
+            else:
+                if desc is None:
+                    desc = f'{i}'
+                else:
+                    desc += f' {i}'
+            bar = tqdm_pickle(total=total, position=i, desc=desc, leave=self.leave, **self.kwargs)
+            self.bars.append(bar)
+        return
+    
+    def __getitem__(self, key): # pragma: no cover
+        return self.bars[key]
+    
+    def __setitem__(self, key, value): # pragma: no cover
+        self.bars[key] = value
+        return
+    
+    def update(self, index=0, amount=1): # pragma: no cover
+        self.bars[index].update(amount)
+        return
+
+
+
 class capture(UserString, str, redirect_stdout):
     '''
-    Captures stdout (e.g., from ``print()``) as a variable.
+    Captures stdout (e.g., from :func:`print()`) as a variable.
 
-    Based on ``contextlib.redirect_stdout``, but saves the user the trouble of
+    Based on :obj:`contextlib.redirect_stdout`, but saves the user the trouble of
     defining and reading from an IO stream. Useful for testing the output of functions
     that are supposed to print certain output.
 
     **Examples**::
 
         # Using with...as
         with sc.capture() as txt1:
@@ -996,15 +1308,15 @@
         txt2.stop()
 
         print('txt1:')
         print(txt1)
         print('txt2:')
         print(txt2)
 
-    New in version 1.3.3.
+    *New in version 1.3.3.*
     '''
 
     def __init__(self, seq='', *args, **kwargs):
         self._io = io.StringIO()
         self.stdout = sys.stdout
         UserString.__init__(self, seq=seq, *args, **kwargs)
         redirect_stdout.__init__(self, self._io)
```

### Comparing `sciris-2.1.0/sciris/sc_profiling.py` & `sciris-3.0.0/sciris/sc_profiling.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Profiling and CPU/memory management functions.
 
 Highlights:
-    - :func:`cpuload`: alias to ``psutil.cpu_percent()``
-    - :func:`loadbalancer`: very basic load balancer
-    - :func:`profile`: a line profiler
-    - :func:`resourcemonitor`: a monitor to kill processes that exceed memory or other limits
+    - :func:`sc.profile() <profile>`: a line profiler
+    - :func:`sc.benchmark() <benchmark>`: quickly check your computer's performance
+    - :func:`sc.loadbalancer() <loadbalancer>`: very basic load balancer
+    - :func:`sc.resourcemonitor() <resourcemonitor>`: a monitor to kill processes that exceed memory or other limits
 """
 
 import os
 import sys
 import time
 import psutil
 import signal
@@ -22,194 +22,336 @@
 import pylab as pl
 import multiprocessing as mp
 from . import sc_utils as scu
 from . import sc_datetime as scd
 from . import sc_odict as sco
 from . import sc_fileio as scf
 from . import sc_nested as scn
+from . import sc_printing as scp
+from . import sc_dataframe as scdf
 
 
 ##############################################################################
-#%% Load balancing functions
+#%% Basic performance functions
 ##############################################################################
 
-__all__ = ['cpu_count', 'cpuload', 'memload', 'loadbalancer']
-
-
-def cpu_count():
-    ''' Alias to ``mp.cpu_count()`` '''
-    return mp.cpu_count()
-
-
-def cpuload(interval=0.1):
-    """
-    Takes a snapshot of current CPU usage via ``psutil``
-
-    Args:
-        interval (float): number of seconds over which to estimate CPU load
-
-    Returns:
-        a float between 0-1 representing the fraction of ``psutil.cpu_percent()`` currently used.
-    """
-    return psutil.cpu_percent(interval=interval)/100
-
-
-def memload():
-    """
-    Takes a snapshot of current fraction of memory usage via ``psutil``
-
-    Note on the different functions:
-
-        - ``sc.memload()`` checks current total system memory consumption
-        - ``sc.checkram()`` checks RAM (virtual memory) used by the current Python process
-        - ``sc.checkmem()`` checks memory consumption by a given object
-
-    Returns:
-        a float between 0-1 representing the fraction of ``psutil.virtual_memory()`` currently used.
-    """
-    return psutil.virtual_memory().percent / 100
-
+__all__ = ['checkmem', 'checkram', 'benchmark']
 
 
-def checkmem(var, descend=True, alphabetical=False, compresslevel=0, plot=False, verbose=False, **kwargs):
+def checkmem(var, descend=1, order='size', compresslevel=0, maxitems=1000, 
+             subtotals=True, plot=False, verbose=False, **kwargs):
     '''
     Checks how much memory the variable or variables in question use by dumping
     them to file.
 
     Note on the different functions:
 
-        - ``sc.memload()`` checks current total system memory consumption
-        - ``sc.checkram()`` checks RAM (virtual memory) used by the current Python process
-        - ``sc.checkmem()`` checks memory consumption by a given object
+        - :func:`sc.memload() <memload>` checks current total system memory consumption
+        - :func:`sc.checkram() <checkram>` checks RAM (virtual memory) used by the current Python process
+        - :func:`sc.checkmem() <checkmem>` checks memory consumption by a given object
 
     Args:
         var (any): the variable being checked
         descend (bool): whether or not to descend one level into the object
-        alphabetical (bool): if descending into a dict or object, whether to list items by name rather than size
+        order (str): order in which to list items: "size" (default), "alphabetical", or "none"
         compresslevel (int): level of compression to use when saving to file (typically 0)
+        maxitems (int): the maximum number of separate entries to check the size of
+        subtotals (bool): whether to include subtotals for different levels of depth
         plot (bool): if descending, show the results as a pie chart
         verbose (bool or int): detail to print, if >1, print repr of objects along the way
-        **kwargs (dict): passed to :func:`load`
+        **kwargs (dict): passed to :func:`sc.load() <load>`
 
-    **Example**::
+    **Examples**::
 
         import numpy as np
         import sciris as sc
-        sc.checkmem(['spiffy', np.random.rand(2483,589)])
+        
+        list_obj = ['label', np.random.rand(2483,589)])
+        sc.checkmem(list_obj)
+        
+        
+        nested_dict = dict(
+            foo = dict(
+                a = np.random.rand(5,10),
+                b = np.random.rand(5,20),
+                c = np.random.rand(5,50),
+            ),
+            bar = [
+                np.random.rand(5,100),
+                np.random.rand(5,200),
+                np.random.rand(5,500),
+            ],
+            cat = np.random.rand(5,10),
+        )
+        sc.checkmem(nested_dict)
+    
+    *New in version 3.0.0:* descend multiple levels; dataframe output; "alphabetical" renamed "order"
     '''
+    
+    # Handle input arguments -- used for recursion
+    _depth  = kwargs.pop('_depth', 0)
+    _prefix = kwargs.pop('_prefix', '')
+    _join   = kwargs.pop('_join', '→')
 
     def check_one_object(variable):
         ''' Check the size of one variable '''
 
-        if verbose>1:
+        if verbose>1: # pragma: no cover
             print(f'  Checking size of {variable}...')
 
         # Create a temporary file, save the object, check the size, remove it
         filename = tempfile.mktemp()
-        scf.save(filename, variable, die='never', compresslevel=compresslevel)
+        scf.save(filename, variable, allow_empty=True, compresslevel=compresslevel)
         filesize = os.path.getsize(filename)
         os.remove(filename)
 
-        # Convert to string
-        factor = 1
-        label = 'B'
-        labels = ['KB','MB','GB']
-        for i,f in enumerate([3,6,9]):
-            if filesize>10**f:
-                factor = 10**f
-                label = labels[i]
-        humansize = float(filesize/float(factor))
-        sizestr = f'{humansize:0.3f} {label}'
+        sizestr = scp.humanize_bytes(filesize)
         return filesize, sizestr
 
     # Initialize
     varnames  = []
     variables = []
-    sizes     = []
-    sizestrs  = []
-
-    # Create the object(s) to check the size(s) of
-    varnames = ['Variable'] # Set defaults
-    variables = [var]
-    if descend or descend is None:
-        if hasattr(var, '__dict__'): # It's an object
-            if verbose>1: print('Iterating over object')
+    columns=dict(
+        variable  = object,
+        humansize = object,
+        bytesize  = int,
+        depth     = int,
+        is_total  = bool,
+    )
+    df = scdf.dataframe(columns=columns)
+    
+    if descend:
+        if isinstance(var, dict): # Handle dicts
+            if verbose>1: print('Iterating over dict')
+            varnames = list(var.keys())
+            variables = var.values()
+        elif hasattr(var, '__dict__'): # It's an object
+            if verbose>1: print('Iterating over class-like object')
             varnames = sorted(list(var.__dict__.keys()))
             variables = [getattr(var, attr) for attr in varnames]
-        elif np.iterable(var): # Handle dicts and lists
-            if isinstance(var, dict): # Handle dicts
-                if verbose>1: print('Iterating over dict')
-                varnames = list(var.keys())
-                variables = var.values()
-            else: # Handle lists and other things
-                if verbose>1: print('Iterating over list')
-                varnames = [f'item {i}' for i in range(len(var))]
-                variables = var
+        elif scu.isiterable(var, exclude=str): # Handle lists, and be sure to skip strings
+            if verbose>1: print('Iterating over list-like object')
+            varnames = [f'item {i}' for i in range(len(var))]
+            variables = var
         else:
-            if descend: # Could also be None
-                print('Object is not iterable: cannot descend') # Print warning and use default
+            descend = 0 # Can't descend
 
-    # Compute the sizes
-    for v,variable in enumerate(variables):
-        if verbose:
-            print(f'Processing variable {v} of {len(variables)}')
-        filesize, sizestr = check_one_object(variable)
-        sizes.append(filesize)
-        sizestrs.append(sizestr)
-
-    if alphabetical:
-        inds = np.argsort(varnames)
+    # Create the object(s) to check the size(s) of
+    if not descend:
+        varname = _prefix if _prefix else 'Variable'
+        bytesize, sizestr = check_one_object(var)
+        df.appendrow(dict(variable=varname, humansize=sizestr, bytesize=bytesize, depth=_depth, is_total=False))
+    
     else:
-        inds = np.argsort(sizes)[::-1]
-
-    data = sco.objdict({varnames[i]:[sizes[i], sizestrs[i]] for i in inds})
+        # Error checking
+        n_variables = len(variables)
+        if n_variables > maxitems: # pragma: no cover
+            errormsg = f'Cannot compute the sizes of {n_variables} items since maxitems is set to {maxitems}'
+            raise RuntimeError(errormsg)
+    
+        # Compute the sizes recursively
+        for v,(varname,variable) in enumerate(zip(varnames, variables)):
+            if verbose: # pragma: no cover
+                print(f'Processing variable {v} of {len(variables)}')
+            label = _join.join([_prefix, varname]) if _prefix else varname
+            this_df = checkmem(variable, descend=descend-1, compresslevel=compresslevel, maxitems=maxitems, plot=False, verbose=False, _prefix=label, _depth=_depth+1)
+            df.concat(this_df, inplace=True)
+    
+    # Handle subtotals
+    if subtotals and len(df) > 1:
+        total_label = _prefix + ' (total)' if _prefix else 'Total'
+        total = df[np.logical_not(df.is_total)].bytesize.sum()
+        human_total = scp.humanize_bytes(total)
+        df.appendrow(dict(variable=total_label, humansize=human_total, bytesize=total, depth=_depth, is_total=True))
+    
+    # Only sort if we're at the highest level
+    if _depth == 0 and len(df) > 1:
+        # if subtotals:
+            
+        if order == 'alphabetical': # pragma: no cover
+            df.sortrows(col='variable')
+        elif order == 'size':
+            df.sortrows(col='bytesize', reverse=True)
 
     if plot: # pragma: no cover
         pl.axes(aspect=1)
-        pl.pie(np.array(sizes)[inds], labels=np.array(varnames)[inds], autopct='%0.2f')
+        pl.pie(df.bytesize, labels=df.variable, autopct='%0.2f')
 
-    return data
+    return df
 
 
 def checkram(unit='mb', fmt='0.2f', start=0, to_string=True):
     '''
     Measure actual memory usage, typically at different points throughout execution.
 
     Note on the different functions:
 
-        - ``sc.memload()`` checks current total system memory consumption
-        - ``sc.checkram()`` checks RAM (virtual memory) used by the current Python process
-        - ``sc.checkmem()`` checks memory consumption by a given object
+        - :func:`sc.memload() <memload>` checks current total system memory consumption
+        - :func:`sc.checkram() <checkram>` checks RAM (virtual memory) used by the current Python process
+        - :func:`sc.checkmem() <checkmem>` checks memory consumption by a given object
 
     **Example**::
 
         import sciris as sc
         import numpy as np
         start = sc.checkram(to_string=False)
         a = np.random.random((1_000, 10_000))
         print(sc.checkram(start=start))
-
-    New in version 1.0.0.
+    
+    *New in version 1.0.0.*
     '''
     process = psutil.Process(os.getpid())
     mapping = {'b':1, 'kb':1e3, 'mb':1e6, 'gb':1e9}
     try:
         factor = mapping[unit.lower()]
     except KeyError: # pragma: no cover
         raise scu.KeyNotFoundError(f'Unit {unit} not found among {scu.strjoin(mapping.keys())}')
     mem_use = process.memory_info().rss/factor - start
     if to_string:
         output = f'{mem_use:{fmt}} {unit.upper()}'
-    else:
+    else: # pragma: no cover
         output = mem_use
     return output
 
 
-def loadbalancer(maxcpu=0.8, maxmem=0.8, index=None, interval=None, cpu_interval=0.1,
-                 maxtime=36000, label=None, verbose=True, **kwargs):
+def benchmark(repeats=5, scale=1, verbose=False, python=True, numpy=True, return_timers=False):
+    '''
+    Benchmark Python performance
+    
+    Performs a set of standard operations in both Python and Numpy and times how
+    long they take. Results are returned in terms of millions of operations per second (MOPS).
+    With default settings, this function should take very approximately 0.1 s to 
+    run (depending on the machine, of course!).
+    
+    For Python, these operations are: for loops, list append/indexing, dict set/get,
+    and arithmetic. For Numpy, these operations are: random floats, random ints,
+    addition, and multiplication.
+    
+    Args:
+        repeats (int): the number of times to repeat each test
+        scale (float): the scale factor to use for the size of the loops/arrays
+        verbose (bool): print out the results after each repeat
+        python (bool): whether to run the Python tests
+        numpy (bool): whether to run the Numpy tests
+        return_timers (bool): if True, return the timer objects instead of the "MOPS" results
+        
+    Returns:
+        A dict with keys "python" and "numpy" for the number of MOPS for each
+    
+    **Examples**::
+        
+        sc.benchmark() # Returns e.g. {'python': 11.43, 'numpy': 236.595}
+        
+        numpy_mops = sc.benchmark(python=False)['numpy']
+        if numpy_mops < 100:
+            print('Your computer is slow')
+        elif numpy_mops > 400: 
+            print('Your computer is fast')
+        else:
+            print('Your computer is normal')
+    
+    *New in version 3.0.0.*
+    '''
+    
+    P = scd.timer(verbose=verbose)
+    N = scd.timer(verbose=verbose)
+    
+    py_outer = 10
+    py_inner = scale*5e2
+    
+    np_outer = 1
+    np_inner = scale*5e5
+    
+    py_ops = (py_outer * py_inner * 18)/1e6
+    np_ops = (np_outer * np_inner * 4)/1e6
+    
+    # Benchmark plain Python
+    if python:
+        for r in range(repeats):
+            l = list()
+            d = dict()
+            result = 0
+            P.tic()
+            for i in range(py_outer):
+                for j in range(int(py_inner)):
+                    l.append([i,j]) # Operation 1: list append
+                    d[str((i,j))] = [i,j] # Operations 2-3: convert to string and dict assign
+                    v1 = l[-1][0] + l[-1][0] # Operations 4-8: list get (x4) and sum
+                    v2 = d[str((i,j))][0] + d[str((i,j))][1] # Operations 9-16: convert to string (x2), list get (x2), dict get (x2), sum
+                    result += v1 + v2 # Operations 17-18: sum (x2)
+            P.toc(f'Python, {py_ops}m operations')
+                 
+    # Benchmark Numpy
+    if numpy:
+        for r in range(repeats):
+            N.tic()
+            for i in range(np_outer):
+                a = np.random.random(int(np_inner)) # Operation 1: random floats
+                b = np.random.randint(10, size=int(np_inner)) # Operation 2: random integers
+                a + b # Operation 3: addition
+                a*b # Operation 4: multiplication
+            N.toc(f'Numpy, {np_ops}m operations')
+    
+    # Handle output
+    if return_timers: # pragma: no cover
+        out = sco.objdict(python=P, numpy=N)
+    else:
+        pymops = py_ops/P.mean() if len(P) else None # Handle if one or the other isn't run
+        npmops = np_ops/N.mean() if len(N) else None
+        out = dict(python=pymops, numpy=npmops)
+        
+    return out
+
+
+##############################################################################
+#%% Load balancing functions
+##############################################################################
+
+__all__ += ['cpu_count', 'cpuload', 'memload', 'loadbalancer']
+
+
+def cpu_count():
+    ''' Alias to :func:`multiprocessing.cpu_count()` '''
+    return mp.cpu_count()
+
+
+def cpuload(interval=0.1):
+    """
+    Takes a snapshot of current CPU usage via :mod:`psutil`
+
+    Args:
+        interval (float): number of seconds over which to estimate CPU load
+
+    Returns:
+        a float between 0-1 representing the fraction of :func:`psutil.cpu_percent()` currently used.
+    """
+    return psutil.cpu_percent(interval=interval)/100
+
+
+def memload():
+    """
+    Takes a snapshot of current fraction of memory usage via :mod:`psutil`
+
+    Note on the different functions:
+
+        - :func:`sc.memload() <memload>` checks current total system memory consumption
+        - :func:`sc.checkram() <checkram>` checks RAM (virtual memory) used by the current Python process
+        - :func:`sc.checkmem() <checkmem>` checks memory consumption by a given object
+
+    Returns:
+        a float between 0-1 representing the fraction of :func:`psutil.virtual_memory()` currently used.
+    """
+    return psutil.virtual_memory().percent / 100
+
+
+
+
+
+def loadbalancer(maxcpu=0.9, maxmem=0.9, index=None, interval=None, cpu_interval=0.1,
+                 maxtime=36_000, label=None, verbose=True, **kwargs):
     '''
     Delay execution while CPU load is too high -- a very simple load balancer.
 
     Arguments:
         maxcpu       (float) : the maximum CPU load to allow for the task to still start
         maxmem       (float) : the maximum memory usage to allow for the task to still start
         index        (int)   : the index of the task -- used to start processes asynchronously (default None)
@@ -222,17 +364,18 @@
     **Examples**::
 
         # Simplest usage -- delay if CPU or memory load is >80%
         sc.loadbalancer()
 
         # Use a maximum CPU load of 50%, maximum memory of 90%, and stagger the start by process number
         for nproc in processlist:
-            sc.loadbalancer(maxload=0.5, maxmem=0.9, index=nproc)
+            sc.loadbalancer(maxload=0.5, maxmem=0.8, index=nproc)
 
-    | New in version 2.0.0: ``maxmem`` argument; ``maxload`` renamed ``maxcpu``
+    | *New in version 2.0.0:* ``maxmem`` argument; ``maxload`` renamed ``maxcpu``
+    | *New in version 3.0.0:* ``maxcpu`` and ``maxmem`` set to 0.9 by default
     '''
 
     # Handle deprecation
     maxload = kwargs.pop('maxload', None)
     if maxload is not None: # pragma: no cover
         maxcpu = maxload
         warnmsg = 'sc.loadbalancer() argument "maxload" has been renamed "maxcpu" as of v2.0.0'
@@ -242,35 +385,35 @@
     if maxcpu   is None or maxcpu  is False: maxcpu  = 1.0
     if maxmem   is None or maxmem  is False: maxmem  = 1.0
     if maxtime  is None or maxtime is False: maxtime = 36000
     
     # Handle the interval
     default_interval = 0.5
     min_interval = 1e-3 # Don't allow intervals of less than 1 ms
-    if interval is None:
+    if interval is None: # pragma: no cover
         interval = default_interval
-    if interval < min_interval:
+    if interval < min_interval: # pragma: no cover
         interval = min_interval
         warnmsg = f'sc.loadbalancer() "interval" should not be less than {min_interval} s'
         warnings.warn(warnmsg, category=UserWarning, stacklevel=2)
 
     if label is None:
         label = ''
-    else:
+    else: # pragma: no cover
         label += ': '
 
     if index is None:
         pause = interval*2*np.random.rand()
         index = ''
-    else:
+    else: # pragma: no cover
         pause = index*interval
 
     if maxcpu>1: maxcpu = maxcpu/100 # If it's >1, assume it was given as a percent
     if maxmem>1: maxmem = maxmem/100
-    if (not 0 < maxcpu < 1) and (not 0 < maxmem < 1):
+    if (not 0 < maxcpu < 1) and (not 0 < maxmem < 1): # pragma: no cover
         return # Return immediately if no max load
     else:
         time.sleep(pause) # Give it time to asynchronize, with a predefined delay
 
     # Loop until load is OK
     toohigh = True # Assume too high
     count = 0
@@ -282,35 +425,36 @@
         mem_current = memload()
         cpu_toohigh = cpu_current > maxcpu
         mem_toohigh = mem_current > maxmem
         cpu_compare = ['<', '>'][cpu_toohigh]
         mem_compare = ['<', '>'][mem_toohigh]
         cpu_str = f'{cpu_current:0.2f}{cpu_compare}{maxcpu:0.2f}'
         mem_str = f'{mem_current:0.2f}{mem_compare}{maxmem:0.2f}'
-        process_str = f'process {index}' if index else 'process'
-        if cpu_toohigh:
+        process_str = f'process {index}' if index is not None else 'process'
+        if cpu_toohigh: # pragma: no cover
             string = label+f'CPU load too high ({cpu_str}); {process_str} queued {count} times'
             scd.randsleep(interval)
-        elif mem_toohigh:
+        elif mem_toohigh: # pragma: no cover
             string = label+f'Memory load too high ({mem_str}); {process_str} queued {count} times'
             scd.randsleep(interval)
         else:
+            ok = 'OK' if scu.getplatform() == 'windows' else '✓' # Windows doesn't support unicode (!)
             toohigh = False
-            string = label+f'CPU ✓ ({cpu_str}), memory ✓ ({mem_str}): starting {process_str} after {count} tries'
+            string = label+f'CPU {ok} ({cpu_str}), memory {ok} ({mem_str}): starting {process_str} after {count} tries'
         if verbose:
             print(string)
     return string
 
 
 
 ##############################################################################
 #%% Profiling functions
 ##############################################################################
 
-__all__ += ['profile', 'mprofile', 'checkmem', 'checkram']
+__all__ += ['profile', 'mprofile']
 
 
 def profile(run, follow=None, print_stats=True, *args, **kwargs):
     '''
     Profile the line-by-line time required by a function.
 
     Args:
@@ -363,33 +507,33 @@
             errormsg = 'The "line_profiler" package is not included by default on Windows;' \
                         'please install using "pip install line_profiler" (note: you will need a ' \
                         'C compiler installed, e.g. Microsoft Visual Studio)'
         else:
             errormsg = 'The "line_profiler" Python package is required to perform profiling'
         raise ModuleNotFoundError(errormsg) from E
 
-    if follow is None:
+    if follow is None: # pragma: no cover
         follow = run
     orig_func = run
 
     lp = LineProfiler()
     follow = scu.tolist(follow)
     for f in follow:
         lp.add_function(f)
     lp.enable_by_count()
-    wrapper = lp(run)
+    wrapper = lp(run) # pragma: no cover
 
     if print_stats: # pragma: no cover
         print('Profiling...')
-    wrapper(*args, **kwargs)
-    run = orig_func
+    wrapper(*args, **kwargs) # pragma: no cover
+    run = orig_func # pragma: no cover
     if print_stats: # pragma: no cover
         lp.print_stats()
         print('Done.')
-    return lp
+    return lp # pragma: no cover
 
 
 def mprofile(run, follow=None, show_results=True, *args, **kwargs):
     '''
     Profile the line-by-line memory required by a function. See profile() for a
     usage example.
 
@@ -410,15 +554,15 @@
             errormsg = 'The "memory_profiler" package is not included by default on Windows;' \
                         'please install using "pip install memory_profiler" (note: you will need a ' \
                         'C compiler installed, e.g. Microsoft Visual Studio)'
         else:
             errormsg = 'The "memory_profiler" Python package is required to perform profiling'
         raise ModuleNotFoundError(errormsg) from E
 
-    if follow is None:
+    if follow is None: # pragma: no cover
         follow = run
 
     lp = mp.LineProfiler()
     follow = scu.tolist(follow)
     for f in follow:
         lp.add_function(f)
     lp.enable_by_count()
@@ -442,35 +586,35 @@
 
 __all__ += ['LimitExceeded', 'resourcemonitor']
 
 
 
 class LimitExceeded(MemoryError, KeyboardInterrupt):
     '''
-    Custom exception for use with the ``sc.resourcemonitor()`` monitor.
+    Custom exception for use with the :func:`sc.resourcemonitor() <resourcemonitor>` monitor.
 
-    It inherits from ``MemoryError`` since this is the most similar built-in Python
-    except, and it inherits from ``KeyboardInterrupt`` since this is the means by
+    It inherits from :obj:`MemoryError` since this is the most similar built-in Python
+    except, and it inherits from :obj:`KeyboardInterrupt` since this is the means by
     which the monitor interrupts the main Python thread.
     '''
     pass
 
 
-class resourcemonitor(scu.prettyobj):
+class resourcemonitor(scu.prettyobj): # pragma: no cover # For some reason pycov doesn't catch this class
     """
     Asynchronously monitor resource (e.g. memory) usage and terminate the process
     if the specified threshold is exceeded.
 
     Args:
         mem (float): maximum virtual memory allowed (as a fraction of total RAM)
         cpu (float): maximum CPU usage (NB: included for completeness only; typically one would not terminate a process just due to high CPU usage)
         time (float): maximum time limit in seconds
         interval (float): how frequently to check memory/CPU usage (in seconds)
         label (str): an optional label to use while printing out progress
-        start (bool): whether to start the resource monitor on initialization (else call ``start()``)
+        start (bool): whether to start the resource monitor on initialization (else call :meth:`start() <resourcemonitor.start>`)
         die (bool): whether to raise an exception if the resource limit is exceeded
         kill_children (bool): whether to kill child processes (if False, will not work with multiprocessing)
         kill_parent (bool): whether to also kill the parent process (will usually exit Python interpreter in the process)
         callback (func): optional callback if the resource limit is exceeded
         verbose (bool): detail to print out (default: if exceeded; True: every step; False: no output)
 
     **Examples**::
@@ -516,15 +660,15 @@
         '''
         Start the monitor running
 
         Args:
             label (str): optional label for printing progress
         '''
 
-        def handler(signum, frame):
+        def handler(signum, frame): # pragma: no cover
             ''' Custom exception handler '''
             if self.exception is not None:
                 raise self.exception
             else:
                 return self._orig_sigint()
 
         if not self.running:
@@ -552,15 +696,15 @@
         self.running = False
         try:
             signal.signal(signal.SIGINT, self._orig_sigint) # Restore original KeyboardInterrupt handling
         except ValueError:
             errormsg = 'Could not reset signal, probably not calling from main thread'
             print(errormsg)
         if self.exception is not None and self.die: # This exception has likely already been raised, but if not, raise it now
-            raise self.exception
+            raise self.exception # pragma: no cover
         return self
 
 
     def __enter__(self, *args, **kwargs):
         ''' For use in a context block '''
         return self.start()
 
@@ -581,15 +725,15 @@
                 if self.callback:
                     self.callback(checkdata, updatestr)
             if not is_ok:
                 self.running = False
                 self.exception = LimitExceeded(checkstr)
                 if self.callback:
                     self.callback(checkdata, checkstr)
-                if self.die:
+                if self.die: # pragma: no cover
                     self.kill()
             time.sleep(self.interval)
 
         return
 
 
     def check(self):
@@ -642,15 +786,15 @@
             datalist += f'Time: {now.time:n} vs {lim.time:n}'
         datastr = '; '.join(datalist)
         checkstr = f'{prefix}: {datastr}'
 
         return is_ok, checkdata, checkstr
 
 
-    def kill(self):
+    def kill(self): # pragma: no cover
         ''' Kill all processes '''
         kill_verbose = self.verbose is not False # Print if self.verbose is True or None (just not False)
         if kill_verbose:
             print(self.exception)
             print('Killing processes...')
 
         parent   = psutil.Process(self.parent)
@@ -677,8 +821,7 @@
         ''' Convert the log into a pandas dataframe '''
         entries = []
         for entry in self.log:
             flat = scn.flattendict(entry, sep='_')
             entries.append(flat)
         self.df = pd.DataFrame(entries)
         return self.df
-
```

### Comparing `sciris-2.1.0/sciris/sc_utils.py` & `sciris-3.0.0/sciris/sc_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,71 +2,70 @@
 Miscellaneous utilities for type checking, printing, dates and times, etc.
 
 Note: there are a lot! The design philosophy has been that it's easier to
 ignore a function that you don't need than write one from scratch that you
 do need.
 
 Highlights:
-    - :func:`dcp`: shortcut to ``copy.deepcopy()``
-    - :func:`pp`: shortcut to ``pprint.pprint()``
-    - :func:`isnumber`: checks if something is any number type
-    - :func:`tolist`: converts any object to a list, for easy iteration
-    - :func:`toarray`: tries to convert any object to an array, for easy use with numpy
-    - :func:`mergedicts`: merges any set of inputs into a dictionary
-    - :func:`mergelists`: merges any set of inputs into a list
-    - :func:`runcommand`: simple way of executing a shell command
-    - :func:`download`: download multiple URLs in parallel
+    - :func:`sc.dcp() <dcp>`: shortcut to :func:`copy.deepcopy()`
+    - :func:`sc.pp() <pp>`: shortcut to :func:`pprint.pprint()`
+    - :func:`sc.isnumber() <isnumber>`: checks if something is any number type
+    - :func:`sc.tolist() <tolist>`: converts any object to a list, for easy iteration
+    - :func:`sc.toarray() <toarray>`: tries to convert any object to an array, for easy use with numpy
+    - :func:`sc.mergedicts() <mergedicts>`: merges any set of inputs into a dictionary
+    - :func:`sc.mergelists() <mergelists>`: merges any set of inputs into a list
+    - :func:`sc.runcommand() <runcommand>`: simple way of executing a shell command
+    - :func:`sc.download() <download>`: download multiple URLs in parallel
 '''
 
 ##############################################################################
 #%% Imports
 ##############################################################################
 
-import os
 import re
 import sys
 import copy
-import time
 import json
-import zlib
-import types
 import string
 import numbers
 import pprint
 import hashlib
+import getpass
+import inspect
 import warnings
+import importlib
 import subprocess
 import unicodedata
 import numpy as np
 import pandas as pd
 import random as rnd
 import uuid as py_uuid
-import packaging.version
 import contextlib as cl
 import traceback as py_traceback
+from pathlib import Path
 
 # Handle types
 _stringtypes = (str, bytes)
 _numtype     = (numbers.Number,)
 _booltypes   = (bool, np.bool_)
 
 
 ##############################################################################
 #%% Adaptations from other libraries
 ##############################################################################
 
 # Define the modules being loaded
-__all__ = ['fast_uuid', 'uuid', 'dcp', 'cp', 'pp', 'sha', 'freeze', 'require',
-           'traceback', 'getplatform', 'iswindows', 'islinux', 'ismac', 'asciify']
+__all__ = ['fast_uuid', 'uuid', 'dcp', 'cp', 'pp', 'sha', 'traceback', 'getuser',
+           'getplatform', 'iswindows', 'islinux', 'ismac', 'isjupyter', 'asciify']
 
 
 def fast_uuid(which=None, length=None, n=1, secure=False, forcelist=False, safety=1000, recursion=0, recursion_limit=10, verbose=True):
     '''
-    Create a fast UID or set of UIDs. Note: for certain applications, :func:`uuid`
-    is faster than :func:`fast_uuid`!
+    Create a fast UID or set of UIDs. Note: for certain applications, :func:`sc.uuid() <uuid>`
+    is faster than :func:`sc.fast_uuid() <fast_uuid>`!
 
     Args:
         which (str): the set of characters to choose from (default ascii)
         length (int): length of UID (default 6)
         n (int): number of UIDs to generate
         secure (bool): whether to generate random numbers from sources provided by the operating system
         forcelist (bool): whether or not to return a list even for a single UID (used for recursive calls)
@@ -113,15 +112,15 @@
         n_possibilities = len(charlist)**length
         allowed = n_possibilities//safety
         if n > allowed:
             errormsg = f'With a UID of type "{which}" and length {length}, there are {n_possibilities} possible UIDs, and you requested {n}, which exceeds the maximum allowed ({allowed})'
             raise ValueError(errormsg)
 
     # Secure uses system random which is secure, but >10x slower
-    if secure:
+    if secure: # pragma: no cover
         choices_func = rnd.SystemRandom().choices
     else:
         choices_func = rnd.choices
 
     # Generate the UUID(s) string as one big block
     uid_str = ''.join(choices_func(charlist, k=length*n))
 
@@ -234,22 +233,22 @@
     return output
 
 
 def dcp(obj, die=True, verbose=True):
     '''
     Shortcut to perform a deep copy operation
 
-    Almost identical to ``copy.deepcopy()``, but optionally fall back to copy()
+    Almost identical to :func:`copy.deepcopy()`, but optionally fall back to :func:`copy.copy()`
     if deepcopy fails.
 
     Args:
         die (bool): if False, fall back to copy()
         verbose (bool): if die is False, then print a warning if deepcopy() fails
 
-    New in version 2.0.0: default die=True instead of False
+    *New in version 2.0.0:* default die=True instead of False
     '''
     try:
         output = copy.deepcopy(obj)
     except Exception as E: # pragma: no cover
         output = cp(obj)
         errormsg = f'Warning: could not perform deep copy: {str(E)}'
         if die: raise RuntimeError(errormsg)
@@ -257,17 +256,17 @@
     return output
 
 
 def cp(obj, die=True, verbose=True):
     '''
     Shortcut to perform a shallow copy operation
 
-    Almost identical to ``copy.copy()``, but optionally allow failures
+    Almost identical to :func:`copy.copy()`, but optionally allow failures
 
-    New in version 2.0.0: default die=True instead of False
+    *New in version 2.0.0:* default die=True instead of False
     '''
     try:
         output = copy.copy(obj)
     except Exception as E:
         output = obj
         errormsg = 'Could not perform shallow copy'
         if die: raise ValueError(errormsg) from E
@@ -288,52 +287,58 @@
 
     # Handle actions/output
     if doprint: print(string)
     if output: return string
     else:      return
 
 
-def pp(obj, jsonify=True, doprint=None, output=False, verbose=False, **kwargs):
+def pp(obj, jsonify=False, doprint=None, output=False, sort_dicts=False, **kwargs):
     '''
     Shortcut for pretty-printing the object.
 
-    Almost identical to ``pprint.pprint()``, but can also be used as an alias for
-    ``pprint.pformat()``.
+    Almost identical to :func:`pprint.pprint()`, but can also be used as an alias for
+    :func:`pprint.pformat()`.
 
     Args:
         obj     (any):  object to print
         jsonify (bool): whether to first convert the object to JSON, to handle things like ordered dicts nicely
         doprint (bool): whether to show output (default true)
         output  (bool): whether to return output as a string (default false)
-        verbose (bool): whether to show warnings when jsonifying the object
-        kwargs  (dict): passed to ``pprint.pprint()``
-
-    New in version 1.3.1: output argument
+        sort_dicts (bool): whether to sort dictionary keys (default false, unlike :func:`pprint.pprint()`)
+        kwargs  (dict): passed to :func:`pprint.pprint()`
+    
+    **Example**::
+        
+        d = {'my very': {'large': 'and', 'unwieldy': {'nested': 'dictionary', 'cannot': 'be', 'easily': 'printed'}}}
+        sc.pp(d)
+        
+    *New in version 1.3.1:* output argument
+    *New in version 3.0.0:* "jsonify" defaults to False; sort_dicts defaults to False; removed "verbose" argument
     '''
 
     # Get object
     if jsonify:
         try:
-            toprint = json.loads(json.dumps(obj)) # This is to handle things like OrderedDicts
+            toprint = json.loads(json.dumps(obj, default=lambda x: f'{x}')) # This is to handle things like OrderedDicts
         except Exception as E:
-            if verbose: print(f'Could not jsonify object ("{str(E)}"), printing default...')
+            print(f'Could not jsonify object ("{str(E)}"), printing default...')
             toprint = obj # If problems are encountered, just return the object
-    else:
+    else: # pragma: no cover
         toprint = obj
 
     # Decide what to do with object
-    string = pprint.pformat(toprint, **kwargs)
+    string = pprint.pformat(toprint, sort_dicts=sort_dicts, **kwargs)
     return _printout(string=string, doprint=doprint, output=output)
 
 
 def sha(obj, encoding='utf-8', digest=False):
     '''
     Shortcut for the standard hashing (SHA) method
 
-    Equivalent to ``hashlib.sha224()``.
+    Equivalent to :obj:`hashlib.sha224()`.
 
     Args:
         obj (any): the object to be hashed; if not a string, converted to one
         encoding (str): the encoding to use
         digest (bool): whether to return the hex digest instead of the hash objet
 
     **Example**::
@@ -342,224 +347,209 @@
         sha2 = sc.sha(dict(foo=1, bar=2), digest=True)
         sha3 = sc.sha(dict(foo=1, bar=3), digest=True)
         assert sha1 == sha2
         assert sha2 != sha3
     '''
     if not isstring(obj): # Ensure it's actually a string
         string = repr(obj)
-    else:
+    else: # pragma: no cover
         string = obj
     needsencoding = isinstance(string, str)
     if needsencoding: # If it's unicode, encode it to bytes first
         string = string.encode(encoding)
     output = hashlib.sha224(string)
-    if digest:
+    if digest: # pragma: no cover
         output = output.hexdigest()
     return output
 
 
-def freeze(lower=False):
-    '''
-    Alias for pip freeze.
-
-    Args:
-        lower (bool): convert all keys to lowercase
-
-    **Example**::
-
-        assert 'numpy' in sc.freeze() # One way to check for versions
-
-    New in version 1.2.2.
-    '''
-    import pkg_resources as pkgr # Imported here since slow (>0.1 s)
-    raw = dict(tuple(str(ws).split()) for ws in pkgr.working_set)
-    keys = sorted(raw.keys())
-    if lower:
-        labels = {k:k.lower() for k in keys}
-    else:
-        labels = {k:k for k in keys}
-    data = {labels[k]:raw[k] for k in keys} # Sort alphabetically
-    return data
-
-
-def require(reqs=None, *args, exact=False, detailed=False, die=True, verbose=True, **kwargs):
+def traceback(*args, **kwargs):
     '''
-    Check whether environment requirements are met. Alias to pkg_resources.require().
-
-    Args:
-        reqs (list/dict): a list of strings, or a dict of package names and versions
-        args (list): additional requirements
-        kwargs (dict): additional requirements
-        exact (bool): use '==' instead of '>=' as the default comparison operator if not specified
-        detailed (bool): return a dict of which requirements are/aren't met
-        die (bool): whether to raise an exception if requirements aren't met
-        verbose (bool): print out the exception if it's not being raised
-
-    **Examples**::
-
-        sc.require('numpy')
-        sc.require(numpy='')
-        sc.require(reqs={'numpy':'1.19.1', 'matplotlib':'3.2.2'})
-        sc.require('numpy>=1.19.1', 'matplotlib==3.2.2', die=False)
-        sc.require(numpy='1.19.1', matplotlib='==4.2.2', die=False, detailed=True)
+    Shortcut for accessing the traceback
 
-    New in version 1.2.2.
+    Alias for :obj:`traceback.format_exc()`.
     '''
-    import pkg_resources as pkgr # Imported here since slow (>0.1 s)
-
-    # Handle inputs
-    reqlist = list(args)
-    reqdict = kwargs
-    if isinstance(reqs, dict):
-        reqdict.update(reqs)
-    else:
-        reqlist = mergelists(reqs, reqlist)
-
-    # Turn into a list of strings
-    comparechars = '<>=!~'
-    for k,v in reqdict.items():
-        if not v:
-            entry = k # If no version is provided, entry is just the module name
-        else:
-            compare = '' if v.startswith(tuple(comparechars)) else ('==' if exact else '>=')
-            entry = k + compare + v
-        reqlist.append(entry)
-
-    # Check the requirements
-    data = dict()
-    errs = dict()
-    for entry in reqlist:
-        try:
-            pkgr.require(entry)
-            data[entry] = True
-        except Exception as E:
-            data[entry] = False
-            errs[entry] = E
-
-    # Figure out output
-    met = all([e==True for e in data.values()])
-
-    # Handle exceptions
-    if not met:
-        errkeys = list(errs.keys())
-        errormsg = '\nThe following requirement(s) were not met:'
-        count = 0
-        for k,v in data.items():
-            if not v:
-                count += 1
-                errormsg += f'\n• "{k}": {str(errs[k])}'
-        errormsg += f'''\n\nIf this is a valid module, you might want to try "pip install {strjoin(errkeys, sep=' ')} --upgrade".'''
-        if die:
-            err = errs[errkeys[-1]]
-            raise ModuleNotFoundError(errormsg) from err
-        elif verbose:
-            print(errormsg)
-
-    # Handle output
-    if detailed:
-        return data, errs
-    else:
-        return met
+    return py_traceback.format_exc(*args, **kwargs)
 
 
-def traceback(*args, **kwargs):
+def getuser():
     '''
-    Shortcut for accessing the traceback
-
-    Alias for ``traceback.format_exc()``.
+    Get the current username 
+    
+    Alias to :func:`getpass.getuser()` -- see https://docs.python.org/3/library/getpass.html#getpass.getuser
+    
+    *New in version 3.0.0.*
     '''
-    return py_traceback.format_exc(*args, **kwargs)
+    return getpass.getuser()
 
 
-def getplatform(expected=None, die=False):
+def getplatform(expected=None, platform=None, die=False):
     '''
-    Return the name of the current platform: 'linux', 'windows', 'mac', or 'other'.
-    Alias (kind of) to sys.platform.
+    Return the name of the current "main" platform (e.g. 'mac')
+    
+    Alias to ``sys.platform``, except maps entries onto one of 'linux', 'windows', 
+    'mac', or 'other'.
 
     Args:
         expected (str): if not None, check if the current platform is this
+        platform (str): if supplied, map this onto one of the "main" platforms, rather than determine it
         die (bool): if True and expected is defined, raise an exception
+    
+    Returns:
+        String, one of: 'linux', 'windows', 'mac', or 'other'
 
-    **Example**::
+    **Examples**::
 
         sc.getplatform() # Get current name of platform
         sc.getplatform('windows', die=True) # Raise an exception if not on Windows
+        sc.getplatform(platform='darwin') # Normalize to 'mac'
     '''
     # Define different aliases for each operating system
     mapping = dict(
         linux   = ['linux', 'posix'],
         windows = ['windows', 'win', 'win32', 'cygwin', 'nt'],
         mac     = ['mac', 'macos', 'darwin', 'osx']
     )
 
     # Check to see what system it is
-    sys_plat = sys.platform
+    sys_plat = sys.platform if platform is None else platform
     plat = 'other'
     for key,aliases in mapping.items():
         if sys_plat.lower() in aliases:
             plat = key
             break
 
     # Handle output
     if expected is not None:
         output = (expected.lower() in mapping[plat]) # Check if it's as expecte
-        if not output and die:
+        if not output and die: # pragma: no cover
             errormsg = f'System is "{plat}", not "{expected}"'
             raise EnvironmentError(errormsg)
-    else:
+    else: # pragma: no cover
         output = plat
     return output
 
 
 def iswindows(die=False):
-    ''' Alias to ``sc.getplatform('windows')`` '''
+    ''' Alias to :func:`sc.getplatform('windows') <getplatform>` '''
     return getplatform('windows', die=die)
 
 def islinux(die=False):
-    ''' Alias to ``sc.getplatform('linux')`` '''
+    ''' Alias to :func:`sc.getplatform('linux') <getplatform>` '''
     return getplatform('linux', die=die)
 
 def ismac(die=False):
-    ''' Alias to ``sc.getplatform('mac')`` '''
+    ''' Alias to :func:`sc.getplatform('mac') <getplatform>` '''
     return getplatform('mac', die=die)
 
 
+def isjupyter(detailed=False):
+    '''
+    Check if a command is running inside a Jupyter notebook.
+    
+    Returns true/false if detailed=False, or a string for the exact type of notebook
+    (e.g., Google Colab) if detailed=True.
+    
+    Args:
+        detailed (bool): return a string of IPython/Jupyter type instead of true/false
+        verbose (bool): print out additional information if IPython can't be imported
+        
+    **Examples**::
+        
+        if sc.isjupyter():
+            sc.options(jupyter=True)
+        
+        if sc.isjupyter(detailed=True) == 'colab':
+            print('You are running on Google Colab')
+    
+    *New in version 3.0.0.*
+    '''
+    # First check if we can import it
+    output = None
+    is_jupyter = False
+    try:
+        from IPython import get_ipython
+        ipython = get_ipython()
+    except Exception as E: # pragma: no cover
+        output = f'Python (Jupyter/IPython is not installed) ({E})'
+        return output if detailed else is_jupyter
+    
+    # It's not IPython
+    if ipython is None:
+        output = 'Python (Jupyter/IPython is installed but not running)'
+        return output if detailed else is_jupyter
+
+    # It is IPython, keep checking
+    else: # pragma: no cover
+    
+        # Get the modules and classes
+        classes = inspect.getmro(ipython.__class__)
+        names = [str(c).lower() for c in classes] # Names as a list
+        firstname = names[0]
+        allnames = ', '.join(names)
+    
+        # Define strings to look for
+        mapping = dict(
+            jupyter = 'zmqinteractive',
+            ipython = 'terminalinteractive',
+            spyder  = 'spyder',
+            colab   = 'colab',
+        )
+        
+        # First check if it's Jupyter, and return if it is
+        if not detailed:
+            if mapping['jupyter'] in allnames and mapping['spyder'] not in allnames: # Spyder inherits from ZMQ, unlike e.g. Colab shell
+                is_jupyter = True
+            return is_jupyter
+        
+        # Otherwise, get the full name
+        else:
+            if   mapping['spyder']  in firstname: output = 'Spyder'
+            elif mapping['colab']   in firstname: output = 'Google Colab'
+            elif mapping['ipython'] in firstname: output = 'IPython'
+            elif mapping['jupyter'] in firstname: output = 'Jupyter'
+            else:
+                output = names[0]
+            
+            return output
+
+
 def asciify(string, form='NFKD', encoding='ascii', errors='ignore', **kwargs):
     '''
     Convert an arbitrary Unicode string to ASCII.
     
     Args:
         form (str): the type of Unicode normalization to use
         encoding (str): the output string to encode to
         errors (str): how to handle errors
-        kwargs (dict): passed to ``string.decode()``
+        kwargs (dict): passed to :meth:`string.decode()`
     
     **Example**:
         sc.asciify('föö→λ ∈ ℝ') # Returns 'foo  R'
     
-    New in version 2.0.1.
+    *New in version 2.0.1.*
     '''
     normalized = unicodedata.normalize(form, string) # First, normalize Unicode encoding
     encoded = normalized.encode(encoding, errors) # Then, convert to ASCII
     decoded = encoded.decode(**kwargs) # Finally, decode back to utf-8
     return decoded
 
 ##############################################################################
 #%% Web/HTML functions
 ##############################################################################
 
 __all__ += ['urlopen', 'wget', 'download', 'htmlify']
 
-def urlopen(url, filename=None, save=False, headers=None, params=None, data=None,
+def urlopen(url, filename=None, save=None, headers=None, params=None, data=None,
             prefix='http', convert=True, die=False, return_response=False, verbose=False):
     '''
     Download a single URL.
 
-    Alias to ``urllib.request.urlopen(url).read()``. See also :func:`download`
-    for downloading multiple URLs. Note: ``sc.urlopen()``/``sc.wget()`` are aliases.
+    Alias to ``urllib.request.urlopen(url).read()``. See also :func:`sc.download() <download>`
+    for downloading multiple URLs. Note: :func:`sc.urlopen() <urlopen>`/:func:`sc.wget() <wget>` are aliases.
 
     Args:
         url (str): the URL to open, either as GET or POST
         filename (str): if supplied, save to file instead of returning output
         save (bool): if supplied instead of ``filename``, then use the default filename
         headers (dict): a dictionary of headers to pass
         params (dict): a dictionary of parameters to pass to the GET request
@@ -572,17 +562,17 @@
 
     **Examples**::
 
         html = sc.urlopen('sciris.org') # Retrieve into variable html
         sc.urlopen('http://sciris.org', filename='sciris.html') # Save to file sciris.html
         sc.urlopen('http://sciris.org', save=True, headers={'User-Agent':'Custom agent'}) # Save to the default filename (here, sciris.org), with headers
 
-    | New in version 2.0.0: renamed from ``wget`` to ``urlopen``; new arguments
-    | New in version 2.0.1: creates folders by default if they do not exist
-    | New in version 2.0.4: "prefix" argument, e.g. prepend "http://" if not present
+    | *New in version 2.0.0:* renamed from ``wget`` to ``urlopen``; new arguments
+    | *New in version 2.0.1:* creates folders by default if they do not exist
+    | *New in version 2.0.4:* "prefix" argument, e.g. prepend "http://" if not present
     '''
     from urllib import request as ur # Need to import these directly, not via urllib
     from urllib import parse as up
     from . import sc_datetime as scd  # To avoid circular import
     from . import sc_fileio as scf # To avoid circular import
 
     T = scd.timer()
@@ -595,17 +585,17 @@
     headers = mergedicts(default_headers, headers)
 
     # Handle parameters and data
     full_url = url
     if prefix is not None:
         if not full_url.startswith(prefix):
             full_url = prefix + '://' + full_url # Leaves https alone, but adds http:// otherwise
-    if params is not None:
+    if params is not None: # pragma: no cover
         full_url = full_url + '?' + up.urlencode(params)
-    if data is not None:
+    if data is not None: # pragma: no cover
         data = up.urlencode(data).encode(encoding='utf-8', errors='ignore')
 
     if verbose: print(f'Downloading {url}...')
     request = ur.Request(full_url, headers=headers, data=data)
     response = ur.urlopen(request)
     output = response.read()
     if convert:
@@ -616,70 +606,73 @@
             if die:
                 raise E
             elif verbose:
                 errormsg = f'Could not decode to text: {str(E)}'
                 print(errormsg)
 
     # Set filename -- from https://stackoverflow.com/questions/31804799/how-to-get-pdf-filename-with-python-requests
-    if filename is None and save:
+    if filename is None and save: # pragma: no cover
         headers = dict(response.getheaders())
         string = "Content-Disposition"
         if string in headers.keys():
             filename = re.findall("filename=(.+)", headers[string])[0]
         else:
             filename = url.rstrip('/').split('/')[-1] # Remove trailing /, then pull out the last chunk
 
-    if filename is not None:
+    if filename is not None and save is not False:
         if verbose: print(f'Saving to {filename}...')
-        filename = scf.makefilepath(filename)
+        filename = scf.makefilepath(filename, makedirs=True)
         if isinstance(output, bytes):
-            with open(filename, 'wb') as f:
+            with open(filename, 'wb') as f: # pragma: no cover
                 f.write(output)
         else:
-            with open(filename, 'w') as f:
+            with open(filename, 'w', encoding='utf-8') as f: # Explicit encoding to avoid issues on Windows
                 f.write(output)
         output = filename
 
     if verbose:
         T.toc(f'Time to download {url}')
-    if return_response:
+    if return_response: # pragma: no cover
         output = response
 
     return output
 
 # Alias for backwards compatibility
 wget = urlopen
 
 
-def download(url, *args, filename=None, save=True, parallel=True, verbose=True, **kwargs):
+def download(url, *args, filename=None, save=True, parallel=True, die=True, verbose=True, **kwargs):
     '''
     Download one or more URLs in parallel and return output or save them to disk.
 
-    A wrapper for :func:`urlopen`, except with ``save=True`` by default.
+    A wrapper for :func:`sc.urlopen() <urlopen>`, except with ``save=True`` by default.
 
     Args:
         url (str/list/dict): either a single URL, a list of URLs, or a dict of URL:filename pairs
         *args (list): additional URLs to download
         filename (str/list): either a string or a list of the same length as ``url`` (if not supplied, return output)
         save (bool): if supplied instead of ``filename``, then use the default filename
         parallel (bool): whether to download multiple URLs in parallel
+        die (bool): whether to raise an exception if a URL can't be retrieved (default true)
         verbose (bool): whether to print progress (if verbose=2, print extra detail on each downloaded URL)
-        **kwargs (dict): passed to :func:`urlopen`
+        **kwargs (dict): passed to :func:`sc.urlopen() <urlopen>`
 
     **Examples**::
 
         html = sc.download('http://sciris.org') # Download a single URL
-        data = sc.download('http://sciris.org', 'http://covasim.org') # Download two in parallel
+        data = sc.download('http://sciris.org', 'http://covasim.org', save=False) # Download two in parallel
         sc.download({'http://sciris.org':'sciris.html', 'http://covasim.org':'covasim.html'}) # Downlaod two and save to disk
         sc.download(['http://sciris.org', 'http://covasim.org'], filename=['sciris.html', 'covasim.html']) # Ditto
 
-    New in version 2.0.0.
+    | *New in version 2.0.0.*
+    | *New in version 3.0.0:* "die" argument
     '''
     from . import sc_parallel as scp # To avoid circular import
     from . import sc_datetime as scd
+    from . import sc_odict as sco
 
     T = scd.timer()
 
     # Parse arguments
     if isinstance(url, dict):
         urls = list(url.keys())
         filenames = list(url.values())
@@ -700,20 +693,33 @@
         print(f'Downloading {n_urls} URL(s)...')
 
     # Get results in parallel
     wget_verbose = (verbose>1) or (verbose and n_urls == 1) # By default, don't print progress on each download
     iterkwargs = dict(url=urls, filename=filenames)
     func_kwargs = mergedicts(dict(save=save, verbose=wget_verbose), kwargs)
     if n_urls > 1 and parallel:
-        outputs = scp.parallelize(urlopen, iterkwargs=iterkwargs, kwargs=func_kwargs, parallelizer='thread')
+        outputs = scp.parallelize(urlopen, iterkwargs=iterkwargs, kwargs=func_kwargs, parallelizer='thread', die=die)
     else:
         outputs = []
         for url,filename in zip(urls, filenames):
-            output = urlopen(url=url, filename=filename, **func_kwargs)
+            try:
+                output = urlopen(url=url, filename=filename, **func_kwargs)
+            except Exception as E: # pragma: no cover
+                if die:
+                    raise E
+                else:
+                    warnmsg = f'Could not download {url}: {E}'
+                    warnings.warn(warnmsg, category=RuntimeWarning, stacklevel=2)
+                    output = E
+                    
             outputs.append(output)
+    
+    # If we're returning the data rather than saving the files, convert to an odict
+    if save is False:
+        outputs = sco.odict({k:v for k,v in zip(urls, outputs)})
 
     if verbose:
         T.toc(f'Time to download {n_urls} URLs')
     if n_urls == 1:
         outputs = outputs[0]
 
     return outputs
@@ -732,77 +738,204 @@
         output = sc.htmlify('foo&amp;<br>bar', reverse=True) # Returns 'foo&\\nbar'
     '''
     import html
     if not reverse: # Convert to HTML
         output = html.escape(string).encode('ascii', 'xmlcharrefreplace') # Replace non-ASCII characters
         output = output.replace(b'\n', b'<br>') # Replace newlines with <br>
         output = output.replace(b'\t', b'&nbsp;&nbsp;&nbsp;&nbsp;') # Replace tabs with 4 spaces
-        if tostring: # Convert from bytestring to unicode
+        if tostring: # Convert from bytestring to unicode # pragma: no cover
             output = output.decode()
     else: # Convert from HTML
         output = html.unescape(string)
         output = output.replace('<br>','\n').replace('<br />','\n').replace('<BR>','\n')
     return output
 
 
 ##############################################################################
 #%% Type functions
 ##############################################################################
 
-__all__ += ['flexstr', 'isiterable', 'checktype', 'isnumber', 'isstring', 'isarray',
+__all__ += ['flexstr', 'sanitizestr', 'isiterable', 'checktype', 'isnumber', 'isstring', 'isarray',
             'toarray', 'tolist', 'promotetoarray', 'promotetolist', 'transposelist',
             'swapdict', 'mergedicts', 'mergelists']
 
-def flexstr(arg, force=True):
+def flexstr(arg, *args, force=True, join=''):
     '''
     Try converting any object to a "regular" string (i.e. ``str``), but proceed
     if it fails. Note: this function calls ``repr()`` rather than ``str()`` to
     ensure a more robust representation of objects.
+    
+    Args:
+        arg (any): the object to convert to a string
+        args (list): additional arguments
+        force (bool): whether to force it to be a string
+        join (str): if multiple arguments are provided, the character to use to join
+    
+    **Example**:
+        
+        sc.flexstr(b'foo', 'bar', [1,2]) # Returns 'foobar[1, 2]'
+    
+    *New in version 3.0.0:* handle multiple inputs
     '''
-    if isinstance(arg, str):
-        return arg
-    elif isinstance(arg, bytes):
-        try:
-            output = arg.decode() # If it's bytes, decode to unicode
-        except: # pragma: no cover
-            if force: output = repr(arg) # If that fails, just print its representation
-            else:     output = arg
-    else: # pragma: no cover
-        if force: output = repr(arg)
-        else:     output = arg # Optionally don't do anything for non-strings
-    return output
+    arglist = mergelists(arg, list(args))
+    outlist = []
+    for arg in arglist:
+        if isinstance(arg, str):
+            output = arg
+        elif isinstance(arg, bytes):
+            try:
+                output = arg.decode() # If it's bytes, decode to unicode
+            except: # pragma: no cover
+                if force: output = repr(arg) # If that fails, just print its representation
+                else:     output = arg
+        else: # pragma: no cover
+            if force: output = repr(arg)
+            else:     output = arg # Optionally don't do anything for non-strings
+        outlist.append(output)
+    
+    if len(outlist) == 1:
+        outstr = outlist[0]
+    else:
+        if force:
+            outstr = join.join(outlist)
+        else:
+            outstr = outlist
+    
+    return outstr
 
 
-def isiterable(obj):
+def sanitizestr(string=None, alphanumeric=False, nospaces=False, asciify=False, 
+                lower=False, validvariable=False, spacechar='_', symchar='?'):
+    '''
+    Remove all non-"standard" characters from a string
+    
+    Can be used to e.g. generate a valid variable name from arbitrary input, remove
+    non-ASCII characters (replacing with equivalent ASCII ones if possible), etc.
+    
+    Args:
+        string (str): the string to sanitize
+        alphanumeric (bool): allow only alphanumeric characters
+        nospaces (bool): remove spaces
+        asciify (bool): remove non-ASCII characters
+        lower (bool): convert uppercase characters to lowercase
+        validvariable (bool): convert to a valid Python variable name (similar to alphanumeric=True, nospaces=True; uses spacechar to substitute)
+        spacechar (str): if nospaces is True, character to replace spaces with (can be blank)
+        symchar (str): character to replace non-alphanumeric characters with (can be blank)
+    
+    **Examples**::
+        
+        string1 = 'This Is a String'
+        sc.sanitizestr(string1, lower=True) # Returns 'this is a string'
+        
+        string2 = 'Lukáš wanted €500‽'
+        sc.sanitizestr(string2, asciify=True, nospaces=True, symchar='*') # Returns 'Lukas_wanted_*500*'
+        
+        string3 = '"Ψ scattering", María said, "at ≤5 μm?"'
+        sc.sanitizestr(string3, asciify=True, alphanumeric=True, nospaces=True, spacechar='') # Returns '??scattering??Mariasaid??at?5?m??'
+    
+        string4 = '4 path/names/to variable!'
+        sc.sanitizestr(string4, validvariable=True, spacechar='') # Returns '_4pathnamestovariable'
+    
+    *New in version 3.0.0.*
     '''
-    Simply determine whether or not the input is iterable.
+    string = flexstr(string)
+    if asciify:
+        newstr = ''
+        for char in string:
+            newchar = unicodedata.normalize('NFKD', char).encode('ascii', 'ignore').decode()
+            if not len(newchar):
+                newchar = symchar
+            newstr += newchar
+        string = newstr
+    if nospaces:
+        string = string.replace(' ', spacechar)
+    if lower:
+        string = string.lower()
+    if alphanumeric:
+        space = spacechar if nospaces else ' '
+        string = re.sub(f'[^0-9a-zA-Z{space}]', symchar, string) # If not for the space string, could use /w
+    if validvariable:
+        string = re.sub(r'\W', spacechar, string) # /W matches an non-alphanumeric character; use a raw string to avoid warnings
+        if not string or str.isdecimal(string[0]): # Don't allow leading decimals: here in case spacechar is None
+            string = '_' + string
+    return string
 
-    Works by trying to iterate via iter(), and if that raises an exception, it's
-    not iterable.
 
-    From http://stackoverflow.com/questions/1952464/in-python-how-do-i-determine-if-an-object-is-iterable
+def isiterable(obj, *args, exclude=None, minlen=None):
     '''
-    try:
-        iter(obj)
-        return True
-    except:
-        return False
+    Determine whether or not the input is iterable, with optional types to exclude.
+    
+    Args:
+        obj (any): object to check for iterability
+        args (any): additional objects to check for iterability
+        exclude (list): list of iterable objects to exclude (e.g., strings)
+        minlen (int): if not None, check that an object has a defined length as well
+    
+    **Examples**::
+        
+        obj1 = [1,2,3]
+        obj2 = 'abc'
+        obj3 = set()
+        
+        sc.isiterable(obj1) # Returns True
+        sc.isiterable(obj1, obj2, obj3, exclude=str, minlen=1) # returns [True, False, False]
+        
+    See also :func:`numpy.iterable()` for a simpler version.
+    
+    *New in version 3.0.0:* "exclude" and "minlen" args; support multiple arguments
+    '''
+    
+    # Handle arguments
+    objlist = [obj]
+    n_args = len(args)
+    exclude = tuple(tolist(exclude))
+    if n_args: # pragma: no cover
+        objlist.extend(args)
+        
+    # Determine iterability
+    output = []
+    for obj in objlist:
+        
+        # Basic test of iterability
+        tf = np.iterable(obj)
+        
+        # Additional checks
+        if tf:
+            
+            # Explicitly exclude types
+            if exclude and checktype(obj, exclude): 
+                tf = False
+            
+            # Check length
+            if minlen is not None: # pragma: no cover
+                try:
+                    assert len(obj) >= minlen
+                except:
+                    tf = False
+                    
+        output.append(tf)
+    
+    if not n_args:
+        output = output[0]
+    
+    return output
 
 
 def checktype(obj=None, objtype=None, subtype=None, die=False):
     '''
     A convenience function for checking instances. If objtype is a type,
     then this function works exactly like isinstance(). But, it can also
     be one of the following strings:
 
         - 'str', 'string': string or bytes object
         - 'num', 'number': any kind of number
         - 'arr', 'array': a Numpy array (equivalent to np.ndarray)
         - 'listlike': a list, tuple, or array
         - 'arraylike': a list, tuple, or array with numeric entries
+        - 'none': a None object
 
     If subtype is not None, then checktype will iterate over the object and check
     recursively that each element matches the subtype.
 
     Args:
         obj     (any):         the object to check the type of
         objtype (str or type): the type to confirm the object belongs to
@@ -812,26 +945,33 @@
     **Examples**::
 
         sc.checktype(rand(10), 'array', 'number') # Returns True
         sc.checktype(['a','b','c'], 'listlike') # Returns True
         sc.checktype(['a','b','c'], 'arraylike') # Returns False
         sc.checktype([{'a':3}], list, dict) # Returns True
     
-    New in version 2.0.1: ``pd.Series`` considered 'array-like'
+    | *New in version 2.0.1:* ``pd.Series`` considered 'array-like'
+    | *New in version 3.0.0:* allow list (in addition to tuple) of types; allow checking for NoneType
     '''
 
     # Handle "objtype" input
-    if   objtype in ['str','string']:          objinstance = _stringtypes
+    if isinstance(objtype, str): # Ensure it's lowercase (e.g. 'None' → 'none')
+        objtype = objtype.lower() 
+    if   objtype in ['none']:                  objinstance = type(None) # NoneType not available in Python <3.10
+    elif objtype in ['str','string']:          objinstance = _stringtypes
     elif objtype in ['num', 'number']:         objinstance = _numtype
     elif objtype in ['bool', 'boolean']:       objinstance = _booltypes
     elif objtype in ['arr', 'array']:          objinstance = np.ndarray
     elif objtype in ['listlike', 'arraylike']: objinstance = (list, tuple, np.ndarray, pd.Series) # Anything suitable as a numerical array
     elif type(objtype) == type:                objinstance = objtype # Don't need to do anything
     elif isinstance(objtype, tuple):           objinstance = objtype # Ditto
-    elif objtype is None:                      return # If not supplied, exit
+    elif isinstance(objtype, list):            objinstance = tuple(objtype) # Convert from a list to a tuple # pragma: no cover
+    elif objtype is None: # pragma: no cover
+        errormsg = "No object type was supplied; did you mean to use objtype='none' instead?"
+        raise ValueError(errormsg)
     else: # pragma: no cover
         errormsg = f'Could not understand what type you want to check: should be either a string or a type, not "{objtype}"'
         raise ValueError(errormsg)
 
     # Do first-round checking
     result = isinstance(obj, objinstance)
 
@@ -862,15 +1002,15 @@
     Args:
         obj (any): the object to check if it's a number
         isnan (bool): an optional additional check to determine whether the number is/isn't NaN
 
     Almost identical to isinstance(obj, numbers.Number).
     '''
     output = checktype(obj, 'number')
-    if output and isnan is not None: # It is a number, so can check for nan
+    if output and isnan is not None: # It is a number, so can check for nan # pragma: no cover
         output = (np.isnan(obj) == isnan) # See if they match
     return output
 
 
 def isstring(obj):
     '''
     Determine whether or not the input is string-like (i.e., str or bytes).
@@ -886,48 +1026,48 @@
 
     Almost the same as ``isinstance(obj, np.ndarray)``.
 
     **Example**::
 
         sc.isarray(np.array([1,2,3]), dtype=float) # False, dtype is int
 
-    New in version 1.0.0.
+    *New in version 1.0.0.*
     '''
     if isinstance(obj, np.ndarray):
         if dtype is None:
             return True
         else:
-            if obj.dtype == dtype:
+            if obj.dtype == dtype: # pragma: no cover
                 return True
             else:
                 return False
 
 
 def toarray(x, keepnone=False, **kwargs):
     '''
     Small function to ensure consistent format for things that should be arrays
-    (note: :func:`toarray()` and :func:`promotetoarray()` are identical).
+    (note: :func:`sc.toarray() <toarray>` and :func:`sc.promotetoarray() <promotetoarray>` are identical).
 
-    Very similar to ``np.array``, with the main difference being that ``sc.toarray(3)``
+    Very similar to :func:`numpy.array`, with the main difference being that :func:`sc.toarray(3) <toarray>`
     will return ``np.array([3])`` (i.e. a 1-d array that can be iterated over), while
     ``np.array(3)`` will return a 0-d array that can't be iterated over.
 
     Args:
         x (any): a number or list of numbers
         keepnone (bool): whether ``sc.toarray(None)`` should return ``np.array([])`` or ``np.array([None], dtype=object)``
-        kwargs (dict): passed to ``np.array()``
+        kwargs (dict): passed to :func:`numpy.array()`
 
     **Examples**::
 
         sc.toarray(5) # Returns np.array([5])
         sc.toarray([3,5]) # Returns np.array([3,5])
         sc.toarray(None, skipnone=True) # Returns np.array([])
 
-    | New in version 1.1.0: replaced "skipnone" with "keepnone"; allowed passing kwargs to ``np.array()``.
-    | New in version 2.0.1: added support for pandas Series and DataFrame
+    | *New in version 1.1.0:* replaced "skipnone" with "keepnone"; allowed passing kwargs to ``np.array()``.
+    | *New in version 2.0.1:* added support for pandas Series and DataFrame
     '''
     skipnone = kwargs.pop('skipnone', None)
     if skipnone is not None: # pragma: no cover
         keepnone = not(skipnone)
         warnmsg = 'sc.toarray() argument "skipnone" has been deprecated as of v1.1.0; use keepnone instead'
         warnings.warn(warnmsg, category=FutureWarning, stacklevel=2)
     if isnumber(x) or (isinstance(x, np.ndarray) and not np.shape(x)): # e.g. 3 or np.array(3)
@@ -938,15 +1078,15 @@
         x = []
     output = np.array(x, **kwargs)
     return output
 
 
 def tolist(obj=None, objtype=None, keepnone=False, coerce='default'):
     '''
-    Make sure object is always a list (note: :func:`tolist`/:func:`promotetolist` are identical).
+    Make sure object is always a list (note: :func:`sc.tolist() <tolist>`/:func:`sc.promotetolist() <promotetolist>` are identical).
 
     Used so functions can handle inputs like ``'a'``  or ``['a', 'b']``. In other
     words, if an argument can either be a single thing (e.g., a single dict key)
     or a list (e.g., a list of dict keys), this function can be used to do the
     conversion, so it's always safe to iterate over the output.
 
     While this usually wraps objects in a list rather than converts them to a list,
@@ -955,18 +1095,20 @@
     - 'none' or None: do not coerce
     - 'default': coerce objects that were lists in Python 2 (range, map, dict_keys, dict_values, dict_items)
     - 'tuple': all the types in default, plus tuples
     - 'full': all the types in default, plus tuples and arrays
 
     Args:
         obj (anything): object to ensure is a list
-        objtype (anything): optional type to check for each element; see :func:`checktype` for details
+        objtype (anything): optional type to check for each element; see :func:`sc.checktype() <checktype>` for details
         keepnone (bool): if ``keepnone`` is false, then ``None`` is converted to ``[]``; else, it's converted to ``[None]``
         coerce (str/tuple):  tuple of additional types to coerce to a list (as opposed to wrapping in a list)
 
+    See also :func:`sc.mergelists() <mergelists>` to handle multiple input arguments.
+
     **Examples**::
 
         sc.tolist(5) # Returns [5]
         sc.tolist(np.array([3,5])) # Returns [np.array([3,5])] -- not [3,5]!
         sc.tolist(np.array([3,5]), coerce=np.ndarray) # Returns [3,5], since arrays are coerced to lists
         sc.tolist(None) # Returns []
         sc.tolist(range(3)) # Returns [0,1,2] since range is coerced by default
@@ -977,31 +1119,33 @@
             for key in keys:
                 print(data[key])
 
         data = {'a':[1,2,3], 'b':[4,5,6]}
         myfunc(data, keys=['a', 'b']) # Works
         myfunc(data, keys='a') # Still works, equivalent to needing to supply keys=['a'] without tolist()
 
-    | New in version 1.1.0: "coerce" argument
-    | New in version 1.2.2: default coerce values
-    | New in version 2.0.2: tuple coersion
+    | *New in version 1.1.0:* "coerce" argument
+    | *New in version 1.2.2:* default coerce values
+    | *New in version 2.0.2:* tuple coersion
     '''
     # Handle coerce
     default_coerce = (range, map, type({}.keys()), type({}.values()), type({}.items()))
     if isinstance(coerce, str):
         if coerce == 'none':
             coerce = None
         elif coerce == 'default':
             coerce = default_coerce
-        elif coerce == 'tuple':
+        elif coerce == 'tuple': # pragma: no cover
             coerce = default_coerce + (tuple,)
+        elif coerce == 'array': # pragma: no cover
+            coerce = default_coerce + (np.ndarray,)
         elif coerce == 'full':
             coerce = default_coerce + (tuple, np.ndarray)
-        else:
-            errormsg = f'Option "{coerce}"; not recognized; must be "none", "default", or "full"'
+        else: # pragma: no cover
+            errormsg = f'Option "{coerce}"; not recognized; must be "none", "default", "tuple", or "full"'
 
     if objtype is None: # Don't do type checking
         if isinstance(obj, list):
             output = obj # If it's already a list and we're not doing type checking, just return
         elif obj is None:
             if keepnone:
                 output = [None] # Wrap in a list
@@ -1031,41 +1175,61 @@
 
 
 # Aliases for core functions
 promotetoarray = toarray
 promotetolist = tolist
 
 
-def transposelist(obj):
+def transposelist(obj, fix_uneven=True):
     '''
     Convert e.g. a list of key-value tuples into a list of keys and a list of values.
+    
+    Args:
+        obj (list): the list-of-lists to be transposed
+        fix_uneven (bool): append None values where needed so all input lists have the same length
 
-    **Example**::
+    **Examples**::
 
         o = sc.odict(a=1, b=4, c=9, d=16)
         itemlist = o.enumitems()
         inds, keys, vals = sc.transposelist(itemlist)
-
-    New in version 1.1.0.
-    '''
+        
+        listoflists = [
+            ['a', 1, 3],
+            ['b', 4, 5],
+            ['c', 7, 8, 9, 10]
+        ]
+        trans = sc.transposelist(listoflists, fix_uneven=True)
+
+    *New in version 1.1.0.*
+    '''
+    if fix_uneven:
+        maxlen = max([len(ls) for ls in obj])
+        newobj = [] # Create a manual copy
+        for ls in obj:
+            row = [item for item in ls] + [None]*(maxlen - len(ls))
+            newobj.append(row)
+        obj = newobj
+        
     return list(map(list, zip(*obj)))
+        
 
 
 def swapdict(d):
     '''
     Swap the keys and values of a dictionary. Equivalent to {v:k for k,v in d.items()}
 
     Args:
         d (dict): dictionary
 
     **Example**::
         d1 = {'a':'foo', 'b':'bar'}
         d2 = sc.swapdict(d1) # Returns {'foo':'a', 'bar':'b'}
 
-    New in version 1.3.0.
+    *New in version 1.3.0.*
     '''
     if not isinstance(d, dict):
         errormsg = f'Not a dictionary: {type(d)}'
         raise TypeError(errormsg)
     try:
         output = {v:k for k,v in d.items()}
     except Exception as E:
@@ -1074,25 +1238,26 @@
         raise exc(errormsg) from E
     return output
 
 
 def mergedicts(*args, _strict=False, _overwrite=True, _copy=False, _sameclass=True, _die=True, **kwargs):
     '''
     Small function to merge multiple dicts together.
-
+    
     By default, skips any input arguments that are ``None``, and allows keys to be set 
     multiple times. This function is similar to dict.update(), except it returns a value.
     The first dictionary supplied will be used for the output type (e.g. if the
     first dictionary is an odict, an odict will be returned).
 
     Note that arguments start with underscores to avoid possible collisions with
-    keywords (e.g. ``sc.mergedicts(dict(loose=True, strict=True), strict=False, _strict=True)``).
+    keywords (e.g. :func:`sc.mergedicts(dict(loose=True, strict=True), strict=False, _strict=True) <mergedicts>`).
 
-    This function is useful for cases, e.g. function arguments, where the default 
-    option is ``None`` but you will need a dict later on.
+    **Note**: This function is similar to the "|" operator introduced in Python 3.9.
+    However, ``sc.mergedicts()`` is useful for cases such as function arguments, where 
+    the default option is ``None`` but you will need a dict later on.
 
     Args:
         _strict    (bool): if True, raise an exception if an argument isn't a dict
         _overwrite (bool): if False, raise an exception if multiple keys are found
         _copy      (bool): whether or not to deepcopy the merged dictionary
         _sameclass (bool): whether to ensure the output has the same type as the first dictionary merged
         _die       (bool): whether to raise an exception if something goes wrong
@@ -1103,37 +1268,39 @@
 
         d0 = sc.mergedicts(user_args) # Useful if user_args might be None, but d0 is always a dict
         d1 = sc.mergedicts({'a':1}, {'b':2}) # Returns {'a':1, 'b':2}
         d2 = sc.mergedicts({'a':1, 'b':2}, {'b':3, 'c':4}, None) # Returns {'a':1, 'b':3, 'c':4}
         d3 = sc.mergedicts(sc.odict({'b':3, 'c':4}), {'a':1, 'b':2}) # Returns sc.odict({'b':2, 'c':4, 'a':1})
         d4 = sc.mergedicts({'b':3, 'c':4}, {'a':1, 'b':2}, _overwrite=False) # Raises exception
 
-    | New in version 1.1.0: "copy" argument
-    | New in version 1.3.3: keywords allowed
-    | New in version 2.0.0: keywords fully enabled; "_sameclass" argument
-    | New in version 2.0.1: fixed bug with "_copy" argument
+    | *New in version 1.1.0:* "copy" argument
+    | *New in version 1.3.3:* keywords allowed
+    | *New in version 2.0.0:* keywords fully enabled; "_sameclass" argument
+    | *New in version 2.0.1:* fixed bug with "_copy" argument
     '''
     # Warn about deprecated keys
     renamed = ['strict', 'overwrite', 'copy']
-    if any([k in kwargs for k in renamed]):
+    if any([k in kwargs for k in renamed]): # pragma: no cover
         warnmsg = f'sc.mergedicts() arguments "{strjoin(renamed)}" have been renamed with underscores as of v1.3.3; using these as keywords is undesirable'
         warnings.warn(warnmsg, category=FutureWarning, stacklevel=2)
 
     # Try to get the output type from the arguments, but revert to a standard dict if that fails
     outputdict = {}
     if _sameclass:
         for arg in args:
             if isinstance(arg, dict):
                 try:
                     outputdict = arg.__class__() # This creates a new instance of the class
                     break
-                except Exception as E:
+                except Exception as E: # pragma: no cover
                     errormsg = f'Could not create new dict of {type(args[0])} from first argument ({str(E)}); set _sameclass=False if this is OK'
-                    if _die: raise TypeError(errormsg) from E
-                    else:    print(errormsg)
+                    if _die:
+                        raise TypeError(errormsg) from E
+                    else:
+                        warnings.warn(errormsg, category=UserWarning, stacklevel=2)
 
     # Merge over the dictionaries in order
     args = list(args)
     args.append(kwargs) # Include any kwargs as the final dict
     for a,arg in enumerate(args):
         is_dict = isinstance(arg, dict)
         if _strict and not is_dict:
@@ -1143,46 +1310,64 @@
             if not _overwrite:
                 intersection = set(outputdict.keys()).intersection(arg.keys())
                 if len(intersection):
                     errormsg = f'Could not merge dicts since keys "{strjoin(intersection)}" overlap and _overwrite=False'
                     raise KeyError(errormsg)
             outputdict.update(arg)
         else:
-            if arg is not None and _die:
+            if arg is not None and _die: # pragma: no cover
                 errormsg = f'Could not handle argument {a} of {type(arg)}: expecting dict or None'
                 raise TypeError(errormsg)
 
     if _copy:
         outputdict = dcp(outputdict, die=_die)
     return outputdict
 
 
-def mergelists(*args, copy=False, **kwargs):
+def mergelists(*args, coerce='default', copy=False, **kwargs):
     '''
     Merge multiple lists together.
+    
+    Often used to flexible handle the input arguments to functions; see example
+    below.
 
     Args:
         args (any): the lists, or items, to be joined together into a list
+        coerce (str): what types of objects to treat as lists; see :func:`sc.tolist() <tolist>` for details
         copy (bool): whether to deepcopy the resultant object
-        kwargs (dict): passed to :func:`tolist`, which is called on each argument
+        kwargs (dict): passed to :func:`sc.tolist() <tolist>`, which is called on each argument
 
     **Examples**::
 
-        sc.mergelists(None) # Returns []
-        sc.mergelists([1,2,3], [4,5,6]) # Returns [1, 2, 3, 4, 5, 6]
-        sc.mergelists([1,2,3], 4, 5, 6) # Returns [1, 2, 3, 4, 5, 6]
-        sc.mergelists([(1,2), (3,4)], (5,6)) # Returns [(1, 2), (3, 4), (5, 6)]
-        sc.mergelists((1,2), (3,4), (5,6)) # Returns [(1, 2), (3, 4), (5, 6)]
-        sc.mergelists((1,2), (3,4), (5,6), coerce=tuple) # Returns [1, 2, 3, 4, 5, 6]
+        # Simple usage
+        sc.mergelists(None)                                # Returns []
+        sc.mergelists([1,2,3], [4,5,6])                    # Returns [1, 2, 3, 4, 5, 6]
+        sc.mergelists([1,2,3], 4, 5, 6)                    # Returns [1, 2, 3, 4, 5, 6]
+        sc.mergelists([(1,2), (3,4)], (5,6))               # Returns [(1, 2), (3, 4), (5, 6)]
+        sc.mergelists((1,2), (3,4), (5,6))                 # Returns [(1, 2), (3, 4), (5, 6)]
+        sc.mergelists((1,2), (3,4), (5,6), coerce='tuple') # Returns [1, 2, 3, 4, 5, 6]
+        
+        # Usage for handling flexible input arguments
+        def my_func(arg=None, *args):
+            arglist = sc.mergelists(arg, list(args))
+            return arglist
+
+        a = my_func()           # Returns []
+        b = my_func([1,2,3])    # Returns [1,2,3]
+        c = my_func(1,2,3)      # Returns [1,2,3]
+        d = my_func([1,2], 3)   # Returns [1,2,3]
+        f = my_func(1, *[2,3])  # Returns [1,2,3]
+        e = my_func(1, [2,3])   # Returns [1,[2,3]] since second argument is ambiguous
+        g = my_func([[1,2]], 3) # Returns [[1,2],3] since first argument is nested
 
-    New in version 1.1.0.
+    *New in version 1.1.0.*
     '''
     obj = []
     for arg in args:
-        arg = tolist(arg, **kwargs)
+        arg = tolist(arg, coerce=coerce, **kwargs)
         obj.extend(arg)
     if copy:
         obj = dcp(obj)
     return obj
 
 
 def _sanitize_iterables(obj, *args):
@@ -1221,16 +1406,16 @@
     return output
 
 
 ##############################################################################
 #%% Misc. functions
 ##############################################################################
 
-__all__ += ['strjoin', 'newlinejoin', 'strsplit', 'runcommand', 'gitinfo', 'compareversions',
-            'uniquename', 'suggest', 'getcaller', 'importbyname']
+__all__ += ['strjoin', 'newlinejoin', 'strsplit', 'runcommand', 'uniquename', 
+            'suggest', 'importbyname', 'importbypath']
 
 
 def strjoin(*args, sep=', '):
     '''
     Like string ``join()``, but handles more flexible inputs, converts items to
     strings. By default, join with commas.
 
@@ -1238,46 +1423,46 @@
         args (list): the list of items to join
         sep (str): the separator string
 
     **Example**::
 
         sc.strjoin([1,2,3], 4, 'five')
 
-    New in version 1.1.0.
+    *New in version 1.1.0.*
     '''
     obj = []
     for arg in args:
         if isstring(arg):
             obj.append(arg)
         elif isiterable(arg):
             obj.extend([str(item) for item in arg])
-        else:
+        else: # pragma: no cover
             obj.append(str(arg))
     output = sep.join(obj)
     return output
 
 
 def newlinejoin(*args):
     '''
     Alias to ``strjoin(*args, sep='\\n')``.
 
     **Example**::
 
         sc.newlinejoin([1,2,3], 4, 'five')
 
-    New in version 1.1.0.
+    *New in version 1.1.0.*
     '''
     return strjoin(*args, sep='\n')
 
 
 def strsplit(string, sep=None, skipempty=True, lstrip=True, rstrip=True):
     '''
     Convenience function to split common types of strings.
 
-    Note: to use regular expressions, use ``re.split()`` instead.
+    Note: to use regular expressions, use :func:`re.split()` instead.
 
     Args:
         string    (str):      the string to split
         sep       (str/list): the types of separator to accept (default space or comma, i.e. [' ', ','])
         skipempty (bool):     whether to skip empty entries (i.e. from consecutive delimiters)
         lstrip    (bool):     whether to strip any extra spaces on the left
         rstrip    (bool):     whether to strip any extra spaces on the right
@@ -1285,23 +1470,23 @@
     Examples:
 
         sc.strsplit('a b c') # Returns ['a', 'b', 'c']
         sc.strsplit('a,b,c') # Returns ['a', 'b', 'c']
         sc.strsplit('a, b, c') # Returns ['a', 'b', 'c']
         sc.strsplit('  foo_bar  ', sep='_') # Returns ['foo', 'bar']
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     '''
     strlist = []
     if sep is None:
         sep = [' ', ',']
 
     # Generate a character sequence that isn't in the string
-    special = '∙' # Pick an obscure character
-    while special in string: # If it exists in the string nonetheless, keep going until it doesn't
+    special = '∙' # Pick an obscure Unicode character
+    while special in string: # If it exists in the string nonetheless, keep going until it doesn't # pragma: no cover
         special += special
 
     # Convert all separators to the special character
     for s in sep:
         string = string.replace(s, special)
 
     # Split the string, filter, and trim
@@ -1316,15 +1501,15 @@
     return strlist
 
 
 def runcommand(command, printinput=False, printoutput=False, wait=True):
     '''
     Make it easier to run shell commands.
 
-    Alias to ``subprocess.Popen()``.
+    Alias to :obj:`subprocess.Popen()`.
 
     **Examples**::
 
         myfiles = sc.runcommand('ls').split('\\n') # Get a list of files in the current folder
         sc.runcommand('sshpass -f %s scp myfile.txt me@myserver:myfile.txt' % 'pa55w0rd', printinput=True, printoutput=True) # Copy a file remotely
         sc.runcommand('sleep 600; mkdir foo', wait=False) # Waits 10 min, then creates the folder "foo", but the function returns immediately
 
@@ -1334,184 +1519,24 @@
         print(command)
     try:
         p = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         if wait: # Whether to run in the background
             stderr = p.stdout.read().decode("utf-8") # Somewhat confusingly, send stderr to stdout
             stdout = p.communicate()[0].decode("utf-8") # ...and then stdout to the pipe
             output = stdout + '\n' + stderr if stderr else stdout # Only include the error if it was non-empty
-        else:
+        else: # pragma: no cover
             output = ''
     except Exception as E: # pragma: no cover
         output = f'runcommand(): shell command failed: {str(E)}' # This is for a Python error, not a shell error -- those get passed to output
     if printoutput:
         print(output)
     return output
 
 
 
-def gitinfo(path=None, hashlen=7, die=False, verbose=True):
-    """
-    Retrieve git info
-
-    This function reads git branch and commit information from a .git directory.
-    Given a path, it will check for a ``.git`` directory. If the path doesn't contain
-    that directory, it will search parent directories for ``.git`` until it finds one.
-    Then, the current information will be parsed.
-
-    Note: if direct directory reading fails, it will attempt to use the gitpython
-    library.
-
-    Args:
-        path (str): A folder either containing a .git directory, or with a parent that contains a .git directory
-        hashlen (int): Length of hash to return (default: 7)
-        die (bool): whether to raise an exception if git information can't be retrieved (default: no)
-        verbose (bool): if not dying, whether to print information about the exception
-
-    Returns:
-        Dictionary containing the branch, hash, and commit date
-
-    **Examples**::
-
-        info = sc.gitinfo() # Get git info for current script repository
-        info = sc.gitinfo(my_package.__file__) # Get git info for a particular Python package
-    """
-
-    if path is None:
-        path = os.getcwd()
-
-    gitbranch = "Branch N/A"
-    githash   = "Hash N/A"
-    gitdate   = "Date N/A"
-
-    try:
-        # First, get the .git directory
-        curpath = os.path.dirname(os.path.abspath(path))
-        while curpath:
-            if os.path.exists(os.path.join(curpath, ".git")):
-                gitdir = os.path.join(curpath, ".git")
-                break
-            else: # pragma: no cover
-                parent, _ = os.path.split(curpath)
-                if parent == curpath:
-                    curpath = None
-                else:
-                    curpath = parent
-        else: # pragma: no cover
-            raise RuntimeError("Could not find .git directory")
-
-        # Then, get the branch and commit
-        with open(os.path.join(gitdir, "HEAD"), "r") as f1:
-            ref = f1.read()
-            if ref.startswith("ref:"):
-                refdir = ref.split(" ")[1].strip()  # The path to the file with the commit
-                gitbranch = refdir.replace("refs/heads/", "")  # / is always used (not os.sep)
-                with open(os.path.join(gitdir, refdir), "r") as f2:
-                    githash = f2.read().strip()  # The hash of the commit
-            else: # pragma: no cover
-                gitbranch = "Detached head (no branch)"
-                githash = ref.strip()
-
-        # Now read the time from the commit
-        with open(os.path.join(gitdir, "objects", githash[0:2], githash[2:]), "rb") as f3:
-            compressed_contents = f3.read()
-            decompressed_contents = zlib.decompress(compressed_contents).decode()
-            for line in decompressed_contents.split("\n"):
-                if line.startswith("author"):
-                    _re_actor_epoch = re.compile(r"^.+? (.*) (\d+) ([+-]\d+).*$")
-                    m = _re_actor_epoch.search(line)
-                    actor, epoch, offset = m.groups()
-                    t = time.gmtime(int(epoch))
-                    gitdate = time.strftime("%Y-%m-%d %H:%M:%S UTC", t)
-
-    except Exception as E: # pragma: no cover
-        try: # Second, try importing gitpython
-            import git
-            rootdir = os.path.abspath(path) # e.g. /user/username/my/folder
-            repo = git.Repo(path=rootdir, search_parent_directories=True)
-            try:
-                gitbranch = str(repo.active_branch.name)  # Just make sure it's a string
-            except TypeError:
-                gitbranch = 'Detached head (no branch)'
-            githash = str(repo.head.object.hexsha)
-            gitdate = str(repo.head.object.authored_datetime.isoformat())
-        except Exception as E2:
-            errormsg = f'''Could not extract git info; please check paths:
-  Method 1 (direct read) error: {str(E)}
-  Method 2 (gitpython) error:   {str(E2)}'''
-            if die:
-                raise RuntimeError(errormsg) from E
-            elif verbose:
-                print(errormsg + f'\nError: {str(E)}')
-
-    # Trim the hash, but not if loading failed
-    if len(githash)>hashlen and 'N/A' not in githash:
-        githash = githash[:hashlen]
-
-    # Assemble output
-    output = {"branch": gitbranch, "hash": githash, "date": gitdate}
-
-    return output
-
-
-def compareversions(version1, version2):
-    '''
-    Function to compare versions, expecting both arguments to be a string of the
-    format 1.2.3, but numeric works too. Returns 0 for equality, -1 for v1<v2, and
-    1 for v1>v2.
-
-    If ``version2`` starts with >, >=, <, <=, or ==, the function returns True or
-    False depending on the result of the comparison.
-
-    **Examples**::
-
-        sc.compareversions('1.2.3', '2.3.4') # returns -1
-        sc.compareversions(2, '2') # returns 0
-        sc.compareversions('3.1', '2.99') # returns 1
-        sc.compareversions('3.1', '>=2.99') # returns True
-        sc.compareversions(mymodule.__version__, '>=1.0') # common usage pattern
-        sc.compareversions(mymodule, '>=1.0') # alias to the above
-
-    New in version 1.2.1: relational operators
-    '''
-    # Handle inputs
-    if isinstance(version1, types.ModuleType):
-        try:
-            version1 = version1.__version__
-        except Exception as E:
-            errormsg = f'{version1} is a module, but does not have a __version__ attribute'
-            raise AttributeError(errormsg) from E
-    v1 = str(version1)
-    v2 = str(version2)
-
-    # Process version2
-    valid = None
-    if   v2.startswith('>'):  valid = [1]
-    elif v2.startswith('>='): valid = [0,1]
-    elif v2.startswith('='):  valid = [0]
-    elif v2.startswith('=='): valid = [0]
-    elif v2.startswith('~='): valid = [-1,1]
-    elif v2.startswith('!='): valid = [-1,1]
-    elif v2.startswith('<='): valid = [0,-1]
-    elif v2.startswith('<'):  valid = [-1]
-    v2 = v2.lstrip('<>=!~')
-
-    # Do comparison
-    if packaging.version.parse(v1) > packaging.version.parse(v2):
-        comparison =  1
-    elif packaging.version.parse(v1) < packaging.version.parse(v2):
-        comparison =  -1
-    else:
-        comparison =  0
-
-    # Return
-    if valid is None:
-        return comparison
-    else:
-        tf = (comparison in valid)
-        return tf
 
 
 def uniquename(name=None, namelist=None, style=None):
     """
     Given a name and a list of other names, find a replacement to the name
     that doesn't conflict with the other names, and pass it back.
 
@@ -1596,15 +1621,15 @@
     order = np.argsort(distance)
     suggestions = [valid_inputs[i] for i in order]
     suggestionstr = strjoin([f'"{sugg}"' for sugg in suggestions[:n]])
 
     # Handle threshold
     if threshold is None:
         threshold = np.ceil(len(user_input)*2/3)
-    if threshold < 0:
+    if threshold < 0: # pragma: no cover
         threshold = np.inf
 
     # Output
     if min(distance) > threshold:
         if die: # pragma: no cover
             errormsg = f'"{user_input}" not found'
             raise ValueError(errormsg)
@@ -1620,124 +1645,76 @@
         else:
             if n==1:
                 return suggestions[0]
             else:
                 return suggestions[:n]
 
 
-def getcaller(frame=2, tostring=True, includelineno=False, includeline=False):
-    '''
-    Try to get information on the calling function, but fail gracefully. See also
-    :func:`thisfile`.
-
-    Frame 1 is the file calling this function, so not very useful. Frame 2 is
-    the default assuming it is being called directly. Frame 3 is used if
-    another function is calling this function internally.
-
-    Args:
-        frame (int): how many frames to descend (e.g. the caller of the caller of the...), default 2
-        tostring (bool): whether to return a string instead of a dict with filename and line number
-        includelineno (bool): if ``tostring``, whether to also include the line number
-        includeline (bool): if not ``tostring``, also store the line contents
-
-    Returns:
-        output (str/dict): the filename (and line number) of the calling function, either as a string or dict
-
-    **Examples**::
-
-        sc.getcaller()
-        sc.getcaller(tostring=False)['filename'] # Equivalent to sc.getcaller()
-        sc.getcaller(frame=3) # Descend one level deeper than usual
-        sc.getcaller(frame=1, tostring=False, includeline=True) # See the line that called sc.getcaller()
-
-    | New in version 1.0.0.
-    | New in version 1.3.3: do not include line by default
-    '''
-    try:
-        import inspect
-        result = inspect.getouterframes(inspect.currentframe(), 2)
-        fname = str(result[frame][1])
-        lineno = result[frame][2]
-        if tostring:
-            output = f'{fname}'
-            if includelineno:
-                output += f', line {lineno}'
-        else:
-            output = {'filename':fname, 'lineno':lineno}
-            if includeline:
-                try:
-                    with open(fname) as f:
-                        lines = f.read().splitlines()
-                        line = lines[lineno-1] # -1 since line numbers start at 1
-                    output['line'] = line
-                except: # Fail silently
-                    output['line'] = 'N/A'
-    except Exception as E: # pragma: no cover
-        if tostring:
-            output = f'Calling function information not available ({str(E)})'
-        else:
-            output = {'filename':'N/A', 'lineno':'N/A'}
-    return output
-
-
-def _assign_to_namespace(var, obj, namespace=None, overwrite=True):
+def _assign_to_namespace(var, obj, namespace=None, overwrite=True): # pragma: no cover
     ''' Helper function to assign an object to the global namespace '''
     if namespace is None:
         namespace = globals()
     if var in namespace and not overwrite:
         errormsg = f'Cannot assign to variable "{var}" since it already exists and overwrite=False'
         raise NameError(errormsg)
     namespace[var] = obj
     return
 
 
-def importbyname(module=None, variable=None, namespace=None, lazy=False, overwrite=True, die=True, verbose=True, **kwargs):
+def importbyname(module=None, variable=None, path=None, namespace=None, lazy=False, overwrite=True, die=True, verbose=True, **kwargs):
     '''
     Import modules by name.
 
     See https://peps.python.org/pep-0690/ for a proposal for incorporating something
     similar into Python by default.
 
     Args:
         module (str): name of the module to import
         variable (str): the name of the variable to assign the module to (by default, the module's name)
+        path (str/path): optionally load from path instead of by name
         namespace (dict): the namespace to load the modules into (by default, globals)
         lazy (bool): whether to create a LazyModule object instead of load the actual module
         overwrite (bool): whether to allow overwriting an existing variable (by default, yes)
         die (bool): whether to raise an exception if encountered
         verbose (bool): whether to print a warning if an module can't be imported
         **kwargs (dict): additional variable:modules pairs to import (see examples below)
 
     **Examples**::
 
-        np = sc.importbyname('numpy')
-        sc.importbyname(pd='pandas', np='numpy')
-        pl = sc.importbyname(pl='matplotlib.pyplot', lazy=True) # Won't actually import until e.g. pl.figure() is called
+        np = sc.importbyname('numpy') # Standard usage
+        sc.importbyname(pd='pandas', np='numpy') # Use dictionary syntax to assign to namespace
+        plt = sc.importbyname(plt='matplotlib.pyplot', lazy=True) # Won't actually import until e.g. pl.figure() is called
+        mymod = sc.importbyname(path='/path/to/mymod') # Import by path rather than name
+    
+    See also :func:`sc.importbypath() <importbypath>`.
 
-    New in version 2.1.0: "verbose" argument
+    | *New in version 2.1.0:* "verbose" argument
+    | *New in version 3.0.0:* "path" argument
     '''
     # Initialize
-    import importlib
     if variable is None:
         variable = module
 
     # Map modules to variables
     mapping = {}
-    if module is not None:
-        mapping[variable] = module
+    if module is not None or path is not None:
+        mapping[variable] = (path or module) # In this order so path takes precedence
     mapping.update(kwargs)
 
     # Load modules
     libs = []
     for variable,module in mapping.items():
         if lazy:
             lib = LazyModule(module=module, variable=variable, namespace=namespace)
         else:
             try:
-                lib = importlib.import_module(module)
+                if path is not None:
+                    lib = importbypath(path, variable)
+                else:
+                    lib = importlib.import_module(module)
             except Exception as E: # pragma: no cover
                 errormsg = f'Cannot import "{module}" since {module} is not installed. Please install {module} and try again.'
                 if verbose and not die:
                     print(errormsg)
                 lib = None
                 if die: raise E
                 else:   return False
@@ -1749,14 +1726,59 @@
 
     if len(libs) == 1:
         libs = libs[0]
 
     return libs
 
 
+def importbypath(path, name=None):
+    '''
+    Import a module by path.
+    
+    Useful for importing multiple versions of the same module for comparison purposes.
+    
+    Args:
+        path (str/path): the path to load the module from (with or without __init__.py)
+        name (str): the name of the loaded module (by default, the file or folder name from the path)
+    
+    **Examples**::
+        
+        # Load a module that isn't importable otherwise
+        mymod = sc.importbypath('my file with spaces.py')
+        
+        # Load two versions of the same folder
+        old = sc.importbypath('/path/to/old/lib', name='oldlib')
+        new = sc.importbypath('/path/to/new/lib', name='newlib')
+    
+    See also :func:`sc.importbyname() <importbyname>`.
+
+    *New in version 3.0.0.*
+    '''
+    # Sanitize the path and filename
+    default_file='__init__.py'
+    filepath = Path(path)
+    parts = list(filepath.parts)
+    if filepath.is_dir():
+        filepath = filepath / default_file # Append default filename
+    elif not filepath.is_file():
+        errormsg = f'Could not import {filepath}: is not a valid file or folder'
+        raise FileNotFoundError(errormsg)
+    
+    # Construct the name from either the filename or the folder name
+    if name is None:
+        basename = parts[-1].removesuffix('.py')
+        name = sanitizestr(basename, validvariable=True) # Convert directory name to a string
+    
+    # From https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
+    spec = importlib.util.spec_from_file_location(name, filepath)
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[name] = module
+    spec.loader.exec_module(module)
+    return module
+
 
 ##############################################################################
 #%% Classes
 ##############################################################################
 
 __all__ += ['KeyNotFoundError', 'LinkException', 'prettyobj', 'autolist', 'Link', 'LazyModule', 'tryexcept']
 
@@ -1772,73 +1794,99 @@
         raise sc.KeyNotFoundError('The key "foo" is not available, but these are: "bar", "cat"')
     '''
 
     def __str__(self): # pragma: no cover
         return Exception.__str__(self)
 
 
-class LinkException(Exception):
+class LinkException(Exception): # pragma: no cover
     '''
     An exception to raise when links are broken, for exclusive use with the Link
     class.
     '''
 
     def __init(self, *args, **kwargs):
         Exception.__init__(self, *args, **kwargs)
 
 
 class prettyobj(object):
     '''
     Use pretty repr for objects, instead of just showing the type and memory pointer
     (the Python default for objects). Can also be used as the base class for custom
     classes.
+    
+    Args:
+        args (dict): dictionaries which are used to assign attributes
+        kwargs (any): can also be used to assign attributes
+
+    **Example 1**::
 
-    **Examples**
+        myobj = sc.prettyobj(a=3)
+        print(myobj)
+        
+        # <sciris.sc_utils.prettyobj at 0x7fbba4a97f40>
+        # ————————————————————————————————————————————————————————————
+        # Methods:
+        #   Methods N/A         
+        # ————————————————————————————————————————————————————————————
+        # a: 3
+        # ————————————————————————————————————————————————————————————
+
+    **Example 2**::
+
+        myobj = sc.prettyobj(a=3)
+        myobj.b = {'a':6}
+        print(myobj)
+        
+        # <sciris.sc_utils.prettyobj at 0x7ffa1e243910>
+        # ————————————————————————————————————————————————————————————
+        # Methods:
+        #   Methods N/A         
+        # ————————————————————————————————————————————————————————————
+        # a: 3
+        # b: {'a': 6}
+        # ————————————————————————————————————————————————————————————
 
-        >>> myobj = sc.prettyobj()
-        >>> myobj.a = 3
-        >>> myobj.b = {'a':6}
-        >>> print(myobj)
-        <sciris.sc_utils.prettyobj at 0x7ffa1e243910>
-        ————————————————————————————————————————————————————————————
-        a: 3
-        b: {'a': 6}
-        ————————————————————————————————————————————————————————————
-
-        >>> class MyObj(sc.prettyobj):
-        >>>
-        >>>     def __init__(self, a, b):
-        >>>         self.a = a
-        >>>         self.b = b
-        >>>
-        >>>     def mult(self):
-        >>>         return self.a * self.b
-        >>>
-        >>> myobj = MyObj(a=4, b=6)
-        >>> print(myobj)
-        <__main__.MyObj at 0x7fd9acd96c10>
-        ————————————————————————————————————————————————————————————
-        Methods:
-          mult()
-        ————————————————————————————————————————————————————————————
-        a: 4
-        b: 6
-        ————————————————————————————————————————————————————————————
 
-    | New in version 2.0.0: allow positional arguments
+    **Example 3**::
+        
+        class MyObj(sc.prettyobj):
+       
+            def __init__(self, a, b):
+                self.a = a
+                self.b = b
+       
+            def mult(self):
+                return self.a * self.b
+       
+        myobj = MyObj(a=4, b=6)
+        print(myobj)
+        
+        # <__main__.MyObj at 0x7fd9acd96c10>
+        # ————————————————————————————————————————————————————————————
+        # Methods:
+        #   mult()
+        # ————————————————————————————————————————————————————————————
+        # a: 4
+        # b: 6
+        # ————————————————————————————————————————————————————————————
+
+    | *New in version 2.0.0:* allow positional arguments
     '''
 
     def __init__(self, *args, **kwargs):
+        ''' Simple initialization '''
         kwargs = mergedicts(*args, kwargs)
         for k,v in kwargs.items():
             self.__dict__[k] = v
         return
 
 
     def __repr__(self):
+        ''' The point of this class: use a more detailed repr by default '''
         from . import sc_printing as scp # To avoid circular import
         output  = scp.prepr(self)
         return output
 
 
 class autolist(list):
     '''
@@ -1857,15 +1905,15 @@
         arglist = mergelists(*args) # Convert non-iterables to iterables
         list.__init__(self, arglist)
         return 
 
     def __add__(self, obj=None):
         ''' Allows non-lists to be concatenated '''
         obj = tolist(obj)
-        new = autolist(list.__add__(self, obj)) # Ensure it returns an autolist
+        new = self.__class__(list.__add__(self, obj)) # Ensure it returns an autolist
         return new
 
     def __iadd__(self, obj):
         ''' Allows += to work correctly -- key feature of autolist '''
         obj = tolist(obj)
         self.extend(obj)
         return self
@@ -1918,28 +1966,28 @@
         return self.__copy__(*args, **kwargs)
 
 
 class LazyModule:
     '''
     Create a "lazy" module that is loaded if and only if an attribute is called.
 
-    Typically not for use by the user, but is used by :func:`importbyname`.
+    Typically not for use by the user, but is used by :func:`sc.importbyname() <importbyname>`.
 
     Args:
         module (str): name of the module to (not) load
         variable (str): variable name to assign the module to
         namespace (dict): the namespace to use (if not supplied, globals())
         overwrite (bool): whether to allow overwriting an existing variable (by default, yes)
 
     **Example**::
 
         pd = sc.LazyModule('pandas', 'pd') # pd is a LazyModule, not actually pandas
         df = pd.DataFrame() # Not only does this work, but pd is now actually pandas
 
-    New in version 2.0.0.
+    *New in version 2.0.0.*
     '''
 
     def __init__(self, module, variable, namespace=None, overwrite=True):
         self._variable  = variable
         self._module    = module
         self._namespace = namespace
         self._overwrite = overwrite
@@ -1950,38 +1998,39 @@
         output = f"<sc.LazyModule({self._variable}='{self._module}') at {hex(id(self))}>"
         return output
 
 
     def __getattr__(self, attr):
         ''' In most cases, when an attribute is retrieved we want to replace this module with the actual one '''
         _builtin_keys = ['_variable', '_module', '_namespace', '_overwrite', '_load']
-        if attr in _builtin_keys:
+        if attr in _builtin_keys: # pragma: no cover
             obj = object.__getattribute__(self, attr)
         else:
             obj = self._load(attr)
         return obj
 
 
     def _load(self, attr=None):
         ''' Stop being lazy and load the module '''
-        import importlib
         var = self._variable
         lib = importlib.import_module(self._module)
         _assign_to_namespace(var, lib, namespace=self._namespace, overwrite=self._overwrite)
         if attr:
             obj = getattr(lib, attr)
-        else:
+        else: # pragma: no cover
             obj = lib
         return obj
     
 
 class tryexcept(cl.suppress):
     '''
-    Simple class to catch exceptions in a single line -- effectively an alias to
-    contextlib.suppress.
+    Simple class to catch exceptions in a single line
+    
+    Effectively an alias to :obj:`contextlib.suppress()`, which itself is a programmatic
+    equivalent to using try-except blocks.
     
     By default, all errors are caught. If ``catch`` is not None, then by default 
     raise all other exceptions; if ``die`` is an exception (list of exceptions, 
     then by default suppress all other exceptions.
     
     Due to Python's fundamental architecture, exceptions can only be caught inside
     a with statement, and the with block will exit immediately as soon as the first
@@ -2011,47 +2060,48 @@
         # Storing the history of multiple exceptions
         tryexc = None
         for i in range(5):
             with sc.tryexcept(history=tryexc) as tryexc:
                 print(values[i])
         tryexc.print()
             
-    New in version 2.1.0.
+    | *New in version 2.1.0.*
+    | *New in version 3.0.0:* renamed "print" to "traceback"; added "to_df" and "disp" options
     '''
 
     def __init__(self, die=None, catch=None, verbose=1, history=None):
         
         # Handle defaults
         dietypes   = []
         catchtypes = []
         if die is None and catch is None: # Default: do not die
             self.defaultdie = False
-        elif die in [True, False, 0, 1]: # It's truthy: use it directly
+        elif die in [True, False, 0, 1]: # It's truthy: use it directly # pragma: no cover
             self.defaultdie = die
         elif die is None and catch is not None: # We're asked to catch some things, so die otherwise
             self.defaultdie = True
             catchtypes = tolist(catch)
         elif die is not None and catch is None: # Vice versa
             self.defaultdie = False
             dietypes = tolist(die)
-        else:
+        else: # pragma: no cover
             errormsg = 'Unexpected input to "die" and "catch": typically only one or the other should be provided'
             raise ValueError(errormsg)
         
         # Finish initialization
         self.dietypes   = tuple(dietypes)
         self.catchtypes = tuple(catchtypes)
         self.verbose    = verbose
         self.exceptions = []
         if history is not None:
-            if isinstance(history, (list, tuple)):
+            if isinstance(history, (list, tuple)): # pragma: no cover
                 self.exceptions.extend(list(history))
             elif isinstance(history, tryexcept):
                 self.exceptions.extend(history.exceptions)
-            else:
+            else: # pragma: no cover
                 errormsg = f'Could not understand supplied history: must be a list or a tryexcept object, not {type(history)}'
                 raise TypeError(errormsg)
         return
     
     
     def __repr__(self):
         from . import sc_printing as scp # To avoid circular import
@@ -2067,26 +2117,41 @@
         if exc_type is not None:
             self.exceptions.append([exc_type, exc_val, traceback])
             die = (self.defaultdie or issubclass(exc_type, self.dietypes))
             live = issubclass(exc_type, self.catchtypes)
             if die and not live:
                 return
             else:
-                if self.verbose > 1: # Print everything
+                if self.verbose > 1: # Print everything # pragma: no cover
                     self.print()
                 elif self.verbose: # Just print the exception type
                     print(exc_type, exc_val)
                 return True
 
     
-    def print(self, which=-1):
+    def traceback(self, which=-1):
         ''' Print the exception (usually the last) '''
         if len(self.exceptions):
             py_traceback.print_exception(*self.exceptions[which])
-        else:
+        else: # pragma: no cover
             print('No exceptions were encountered; nothing to trace')
         return
     
     
+    def to_df(self):
+        ''' Convert the exceptions to a dataframe '''
+        from . import sc_dataframe as scd # To avoid circular import
+        df = scd.dataframe(self.exceptions, columns=['type','value','traceback'])
+        self.df = df
+        return df
+    
+    
+    def disp(self):
+        ''' Display all exceptions as a table '''
+        df = self.to_df()
+        df.disp()
+        return
+    
+    
     @property
     def died(self):
         return len(self.exceptions) > 0
```

### Comparing `sciris-2.1.0/setup.py` & `sciris-3.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,42 +3,25 @@
 '''
 Sciris is a flexible open source framework for building scientific web
 applications using Python and JavaScript. This library provides the underlying
 functions and data structures that support the webapp features, as well as
 being generally useful for scientific computing.
 '''
 
-from setuptools import setup, find_packages
 import os
 import sys
 import runpy
+from setuptools import setup, find_packages
 
 # Get the current folder
 cwd = os.path.abspath(os.path.dirname(__file__))
 
-# Define the requirements for core functionality
-requirements = [
-        'matplotlib',   # Plotting
-        'numpy',        # Numerical functions
-        'pandas',       # Dataframes and spreadsheet input
-        'openpyxl',     # To read Excel files; removed as a dependency of pandas as of version 1.3
-        'xlsxwriter',   # Spreadsheet output
-        'psutil',       # Load monitoring
-        'dill',         # For pickling more complex object types
-        'zstandard',    # For a more efficient compression algorithm
-        'multiprocess', # More flexible version of multiprocessing
-        'jsonpickle',   # For converting arbitrary objects to JSON
-        'pyyaml',       # For loading/saving YAML
-        'packaging',    # For parsing versions
-        'gitpython',    # Git version information
-        'jellyfish',    # For fuzzy string matching
-        'line_profiler ;   platform_system == "Linux"',   # For the line profiler -- only install on Linux
-        'memory_profiler ; platform_system == "Linux"',   # For the memory profiler -- only install on Linux
-        'colorama ;        platform_system == "Windows"', # For colored text output -- only install on Windows
-        ]
+# Load requirements from txt file
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
 
 # Get version
 versionpath = os.path.join(cwd, 'sciris', 'sc_version.py')
 version = runpy.run_path(versionpath)['__version__']
 
 # Get the documentation
 with open(os.path.join(cwd, 'README.rst'), "r") as fh:
@@ -51,14 +34,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Scientific/Engineering',
 ]
 
 setup(
     name='sciris',
     version=version,
```

