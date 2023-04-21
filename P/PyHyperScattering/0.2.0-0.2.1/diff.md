# Comparing `tmp/PyHyperScattering-0.2.0.tar.gz` & `tmp/PyHyperScattering-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHyperScattering-0.2.0.tar", last modified: Wed Apr  5 18:01:07 2023, max compression
+gzip compressed data, was "PyHyperScattering-0.2.1.tar", last modified: Fri Apr 21 13:12:37 2023, max compression
```

## Comparing `PyHyperScattering-0.2.0.tar` & `PyHyperScattering-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:01:07.004974 PyHyperScattering-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/src/PyHyperScattering/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10030 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/ALS11012RSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/ESRFID2Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/FileIO.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9282 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/FileLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12893 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/Fitting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4242 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/HDR.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/IntegrationUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/Nexus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10274 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/PFEnergySeriesIntegrator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/PFGeneralIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/PlotTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/RSoXS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/SMIRSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    51075 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/SST1RSoXSDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/SST1RSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/WPIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/src/PyHyperScattering/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/cyrsoxsLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/src/PyHyperScattering/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-05 18:01:06.000000 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-05 18:01:07.000000 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 18:01:06.000000 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 18:01:06.000000 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 18:01:06.000000 PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:01:07.008973 PyHyperScattering-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_11012Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_PFIntegrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_RSoXS.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_SMILoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_SST1Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_WPintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_autoversioning.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_cyrsoxsLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-05 18:00:57.000000 PyHyperScattering-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:12:37.136153 PyHyperScattering-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/src/PyHyperScattering/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10030 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/ALS11012RSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/ESRFID2Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/FileIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9282 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/FileLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12893 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/Fitting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4242 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/HDR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/IntegrationUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/Nexus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10274 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/PFEnergySeriesIntegrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/PFGeneralIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/PlotTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/RSoXS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/SMIRSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50951 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/SST1RSoXSDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/SST1RSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/WPIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/src/PyHyperScattering/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/cyrsoxsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/src/PyHyperScattering/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-21 13:12:37.000000 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-21 13:12:37.000000 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:12:37.000000 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 13:12:37.000000 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 13:12:37.000000 PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:12:37.140153 PyHyperScattering-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_11012Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_PFIntegrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_RSoXS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_SMILoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_SST1Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_WPintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_autoversioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_cyrsoxsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-21 13:12:21.000000 PyHyperScattering-0.2.1/versioneer.py
```

### Comparing `PyHyperScattering-0.2.0/LICENSE` & `PyHyperScattering-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/PKG-INFO` & `PyHyperScattering-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHyperScattering
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for loading, reducing, fitting, and plotting hyperspectral x-ray and neutron scattering data.
 Home-page: https://github.com/usnistgov/pyhyperscattering
 Author: Peter Beaucage
 Author-email: peter.beaucage@nist.gov
 Project-URL: Github, https://github.com/usnistgov/pyhyperscattering
 Project-URL: Project Site, https://www.nist.gov/laboratories/tools-instruments/polarized-resonant-soft-x-ray-scattering-p-rsoxs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyHyperScattering-0.2.0/README.md` & `PyHyperScattering-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/setup.cfg` & `PyHyperScattering-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/ALS11012RSoXSLoader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/ALS11012RSoXSLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/ESRFID2Loader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/ESRFID2Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/FileIO.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/FileIO.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/FileLoader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/FileLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/Fitting.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/HDR.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/HDR.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/IntegrationUtils.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/IntegrationUtils.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/Nexus.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/Nexus.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/PFEnergySeriesIntegrator.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/PFEnergySeriesIntegrator.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/PFGeneralIntegrator.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/PFGeneralIntegrator.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/PlotTools.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/PlotTools.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/RSoXS.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/RSoXS.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/SMIRSoXSLoader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/SMIRSoXSLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/SST1RSoXSDB.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/SST1RSoXSDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import copy
 try:
     os.environ["TILED_SITE_PROFILES"] = "/nsls2/software/etc/tiled/profiles"
     from tiled.client import from_profile
     from httpx import HTTPStatusError
     import tiled
     import dask
