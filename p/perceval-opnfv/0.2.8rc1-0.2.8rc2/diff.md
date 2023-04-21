# Comparing `tmp/perceval_opnfv-0.2.8rc1.tar.gz` & `tmp/perceval_opnfv-0.2.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_opnfv-0.2.8rc1.tar", max compression
+gzip compressed data, was "perceval_opnfv-0.2.8rc2.tar", max compression
```

## Comparing `perceval_opnfv-0.2.8rc1.tar` & `perceval_opnfv-0.2.8rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      292 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/LICENSE
--rw-r--r--   0        0        0      792 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/NEWS
--rw-r--r--   0        0        0     2250 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/perceval/backends/opnfv/__init__.py
--rw-r--r--   0        0        0       91 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/perceval/backends/opnfv/_version.py
--rw-r--r--   0        0        0     7996 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/perceval/backends/opnfv/functest.py
--rw-r--r--   0        0        0     1392 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/base.py
--rw-r--r--   0        0        0    46769 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results.json
--rw-r--r--   0        0        0      101 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results_empty.json
--rw-r--r--   0        0        0    41641 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results_page_1.json
--rw-r--r--   0        0        0     5312 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results_page_2.json
--rwxr-xr-x   0        0        0     1017 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/run_tests.py
--rw-r--r--   0        0        0    13686 2023-04-20 15:36:20.276760 perceval_opnfv-0.2.8rc1/tests/test_functest.py
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 perceval_opnfv-0.2.8rc1/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/LICENSE
+-rw-r--r--   0        0        0      792 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/NEWS
+-rw-r--r--   0        0        0     2250 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/perceval/backends/opnfv/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/perceval/backends/opnfv/_version.py
+-rw-r--r--   0        0        0     7996 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/perceval/backends/opnfv/functest.py
+-rw-r--r--   0        0        0     1392 2023-04-21 09:54:38.681162 perceval_opnfv-0.2.8rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/base.py
+-rw-r--r--   0        0        0    46769 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results.json
+-rw-r--r--   0        0        0      101 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results_empty.json
+-rw-r--r--   0        0        0    41641 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results_page_1.json
+-rw-r--r--   0        0        0     5312 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results_page_2.json
+-rwxr-xr-x   0        0        0     1017 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/run_tests.py
+-rw-r--r--   0        0        0    13686 2023-04-21 09:54:38.685162 perceval_opnfv-0.2.8rc2/tests/test_functest.py
+-rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 perceval_opnfv-0.2.8rc2/PKG-INFO
```

### Comparing `perceval_opnfv-0.2.8rc1/LICENSE` & `perceval_opnfv-0.2.8rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/NEWS` & `perceval_opnfv-0.2.8rc2/NEWS`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/README.md` & `perceval_opnfv-0.2.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/perceval/backends/opnfv/functest.py` & `perceval_opnfv-0.2.8rc2/perceval/backends/opnfv/functest.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/pyproject.toml` & `perceval_opnfv-0.2.8rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-opnfv"
-version = "0.2.8-rc.1"
+version = "0.2.8-rc.2"
 description = "Bundle of Perceval backends for OPNFV ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_opnfv-0.2.8rc1/tests/base.py` & `perceval_opnfv-0.2.8rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results.json` & `perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results_page_1.json` & `perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/tests/data/functest/functest_results_page_2.json` & `perceval_opnfv-0.2.8rc2/tests/data/functest/functest_results_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/tests/run_tests.py` & `perceval_opnfv-0.2.8rc2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/tests/test_functest.py` & `perceval_opnfv-0.2.8rc2/tests/test_functest.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.8rc1/PKG-INFO` & `perceval_opnfv-0.2.8rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-opnfv
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: Bundle of Perceval backends for OPNFV ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

