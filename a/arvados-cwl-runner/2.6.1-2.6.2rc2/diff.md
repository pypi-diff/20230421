# Comparing `tmp/arvados-cwl-runner-2.6.1.tar.gz` & `tmp/arvados-cwl-runner-2.6.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.1.tar", last modified: Mon Apr 17 21:06:18 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.2rc2.tar", last modified: Fri Apr 21 19:29:36 2023, max compression
```

## Comparing `arvados-cwl-runner-2.6.1.tar` & `arvados-cwl-runner-2.6.2rc2.tar`

### file list

```diff
@@ -1,54 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19885 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31804 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44286 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8005 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17931 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1353 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1174 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      174 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17280 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2058 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20122 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31804 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44521 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1353 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2058 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.1/LICENSE-2.0.txt` & `arvados-cwl-runner-2.6.2rc2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/PKG-INFO` & `arvados-cwl-runner-2.6.2rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.1
+Version: 2.6.2rc2
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,14 +349,20 @@
         return 1
     except Exception:
         logger.exception("Error creating the Arvados CWL Executor")
         return 1
 
     # Note that unless in debug mode, some stack traces related to user
     # workflow errors may be suppressed.
+
+    # Set the logging on most modules INFO (instead of default which is WARNING)
+    logger.setLevel(logging.INFO)
+    logging.getLogger('arvados').setLevel(logging.INFO)
+    logging.getLogger('arvados.keep').setLevel(logging.WARNING)
+
     if arvargs.debug:
         logger.setLevel(logging.DEBUG)
         logging.getLogger('arvados').setLevel(logging.DEBUG)
 
     if arvargs.quiet:
         logger.setLevel(logging.WARN)
         logging.getLogger('arvados').setLevel(logging.WARN)
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvcontainer.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/context.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/done.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/executor.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,30 +262,30 @@
     def runtime_status_update(self, kind, message, detail=None):
         """
         Updates the runtime_status field on the runner container.
         Called when there's a need to report errors, warnings or just
         activity statuses, for example in the RuntimeStatusLoggingHandler.
         """
 
-        if kind not in ('error', 'warning'):
+        if kind not in ('error', 'warning', 'activity'):
             # Ignore any other status kind
             return
 
         with self.workflow_eval_lock:
             current = None
             try:
                 current = arvados_cwl.util.get_current_container(self.api, self.num_retries, logger)
             except Exception as e:
                 logger.info("Couldn't get current container: %s", e)
             if current is None:
                 return
             runtime_status = current.get('runtime_status', {})
 
             original_updatemessage = updatemessage = runtime_status.get(kind, "")
-            if not updatemessage:
+            if kind == "activity" or not updatemessage:
                 updatemessage = message
 
             # Subsequent messages tacked on in detail
             original_updatedetail = updatedetail = runtime_status.get(kind+'Detail', "")
             maxlines = 40
             if updatedetail.count("\n") < maxlines:
                 if updatedetail:
@@ -589,14 +589,16 @@
         for cr in resp["items"]:
             cr["properties"].update({k.replace("http://arvados.org/cwl#", "arv:"): v for k, v in properties.items()})
             self.api.container_requests().update(uuid=cr["uuid"], body={"container_request": {"properties": cr["properties"]}}).execute(num_retries=self.num_retries)
 
     def arv_executor(self, updated_tool, job_order, runtimeContext, logger=None):
         self.debug = runtimeContext.debug
 
+        self.runtime_status_update("activity", "initialization")
+
         git_info = self.get_git_info(updated_tool) if self.git_info else {}
         if git_info:
             logger.info("Git provenance")
             for g in git_info:
                 if git_info[g]:
                     logger.info("  %s: %s", g.split("#", 1)[1], git_info[g])
 
@@ -651,14 +653,16 @@
             # gets uploaded goes into the same parent project, unless
             # an alternate --project-uuid was provided.
             existing_wf = self.api.workflows().get(uuid=runtimeContext.update_workflow).execute()
             runtimeContext.project_uuid = existing_wf["owner_uuid"]
 
         self.project_uuid = runtimeContext.project_uuid
 
+        self.runtime_status_update("activity", "data transfer")
+
         # Upload local file references in the job order.
         with Perf(metrics, "upload_job_order"):
             job_order, jobmapper = upload_job_order(self, "%s input" % runtimeContext.name,
                                          updated_tool, job_order, runtimeContext)
 
         # determine if we are submitting or directly executing the workflow.
         #