-    from databroker.queries import RawMongo, Key, FullText, Contains, Regex
+    from databroker.queries import RawMongo, Key, FullText, Contains, Regex, ScanIDRange
+    from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 except:
     print(
         "Imports failed.  Are you running on a machine with proper libraries for databroker, tiled, etc.?"
     )
 
 import copy
 
@@ -136,17 +137,18 @@
         user: str = None,
         institution: str = None,
         project: str = None,
         sample: str = None,
         sampleID: str = None,
         plan: str = None,
         userOutputs: list = [],
+        debugWarnings: bool = False,
         **kwargs,
     ) -> pd.DataFrame:
-        """Search the databroker.client.CatalogOfBlueskyRuns for scans matching all provided keywords and return metadata as a dataframe.
+        """Search the Bluesky catalog for scans matching all provided keywords and return metadata as a dataframe.
 
         Matches are made based on the values in the top level of the 'start' dict within the metadata of each
         entry in the Bluesky Catalog (databroker.client.CatalogOfBlueskyRuns). Based on the search arguments provided,
         a pandas dataframe is returned where rows correspond to catalog entries (scans) and columns contain  metadata.
         Several presets are provided for choosing which columns are generated, along with an interface for
         user-provided search arguments and additional metadata. Fails gracefully on bad user input/ changes to
         underlying metadata scheme.
@@ -196,17 +198,17 @@
                     db_loader.summarize_run(sample="BBP_PFP09A", outputType='scans', **kwargs)
             userOutputs (list of lists, optional): Additional metadata to be added to output can be specified as a list of lists. Each
                 sub-list specifies a metadata field as a 3 element list of format:
                 [Output column title (str), Metadata label (str), Metadata Source (raw str)],
                 Valid options for the Metadata Source are any of [r'catalog.start', r'catalog.start["plan_args"], r'catalog.stop',
                 r'catalog.stop["num_events"]']
                 e.g., userOutputs = [["Exposure Multiplier","exptime", r'catalog.start'], ["Stop Time","time",r'catalog.stop']]
-
+            debugWarnings (bool, optional): if True, raises a warning with debugging information whenever a key can't be found.
         Returns:
