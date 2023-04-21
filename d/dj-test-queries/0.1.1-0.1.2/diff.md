# Comparing `tmp/dj-test-queries-0.1.1.tar.gz` & `tmp/dj-test-queries-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-test-queries-0.1.1.tar", last modified: Fri Apr 21 12:46:42 2023, max compression
+gzip compressed data, was "dj-test-queries-0.1.2.tar", last modified: Fri Apr 21 13:46:36 2023, max compression
```

## Comparing `dj-test-queries-0.1.1.tar` & `dj-test-queries-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2228 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/dj_test_queries.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3929 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      805 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 12:46:42.000000 dj-test-queries-0.1.1/dj_test_queries.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.138995 dj-test-queries-0.1.1/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       35 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/test_queries/
--rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/test_queries/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4644 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/test_queries/test_num_queries.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:42.142995 dj-test-queries-0.1.1/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tests/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 12:46:41.000000 dj-test-queries-0.1.1/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       97 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      180 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2324 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/dj_test_queries.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4041 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      843 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       21 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       13 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/dj_test_queries.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8191 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      215 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       56 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      109 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      256 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2419 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2219 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/test_queries/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       68 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/test_queries/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4701 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/test_queries/test_num_queries.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.903908 dj-test-queries-0.1.2/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3076 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      285 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      389 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tests/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      418 2023-04-21 13:46:36.000000 dj-test-queries-0.1.2/tox.ini
```

### Comparing `dj-test-queries-0.1.1/.travis.yml` & `dj-test-queries-0.1.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/CONTRIBUTING.rst` & `dj-test-queries-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/LICENSE` & `dj-test-queries-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/PKG-INFO` & `dj-test-queries-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
         =============================
         
         .. image:: https://badge.fury.io/py/dj-test-queries.svg
             :target: https://badge.fury.io/py/dj-test-queries
         
-        .. image:: https://travis-ci.org/PetrDlouhy/dj-test-queries.svg?branch=master
-            :target: https://travis-ci.org/PetrDlouhy/dj-test-queries
-        
         .. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
         
         Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
         
         Documentation
         -------------
         
         The full documentation is at https://dj-test-queries.readthedocs.io.
         
         Quickstart
         ----------
         
-        Install ``django-debug-toolbar`` dependency to your project:
+        Install ``dj-test-queries``:
         
         .. code-block:: bash
         
-           pip install django-debug-toolbar
+           pip install dj-test-queries
         
         Apply ``NumQueriesMixin`` to your test and use ``assertNumQueries`` as you would normally do:
         
         .. code-block:: python
         
             from test_queries import NumQueriesMixin
         
             class XYZTests(NumQueriesMixin, TestCase):
                 def test_xyz(self):
                     with self.assertNumQueries(3):
                         xyz()
         
+        Generating SQL log records
+        --------------------------
+        
         Run the tests with ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable to generate sqllog files:
         
         .. code-block:: bash
         
             TEST_QUERIES_REWRITE_SQLLOGS="true" manage.py test
         
         Files like ``test_views.XYZTests.test_xyz.sqllog`` will appear in ``sqllog`` directory next to your ``test_views.py`` file.
         
         If you will run the test next time and the queries will differ from previous, the test will print out output detailing the change with stacktrace from where the query was executed.
         You can also enlist the ``*.sqllog`` files to your repository to see the changes.
         
+        If the tests are executed without the ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable, the logs are created to files named like ``test_views.XYZTests.test_xyz.sqllog`` to make possible to compare the difference.
+        
         Running Tests
         -------------
         
         Does the code actually work?
         
         ::
```

### Comparing `dj-test-queries-0.1.1/README.rst` & `dj-test-queries-0.1.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 =============================
 Django test queries
 =============================
 
 .. image:: https://badge.fury.io/py/dj-test-queries.svg
     :target: https://badge.fury.io/py/dj-test-queries
 
-.. image:: https://travis-ci.org/PetrDlouhy/dj-test-queries.svg?branch=master
-    :target: https://travis-ci.org/PetrDlouhy/dj-test-queries
-
 .. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
 
 Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
 
 Documentation
 -------------
 
 The full documentation is at https://dj-test-queries.readthedocs.io.
 
 Quickstart
 ----------
 
-Install ``django-debug-toolbar`` dependency to your project:
+Install ``dj-test-queries``:
 
 .. code-block:: bash
 
-   pip install django-debug-toolbar
+   pip install dj-test-queries
 
 Apply ``NumQueriesMixin`` to your test and use ``assertNumQueries`` as you would normally do:
 
 .. code-block:: python
 
     from test_queries import NumQueriesMixin
 
     class XYZTests(NumQueriesMixin, TestCase):
         def test_xyz(self):
             with self.assertNumQueries(3):
                 xyz()
 
+Generating SQL log records
+--------------------------
+
 Run the tests with ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable to generate sqllog files:
 
 .. code-block:: bash
 
     TEST_QUERIES_REWRITE_SQLLOGS="true" manage.py test
 
 Files like ``test_views.XYZTests.test_xyz.sqllog`` will appear in ``sqllog`` directory next to your ``test_views.py`` file.
 
 If you will run the test next time and the queries will differ from previous, the test will print out output detailing the change with stacktrace from where the query was executed.
 You can also enlist the ``*.sqllog`` files to your repository to see the changes.
 
