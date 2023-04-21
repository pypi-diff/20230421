# Comparing `tmp/magma_suite-1.2.2.1b2.tar.gz` & `tmp/magma_suite-1.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-1.2.2.1b2.tar", max compression
+gzip compressed data, was "magma_suite-1.2.2b1.tar", max compression
```

## Comparing `magma_suite-1.2.2.1b2.tar` & `magma_suite-1.2.2b1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1083 2023-04-17 13:06:49.055030 magma_suite-1.2.2.1b2/LICENSE.txt
--rw-r--r--   0        0        0       96 2023-04-17 13:06:49.055168 magma_suite-1.2.2.1b2/README.md
--rw-r--r--   0        0        0        1 2023-04-17 13:06:49.056496 magma_suite-1.2.2.1b2/magma/__init__.py
--rw-r--r--   0        0        0     3444 2023-04-17 13:06:49.056599 magma_suite-1.2.2.1b2/magma/checkstatus.py
--rw-r--r--   0        0        0    12922 2023-04-17 13:06:49.056747 magma_suite-1.2.2.1b2/magma/inputgenerator.py
--rw-r--r--   0        0        0    15898 2023-04-17 13:06:49.056890 magma_suite-1.2.2.1b2/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2023-04-17 13:06:49.057016 magma_suite-1.2.2.1b2/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2023-04-17 13:06:49.057111 magma_suite-1.2.2.1b2/magma/runupdate.py
--rw-r--r--   0        0        0        0 2023-04-17 13:06:49.057170 magma_suite-1.2.2.1b2/magma_ff/__init__.py
--rw-r--r--   0        0        0     2391 2023-04-17 13:06:49.057253 magma_suite-1.2.2.1b2/magma_ff/checkstatus.py
--rw-r--r--   0        0        0    45467 2023-04-17 13:06:49.057516 magma_suite-1.2.2.1b2/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2023-04-17 13:06:49.057654 magma_suite-1.2.2.1b2/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2023-04-17 13:06:49.057752 magma_suite-1.2.2.1b2/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2023-04-17 13:06:49.057830 magma_suite-1.2.2.1b2/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2023-04-17 13:06:49.057893 magma_suite-1.2.2.1b2/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2023-04-17 13:06:49.058001 magma_suite-1.2.2.1b2/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2023-04-17 13:06:49.058109 magma_suite-1.2.2.1b2/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2023-04-17 13:06:49.058190 magma_suite-1.2.2.1b2/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2023-04-17 13:06:49.058247 magma_suite-1.2.2.1b2/magma_ff/runupdate.py
--rw-r--r--   0        0        0     5650 2023-04-17 13:06:49.058329 magma_suite-1.2.2.1b2/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2023-04-17 13:06:49.058411 magma_suite-1.2.2.1b2/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3021 2023-04-17 13:06:49.058499 magma_suite-1.2.2.1b2/magma_ff/utils.py
--rw-r--r--   0        0        0     4066 2023-04-17 13:06:49.058584 magma_suite-1.2.2.1b2/magma_ff/wfrutils.py
--rw-r--r--   0        0        0      858 2023-04-21 20:48:28.565315 magma_suite-1.2.2.1b2/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 magma_suite-1.2.2.1b2/setup.py
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 magma_suite-1.2.2.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2021-12-04 12:27:49.522554 magma_suite-1.2.2b1/LICENSE.txt
+-rw-r--r--   0        0        0       96 2021-12-04 12:27:49.522647 magma_suite-1.2.2b1/README.md
+-rw-r--r--   0        0        0        1 2021-12-04 12:27:49.524453 magma_suite-1.2.2b1/magma/__init__.py
+-rw-r--r--   0        0        0     3444 2022-06-30 15:42:36.924381 magma_suite-1.2.2b1/magma/checkstatus.py
+-rw-r--r--   0        0        0    12922 2022-06-30 15:42:36.925024 magma_suite-1.2.2b1/magma/inputgenerator.py
+-rw-r--r--   0        0        0    15898 2023-02-23 21:12:29.226971 magma_suite-1.2.2b1/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2022-06-30 15:42:36.926246 magma_suite-1.2.2b1/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2022-06-30 15:42:36.926668 magma_suite-1.2.2b1/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2021-12-04 12:27:49.525213 magma_suite-1.2.2b1/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2391 2022-07-28 17:12:25.211617 magma_suite-1.2.2b1/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0    45467 2023-04-20 19:52:37.302115 magma_suite-1.2.2b1/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2022-06-30 15:42:36.928302 magma_suite-1.2.2b1/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2022-06-30 15:42:36.928742 magma_suite-1.2.2b1/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2021-12-04 12:27:49.525871 magma_suite-1.2.2b1/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2023-03-08 16:08:26.869788 magma_suite-1.2.2b1/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2022-06-30 15:42:36.929823 magma_suite-1.2.2b1/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2022-06-30 15:42:36.930301 magma_suite-1.2.2b1/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2022-06-30 15:42:36.930893 magma_suite-1.2.2b1/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2021-12-04 12:27:49.526349 magma_suite-1.2.2b1/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     5650 2023-03-08 16:08:26.870983 magma_suite-1.2.2b1/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2022-06-30 15:42:36.931870 magma_suite-1.2.2b1/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3021 2023-04-20 19:52:37.303019 magma_suite-1.2.2b1/magma_ff/utils.py
+-rw-r--r--   0        0        0     4066 2023-03-07 22:19:37.427723 magma_suite-1.2.2b1/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0      857 2023-04-20 20:14:08.561130 magma_suite-1.2.2b1/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 magma_suite-1.2.2b1/PKG-INFO
```

### Comparing `magma_suite-1.2.2.1b2/LICENSE.txt` & `magma_suite-1.2.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma/checkstatus.py` & `magma_suite-1.2.2b1/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma/inputgenerator.py` & `magma_suite-1.2.2b1/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma/metawfl.py` & `magma_suite-1.2.2b1/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma/metawflrun.py` & `magma_suite-1.2.2b1/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma/runupdate.py` & `magma_suite-1.2.2b1/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/checkstatus.py` & `magma_suite-1.2.2b1/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/create_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/create_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/import_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/inputgenerator.py` & `magma_suite-1.2.2b1/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/metawfl.py` & `magma_suite-1.2.2b1/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/metawflrun.py` & `magma_suite-1.2.2b1/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/parser.py` & `magma_suite-1.2.2b1/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/reset_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/run_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/status_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/update_cost_metawfr.py` & `magma_suite-1.2.2b1/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/utils.py` & `magma_suite-1.2.2b1/magma_ff/utils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/magma_ff/wfrutils.py` & `magma_suite-1.2.2b1/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2.1b2/pyproject.toml` & `magma_suite-1.2.2b1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "1.2.2.1b2"
+version = "1.2.2-b1"
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
@@ -17,16 +17,16 @@
     { include="magma" },
     { include="magma_ff" }
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
-dcicutils = "^7.2.0"
-tibanna-ff = "^1.0.0"
+dcicutils = "^7.0.0"
+tibanna-ff = "^1.3.3"
 
 
 [tool.poetry.dev-dependencies]
 mock = "*"
 pytest = "*"
```

### Comparing `magma_suite-1.2.2.1b2/PKG-INFO` & `magma_suite-1.2.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: magma-suite
-Version: 1.2.2.1b2
+Version: 1.2.2b1
 Summary: Collection of tools to manage meta-workflows automation.
 Home-page: https://github.com/dbmi-bgm/magma
 License: MIT
 Author: Michele Berselli
 Author-email: berselli.michele@gmail.com
 Requires-Python: >=3.7,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: dcicutils (>=7.2.0,<8.0.0)
-Requires-Dist: tibanna-ff (>=1.0.0,<2.0.0)
+Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
+Requires-Dist: tibanna-ff (>=1.3.3,<2.0.0)
 Project-URL: Repository, https://github.com/dbmi-bgm/magma
 Description-Content-Type: text/markdown
 
 # magma
 
 [*Documentation*](https://magma-suite.readthedocs.io/en/latest/ "magma documentation")
```

