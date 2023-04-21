# Comparing `tmp/dj-test-queries-0.1.0.tar.gz` & `tmp/dj-test-queries-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-test-queries-0.1.0.tar", last modified: Fri Apr 21 11:12:01 2023, max compression
+gzip compressed data, was "dj-test-queries-0.1.1.tar", last modified: Fri Apr 21 12:46:42 2023, max compression
```

## Comparing `dj-test-queries-0.1.0.tar` & `dj-test-queries-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.621098 dj-test-queries-0.1.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.617098 dj-test-queries-0.1.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 11:12:01.621098 dj-test-queries-0.1.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2228 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.617098 dj-test-queries-0.1.0/dj_test_queries.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/dj_test_queries.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      805 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/dj_test_queries.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/dj_test_queries.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/dj_test_queries.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/dj_test_queries.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.617098 dj-test-queries-0.1.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       35 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 11:12:01.621098 dj-test-queries-0.1.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.617098 dj-test-queries-0.1.0/test_queries/
--rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/test_queries/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4087 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/test_queries/test_num_queries.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.621098 dj-test-queries-0.1.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tests/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 11:12:01.000000 dj-test-queries-0.1.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2228 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/dj_test_queries.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      805 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       35 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/test_queries/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/test_queries/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4644 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/test_queries/test_num_queries.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tox.ini
```

### Comparing `dj-test-queries-0.1.0/.travis.yml` & `dj-test-queries-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/CONTRIBUTING.rst` & `dj-test-queries-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/LICENSE` & `dj-test-queries-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/PKG-INFO` & `dj-test-queries-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
```

### Comparing `dj-test-queries-0.1.0/README.rst` & `dj-test-queries-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/dj_test_queries.egg-info/PKG-INFO` & `dj-test-queries-0.1.1/dj_test_queries.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
```

### Comparing `dj-test-queries-0.1.0/dj_test_queries.egg-info/SOURCES.txt` & `dj-test-queries-0.1.1/dj_test_queries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/docs/Makefile` & `dj-test-queries-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/docs/conf.py` & `dj-test-queries-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/docs/make.bat` & `dj-test-queries-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/runtests.py` & `dj-test-queries-0.1.1/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/setup.py` & `dj-test-queries-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/tasks.py` & `dj-test-queries-0.1.1/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/test_queries/test_num_queries.py` & `dj-test-queries-0.1.1/test_queries/test_num_queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,59 +35,70 @@
 
 class _AssertQueriesContext(_AssertNumQueriesContext):
     def __init__(self, test_case, num, connection, context_dict):
         self.context_dict = context_dict
         super().__init__(test_case, num, connection)
 
     def __exit__(self, exc_type, exc_value, traceback):
-        with open(self.context_dict["filename"], "r") as f:
-            lines = f.readlines()
-        lines = [line.strip() for line in lines]
+        unwrap_cursor(self.connection)
+        filename = self.context_dict["filename"]
+        try:
+            with open(filename, "r") as f:
+                lines = f.readlines()
+        except FileNotFoundError:
+            lines = None
         raw_queries = [s["raw_sql"] for s in self.context_dict["records"]]
-        s = SequenceMatcher(None, lines, raw_queries)
-        for tag, i1, i2, j1, j2 in s.get_opcodes():
-            if tag not in ["insert", "equal"]:
-                print(
-                    "{:7}   a[{}:{}] --> b[{}:{}] {!r:>8} --> {!r}".format(
-                        tag,
-                        i1,
-                        i2,
-                        j1,
-                        j2,
-                        [s[:50] + "..." for s in lines[i1:i2]],
-                        [s[:50] + "..." for s in raw_queries[j1:j2]],
-                    )
-                )
-            if tag == "insert":
-                for j in range(j1, j2):
-                    string = "New query was recorded:\n"
-                    string += raw_queries[j1]
-                    string += "\n"
-                    string += "Stacktrace:\n"
-                    string += "\n".join(
-                        f'  File: "{s[0]}", Line: {s[1]}, in {s[2]}\n    {s[3]}'
-                        for s in self.context_dict["records"][j]["stacktrace"]
+        if lines:
+            lines = [line.strip() for line in lines]
+            s = SequenceMatcher(None, lines, raw_queries)
+            for tag, i1, i2, j1, j2 in s.get_opcodes():
+                if tag not in ["insert", "replace", "equal"]:
+                    print(
+                        "{:7}   a[{}:{}] --> b[{}:{}] {!r:>8} --> {!r}".format(
+                            tag,
+                            i1,
+                            i2,
+                            j1,
+                            j2,
+                            [s[:50] + "..." for s in lines[i1:i2]],
+                            [s[:50] + "..." for s in raw_queries[j1:j2]],
+                        )
                     )
-                    string += "\n"
-                    string += "\n".join(
-                        [
-                            f"{rk}: {rv}"
-                            for rk, rv in self.context_dict["records"][j].items()
-                            if rk not in ["raw_sql", "stacktrace"]
-                        ]
-                    )
-                    string += "\n"
-                    string += "-----------------------------------------"
-                    print(string)
-
-        if os.environ.get("TEST_QUERIES_REWRITE_SQLLOGS"):
-            with open(self.context_dict["filename"], "w") as f:
-                f.write("\n".join(raw_queries))
+                if tag in ["insert", "replace"]:
+                    for j in range(j1, j2):
+                        string = ""
+                        if tag == "insert":
+                            string += "New query was recorded:\n"
+                        elif tag == "replace":
+                            string += "Query was replaced:\n"
+                        string += raw_queries[j1]
+                        string += "\n"
+                        string += "Stacktrace:\n"
+                        string += "\n".join(
+                            f'  File: "{s[0]}", Line: {s[1]}, in {s[2]}\n    {s[3]}'
+                            for s in self.context_dict["records"][j]["stacktrace"]
+                        )
+                        string += "\n"
+                        string += "\n".join(
+                            [
+                                f"{rk}: {rv}"
+                                for rk, rv in self.context_dict["records"][j].items()
+                                if rk not in ["raw_sql", "stacktrace"]
+                            ]
+                        )
+                        string += "\n"
+                        string += "-----------------------------------------"
+                        print(string)
+
+        if not os.environ.get("TEST_QUERIES_REWRITE_SQLLOGS"):
+            filename += ".new"
+        os.makedirs(filename.rsplit("/", 1)[0], exist_ok=True)
+        with open(filename, "w") as f:
+            f.write("\n".join(raw_queries))
 
-        unwrap_cursor(self.connection)
         return super().__exit__(exc_type, exc_value, traceback)
 
 
 class NumQueriesMixin(TransactionTestCase):
     context: Dict[str, Any] = {
         "records": [],
     }
```

### Comparing `dj-test-queries-0.1.0/tests/README.md` & `dj-test-queries-0.1.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.0/tests/settings.py` & `dj-test-queries-0.1.1/tests/settings.py`

 * *Files identical despite different names*

