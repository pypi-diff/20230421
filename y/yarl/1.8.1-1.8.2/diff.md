# Comparing `tmp/yarl-1.8.1.tar.gz` & `tmp/yarl-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yarl-1.8.1.tar", last modified: Mon Aug  1 21:35:54 2022, max compression
+gzip compressed data, was "yarl-1.8.2.tar", last modified: Sat Dec  3 03:07:53 2022, max compression
```

## Comparing `yarl-1.8.1.tar` & `yarl-1.8.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.061226 yarl-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    14881 2022-08-01 21:35:35.000000 yarl-1.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-08-01 21:35:35.000000 yarl-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-01 21:35:35.000000 yarl-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    21039 2022-08-01 21:35:54.061226 yarl-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5376 2022-08-01 21:35:35.000000 yarl-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.057226 yarl-1.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.057226 yarl-1.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/_static/yarl-icon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (121)    27909 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11420 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7728 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)    38924 2022-08-01 21:35:35.000000 yarl-1.8.1/docs/yarl-icon-128x128.xcf
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-01 21:35:35.000000 yarl-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-01 21:35:54.061226 yarl-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-08-01 21:35:35.000000 yarl-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.057226 yarl-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_normalize_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)    11850 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_quoting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10769 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_update_query.py
--rw-r--r--   0 runner    (1001) docker     (121)    41065 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url_cmp_and_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)    17195 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     6264 2022-08-01 21:35:35.000000 yarl-1.8.1/tests/test_url_update_netloc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.061226 yarl-1.8.1/yarl/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/_quoting.py
--rw-r--r--   0 runner    (1001) docker     (121)   466895 2022-08-01 21:35:53.000000 yarl-1.8.1/yarl/_quoting_c.c
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/_quoting_c.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11498 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/_quoting_c.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     6370 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/_quoting_py.py
--rw-r--r--   0 runner    (1001) docker     (121)    36426 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/_url.py
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-01 21:35:35.000000 yarl-1.8.1/yarl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 21:35:54.061226 yarl-1.8.1/yarl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21039 2022-08-01 21:35:53.000000 yarl-1.8.1/yarl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-08-01 21:35:54.000000 yarl-1.8.1/yarl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 21:35:53.000000 yarl-1.8.1/yarl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-01 21:35:53.000000 yarl-1.8.1/yarl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-01 21:35:53.000000 yarl-1.8.1/yarl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.682745 yarl-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    14994 2022-12-03 03:07:42.000000 yarl-1.8.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2022-12-03 03:07:42.000000 yarl-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-03 03:07:42.000000 yarl-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21152 2022-12-03 03:07:53.682745 yarl-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5376 2022-12-03 03:07:42.000000 yarl-1.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.678745 yarl-1.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7707 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.678745 yarl-1.8.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)    17870 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/_static/yarl-icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27909 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11420 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5217 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7728 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    38924 2022-12-03 03:07:42.000000 yarl-1.8.2/docs/yarl-icon-128x128.xcf
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2022-12-03 03:07:42.000000 yarl-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-03 03:07:53.682745 yarl-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2022-12-03 03:07:42.000000 yarl-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.678745 yarl-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_normalize_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11850 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_update_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41065 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7414 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url_cmp_and_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17195 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6264 2022-12-03 03:07:42.000000 yarl-1.8.2/tests/test_url_update_netloc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.682745 yarl-1.8.2/yarl/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3883 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (122)   466895 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl/_quoting_c.c
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/_quoting_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    11498 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/_quoting_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/_quoting_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36426 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-03 03:07:42.000000 yarl-1.8.2/yarl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 03:07:53.682745 yarl-1.8.2/yarl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21152 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2022-12-03 03:07:53.000000 yarl-1.8.2/yarl.egg-info/top_level.txt
```

### Comparing `yarl-1.8.1/CHANGES.rst` & `yarl-1.8.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.8.2 (2022-12-03)
+==================
+
+This is the first release that started shipping wheels for Python 3.11.
+
+
 1.8.1 (2022-08-01)
 ==================
 
 Misc
 ----
 
 - `#694 <https://github.com/aio-libs/yarl/issues/694>`_, `#699 <https://github.com/aio-libs/yarl/issues/699>`_, `#700 <https://github.com/aio-libs/yarl/issues/700>`_, `#701 <https://github.com/aio-libs/yarl/issues/701>`_, `#702 <https://github.com/aio-libs/yarl/issues/702>`_, `#703 <https://github.com/aio-libs/yarl/issues/703>`_, `#739 <https://github.com/aio-libs/yarl/issues/739>`_
