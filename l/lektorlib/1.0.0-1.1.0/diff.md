# Comparing `tmp/lektorlib-1.0.0.tar.gz` & `tmp/lektorlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektorlib-1.0.0.tar", last modified: Fri Jan 28 21:55:11 2022, max compression
+gzip compressed data, was "lektorlib-1.1.0.tar", last modified: Fri Apr 21 02:16:01 2023, max compression
```

## Comparing `lektorlib-1.0.0.tar` & `lektorlib-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.883616 lektorlib-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.883616 lektorlib-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-01-28 21:54:59.000000 lektorlib-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-28 21:54:59.000000 lektorlib-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-01-28 21:54:59.000000 lektorlib-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-01-28 21:54:59.000000 lektorlib-1.0.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-01-28 21:54:59.000000 lektorlib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-01-28 21:54:59.000000 lektorlib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-01-28 21:55:11.887616 lektorlib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-01-28 21:54:59.000000 lektorlib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.883616 lektorlib-1.0.0/lektorlib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 21:54:59.000000 lektorlib-1.0.0/lektorlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-01-28 21:54:59.000000 lektorlib-1.0.0/lektorlib/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-01-28 21:54:59.000000 lektorlib-1.0.0/lektorlib/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-01-28 21:54:59.000000 lektorlib-1.0.0/lektorlib/recordcache.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-01-28 21:54:59.000000 lektorlib-1.0.0/lektorlib/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/lektorlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-01-28 21:55:11.000000 lektorlib-1.0.0/lektorlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-28 21:55:11.000000 lektorlib-1.0.0/lektorlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 21:55:11.000000 lektorlib-1.0.0/lektorlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-28 21:55:11.000000 lektorlib-1.0.0/lektorlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-01-28 21:54:59.000000 lektorlib-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-01-28 21:55:11.887616 lektorlib-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/Test Site.lektorproject
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.883616 lektorlib-1.0.0/tests/test-site/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/assets/static/
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/assets/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/content/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/content/about/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/content/about/contents.lr
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/content/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/content/projects/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/content/projects/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/models/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/models/page.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 21:55:11.887616 lektorlib-1.0.0/tests/test-site/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/templates/macros/pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test-site/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     8641 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test_recordcache.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-01-28 21:54:59.000000 lektorlib-1.0.0/tox.ini
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      101 2022-01-28 23:09:49.000000 lektorlib-1.1.0/.gitignore
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      380 2023-04-21 02:13:38.000000 lektorlib-1.1.0/CHANGES.md
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1062 2020-05-05 17:14:03.000000 lektorlib-1.1.0/LICENSE
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       14 2023-04-20 22:36:48.000000 lektorlib-1.1.0/MANIFEST.in
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4649 2023-04-21 02:16:01.364485 lektorlib-1.1.0/PKG-INFO
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2071 2022-01-28 20:29:23.000000 lektorlib-1.1.0/README.md
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/lektorlib/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)        0 2020-04-26 00:52:06.000000 lektorlib-1.1.0/lektorlib/__init__.py
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      886 2023-04-20 22:36:48.000000 lektorlib-1.1.0/lektorlib/context.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)     5087 2022-01-28 19:26:47.000000 lektorlib-1.1.0/lektorlib/query.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      756 2022-01-28 19:17:12.000000 lektorlib-1.1.0/lektorlib/recordcache.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      466 2022-01-28 19:27:18.000000 lektorlib-1.1.0/lektorlib/testing.py
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/lektorlib.egg-info/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4649 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/PKG-INFO
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      798 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       10 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/top_level.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1173 2023-04-20 22:36:48.000000 lektorlib-1.1.0/pyproject.toml
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       38 2023-04-21 02:16:01.364485 lektorlib-1.1.0/setup.cfg
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)        0 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/__init__.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1015 2022-01-28 19:27:52.000000 lektorlib-1.1.0/tests/conftest.py
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)       27 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/Test Site.lektorproject
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/tests/test-site/assets/
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/assets/static/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      538 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/assets/static/style.css
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/about/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      144 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/about/contents.lr
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      135 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/contents.lr
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/projects/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)       96 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/projects/contents.lr
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/models/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      133 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/models/page.ini
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/templates/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      804 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/layout.html
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/templates/macros/
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      475 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/macros/pagination.html
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      154 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/page.html
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2123 2023-04-20 22:36:48.000000 lektorlib-1.1.0/tests/test_context.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)     8641 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_query.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)     2112 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_recordcache.py
+-rw-r--r--   0 dairiki   (1000) dairiki   (1000)      729 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_testing.py
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1002 2023-04-20 22:36:48.000000 lektorlib-1.1.0/tox.ini
```

### Comparing `lektorlib-1.0.0/LICENSE` & `lektorlib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/README.md` & `lektorlib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/lektorlib/context.py` & `lektorlib-1.1.0/lektorlib/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 
     def __init__(self, ctx):
         self._ctx = ctx
 
     def __getattr__(self, attr):
         return getattr(self._ctx, attr)
 