+If the tests are executed without the ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable, the logs are created to files named like ``test_views.XYZTests.test_xyz.sqllog`` to make possible to compare the difference.
+
 Running Tests
 -------------
 
 Does the code actually work?
 
 ::
```

### Comparing `dj-test-queries-0.1.1/dj_test_queries.egg-info/PKG-INFO` & `dj-test-queries-0.1.2/dj_test_queries.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 Metadata-Version: 2.1
 Name: dj-test-queries
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.[
 Home-page: https://github.com/PetrDlouhy/dj-test-queries
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Description: =============================
         Django test queries
         =============================
         
         .. image:: https://badge.fury.io/py/dj-test-queries.svg
             :target: https://badge.fury.io/py/dj-test-queries
         
-        .. image:: https://travis-ci.org/PetrDlouhy/dj-test-queries.svg?branch=master
-            :target: https://travis-ci.org/PetrDlouhy/dj-test-queries
-        
         .. image:: https://codecov.io/gh/PetrDlouhy/dj-test-queries/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/PetrDlouhy/dj-test-queries
         
         Extension of assertNumQueries that can record queries that were executed and show the differences in future runs.
         
         Documentation
         -------------
         
         The full documentation is at https://dj-test-queries.readthedocs.io.
         
         Quickstart
         ----------
         
-        Install ``django-debug-toolbar`` dependency to your project:
+        Install ``dj-test-queries``:
         
         .. code-block:: bash
         
-           pip install django-debug-toolbar
+           pip install dj-test-queries
         
         Apply ``NumQueriesMixin`` to your test and use ``assertNumQueries`` as you would normally do:
         
         .. code-block:: python
         
             from test_queries import NumQueriesMixin
         
             class XYZTests(NumQueriesMixin, TestCase):
                 def test_xyz(self):
                     with self.assertNumQueries(3):
                         xyz()
         
+        Generating SQL log records
+        --------------------------
+        
         Run the tests with ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable to generate sqllog files:
         
         .. code-block:: bash
         
             TEST_QUERIES_REWRITE_SQLLOGS="true" manage.py test
         
         Files like ``test_views.XYZTests.test_xyz.sqllog`` will appear in ``sqllog`` directory next to your ``test_views.py`` file.
         
         If you will run the test next time and the queries will differ from previous, the test will print out output detailing the change with stacktrace from where the query was executed.
         You can also enlist the ``*.sqllog`` files to your repository to see the changes.
         
+        If the tests are executed without the ``TEST_QUERIES_REWRITE_SQLLOGS`` environment variable, the logs are created to files named like ``test_views.XYZTests.test_xyz.sqllog`` to make possible to compare the difference.
+        
         Running Tests
         -------------
         
         Does the code actually work?
         
         ::
```

### Comparing `dj-test-queries-0.1.1/dj_test_queries.egg-info/SOURCES.txt` & `dj-test-queries-0.1.2/dj_test_queries.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 tasks.py
 tox.ini
 .github/ISSUE_TEMPLATE.md
 dj_test_queries.egg-info/PKG-INFO
 dj_test_queries.egg-info/SOURCES.txt
 dj_test_queries.egg-info/dependency_links.txt
 dj_test_queries.egg-info/not-zip-safe
+dj_test_queries.egg-info/requires.txt
 dj_test_queries.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
```

### Comparing `dj-test-queries-0.1.1/docs/Makefile` & `dj-test-queries-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/docs/conf.py` & `dj-test-queries-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/docs/make.bat` & `dj-test-queries-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/runtests.py` & `dj-test-queries-0.1.2/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/setup.py` & `dj-test-queries-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/tasks.py` & `dj-test-queries-0.1.2/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/test_queries/test_num_queries.py` & `dj-test-queries-0.1.2/test_queries/test_num_queries.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,36 +89,37 @@
                         string += "-----------------------------------------"
                         print(string)
 
         if not os.environ.get("TEST_QUERIES_REWRITE_SQLLOGS"):
             filename += ".new"
         os.makedirs(filename.rsplit("/", 1)[0], exist_ok=True)
         with open(filename, "w") as f:
-            f.write("\n".join(raw_queries))
+            f.write("\n".join(raw_queries) + "\n")
 
         return super().__exit__(exc_type, exc_value, traceback)
 
 
 class NumQueriesMixin(TransactionTestCase):
+    executed_times = 0
     context: Dict[str, Any] = {
         "records": [],
     }
 
     def assertNumQueries(  # noqa: N802
         self, num, func=None, *args, using=DEFAULT_DB_ALIAS, **kwargs
     ):
         conn = connections[using]
         path, file_prefix = inspect.getmodule(self).__file__[:-3].rsplit("/", 1)
         filename = (
             f"{path}/sqllog/{file_prefix}."
             f"{self.__class__.__name__}."
             f"{self._testMethodName}.sqllog"
+            f"{self._testMethodName}.{self.executed_times}.sqllog"
         )
-        # if os.path.exists(filename):
-        #     os.remove(filename)
+        self.executed_times += 1
         self.context["filename"] = filename
         logger = Logger(context=self.context)
 
         wrap_cursor(conn, logger)
         context = _AssertQueriesContext(self, num, conn, self.context)
 
         if func is None:
```

### Comparing `dj-test-queries-0.1.1/tests/README.md` & `dj-test-queries-0.1.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `dj-test-queries-0.1.1/tests/settings.py` & `dj-test-queries-0.1.2/tests/settings.py`

 * *Files identical despite different names*