-            pd.Dataframe containing the results of the search, or an empty dataframe if the search fails
+            Pandas dataframe containing the results of the search, or an empty dataframe if the search fails
         """
 
         # Pull in the reference to the databroker.client.CatalogOfBlueskyRuns attribute
         bsCatalog = self.c
 
         ### Part 1: Search the database sequentially, reducing based on matches to search terms
         # Plan the 'default' search through the keyword parameters, build list of [metadata ID, user input value, match type]
@@ -229,34 +231,28 @@
             if isinstance(value, str):
                 userSearchList.append([userLabel, value, ""])
             elif isinstance(value, int) or isinstance(value, float):
                 userSearchList.append([userLabel, value, "numeric"])
             elif isinstance(value, list) and len(value) == 2:
                 userSearchList.append([userLabel, value[0], value[1]])
             else:  # bad user input
-                warnString = (
-                    "Error parsing a keyword search term, check the format.\nSkipped argument: "
-                    + str(value)
-                )
-                warnings.warn(warnString, stacklevel=2)
+                raise ValueError(
+                    f"Error parsing a keyword search term, check the format.  Skipped argument: {value} ")
 
         # combine the lists of lists
         fullSearchList = defaultSearchDetails + userSearchList
 
         df_SearchDet = pd.DataFrame(
             fullSearchList, columns=["Metadata field:", "User input:", "Search scheme:"]
         )
 
         # Iterate through search terms sequentially, reducing the size of the catalog based on successful matches
 
         reducedCatalog = bsCatalog
-        loopDesc = "Searching by keyword arguments"
-        for index, searchSeries in tqdm(
-            df_SearchDet.iterrows(), total=df_SearchDet.shape[0], desc=loopDesc
-        ):
+        for _,searchSeries in tqdm(df_SearchDet.iterrows(),total = df_SearchDet.shape[0], desc = "Running catalog search..."):
 
             # Skip arguments with value None, and quits if the catalog was reduced to 0 elements
             if (searchSeries[1] is not None) and (len(reducedCatalog) > 0):
 
                 # For numeric entries, do Key equality
                 if "numeric" in str(searchSeries[2]):
                     reducedCatalog = reducedCatalog.search(
@@ -282,52 +278,47 @@
                     reducedCatalog = reducedCatalog.search(
                         Regex(searchSeries[0], regexString)
                     )
 
                 # If a match fails, notify the user which search parameter yielded 0 results
                 if len(reducedCatalog) == 0:
                     warnString = (
-                        "Catalog reduced to zero when attempting to match the following condition:\n"
-                        + searchSeries.to_string()
-                        + "\n If this is a user-provided search parameter, check spelling/syntax.\n"
+                        f"Catalog reduced to zero when attempting to match {searchSeries}\n"
+                        +f"If this is a user-provided search parameter, check spelling/syntax."
                     )
                     warnings.warn(warnString, stacklevel=2)
                     return pd.DataFrame()
 
         ### Part 2: Build and return output dataframe
 
-        if (
-            outputType == "scans"
-        ):  # Branch 2.1, if only scan IDs needed, build and return a 1-column dataframe
+        if (outputType == "scans"):  
+            # Branch 2.1, if only scan IDs needed, build and return a 1-column dataframe
             scan_ids = []
-            loopDesc = "Building scan list"
-            for index, scanEntry in tqdm(
-                (enumerate(reducedCatalog)), total=len(reducedCatalog), desc=loopDesc
-            ):
-                scan_ids.append(reducedCatalog[scanEntry].start["scan_id"])
+            for scanEntry in tqdm(reducedCatalog.values(), desc = "Building scan list"):
+                scan_ids.append(scanEntry.start["scan_id"])
             return pd.DataFrame(scan_ids, columns=["Scan ID"])
 
         else:  # Branch 2.2, Output metadata from a variety of sources within each the catalog entry
-
+            missesDuringLoad = False
             # Store details of output values as a list of lists
             # List elements are [Output Column Title, Bluesky Metadata Code, Metadata Source location, Applicable Output flag]
             outputValueLibrary = [
                 ["scan_id", "scan_id", r"catalog.start", "default"],
                 ["uid", "uid", r"catalog.start", "ext_bio"],
-                ["start time", "time", r"catalog.start", "default"],
+                ["start_time", "time", r"catalog.start", "default"],
                 ["cycle", "cycle", r"catalog.start", "default"],
                 ["saf", "SAF", r"catalog.start", "ext_bio"],
                 ["user_name", "user_name", r"catalog.start", "ext_bio"],
                 ["institution", "institution", r"catalog.start", "default"],
                 ["project", "project_name", r"catalog.start", "default"],
                 ["sample_name", "sample_name", r"catalog.start", "default"],
                 ["sample_id", "sample_id", r"catalog.start", "default"],
                 ["bar_spot", "bar_spot", r"catalog.start", "ext_msmt"],
                 ["plan", "plan_name", r"catalog.start", "default"],
-                ["detector", "RSoXS_Main_DET", r"catalog.start", "default"],
+                ["detector", "RSoXS_Main_DET", r"catalog.start", "default"], 
                 ["polarization", "pol", r'catalog.start["plan_args"]', "default"],
                 ["sample_rotation", "angle", r"catalog.start", "ext_msmt"],
                 ["exit_status", "exit_status", r"catalog.stop", "default"],
                 ["num_Images", "primary", r'catalog.stop["num_events"]', "default"],
             ]
 
             # Subset the library based on the output flag selected
@@ -346,19 +337,15 @@
             userOutputList = []
             for userOutEntry in userOutputs:
                 # Minimial check for bad user input
                 if isinstance(userOutEntry, list) and len(userOutEntry) == 3:
                     activeOutputValues.append(userOutEntry)
                     activeOutputLabels.append(userOutEntry[0])
                 else:  # bad user input
-                    warnString = (
-                        "Error parsing user-provided output request, check the format.\nSkipped: "
-                        + str(userOutEntry)
-                    )
-                    warnings.warn(warnString, stacklevel=2)
+                    raise ValueError(f"Error parsing user-provided output request {userOutEntry}, check the format.", stacklevel=2)
 
             # Add any user-provided search terms
             for userSearchEntry in userSearchList:
                 activeOutputValues.append(
                     [
                         userSearchEntry[0],
                         userSearchEntry[0],
@@ -367,78 +354,71 @@
                     ]
                 )
                 activeOutputLabels.append(userSearchEntry[0])
 
             # Build output dataframe as a list of lists
             outputList = []
 
-            # Outer loop: Catalog entries
-            loopDesc = "Building output dataframe"
-            for index, scanEntry in tqdm(
-                (enumerate(reducedCatalog)), total=len(reducedCatalog), desc=loopDesc
-            ):
-
+            # Outer loop: Catalog entries 
+            for scanEntry in tqdm(reducedCatalog.values(),desc = "Retrieving results..."):
                 singleScanOutput = []
 
                 # Pull the start and stop docs once
-                currentCatalogStart = reducedCatalog[scanEntry].start
-                currentCatalogStop = reducedCatalog[scanEntry].stop
-
+                               
+                currentCatalogStart = scanEntry.start
+                currentCatalogStop = scanEntry.stop
+                
                 currentScanID = currentCatalogStart["scan_id"]
-
+                
                 # Inner loop: append output values
                 for outputEntry in activeOutputValues:
                     outputVariableName = outputEntry[0]
                     metaDataLabel = outputEntry[1]
                     metaDataSource = outputEntry[2]
 
                     try:  # Add the metadata value depending on where it is located
-                        if metaDataSource == r"catalog.start":
+                        if metaDataLabel == 'time':
+                            singleScanOutput.append(datetime.datetime.fromtimestamp(currentCatalogStart['time']))
+                            # see Zen of Python # 9,8 for justification
+                        elif metaDataSource == r"catalog.start":
                             singleScanOutput.append(currentCatalogStart[metaDataLabel])
                         elif metaDataSource == r'catalog.start["plan_args"]':
                             singleScanOutput.append(
                                 currentCatalogStart["plan_args"][metaDataLabel]
                             )
                         elif metaDataSource == r"catalog.stop":
                             singleScanOutput.append(currentCatalogStop[metaDataLabel])
                         elif metaDataSource == r'catalog.stop["num_events"]':
                             singleScanOutput.append(
                                 currentCatalogStop["num_events"][metaDataLabel]
                             )
                         else:
-                            warnString = (
-                                "Scan: > "
-                                + str(currentScanID)
-                                + " < Failed to locate metaData entry for > "
-                                + str(outputVariableName)
-                                + " <\n Tried looking for label: > "
-                                + str(metaDataLabel)
-                                + " < in: "
-                                + str(metaDataSource)
-                            )
-                            warnings.warn(warnString, stacklevel=2)
+                            if debugWarnings:
+                                warnings.warn(
+                                f'Failed to locate metadata for {outputVariableName} in scan {currentScanID}.',
+                                    stacklevel=2)
+                            missesDuringLoad = True
 
                     except (KeyError, TypeError):
-                        warnString = (
-                            "Scan: > "
-                            + str(currentScanID)
-                            + " < Failed to locate metaData entry for > "
-                            + str(outputVariableName)
-                            + " <\n Tried looking for label: > "
-                            + str(metaDataLabel)
-                            + " < in: "
-                            + str(metaDataSource)
-                        )
-                        warnings.warn(warnString, stacklevel=2)
+                        if debugWarnings:
+                            warnings.warn(
+                                f'Failed to locate metadata for {outputVariableName} in scan {currentScanID}.',
+                                    stacklevel=2)
+                        missesDuringLoad = True
                         singleScanOutput.append("N/A")
 
                 # Append to the filled output list for this entry to the list of lists
                 outputList.append(singleScanOutput)
-
+                
+                 
             # Convert to dataframe for export
+            if missesDuringLoad:
+                            warnings.warn(
+                                f'One or more missing field(s) during this load were replaced with "N/A".  Re-run with debugWarnings=True to see details.',
+                                    stacklevel=2)
             return pd.DataFrame(outputList, columns=activeOutputLabels)
 
     def background(f):
         def wrapped(*args, **kwargs):
             return asyncio.get_event_loop().run_in_executor(None, f, *args, **kwargs)
 
         return wrapped
@@ -777,15 +757,15 @@
             Bluesky Document containing run information.
             ex: phs.load.SST1RSoXSDB.c[scanID] or databroker.client.CatalogOfBlueskyRuns[scanID]
         integrate_onto_images : bool, optional
             whether or not to map timepoints to the image measurement times (as held by the 'primary' stream), by default True
             Presently bins are averaged between measurements intervals.
         useShutterThinning : bool, optional
             Whether or not to attempt to thin (filter) the raw time streams to remove data collected during shutter opening/closing, by default False
-            As of 230209 at NSLS2 SST1, using useShutterThinning= True for exposure times of < 0.5s is
+            As of 9 Feb 2023 at NSLS2 SST1, using useShutterThinning= True for exposure times of < 0.5s is
             not recommended because the shutter data is unreliable and too many points will be culled
         n_thinning_iters : int, optional
             how many iterations of thinning to perform, by default 5
             If the data is becoming too sparse, try fewer iterations
         Returns
         -------
         xr.Dataset
@@ -869,15 +849,15 @@
                     .drop_indexes("time_bins")
                     .reset_coords("time_bins", drop=True)
                 )
 
             except Exception as e:
                 # raise e # for testing
                 warnings.warn(
-                    "Error while time-integrating onto images.  Check data.",
+                    "Error while time-integrating monitors onto images.  Usually, this indicates a problem with the monitors, this is a critical error if doing normalization otherwise fine to ignore.",
                     stacklevel=2,
                 )
         return monitors
 
     def loadMd(self, run):
         """
         return a dict of metadata entries from the databroker run xarray
