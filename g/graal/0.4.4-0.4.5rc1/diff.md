# Comparing `tmp/graal-0.4.4.tar.gz` & `tmp/graal-0.4.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graal-0.4.4.tar", max compression
+gzip compressed data, was "graal-0.4.5rc1.tar", max compression
```

## Comparing `graal-0.4.4.tar` & `graal-0.4.5rc1.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0      240 2023-02-03 08:18:32.364586 graal-0.4.4/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-03 08:18:32.364586 graal-0.4.4/LICENSE
--rw-r--r--   0        0        0     1425 2023-02-03 08:18:32.364586 graal-0.4.4/NEWS
--rw-r--r--   0        0        0    13761 2023-02-03 08:18:32.364586 graal-0.4.4/README.md
--rw-r--r--   0        0        0      876 2023-02-03 08:18:32.364586 graal-0.4.4/graal/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 08:18:32.364586 graal-0.4.4/graal/_version.py
--rw-r--r--   0        0        0      876 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/__init__.py
--rw-r--r--   0        0        0      883 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/__init__.py
--rw-r--r--   0        0        0     1192 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/analyzer.py
--rw-r--r--   0        0        0     4594 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/bandit.py
--rw-r--r--   0        0        0     4543 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/cloc.py
--rw-r--r--   0        0        0     2479 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/flake8.py
--rw-r--r--   0        0        0     2317 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/jadolint.py
--rw-r--r--   0        0        0     2243 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/linguist.py
--rw-r--r--   0        0        0     5383 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/lizard.py
--rw-r--r--   0        0        0     2360 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/nomos.py
--rw-r--r--   0        0        0     2852 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/pylint.py
--rw-r--r--   0        0        0     2620 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/reverse.py
--rw-r--r--   0        0        0     4563 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/scancode.py
--rw-r--r--   0        0        0     4504 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/analyzers/scc.py
--rw-r--r--   0        0        0    11691 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/cocom.py
--rw-r--r--   0        0        0     8463 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/codep.py
--rw-r--r--   0        0        0     6344 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/colang.py
--rw-r--r--   0        0        0     8182 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/colic.py
--rw-r--r--   0        0        0     9186 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/coqua.py
--rw-r--r--   0        0        0     5662 2023-02-03 08:18:32.364586 graal-0.4.4/graal/backends/core/covuln.py
--rwxr-xr-x   0        0        0     4425 2023-02-03 08:18:32.364586 graal-0.4.4/graal/bin/graal.py
--rw-r--r--   0        0        0    23643 2023-02-03 08:18:32.364586 graal-0.4.4/graal/graal.py
--rw-r--r--   0        0        0     1499 2023-02-03 08:18:32.368586 graal-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 08:18:32.368586 graal-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     2072 2023-02-03 08:18:32.368586 graal-0.4.4/tests/base_analyzer.py
--rw-r--r--   0        0        0     2056 2023-02-03 08:18:32.368586 graal-0.4.4/tests/base_repo.py
--rw-r--r--   0        0        0     1575 2023-02-03 08:18:32.368586 graal-0.4.4/tests/data/Dockerfile
--rw-r--r--   0        0        0   132358 2023-02-03 08:18:32.368586 graal-0.4.4/tests/data/graaltest-dockerfile.zip
--rw-r--r--   0        0        0   126651 2023-02-03 08:18:32.368586 graal-0.4.4/tests/data/graaltest.zip
--rw-r--r--   0        0        0     4482 2023-02-03 08:18:32.368586 graal-0.4.4/tests/data/sample_code.py
--rwxr-xr-x   0        0        0     1174 2023-02-03 08:18:32.368586 graal-0.4.4/tests/run_tests.py
--rw-r--r--   0        0        0     1222 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_analyzer.py
--rw-r--r--   0        0        0     5650 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_bandit.py
--rw-r--r--   0        0        0     3341 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_cloc.py
--rw-r--r--   0        0        0    14713 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_cocom.py
--rw-r--r--   0        0        0    14625 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_codep.py
--rw-r--r--   0        0        0     8707 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_colang.py
--rw-r--r--   0        0        0    13445 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_colic.py
--rw-r--r--   0        0        0    20057 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_coqua.py
--rw-r--r--   0        0        0     7611 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_covuln.py
--rw-r--r--   0        0        0     2846 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_flake8.py
--rw-r--r--   0        0        0    29236 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_graal.py
--rw-r--r--   0        0        0     6391 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_jadolint.py
--rw-r--r--   0        0        0     2456 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_linguist.py
--rw-r--r--   0        0        0     4980 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_lizard.py
--rw-r--r--   0        0        0     2321 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_nomos.py
--rw-r--r--   0        0        0     3181 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_pylint.py
--rw-r--r--   0        0        0     2481 2023-02-03 08:18:32.368586 graal-0.4.4/tests/test_reverse.py
--rw-r--r--   0        0        0     3538 2023-02-03 08:18:32.372585 graal-0.4.4/tests/test_scancode.py
--rw-r--r--   0        0        0     4022 2023-02-03 08:18:32.372585 graal-0.4.4/tests/test_scc.py
--rw-r--r--   0        0        0     1191 2023-02-03 08:18:32.372585 graal-0.4.4/tests/utils.py
--rw-r--r--   0        0        0    15041 1970-01-01 00:00:00.000000 graal-0.4.4/setup.py
--rw-r--r--   0        0        0    15164 1970-01-01 00:00:00.000000 graal-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-04-21 07:26:08.869516 graal-0.4.5rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-21 07:26:08.869516 graal-0.4.5rc1/LICENSE
+-rw-r--r--   0        0        0     1425 2023-04-21 07:26:08.869516 graal-0.4.5rc1/NEWS
+-rw-r--r--   0        0        0    13761 2023-04-21 07:26:08.869516 graal-0.4.5rc1/README.md
+-rw-r--r--   0        0        0      876 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/_version.py
+-rw-r--r--   0        0        0      876 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/analyzer.py
+-rw-r--r--   0        0        0     4594 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/bandit.py
+-rw-r--r--   0        0        0     4543 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/cloc.py
+-rw-r--r--   0        0        0     2479 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/flake8.py
+-rw-r--r--   0        0        0     2317 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/jadolint.py
+-rw-r--r--   0        0        0     2243 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/linguist.py
+-rw-r--r--   0        0        0     5383 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/lizard.py
+-rw-r--r--   0        0        0     2360 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/nomos.py
+-rw-r--r--   0        0        0     2852 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/pylint.py
+-rw-r--r--   0        0        0     2620 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/reverse.py
+-rw-r--r--   0        0        0     4563 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/scancode.py
+-rw-r--r--   0        0        0     4504 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/analyzers/scc.py
+-rw-r--r--   0        0        0    11691 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/cocom.py
+-rw-r--r--   0        0        0     8463 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/codep.py
+-rw-r--r--   0        0        0     6344 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/colang.py
+-rw-r--r--   0        0        0     8182 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/colic.py
+-rw-r--r--   0        0        0     9186 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/coqua.py
+-rw-r--r--   0        0        0     5662 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/backends/core/covuln.py
+-rwxr-xr-x   0        0        0     4425 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/bin/graal.py
+-rw-r--r--   0        0        0    23643 2023-04-21 07:26:08.869516 graal-0.4.5rc1/graal/graal.py
+-rw-r--r--   0        0        0     1584 2023-04-21 07:26:08.873517 graal-0.4.5rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/base_analyzer.py
+-rw-r--r--   0        0        0     2056 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/base_repo.py
+-rw-r--r--   0        0        0     1575 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/data/Dockerfile
+-rw-r--r--   0        0        0   132358 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/data/graaltest-dockerfile.zip
+-rw-r--r--   0        0        0   126651 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/data/graaltest.zip
+-rw-r--r--   0        0        0     4482 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/data/sample_code.py
+-rwxr-xr-x   0        0        0     1174 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     1222 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_analyzer.py
+-rw-r--r--   0        0        0     5650 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_bandit.py
+-rw-r--r--   0        0        0     3341 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_cloc.py
+-rw-r--r--   0        0        0    14713 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_cocom.py
+-rw-r--r--   0        0        0    14625 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_codep.py
+-rw-r--r--   0        0        0     8707 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_colang.py
+-rw-r--r--   0        0        0    13445 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_colic.py
+-rw-r--r--   0        0        0    20057 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_coqua.py
+-rw-r--r--   0        0        0     7611 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_covuln.py
+-rw-r--r--   0        0        0     2846 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_flake8.py
+-rw-r--r--   0        0        0    29236 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_graal.py
+-rw-r--r--   0        0        0     6391 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_jadolint.py
+-rw-r--r--   0        0        0     2456 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_linguist.py
+-rw-r--r--   0        0        0     4980 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_lizard.py
+-rw-r--r--   0        0        0     2321 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_nomos.py
+-rw-r--r--   0        0        0     3181 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_pylint.py
+-rw-r--r--   0        0        0     2481 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_reverse.py
+-rw-r--r--   0        0        0     3538 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_scancode.py
+-rw-r--r--   0        0        0     4022 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/test_scc.py
+-rw-r--r--   0        0        0     1191 2023-04-21 07:26:08.873517 graal-0.4.5rc1/tests/utils.py
+-rw-r--r--   0        0        0    15214 1970-01-01 00:00:00.000000 graal-0.4.5rc1/PKG-INFO
```

### Comparing `graal-0.4.4/LICENSE` & `graal-0.4.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/NEWS` & `graal-0.4.5rc1/NEWS`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/README.md` & `graal-0.4.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/__init__.py` & `graal-0.4.5rc1/graal/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/__init__.py` & `graal-0.4.5rc1/graal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/__init__.py` & `graal-0.4.5rc1/graal/backends/core/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/analyzer.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/bandit.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/cloc.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/flake8.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/jadolint.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/linguist.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/lizard.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/nomos.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/pylint.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/reverse.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/scancode.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/analyzers/scc.py` & `graal-0.4.5rc1/graal/backends/core/analyzers/scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/cocom.py` & `graal-0.4.5rc1/graal/backends/core/cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/codep.py` & `graal-0.4.5rc1/graal/backends/core/codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/colang.py` & `graal-0.4.5rc1/graal/backends/core/colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/colic.py` & `graal-0.4.5rc1/graal/backends/core/colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/coqua.py` & `graal-0.4.5rc1/graal/backends/core/coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/backends/core/covuln.py` & `graal-0.4.5rc1/graal/backends/core/covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/bin/graal.py` & `graal-0.4.5rc1/graal/bin/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/graal/graal.py` & `graal-0.4.5rc1/graal/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/pyproject.toml` & `graal-0.4.5rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graal"
-version = "0.4.4"
+version = "0.4.5-rc.1"
 description = "A generic source code analyzer"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -52,14 +52,17 @@
 pydot = ">=1.2.4"
 bandit = ">=1.4.0"
 perceval = { version = ">=0.19", allow-prereleases = true }
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 cloc = "^0.2.5"
 execnet = "^1.9.0"
 
+# Pinned because 'myst-parser = ^0.15.2' in Perceval
+markdown-it-py = "^1.0.0"
+
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 coverage = "^6.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `graal-0.4.4/tests/base_analyzer.py` & `graal-0.4.5rc1/tests/base_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/base_repo.py` & `graal-0.4.5rc1/tests/base_repo.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/data/Dockerfile` & `graal-0.4.5rc1/tests/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/data/graaltest-dockerfile.zip` & `graal-0.4.5rc1/tests/data/graaltest-dockerfile.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/data/graaltest.zip` & `graal-0.4.5rc1/tests/data/graaltest.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/data/sample_code.py` & `graal-0.4.5rc1/tests/data/sample_code.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/run_tests.py` & `graal-0.4.5rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_analyzer.py` & `graal-0.4.5rc1/tests/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_bandit.py` & `graal-0.4.5rc1/tests/test_bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_cloc.py` & `graal-0.4.5rc1/tests/test_cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_cocom.py` & `graal-0.4.5rc1/tests/test_cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_codep.py` & `graal-0.4.5rc1/tests/test_codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_colang.py` & `graal-0.4.5rc1/tests/test_colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_colic.py` & `graal-0.4.5rc1/tests/test_colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_coqua.py` & `graal-0.4.5rc1/tests/test_coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_covuln.py` & `graal-0.4.5rc1/tests/test_covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_flake8.py` & `graal-0.4.5rc1/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_graal.py` & `graal-0.4.5rc1/tests/test_graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_jadolint.py` & `graal-0.4.5rc1/tests/test_jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_linguist.py` & `graal-0.4.5rc1/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_lizard.py` & `graal-0.4.5rc1/tests/test_lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_nomos.py` & `graal-0.4.5rc1/tests/test_nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_pylint.py` & `graal-0.4.5rc1/tests/test_pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_reverse.py` & `graal-0.4.5rc1/tests/test_reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_scancode.py` & `graal-0.4.5rc1/tests/test_scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/test_scc.py` & `graal-0.4.5rc1/tests/test_scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/tests/utils.py` & `graal-0.4.5rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.4/setup.py` & `graal-0.4.5rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,266 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: graal
+Version: 0.4.5rc1
+Summary: A generic source code analyzer
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: bandit (>=1.4.0)
+Requires-Dist: cloc (>=0.2.5,<0.3.0)
+Requires-Dist: execnet (>=1.9.0,<2.0.0)
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: grimoirelab-toolkit (>=0.3)
+Requires-Dist: lizard (==1.16.6)
+Requires-Dist: markdown-it-py (>=1.0.0,<2.0.0)
+Requires-Dist: networkx (>=2.1)
+Requires-Dist: perceval (>=0.19)
+Requires-Dist: pydot (>=1.2.4)
+Requires-Dist: pylint (>=1.8.4)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-graal/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-graal
+Description-Content-Type: text/markdown
 
