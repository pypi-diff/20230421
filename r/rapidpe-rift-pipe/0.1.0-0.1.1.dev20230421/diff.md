# Comparing `tmp/rapidpe_rift_pipe-0.1.0.tar.gz` & `tmp/rapidpe_rift_pipe-0.1.1.dev20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.1.0.tar", last modified: Thu Apr 20 19:21:14 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.1.1.dev20230421.tar", last modified: Fri Apr 21 05:14:57 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.1.0.tar` & `rapidpe_rift_pipe-0.1.1.dev20230421.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.770469 rapidpe_rift_pipe-0.1.0/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.772469 rapidpe_rift_pipe-0.1.0/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)     9851 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-20 19:21:14.778469 rapidpe_rift_pipe-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.770469 rapidpe_rift_pipe-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.775469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-20 18:16:57.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37438 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18220 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.776469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-19 02:10:50.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31369 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-20 16:12:20.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.776469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.215358 rapidpe_rift_pipe-0.1.1.dev20230421/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.217358 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)     9851 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.215358 rapidpe_rift_pipe-0.1.1.dev20230421/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.219358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37438 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18220 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31369 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.1.0/COPYING` & `rapidpe_rift_pipe-0.1.1.dev20230421/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/PKG-INFO` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe_rift_pipe
-Version: 0.1.0
+Name: rapidpe-rift-pipe
+Version: 0.1.1.dev20230421
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.1.0/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/setup.cfg` & `rapidpe_rift_pipe-0.1.1.dev20230421/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = 
+tag_build = dev.20230421
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/pastro.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             lambda x: np.exp(lnb(x)), xmin, np.inf, limit=1000
         )
 
         A, dA = scipy.integrate.quad(
             lambda x: np.exp(x + lnb(x) - np.log(B)), xmin, np.inf, limit=1000
         )
 
-        return A
+        return np.reciprocal(A)
 
     def pipeline_bayesfactor(self):
         return self.normalize_f_over_b() * np.exp(self.likelihood)
 
     def compute_pastro(self):
         R_tot = sum(self.rate_dict.values())
```

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.1.1.dev20230421/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe-rift-pipe
-Version: 0.1.0
+Name: rapidpe_rift_pipe
+Version: 0.1.1.dev20230421
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