-    def record_dependency(self, filename):
+    def record_dependency(self, filename, affects_url=None):
         pass
 
     def record_virtual_dependency(self, virtual_source):
         pass
```

### Comparing `lektorlib-1.0.0/lektorlib/query.py` & `lektorlib-1.1.0/lektorlib/query.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/lektorlib/recordcache.py` & `lektorlib-1.1.0/lektorlib/recordcache.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/lektorlib.egg-info/SOURCES.txt` & `lektorlib-1.1.0/lektorlib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 .gitignore
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 tox.ini
-.github/workflows/publish.yml
-.github/workflows/tests.yml
 lektorlib/__init__.py
 lektorlib/context.py
 lektorlib/query.py
 lektorlib/recordcache.py
 lektorlib/testing.py
 lektorlib.egg-info/PKG-INFO
 lektorlib.egg-info/SOURCES.txt
```

### Comparing `lektorlib-1.0.0/tests/conftest.py` & `lektorlib-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tests/test-site/assets/static/style.css` & `lektorlib-1.1.0/tests/test-site/assets/static/style.css`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tests/test-site/templates/layout.html` & `lektorlib-1.1.0/tests/test-site/templates/layout.html`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tests/test_context.py` & `lektorlib-1.1.0/tests/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,13 +48,17 @@
         assert lektor_context.cache['test'] == 'value'
 
     def test_record_dependency(self, proxy, lektor_context):
         lektor_context.record_dependency('a')
         proxy.record_dependency('b')
         assert proxy.referenced_dependencies == set('a')
 
+    def test_record_dependency_accepts_affects_url(self, proxy):
+        proxy.record_dependency('b', affects_url=True)
+        assert proxy.referenced_dependencies == set()
+
     def test_record_virtual_dependency(self, proxy, lektor_context,
                                        lektor_pad):
         proxy.record_virtual_dependency(lektor_pad.get('/projects@1'))
         assert not proxy.referenced_virtual_dependencies
         lektor_context.record_virtual_dependency(lektor_pad.get('/projects@2'))
         assert proxy.referenced_virtual_dependencies
```

### Comparing `lektorlib-1.0.0/tests/test_query.py` & `lektorlib-1.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tests/test_recordcache.py` & `lektorlib-1.1.0/tests/test_recordcache.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tests/test_testing.py` & `lektorlib-1.1.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.0.0/tox.ini` & `lektorlib-1.1.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 [tox]
 minversion = 3.3
 isolated_build = true
-envlist = {py37,py38,py39,py310}{,-lektor32},lint
+envlist = {py37,py38,py39,py310,py311}{,-lektor33},lint
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310, lint
+    3.10: py310
+    3.11: py311, lint
 
 [testenv]
 deps =
     pytest
     pytest-cov
-    lektor
-    lektor32: lektor<3.3
+    !lektor33: lektor>=3.4.0a1
+    lektor33: lektor<3.4
     
 setenv =
     # Prevent parallel pytest-cov runs from clobbering each others .coverage file
     COVERAGE_FILE = .coverage.{envname}
 commands =
     pytest --cov=lektorlib --cov-report=term-missing --cov-report=html \
         {posargs:--cov-fail-under=100 tests}
 
+# workaround for pip cache contention under `tox p` with older pips
+download = true
+
 [testenv:lint]
 skip_install = True
 deps =
     build
     flake8
     twine
-    check-manifest
 commands =
     python -m build --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
     flake8 lektorlib tests
-    check-manifest
 
 [flake8]
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs,
```