```

### Comparing `yarl-1.8.1/LICENSE` & `yarl-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/PKG-INFO` & `yarl-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarl
-Version: 1.8.1
+Version: 1.8.2
 Summary: Yet another URL library
 Home-page: https://github.com/aio-libs/yarl/
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -236,14 +236,20 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.8.2 (2022-12-03)
+==================
+
+This is the first release that started shipping wheels for Python 3.11.
+
+
 1.8.1 (2022-08-01)
 ==================
 
 Misc
 ----
 
 - `#694 <https://github.com/aio-libs/yarl/issues/694>`_, `#699 <https://github.com/aio-libs/yarl/issues/699>`_, `#700 <https://github.com/aio-libs/yarl/issues/700>`_, `#701 <https://github.com/aio-libs/yarl/issues/701>`_, `#702 <https://github.com/aio-libs/yarl/issues/702>`_, `#703 <https://github.com/aio-libs/yarl/issues/703>`_, `#739 <https://github.com/aio-libs/yarl/issues/739>`_
```

### Comparing `yarl-1.8.1/README.rst` & `yarl-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/Makefile` & `yarl-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/_static/yarl-icon-128x128.png` & `yarl-1.8.2/docs/_static/yarl-icon-128x128.png`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/api.rst` & `yarl-1.8.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/conf.py` & `yarl-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/index.rst` & `yarl-1.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/make.bat` & `yarl-1.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/docs/yarl-icon-128x128.xcf` & `yarl-1.8.2/docs/yarl-icon-128x128.xcf`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/setup.py` & `yarl-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_cache.py` & `yarl-1.8.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_cached_property.py` & `yarl-1.8.2/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_normalize_path.py` & `yarl-1.8.2/tests/test_normalize_path.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_quoting.py` & `yarl-1.8.2/tests/test_quoting.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_update_query.py` & `yarl-1.8.2/tests/test_update_query.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url.py` & `yarl-1.8.2/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url_build.py` & `yarl-1.8.2/tests/test_url_build.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url_cmp_and_hash.py` & `yarl-1.8.2/tests/test_url_cmp_and_hash.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url_parsing.py` & `yarl-1.8.2/tests/test_url_parsing.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url_query.py` & `yarl-1.8.2/tests/test_url_query.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/tests/test_url_update_netloc.py` & `yarl-1.8.2/tests/test_url_update_netloc.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/__init__.pyi` & `yarl-1.8.2/yarl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/_quoting.py` & `yarl-1.8.2/yarl/_quoting.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/_quoting_c.c` & `yarl-1.8.2/yarl/_quoting_c.c`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/_quoting_c.pyx` & `yarl-1.8.2/yarl/_quoting_c.pyx`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/_quoting_py.py` & `yarl-1.8.2/yarl/_quoting_py.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl/_url.py` & `yarl-1.8.2/yarl/_url.py`

 * *Files identical despite different names*

### Comparing `yarl-1.8.1/yarl.egg-info/PKG-INFO` & `yarl-1.8.2/yarl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarl
-Version: 1.8.1
+Version: 1.8.2
 Summary: Yet another URL library
 Home-page: https://github.com/aio-libs/yarl/
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -236,14 +236,20 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.8.2 (2022-12-03)
+==================
+
+This is the first release that started shipping wheels for Python 3.11.
+
+
 1.8.1 (2022-08-01)
 ==================
 
 Misc
 ----
 
 - `#694 <https://github.com/aio-libs/yarl/issues/694>`_, `#699 <https://github.com/aio-libs/yarl/issues/699>`_, `#700 <https://github.com/aio-libs/yarl/issues/700>`_, `#701 <https://github.com/aio-libs/yarl/issues/701>`_, `#702 <https://github.com/aio-libs/yarl/issues/702>`_, `#703 <https://github.com/aio-libs/yarl/issues/703>`_, `#739 <https://github.com/aio-libs/yarl/issues/739>`_
```

### Comparing `yarl-1.8.1/yarl.egg-info/SOURCES.txt` & `yarl-1.8.2/yarl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

