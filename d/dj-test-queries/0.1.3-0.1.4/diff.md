# Comparing `tmp/dj-test-queries-0.1.3.tar.gz` & `tmp/dj-test-queries-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-test-queries-0.1.3.tar", last modified: Fri Apr 21 14:04:04 2023, max compression
+gzip compressed data, was "dj-test-queries-0.1.4.tar", last modified: Fri Apr 21 14:44:22 2023, max compression
```

## Comparing `dj-test-queries-0.1.3.tar` & `dj-test-queries-0.1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.091447 dj-test-queries-0.1.3/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2324 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/dj_test_queries.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      843 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       21 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 14:04:04.000000 dj-test-queries-0.1.3/dj_test_queries.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       56 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/test_queries/
--rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/test_queries/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4656 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/test_queries/test_num_queries.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:04.095448 dj-test-queries-0.1.3/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tests/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 14:04:03.000000 dj-test-queries-0.1.3/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 14:44:22.447962 dj-test-queries-0.1.4/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2324 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/dj_test_queries.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      843 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       21 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 14:44:22.000000 dj-test-queries-0.1.4/dj_test_queries.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       56 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 14:44:22.447962 dj-test-queries-0.1.4/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/test_queries/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/test_queries/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4665 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/test_queries/test_num_queries.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:22.443962 dj-test-queries-0.1.4/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tests/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 14:44:21.000000 dj-test-queries-0.1.4/tox.ini
```

### Comparing `dj-test-queries-0.1.3/.travis.yml` & `dj-test-queries-0.1.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/CONTRIBUTING.rst` & `dj-test-queries-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/LICENSE` & `dj-test-queries-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/PKG-INFO` & `dj-test-queries-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
```

### Comparing `dj-test-queries-0.1.3/README.rst` & `dj-test-queries-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/dj_test_queries.egg-info/PKG-INFO` & `dj-test-queries-0.1.4/dj_test_queries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
```

### Comparing `dj-test-queries-0.1.3/dj_test_queries.egg-info/SOURCES.txt` & `dj-test-queries-0.1.4/dj_test_queries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/docs/Makefile` & `dj-test-queries-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/docs/conf.py` & `dj-test-queries-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/docs/make.bat` & `dj-test-queries-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/runtests.py` & `dj-test-queries-0.1.4/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/setup.py` & `dj-test-queries-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/tasks.py` & `dj-test-queries-0.1.4/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/test_queries/test_num_queries.py` & `dj-test-queries-0.1.4/test_queries/test_num_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,30 +96,29 @@
             f.write("\n".join(raw_queries) + "\n")
 
         return super().__exit__(exc_type, exc_value, traceback)
 
 
 class NumQueriesMixin(TransactionTestCase):
     executed_times = 0
-    context: Dict[str, Any] = {
-        "records": [],
-    }
+    context: Dict[str, Any] = {}
 
     def assertNumQueries(  # noqa: N802
         self, num, func=None, *args, using=DEFAULT_DB_ALIAS, **kwargs
     ):
         conn = connections[using]
         path, file_prefix = inspect.getmodule(self).__file__[:-3].rsplit("/", 1)
         filename = (
             f"{path}/sqllog/{file_prefix}."
             f"{self.__class__.__name__}."
             f"{self._testMethodName}.{self.executed_times}.sqllog"
         )
         self.executed_times += 1
         self.context["filename"] = filename
+        self.context["records"] = []
         logger = Logger(context=self.context)
 
         wrap_cursor(conn, logger)
         context = _AssertQueriesContext(self, num, conn, self.context)
 
         if func is None:
             return context
```

### Comparing `dj-test-queries-0.1.3/tests/README.md` & `dj-test-queries-0.1.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.3/tests/settings.py` & `dj-test-queries-0.1.4/tests/settings.py`

 * *Files identical despite different names*