-packages = \
-['graal',
- 'graal.backends',
- 'graal.backends.core',
- 'graal.backends.core.analyzers',
- 'graal.bin',
- 'tests',
- 'tests.data']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bandit>=1.4.0',
- 'cloc>=0.2.5,<0.3.0',
- 'execnet>=1.9.0,<2.0.0',
- 'flake8>=4.0.1,<5.0.0',
- 'grimoirelab-toolkit>=0.3',
- 'lizard==1.16.6',
- 'networkx>=2.1',
- 'perceval>=0.19',
- 'pydot>=1.2.4',
- 'pylint>=1.8.4']
-
-entry_points = \
-{'console_scripts': ['graal = graal.bin.graal:main']}
-
-setup_kwargs = {
-    'name': 'graal',
-    'version': '0.4.4',
-    'description': 'A generic source code analyzer',
-    'long_description': "# Graal: a Generic Repository AnALyzer [![Build Status](https://github.com/chaoss/grimoirelab-graal/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-graal/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-graal/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-graal?branch=master)  [![PyPI version](https://badge.fury.io/py/graal.svg)](https://badge.fury.io/py/graal)\n\nGraal leverages on the Git backend of [Perceval](https://github.com/chaoss/grimoirelab-perceval) and enhances it to set up ad-hoc\nsource code analysis. Thus, it fetches the commits from a Git repository and provides a mechanism to plug third party tools/libraries focused on source code analysis.\n\n## How it works\nThe Perceval Git backend creates a local mirror of a Git repository (local or remote), fetches the metadata of commits in chronological order and returns them as a list of JSON documents\n(one per commit). Graal leverages on the incremental functionalities provided by the Git backend and enhances the logic to handle Git repositories by creating a\nworking tree to perform checkout operations (which are not possible on a Git mirror). Graal intercepts each JSON document and enables the user to perform the following steps:\n- **Filter.** The filtering is used to select or discard commits based on the information available in the JSON document and/or via the Graal parameters. For any selected commit,\nGraal executes a checkout on the working tree using the commit hash, thus setting the state of the working tree at that given revision.\n- **Analyze.** The analysis takes the JSON document and the current working tree and enables the user to set up ad-hoc source code analysis by plugging existing tools through system calls\nor their Python interfaces, when possible. The results of the analysis are parsed and manipulated by the user and then automatically embedded in the JSON document. It is worth\nnoting that in this step the user can rely on some predefined functionalities of Graal to deal with the repository snapshot (e.g., listing files, creating archives).\n- **Post-process.** In the final step, the inflated JSON document can be optionally processed to alter (e.g., renaming, removing) its attributes, thus granting the user complete control over the output of Graal executions.\n\nSeveral parameters (inherited from the [Git backend](http://perceval.readthedocs.io/en/latest/perceval.backends.core.html#module-perceval.backends.core.git)) are available to control the execution; for instance, **from_date** and **to_date**\nallow to select commits authored since and before a given date, **branches** allows to fetch commits only from specific branches,\nand **latest_items** returns only those commits which are new since the last fetch operation. Graal includes additional parameters to drive\nthe analysis to filter in/out files and directories in the repository (**in_paths** and **out_paths**), set the **entrypoint**\nand define the **details** level of the analysis (useful when analyzing large software projects).\n\n## Requirements\n\n\n * Python >= 3.7\n * Poetry >= 1.2\n * [github-linguist](https://github.com/github/linguist)\n * [FOSSology](https://github.com/fossology/fossology)\n * [cloc](https://github.com/AlDanial/cloc)\n * [scc](https://github.com/boyter/scc)\n * [ScanCode toolkit](https://github.com/nexB/scancode-toolkit)\n * [crossJadoLint](https://github.com/crossminer/crossJadolint/)\n\nYou will also need some other Python libraries for running the tool, you can find the\nwhole list of dependencies in [pyproject.toml](pyproject.toml) file.\n\n### How to install and create the executables:\n- **github-linguist**\n \n  Library is used to detect blob languages, ignore binary or vendored files, suppress generated files in diffs, and generate language breakdown graphs.\n  ```\n  $ gem install github-linguist -v 7.15\n  ```\n- **FOSSology**\n\n  Open source license compliance software system and toolkit. You can run license, copyright, and export control scans from the command line.\n  ```\n  $ wget https://github.com/fossology/fossology/releases/download/3.11.0/FOSSology-3.11.0-ubuntu-focal.tar.gz\n  $ tar -xzf FOSSology-3.11.0-ubuntu-focal.tar.gz\n  $ sudo apt-get -y install ./packages/fossology-common_3.11.0-1_amd64.deb \\\n                            ./packages/fossology-nomos_3.11.0-1_amd64.deb\n  ```\n\n- **Cloc**\n\n  Count blank lines, comment lines, and physical lines of source code in many programming languages.\n  ```\n  $ sudo apt-get install cloc\n  ```\n\n- **SCC**\n\n  A tool similar to cloc - for counting physical the lines of code, blank lines, comment lines, and physical lines of source code in many programming languages and COCOMO estimates written in pure Go.\n  ```\n  $ go install github.com/boyter/scc@latest\n  ```\n\n- **ScanCode Toolkit**\n\n  ScanCode detects licenses, copyrights, package manifests & dependencies and more by scanning code.\n  ```\n  $ mkdir exec\n  $ cd exec\n  $ git clone https://github.com/nexB/scancode-toolkit.git\n  $ cd scancode-toolkit\n  $ git checkout -b test_scancli 96069fd84066c97549d54f66bd2fe8c7813c6b52\n  $ ./scancode --help\n  ```\n\n  *Note: We're now using a clone of scancode-toolkit instead of a release, as the latest release is of 15th February 2019 and the `scancli.py` script (required for execution of scancode_cli) was incorporated later i.e 5th March 2019 and there hasn't been a release since.*\n\n- **crossJadolint**\n\n  This is a Dockerfile linter tool, implemented in Java and essentialy is a port of Hadolint (Haskell Dockerfile Linter)\n  ```\n  $ cd exec\n  $ wget https://github.com/crossminer/crossJadolint/releases/download/Pre-releasev2/jadolint.jar\n  ```\n\n## Installation\n\nThere are several ways to install Graal on your system: packages or source \ncode using Poetry or pip.\n\n### PyPI\n\nGraal can be installed using pip, a tool for installing Python packages. \nTo do it, run the next command:\n```\n$ pip install graal\n```\n\n### Source code\n\nTo install from the source code you will need to clone the repository first:\n```\n$ git clone https://github.com/chaoss/grimoirelab-graal\n$ cd grimoirelab-graal\n```\n\nThen use pip or Poetry to install the package along with its dependencies.\n\n#### Pip\nTo install the package from local directory run the following command:\n```\n$ pip install .\n```\nIn case you are a developer, you should install graal in editable mode:\n```\n$ pip install -e .\n```\n\n#### Poetry\nWe use [poetry](https://python-poetry.org/) for dependency management and \npackaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).\nOnce you have installed it, you can install graal and the dependencies in \na project isolated environment using:\n```\n$ poetry install\n```\nTo spaw a new shell within the virtual environment use:\n```\n$ poetry shell\n```\n\n## Backends\nSeveral backends have been developed to assess the genericity of Graal. Those backends leverage on source code analysis\ntools, where executions are triggered via system calls or their Python interfaces. In the current status, the backends\nmostly target Python code, however other backends can be easily developed to cover other programming languages. The\ncurrently available backends are:\n- **CoCom** gathers data about code complexity (e.g., cyclomatic complexity, LOC) from projects written in popular programming languages such as: C/C++, Java, Scala, JavaScript, Ruby, Python, Lua and Golang. It leverages on [Cloc](http://cloc.sourceforge.net/), [Lizard](https://github.com/terryyin/lizard) and [scc](https://github.com/boyter/scc). The tool can be exectued at `file` and `repository` levels activated with the help of category: `code_complexity_lizard_file` or `code_complexity_lizard_repository`.\n- **CoDep** extracts package and class dependencies of a Python module and serialized them as JSON structures, composed of edges and nodes, thus easing the bridging with front-end technologies for graph visualizations. It combines [PyReverse](https://pypi.org/project/pyreverse/) and [NetworkX](https://networkx.github.io/).\n- **CoQua** retrieves code quality insights, such as checks about line-code’s length, well-formed variable names, unused imported modules and code clones. It uses [PyLint](https://www.pylint.org/) and [Flake8](http://flake8.pycqa.org/en/latest/index.html). The tools can be activated by passing the corresponding category: `code_quality_pylint` or `code_quality_flake8`.\n- **CoVuln** scans the code to identify security vulnerabilities such as potential SQL and Shell injections, hard-coded passwords and weak cryptographic key size. It relies on [Bandit](https://github.com/PyCQA/bandit).\n- **CoLic** scans the code to extract license & copyright information. It currently supports [Nomos](https://github.com/fossology/fossology/tree/master/src/nomos) and [ScanCode](https://github.com/nexB/scancode-toolkit). They can be activated by passing the corresponding category: `code_license_nomos`, `code_license_scancode`, or `code_license_scancode_cli`.\n- **CoLang** gathers insights about code language distribution of a git repository. It relies on [Linguist](https://github.com/github/linguist) and [Cloc](http://cloc.sourceforge.net/) tools. They can be activated by passing the corresponding category: `code_language_linguist` or `code_language_cloc`.\n\n### How to develop a backend\nCreating your own backend is pretty easy, you only need to redefine the following methods of Graal:\n- **_filter_commit.** This method is used to select or discard commits based on the information available in the JSON document\nand/or via the Graal parameters (e.g., the commits authored by a given user or targeting a given software component).\nFor any selected commit, Graal executes a checkout on the working tree using the commit hash, thus setting the state of\nthe working tree at that given revision.\n- **_analyze.** This method takes the document and the current working tree and allows to connect existing tools through system calls or their Python interfaces, when possible.\nThe results of the analysis, parsed and manipulated by the user, are automatically embedded in the JSON document.\n- **_post.** This method allows to alter (e.g., renaming, removing) the attributes of the inflated JSON documents.\n\n## How to use\n\n### From command line\nLaunching Graal from command line does not require much effort, but only some basic knowledge of GNU/Linux shell commands.\n\nThe example below shows how easy it is to fetch code complexity information from a Git repository. The **CoCom** backend\nrequires the URL where the repository is located (_https://github.com/chaoss/grimoirelab-perceval_) and the local path\nwhere to mirror the repository (_/tmp/graal-cocom_). Then, the JSON documents produced are redirected to the file _graal-cocom.test_.\n\n- **CoCom Backend**\n\n```\n$ graal cocom https://github.com/chaoss/grimoirelab-perceval --git-path /tmp/graal-cocom > /graal-cocom.test\nStarting the quest for the Graal.\nGit worktree /tmp/... created!\nFetching commits: ...\nGit worktree /tmp/... deleted!\nFetch process completed: .. commits inspected\nQuest completed.\n```\n\n- **CoLic Backend**\n\n```\ngraal colic https://github.com/chaoss/grimoirelab-toolkit --git-path /tmp/scancode_cli --exec-path /home/scancode-toolkit/etc/scripts/scancli.py --category code_license_scancode_cli\nStarting the quest for the Graal.\nGit worktree /tmp/... created!\nFetching commits: ...\nGit worktree /tmp/... deleted!\nFetch process completed: .. commits inspected\nQuest completed.\n```\n\nIn the above example, we're using scancode_cli analyzer. Similarly, we can use the scancode analyzer by providing the category as `code_license_scancode` and it's corresponding executable path.\n\n### From Python\nGraal’s functionalities can be embedded in Python scripts. Again, the effort of using Graal is minimum. In this case the user\nonly needs some knowledge of Python scripting. The example below shows how to use Graal in a script.\n\nThe **graal.backends.core.cocom** module is imported at the beginning of the file, then the **repo_uri** and **repo_dir** variables\nare set to the URI of the Git repository and the local path where to mirror it. These variables are used to initialize a\n**CoCom class object**. In the last line of the script, the commits inflated with the result of the analysis are retrieved\nusing the fetch method. The fetch method inherits its argument from **Perceval**, thus it optionally accept two Datetime\nobjects to gather only those commits after and before a given date, a list of branches to focus on specific development\nactivities, and a flag to collect the commits available after the last execution.\n\n```\n#! /usr/bin/env python3\nfrom graal.backends.core.cocom import CoCom\n\n# URL for the git repo to analyze\nrepo_uri = ’http://github.com/chaoss/grimoirelab-perceval’\n\n# directory where to mirror the repo\nrepo_dir = ’/tmp/graal-cocom’\n\n# Cocom object initialization\ncc = CoCom(uri=repo_uri, git_path=repo_dir)\n\n# fetch all commits\ncommits = [commit for commit in cc.fetch()]\n```\n\n## How to integrate it with Arthur\n[Arthur](https://github.com/chaoss/grimoirelab-kingarthur) is another tool of the [Grimoirelab ecosystem](https://chaoss.github.io/grimoirelab/). It was originally designed to allow to schedule\nand run Perceval executions at scale through distributed **Redis** queues, and store the obtained results in an **ElasticSearch** database.\n\nArthur has been extended to allow handling Graal tasks, which inherit from Perceval Git tasks. The code to make this extension possible is\navailable at: https://github.com/chaoss/grimoirelab-kingarthur/pull/33.\n\nInformation about Arthur is available at https://github.com/chaoss/grimoirelab-kingarthur.\n",
-    'author': 'GrimoireLab Developers',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://chaoss.github.io/grimoirelab/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+# Graal: a Generic Repository AnALyzer [![Build Status](https://github.com/chaoss/grimoirelab-graal/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-graal/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-graal/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-graal?branch=master)  [![PyPI version](https://badge.fury.io/py/graal.svg)](https://badge.fury.io/py/graal)
 
+Graal leverages on the Git backend of [Perceval](https://github.com/chaoss/grimoirelab-perceval) and enhances it to set up ad-hoc
+source code analysis. Thus, it fetches the commits from a Git repository and provides a mechanism to plug third party tools/libraries focused on source code analysis.
+
+## How it works
+The Perceval Git backend creates a local mirror of a Git repository (local or remote), fetches the metadata of commits in chronological order and returns them as a list of JSON documents
+(one per commit). Graal leverages on the incremental functionalities provided by the Git backend and enhances the logic to handle Git repositories by creating a
+working tree to perform checkout operations (which are not possible on a Git mirror). Graal intercepts each JSON document and enables the user to perform the following steps:
+- **Filter.** The filtering is used to select or discard commits based on the information available in the JSON document and/or via the Graal parameters. For any selected commit,
+Graal executes a checkout on the working tree using the commit hash, thus setting the state of the working tree at that given revision.
+- **Analyze.** The analysis takes the JSON document and the current working tree and enables the user to set up ad-hoc source code analysis by plugging existing tools through system calls
+or their Python interfaces, when possible. The results of the analysis are parsed and manipulated by the user and then automatically embedded in the JSON document. It is worth
+noting that in this step the user can rely on some predefined functionalities of Graal to deal with the repository snapshot (e.g., listing files, creating archives).
+- **Post-process.** In the final step, the inflated JSON document can be optionally processed to alter (e.g., renaming, removing) its attributes, thus granting the user complete control over the output of Graal executions.
+
+Several parameters (inherited from the [Git backend](http://perceval.readthedocs.io/en/latest/perceval.backends.core.html#module-perceval.backends.core.git)) are available to control the execution; for instance, **from_date** and **to_date**
+allow to select commits authored since and before a given date, **branches** allows to fetch commits only from specific branches,
+and **latest_items** returns only those commits which are new since the last fetch operation. Graal includes additional parameters to drive
+the analysis to filter in/out files and directories in the repository (**in_paths** and **out_paths**), set the **entrypoint**
+and define the **details** level of the analysis (useful when analyzing large software projects).
+
+## Requirements
+
+
+ * Python >= 3.7
+ * Poetry >= 1.2
+ * [github-linguist](https://github.com/github/linguist)
+ * [FOSSology](https://github.com/fossology/fossology)
+ * [cloc](https://github.com/AlDanial/cloc)
+ * [scc](https://github.com/boyter/scc)
+ * [ScanCode toolkit](https://github.com/nexB/scancode-toolkit)
+ * [crossJadoLint](https://github.com/crossminer/crossJadolint/)
+
+You will also need some other Python libraries for running the tool, you can find the
+whole list of dependencies in [pyproject.toml](pyproject.toml) file.
+
+### How to install and create the executables:
+- **github-linguist**
+ 
+  Library is used to detect blob languages, ignore binary or vendored files, suppress generated files in diffs, and generate language breakdown graphs.
+  ```
+  $ gem install github-linguist -v 7.15
+  ```
+- **FOSSology**
+
+  Open source license compliance software system and toolkit. You can run license, copyright, and export control scans from the command line.
+  ```
+  $ wget https://github.com/fossology/fossology/releases/download/3.11.0/FOSSology-3.11.0-ubuntu-focal.tar.gz
+  $ tar -xzf FOSSology-3.11.0-ubuntu-focal.tar.gz
+  $ sudo apt-get -y install ./packages/fossology-common_3.11.0-1_amd64.deb \
+                            ./packages/fossology-nomos_3.11.0-1_amd64.deb
+  ```
+
+- **Cloc**
+
+  Count blank lines, comment lines, and physical lines of source code in many programming languages.
+  ```
+  $ sudo apt-get install cloc
+  ```
+
+- **SCC**
+
+  A tool similar to cloc - for counting physical the lines of code, blank lines, comment lines, and physical lines of source code in many programming languages and COCOMO estimates written in pure Go.
+  ```
+  $ go install github.com/boyter/scc@latest
+  ```
+
+- **ScanCode Toolkit**
+
+  ScanCode detects licenses, copyrights, package manifests & dependencies and more by scanning code.
+  ```
+  $ mkdir exec
+  $ cd exec
+  $ git clone https://github.com/nexB/scancode-toolkit.git
+  $ cd scancode-toolkit
+  $ git checkout -b test_scancli 96069fd84066c97549d54f66bd2fe8c7813c6b52
+  $ ./scancode --help
+  ```
+
+  *Note: We're now using a clone of scancode-toolkit instead of a release, as the latest release is of 15th February 2019 and the `scancli.py` script (required for execution of scancode_cli) was incorporated later i.e 5th March 2019 and there hasn't been a release since.*
+
+- **crossJadolint**
+
+  This is a Dockerfile linter tool, implemented in Java and essentialy is a port of Hadolint (Haskell Dockerfile Linter)
+  ```
+  $ cd exec
+  $ wget https://github.com/crossminer/crossJadolint/releases/download/Pre-releasev2/jadolint.jar
+  ```
+
+## Installation
+
+There are several ways to install Graal on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI
+
+Graal can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install graal
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-graal
+$ cd grimoirelab-graal
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install graal in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install graal and the dependencies in 
+a project isolated environment using:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
+## Backends
+Several backends have been developed to assess the genericity of Graal. Those backends leverage on source code analysis
+tools, where executions are triggered via system calls or their Python interfaces. In the current status, the backends
+mostly target Python code, however other backends can be easily developed to cover other programming languages. The
+currently available backends are:
+- **CoCom** gathers data about code complexity (e.g., cyclomatic complexity, LOC) from projects written in popular programming languages such as: C/C++, Java, Scala, JavaScript, Ruby, Python, Lua and Golang. It leverages on [Cloc](http://cloc.sourceforge.net/), [Lizard](https://github.com/terryyin/lizard) and [scc](https://github.com/boyter/scc). The tool can be exectued at `file` and `repository` levels activated with the help of category: `code_complexity_lizard_file` or `code_complexity_lizard_repository`.
+- **CoDep** extracts package and class dependencies of a Python module and serialized them as JSON structures, composed of edges and nodes, thus easing the bridging with front-end technologies for graph visualizations. It combines [PyReverse](https://pypi.org/project/pyreverse/) and [NetworkX](https://networkx.github.io/).
+- **CoQua** retrieves code quality insights, such as checks about line-code’s length, well-formed variable names, unused imported modules and code clones. It uses [PyLint](https://www.pylint.org/) and [Flake8](http://flake8.pycqa.org/en/latest/index.html). The tools can be activated by passing the corresponding category: `code_quality_pylint` or `code_quality_flake8`.
+- **CoVuln** scans the code to identify security vulnerabilities such as potential SQL and Shell injections, hard-coded passwords and weak cryptographic key size. It relies on [Bandit](https://github.com/PyCQA/bandit).
+- **CoLic** scans the code to extract license & copyright information. It currently supports [Nomos](https://github.com/fossology/fossology/tree/master/src/nomos) and [ScanCode](https://github.com/nexB/scancode-toolkit). They can be activated by passing the corresponding category: `code_license_nomos`, `code_license_scancode`, or `code_license_scancode_cli`.
+- **CoLang** gathers insights about code language distribution of a git repository. It relies on [Linguist](https://github.com/github/linguist) and [Cloc](http://cloc.sourceforge.net/) tools. They can be activated by passing the corresponding category: `code_language_linguist` or `code_language_cloc`.
+
+### How to develop a backend
+Creating your own backend is pretty easy, you only need to redefine the following methods of Graal:
+- **_filter_commit.** This method is used to select or discard commits based on the information available in the JSON document
+and/or via the Graal parameters (e.g., the commits authored by a given user or targeting a given software component).
+For any selected commit, Graal executes a checkout on the working tree using the commit hash, thus setting the state of
+the working tree at that given revision.
+- **_analyze.** This method takes the document and the current working tree and allows to connect existing tools through system calls or their Python interfaces, when possible.
+The results of the analysis, parsed and manipulated by the user, are automatically embedded in the JSON document.
+- **_post.** This method allows to alter (e.g., renaming, removing) the attributes of the inflated JSON documents.
+
+## How to use
+
+### From command line
+Launching Graal from command line does not require much effort, but only some basic knowledge of GNU/Linux shell commands.
+
+The example below shows how easy it is to fetch code complexity information from a Git repository. The **CoCom** backend
+requires the URL where the repository is located (_https://github.com/chaoss/grimoirelab-perceval_) and the local path
+where to mirror the repository (_/tmp/graal-cocom_). Then, the JSON documents produced are redirected to the file _graal-cocom.test_.
+
+- **CoCom Backend**
+
+```
+$ graal cocom https://github.com/chaoss/grimoirelab-perceval --git-path /tmp/graal-cocom > /graal-cocom.test
+Starting the quest for the Graal.
+Git worktree /tmp/... created!
+Fetching commits: ...
+Git worktree /tmp/... deleted!
+Fetch process completed: .. commits inspected
+Quest completed.
+```
+
+- **CoLic Backend**
+
+```
+graal colic https://github.com/chaoss/grimoirelab-toolkit --git-path /tmp/scancode_cli --exec-path /home/scancode-toolkit/etc/scripts/scancli.py --category code_license_scancode_cli
+Starting the quest for the Graal.
+Git worktree /tmp/... created!
+Fetching commits: ...
+Git worktree /tmp/... deleted!
+Fetch process completed: .. commits inspected
+Quest completed.
+```
+
+In the above example, we're using scancode_cli analyzer. Similarly, we can use the scancode analyzer by providing the category as `code_license_scancode` and it's corresponding executable path.
+
+### From Python
+Graal’s functionalities can be embedded in Python scripts. Again, the effort of using Graal is minimum. In this case the user
+only needs some knowledge of Python scripting. The example below shows how to use Graal in a script.
+
+The **graal.backends.core.cocom** module is imported at the beginning of the file, then the **repo_uri** and **repo_dir** variables
+are set to the URI of the Git repository and the local path where to mirror it. These variables are used to initialize a
+**CoCom class object**. In the last line of the script, the commits inflated with the result of the analysis are retrieved
+using the fetch method. The fetch method inherits its argument from **Perceval**, thus it optionally accept two Datetime
+objects to gather only those commits after and before a given date, a list of branches to focus on specific development
+activities, and a flag to collect the commits available after the last execution.
+
+```
+#! /usr/bin/env python3
+from graal.backends.core.cocom import CoCom
+
+# URL for the git repo to analyze
+repo_uri = ’http://github.com/chaoss/grimoirelab-perceval’
+
+# directory where to mirror the repo
+repo_dir = ’/tmp/graal-cocom’
+
+# Cocom object initialization
+cc = CoCom(uri=repo_uri, git_path=repo_dir)
+
+# fetch all commits
+commits = [commit for commit in cc.fetch()]
+```
+
+## How to integrate it with Arthur
+[Arthur](https://github.com/chaoss/grimoirelab-kingarthur) is another tool of the [Grimoirelab ecosystem](https://chaoss.github.io/grimoirelab/). It was originally designed to allow to schedule
+and run Perceval executions at scale through distributed **Redis** queues, and store the obtained results in an **ElasticSearch** database.
+
+Arthur has been extended to allow handling Graal tasks, which inherit from Perceval Git tasks. The code to make this extension possible is
+available at: https://github.com/chaoss/grimoirelab-kingarthur/pull/33.
+
+Information about Arthur is available at https://github.com/chaoss/grimoirelab-kingarthur.
 
-setup(**setup_kwargs)
```