@@ -819,14 +823,16 @@
             runnerjob.run(runtimeContext)
             self.stdout.write(runnerjob.uuid+"\n")
             return (None, "success")
 
         # We either running the workflow directly, or submitting it
         # and will wait for a final result.
 
+        self.runtime_status_update("activity", "workflow execution")
+
         current_container = arvados_cwl.util.get_current_container(self.api, self.num_retries, logger)
         if current_container:
             logger.info("Running inside container %s", current_container.get("uuid"))
             self.set_container_request_properties(current_container, git_info)
 
         self.poll_api = arvados.api('v1', timeout=runtimeContext.http_timeout)
         self.polling_thread = threading.Thread(target=self.poll_states)
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/pathmapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from arvados.errors import ApiError
 from cwltool.pathmapper import PathMapper, MapperEnt
 from cwltool.utils import adjustFileObjs, adjustDirObjs
 from cwltool.stdfsaccess import abspath
 from cwltool.workflow import WorkflowException
 
-from .http import http_to_keep
+from arvados.http_to_keep import http_to_keep
 
 logger = logging.getLogger('arvados.cwl-runner')
 
 def trim_listing(obj):
     """Remove 'listing' field from Directory objects that are keep references.
 
     When Directory objects represent Keep references, it is redundant and
@@ -105,17 +105,17 @@
                     raise WorkflowException("Directory literal '%s' is missing `listing`" % src)
             elif src.startswith("http:") or src.startswith("https:"):
                 try:
                     if self.arvrunner.defer_downloads:
                         # passthrough, we'll download it later.
                         self._pathmap[src] = MapperEnt(src, src, srcobj["class"], True)
                     else:
-                        keepref = http_to_keep(self.arvrunner.api, self.arvrunner.project_uuid, src,
-                                               varying_url_params=self.arvrunner.toplevel_runtimeContext.varying_url_params,
-                                               prefer_cached_downloads=self.arvrunner.toplevel_runtimeContext.prefer_cached_downloads)
+                        keepref = "keep:%s/%s" % http_to_keep(self.arvrunner.api, self.arvrunner.project_uuid, src,
+                                                              varying_url_params=self.arvrunner.toplevel_runtimeContext.varying_url_params,
+                                                              prefer_cached_downloads=self.arvrunner.toplevel_runtimeContext.prefer_cached_downloads)
                         logger.info("%s is %s", src, keepref)
                         self._pathmap[src] = MapperEnt(keepref, keepref, srcobj["class"], True)
                 except Exception as e:
                     logger.warning(str(e))
             else:
                 self._pathmap[src] = MapperEnt(src, src, srcobj["class"], True)
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/perf.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/runner.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl/util.py` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.1
+Version: 2.6.2rc2
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 arvados_cwl/arvdocker.py
 arvados_cwl/arvtool.py
 arvados_cwl/arvworkflow.py
 arvados_cwl/context.py
 arvados_cwl/done.py
 arvados_cwl/executor.py
 arvados_cwl/fsaccess.py
-arvados_cwl/http.py
 arvados_cwl/pathmapper.py
 arvados_cwl/perf.py
 arvados_cwl/runner.py
 arvados_cwl/util.py
 arvados_cwl_runner.egg-info/PKG-INFO
 arvados_cwl_runner.egg-info/SOURCES.txt
 arvados_cwl_runner.egg-info/dependency_links.txt
@@ -33,15 +32,14 @@
 tests/__init__.py
 tests/hw.py
 tests/matcher.py
 tests/mock_discovery.py
 tests/test_container.py
 tests/test_copy_deps.py
 tests/test_fsaccess.py
-tests/test_http.py
 tests/test_make_output.py
 tests/test_pathmapper.py
 tests/test_set_output_prop.py
 tests/test_submit.py
 tests/test_tq.py
 tests/test_urljoin.py
 tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.1/arvados_version.py` & `arvados-cwl-runner-2.6.2rc2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/setup.py` & `arvados-cwl-runner-2.6.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/matcher.py` & `arvados-cwl-runner-2.6.2rc2/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_container.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_copy_deps.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_fsaccess.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_make_output.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_pathmapper.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_submit.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_tq.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_urljoin.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.1/tests/test_util.py` & `arvados-cwl-runner-2.6.2rc2/tests/test_util.py`

 * *Files identical despite different names*