```

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/SST1RSoXSLoader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/SST1RSoXSLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/WPIntegrator.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/WPIntegrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,17 @@
             assert len(stacked_axis)==1, f"More than one axis left ({stacked_axis}) after removing qx and qy, not sure how to handle"
             stacked_axis = stacked_axis[0]
             system_to_integ = img.__getattr__(stacked_axis)
         except AttributeError:
             pass
         
         if self.MACHINE_HAS_CUDA:
-            TwoD = self.warp_polar_gpu(img_to_integ,center=(center_x,center_y), radius = np.nanmax(img_to_integ.shape))
+            TwoD = self.warp_polar_gpu(img_to_integ,center=(center_x,center_y), radius = np.sqrt((img_to_integ.shape[0] - center_x)**2 + (img_to_integ.shape[1] - center_y)**2))
         else:
-            TwoD = skimage.transform.warp_polar(img_to_integ,center=(center_x,center_y), radius = np.nanmax(img_to_integ.shape))
+            TwoD = skimage.transform.warp_polar(img_to_integ,center=(center_x,center_y), radius = np.sqrt((img_to_integ.shape[0] - center_x)**2 + (img_to_integ.shape[1] - center_y)**2))
 
         
         qx = img.qx
         qy = img.qy
         q = np.sqrt(qy**2+qx**2)
         q = np.linspace(0,np.amax(q), TwoD.shape[1])
```

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering/cyrsoxsLoader.py` & `PyHyperScattering-0.2.1/src/PyHyperScattering/cyrsoxsLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/PKG-INFO` & `PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHyperScattering
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for loading, reducing, fitting, and plotting hyperspectral x-ray and neutron scattering data.
 Home-page: https://github.com/usnistgov/pyhyperscattering
 Author: Peter Beaucage
 Author-email: peter.beaucage@nist.gov
 Project-URL: Github, https://github.com/usnistgov/pyhyperscattering
 Project-URL: Project Site, https://www.nist.gov/laboratories/tools-instruments/polarized-resonant-soft-x-ray-scattering-p-rsoxs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyHyperScattering-0.2.0/src/PyHyperScattering.egg-info/SOURCES.txt` & `PyHyperScattering-0.2.1/src/PyHyperScattering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_11012Loader.py` & `PyHyperScattering-0.2.1/tests/test_11012Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_PFIntegrators.py` & `PyHyperScattering-0.2.1/tests/test_PFIntegrators.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_RSoXS.py` & `PyHyperScattering-0.2.1/tests/test_RSoXS.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_SMILoader.py` & `PyHyperScattering-0.2.1/tests/test_SMILoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_SST1Loader.py` & `PyHyperScattering-0.2.1/tests/test_SST1Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_WPintegrator.py` & `PyHyperScattering-0.2.1/tests/test_WPintegrator.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/tests/test_cyrsoxsLoader.py` & `PyHyperScattering-0.2.1/tests/test_cyrsoxsLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.0/versioneer.py` & `PyHyperScattering-0.2.1/versioneer.py`

 * *Files identical despite different names*

