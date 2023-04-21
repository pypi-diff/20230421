# Comparing `tmp/datadiligence-0.1.1-3.tar.gz` & `tmp/datadiligence-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadiligence-0.1.1.tar", last modified: Thu Apr 20 14:30:11 2023, max compression
+gzip compressed data, was "datadiligence-0.1.2.tar", last modified: Fri Apr 21 16:08:07 2023, max compression
```

## Comparing `datadiligence-0.1.1-3.tar` & `datadiligence-0.1.2.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.794714 datadiligence-0.1.1/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      596 2023-04-20 12:54:12.000000 datadiligence-0.1.1/.coveragerc
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      587 2023-04-20 12:55:53.000000 datadiligence-0.1.1/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2023-04-20 12:54:24.000000 datadiligence-0.1.1/.readthedocs.yml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      149 2023-04-20 12:54:30.000000 datadiligence-0.1.1/AUTHORS.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       87 2023-04-20 12:54:35.000000 datadiligence-0.1.1/CHANGELOG.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12356 2023-04-20 12:54:43.000000 datadiligence-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1080 2023-04-20 12:54:47.000000 datadiligence-0.1.1/LICENSE.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4024 2023-04-20 14:30:11.794810 datadiligence-0.1.1/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3223 2023-04-20 14:29:14.000000 datadiligence-0.1.1/README.rst
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.789570 datadiligence-0.1.1/docs/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/Makefile
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.789705 datadiligence-0.1.1/docs/_static/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5988 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/advanced.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/authors.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/changelog.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9764 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/conf.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       33 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/contributing.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1421 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/index.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/license.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9294 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/quickstart.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/readme.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2023-04-20 12:53:36.000000 datadiligence-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.790207 datadiligence-0.1.1/examples/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      168 2023-04-20 12:53:39.000000 datadiligence-0.1.1/examples/http_headers.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      913 2023-04-20 12:53:39.000000 datadiligence-0.1.1/examples/pre_and_post_processing.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      491 2023-04-20 12:53:39.000000 datadiligence-0.1.1/examples/spawning_api.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2023-04-20 12:54:54.000000 datadiligence-0.1.1/pyproject.toml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1622 2023-04-20 14:30:11.795158 datadiligence-0.1.1/setup.cfg
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      708 2023-04-20 12:55:19.000000 datadiligence-0.1.1/setup.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.784708 datadiligence-0.1.1/src/
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.791017 datadiligence-0.1.1/src/datadiligence/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      900 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2766 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/bootstrap.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.792520 datadiligence-0.1.1/src/datadiligence/evaluators/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      200 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/evaluators/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      814 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/evaluators/base.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      853 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/evaluators/http.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      924 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/evaluators/postprocess.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1354 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/evaluators/preprocess.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2243 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/exceptions.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.793188 datadiligence-0.1.1/src/datadiligence/rules/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      128 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/rules/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1039 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/rules/base.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      447 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/rules/c2pa.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5165 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/rules/http.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     8764 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/rules/spawning.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      576 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence/utils.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.791848 datadiligence-0.1.1/src/datadiligence.egg-info/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4024 2023-04-20 14:30:11.000000 datadiligence-0.1.1/src/datadiligence.egg-info/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1391 2023-04-20 14:30:11.000000 datadiligence-0.1.1/src/datadiligence.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-04-20 14:30:11.000000 datadiligence-0.1.1/src/datadiligence.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-04-20 12:53:51.000000 datadiligence-0.1.1/src/datadiligence.egg-info/not-zip-safe
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      124 2023-04-20 14:30:11.000000 datadiligence-0.1.1/src/datadiligence.egg-info/requires.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       14 2023-04-20 14:30:11.000000 datadiligence-0.1.1/src/datadiligence.egg-info/top_level.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.794304 datadiligence-0.1.1/tests/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      281 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/conftest.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.794447 datadiligence-0.1.1/tests/samples/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      841 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/samples/custom.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-20 14:30:11.794585 datadiligence-0.1.1/tests/server/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1884 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/server/app.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2247 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_bootstrapper.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      263 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_cp2a.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6826 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_evaluators.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5159 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_spawningapi.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      468 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_utils.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5757 2023-04-20 12:53:54.000000 datadiligence-0.1.1/tests/test_xrobotsheader.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2826 2023-04-20 12:55:24.000000 datadiligence-0.1.1/tox.ini
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.529111 datadiligence-0.1.2/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      596 2023-04-20 12:54:12.000000 datadiligence-0.1.2/.coveragerc
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.517724 datadiligence-0.1.2/.github/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.521551 datadiligence-0.1.2/.github/workflows/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      831 2023-04-21 15:00:32.000000 datadiligence-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      587 2023-04-20 12:55:53.000000 datadiligence-0.1.2/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2023-04-20 12:54:24.000000 datadiligence-0.1.2/.readthedocs.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      149 2023-04-20 12:54:30.000000 datadiligence-0.1.2/AUTHORS.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       87 2023-04-20 12:54:35.000000 datadiligence-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12356 2023-04-20 12:54:43.000000 datadiligence-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1080 2023-04-20 12:54:47.000000 datadiligence-0.1.2/LICENSE.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-04-21 16:08:07.529200 datadiligence-0.1.2/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3279 2023-04-21 16:03:48.000000 datadiligence-0.1.2/README.rst
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.523864 datadiligence-0.1.2/docs/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/Makefile
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.524026 datadiligence-0.1.2/docs/_static/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6444 2023-04-21 16:03:48.000000 datadiligence-0.1.2/docs/advanced.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/authors.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/changelog.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9764 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/conf.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       33 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/contributing.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1421 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/index.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/license.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9449 2023-04-21 16:03:48.000000 datadiligence-0.1.2/docs/quickstart.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/readme.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2023-04-20 12:53:36.000000 datadiligence-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.524665 datadiligence-0.1.2/examples/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      154 2023-04-21 16:03:48.000000 datadiligence-0.1.2/examples/http_headers.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      936 2023-04-21 16:03:48.000000 datadiligence-0.1.2/examples/pre_and_post_processing.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      481 2023-04-21 16:03:48.000000 datadiligence-0.1.2/examples/spawning_api.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2023-04-20 12:54:54.000000 datadiligence-0.1.2/pyproject.toml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1622 2023-04-21 16:08:07.529546 datadiligence-0.1.2/setup.cfg
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      708 2023-04-20 12:55:19.000000 datadiligence-0.1.2/setup.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.518107 datadiligence-0.1.2/src/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.525411 datadiligence-0.1.2/src/datadiligence/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      916 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3316 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/bootstrap.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.526921 datadiligence-0.1.2/src/datadiligence/evaluators/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      200 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/evaluators/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      966 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/evaluators/base.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      642 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/evaluators/http.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      924 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/evaluators/postprocess.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2095 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/evaluators/preprocess.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2243 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/exceptions.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.527586 datadiligence-0.1.2/src/datadiligence/rules/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      128 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/rules/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1045 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/rules/base.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      447 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/rules/c2pa.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5165 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/rules/http.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    10044 2023-04-21 16:03:48.000000 datadiligence-0.1.2/src/datadiligence/rules/spawning.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      576 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence/utils.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.526251 datadiligence-0.1.2/src/datadiligence.egg-info/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-04-21 16:08:07.000000 datadiligence-0.1.2/src/datadiligence.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1428 2023-04-21 16:08:07.000000 datadiligence-0.1.2/src/datadiligence.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-04-21 16:08:07.000000 datadiligence-0.1.2/src/datadiligence.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-04-20 12:53:51.000000 datadiligence-0.1.2/src/datadiligence.egg-info/not-zip-safe
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      124 2023-04-21 16:08:07.000000 datadiligence-0.1.2/src/datadiligence.egg-info/requires.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       14 2023-04-21 16:08:07.000000 datadiligence-0.1.2/src/datadiligence.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.528559 datadiligence-0.1.2/tests/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      281 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/conftest.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.528811 datadiligence-0.1.2/tests/samples/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      841 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/samples/custom.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-04-21 16:08:07.528986 datadiligence-0.1.2/tests/server/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1884 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/server/app.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4234 2023-04-21 16:03:48.000000 datadiligence-0.1.2/tests/test_bootstrapper.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      263 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/test_cp2a.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7753 2023-04-21 16:03:48.000000 datadiligence-0.1.2/tests/test_evaluators.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6689 2023-04-21 16:03:48.000000 datadiligence-0.1.2/tests/test_spawningapi.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      468 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/test_utils.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5757 2023-04-20 12:53:54.000000 datadiligence-0.1.2/tests/test_xrobotsheader.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2821 2023-04-21 16:03:48.000000 datadiligence-0.1.2/tox.ini
```

### Comparing `datadiligence-0.1.1/.coveragerc` & `datadiligence-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/.gitignore` & `datadiligence-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/.readthedocs.yml` & `datadiligence-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/CONTRIBUTING.rst` & `datadiligence-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/LICENSE.txt` & `datadiligence-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/PKG-INFO` & `datadiligence-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadiligence
-Version: 0.1.1
+Version: 0.1.2
 Summary: Respect generative AI opt-outs in your ML and training pipeline.
 Home-page: https://github.com/Spawning-Inc/datadiligence/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://datadiligence.readthedocs.io/en/latest/quickstart.html
 Project-URL: Source, https://github.com/Spawning-Inc/datadiligence/
@@ -65,16 +65,19 @@
 
    pip install datadiligence
 
 Add bulk pre-processing for URLs in your pipeline (requires Spawning API Key)::
 
    >>> import datadiligence as dd
    >>> urls = ["https://www.example.com/art-123456789.jpg", "https://www.example.com/art-987654321.jpg"]
+   >>> dd.filter_allowed(urls=urls)
+    ["https://www.example.com/art-123456789.jpg"]
    >>> dd.is_allowed(urls=urls)
-   ["https://www.example.com/art-123456789.jpg"]
+    [True, False]
+
 
 Check HTTP responses in post-processing::
 
    >>> response = requests.get("https://www.example.com/art-123456789.jpg")
    >>> is_allowed = dd.is_allowed(response=response)
    True
    >>> if is_allowed:
```

### Comparing `datadiligence-0.1.1/README.rst` & `datadiligence-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,19 @@
 
    pip install datadiligence
 
 Add bulk pre-processing for URLs in your pipeline (requires Spawning API Key)::
 
    >>> import datadiligence as dd
    >>> urls = ["https://www.example.com/art-123456789.jpg", "https://www.example.com/art-987654321.jpg"]
+   >>> dd.filter_allowed(urls=urls)
+    ["https://www.example.com/art-123456789.jpg"]
    >>> dd.is_allowed(urls=urls)
-   ["https://www.example.com/art-123456789.jpg"]
+    [True, False]
+
 
 Check HTTP responses in post-processing::
 
    >>> response = requests.get("https://www.example.com/art-123456789.jpg")
    >>> is_allowed = dd.is_allowed(response=response)
    True
    >>> if is_allowed:
```

### Comparing `datadiligence-0.1.1/docs/Makefile` & `datadiligence-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/docs/advanced.rst` & `datadiligence-0.1.2/docs/advanced.rst`

 * *Files 7% similar despite different names*

```diff
@@ -105,36 +105,46 @@
 
 For example, `PostprocessEvaluator` and `PreprocessEvaluator` were both created with the **img2dataset** workflow in mind. However,
 other workflows may not already have HTTP responses, thus other evaluators may consume a URL and download the response directly.
 
 -----------------------
 Make your own Bulk Rule
 -----------------------
-Bulk `Rules` are handled slightly differently than normal `Rules`. They are intended to be a subclass of `datadiligence.rules.BulkRule` and implement the `get_allowed` function::
+Bulk `Rules` are handled slightly differently than normal `Rules`. They are intended to be a subclass of `datadiligence.rules.BulkRule` and implement the `filter_allowed` function::
 
     from datadiligence.rules import BulkRule
 
     class MyBulkRule(BulkRule):
         def is_ready(self):
             return True
 
-        def get_allowed(self, **kwargs):
+        def filter_allowed(self, **kwargs):
             return []
 
-Notice the `get_allowed` function should be called for `BulkRule` classes. This function is usually hidden behind an Evaluator,
-but it helps the developer clarify we're using a different function for bulk rules.
+Notice the ``filter_allowed`` function should be called for ``BulkRule`` classes. The `Evaluator` should also have the ``filter_allowed`` function implemented::
+
+        class MyEvaluator(Evaluator):
+            def filter_allowed(self, urls= [] **kwargs):
+                # set default to allow everything
+                allowed = [True] * len(urls)
+                for rule in self.rules:
+                    if rule.is_ready():
+                        rule_results = rule.is_allowed(urls=urls)
+
+                        # set each url as disallowed, and never re-enable it
+                        allowed = [a and b for a, b in zip(allowed, rule_results)]
 
 Notice the response type is also not a boolean, but a list. The responses should be a list of approved URLs. As a best practice,
 the rules that will catch the most URLs should be run first, and the rules that will catch the least URLs should be run last.
 
 --------------------------
 Only Run the Spawning API
 --------------------------
 If you only want to check your URLs against the Spawning API, perform the following setup::
 
     $ export SPAWNING_API_KEY=<your_key>
     $ python
     >>> from datadiligence.rules import SpawningAPI
     >>> urls = ['http://example.com', 'https://example.com']
     >>> spawning_rule = SpawningAPI(user_agent="my-user-agent")
-    >>> spawning_rule.get_allowed(urls=urls)
+    >>> spawning_rule.filter_allowed(urls=urls)
     []
```

### Comparing `datadiligence-0.1.1/docs/conf.py` & `datadiligence-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/docs/index.rst` & `datadiligence-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/docs/quickstart.rst` & `datadiligence-0.1.2/docs/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,44 +55,51 @@
 
     import datadiligence as dd
 
 This will also instantiate some default Evaluators for you to use. We can pass a list of urls to
 the package directly to use one of these defaults::
 
     >>> urls = ['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com']
-    >>> approved_urls = dd.is_allowed(urls=urls)
+    >>> approved_urls = dd.filter_allowed(urls=urls)
     >>> approved_urls
     ['https://www.google.com']
 
-The response is a list of the URLs that are allowed. In this case, only Google is allowed.
-You can then continue to use this list of approved URLs throughout the ML pipeline.
+The response is a list of the URLs that are allowed. Additionally,
+you can use ``is_allowed`` to return a list of boolean responses::
+
+    >>> urls = ['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com']
+    >>> approved_urls = dd.is_allowed(urls=urls)
+    >>> approved_urls
+    [True, False, False]
+
+In both cases, only Google is allowed.
 
 If you're using `pyarrow` or `pandas`, you must first convert the urls to a python list::
 
     >>> # pyarrow example
     >>> import pyarrow as pa
     >>> urls = pa.array(['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com'])
     >>> approved_urls = dd.is_allowed(urls=urls.to_pylist())
     >>> approved_urls
-    ['https://www.google.com']
+    [True]
 
     >>> # pandas example
     >>> import pandas as pd
     >>> urls = pd.Series(['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com'])
     >>> approved_urls = dd.is_allowed(urls=urls.to_list())
     >>> approved_urls
-    ['https://www.google.com']
+    [True]
 
 Some rules require additional information or dependencies, such as API Keys in the case of Spawning (see below).
 If the required dependencies are not met, the related rule will NOT evaluate, and the response will be the same as if the rule was not included.
 
 For example, if the Spawning API Key is not set in your environment variables::
 
     >>> urls = ['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com']
-    >>> approved_urls = dd.is_allowed(urls=urls)
+    >>> approved_urls = dd.filter_allowed(urls=urls)
     Spawning API key not found. Please set your API key to the environment variable SPAWNING_API_KEY
     >>> approved_urls
     ['https://www.google.com', 'https://www.yahoo.com', 'https://www.bing.com']
 
 ****************
 Spawning API Key
 ****************
```

### Comparing `datadiligence-0.1.1/examples/pre_and_post_processing.py` & `datadiligence-0.1.2/examples/pre_and_post_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 md = csv.read_csv("/path/to/urls.tsv", read_options=csv.ReadOptions(encoding="utf-8"), parse_options=csv.ParseOptions(delimiter='\t'))
 
 # convert it to list
 d = md.select(["url"]).to_pandas()
 urls = d.iloc[:, 0].to_list()
 
 # send through pre-process steps (only includes Spawning API currently)
-verified_urls = dd.is_allowed("preprocess", urls=urls)
+verified_urls = dd.filter_allowed(urls=urls)  # use dd.is_allowed to get a list of booleans instead
 
 # you'll probably be downloading these images in your pipeline, this is a placeholder for that
 for url in verified_urls:
     response = requests.get(url)
     if response.status_code == 200:
         # this is the only new code you need here
-        is_allowed = dd.is_allowed("postprocess", headers=response.headers)
+        is_allowed = dd.is_allowed(response=response)
         if not is_allowed:
             continue
 
         # image is allowed after this point
```

### Comparing `datadiligence-0.1.1/setup.cfg` & `datadiligence-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/setup.py` & `datadiligence-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/src/datadiligence/__init__.py` & `datadiligence-0.1.2/src/datadiligence/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 from .evaluators import HttpEvaluator, PostprocessEvaluator, PreprocessEvaluator, Evaluator
 
 # bootstrap methods
-from .bootstrap import load_defaults, register_evaluator, is_allowed, get_evaluator, deregister_evaluator, list_evaluators
+from .bootstrap import load_defaults, register_evaluator, is_allowed, filter_allowed, get_evaluator, deregister_evaluator, list_evaluators
```

### Comparing `datadiligence-0.1.1/src/datadiligence/bootstrap.py` & `datadiligence-0.1.2/src/datadiligence/bootstrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 functions to preload default evaluators and make accessible globally
 """
 
 from .exceptions import EvaluatorAlreadyRegistered, EvaluatorNotRegistered, NotEvaluator, DefaultEvaluatorNotFound
-from .evaluators import Evaluator, PreprocessEvaluator, PostprocessEvaluator, HttpEvaluator
+from .evaluators import Evaluator, PreprocessEvaluator, PostprocessEvaluator
 
 bootstrap_dictionary = {}
 
 
 def load_defaults(user_agent=None):
     """Load the default evaluators."""
     register_evaluator(PreprocessEvaluator(user_agent=user_agent), overwrite=True)
     register_evaluator(PostprocessEvaluator(user_agent=user_agent), overwrite=True)
-    register_evaluator(HttpEvaluator(user_agent=user_agent), overwrite=True)
 
 
 def list_evaluators():
     """List the evaluators."""
     return list(bootstrap_dictionary.keys())
 
 
@@ -75,16 +74,35 @@
             raise EvaluatorNotRegistered(name)
         return bootstrap_dictionary[name].is_allowed(**kwargs)
     else:
         # since we are preloading evaluators manually, we can check to see which one to call
         # based on the kwargs
         if "urls" in kwargs:
             return bootstrap_dictionary["preprocess"].is_allowed(**kwargs)
-        elif "response" in kwargs or "headers" in kwargs:
+        elif "url" in kwargs or "response" in kwargs or "headers" in kwargs:
             return bootstrap_dictionary["postprocess"].is_allowed(**kwargs)
-        elif "url" in kwargs:
-            return bootstrap_dictionary["http"].is_allowed(**kwargs)
+        else:
+            raise DefaultEvaluatorNotFound(list(kwargs.keys()))
+
+
+def filter_allowed(name=None, **kwargs):
+    """
+    Filter a list of content.
+
+    Args:
+        name (str): The name of a specific evaluator.
+        **kwargs: Arbitrary keyword arguments to read args from.
+    """
+    if name is not None:
+        if name not in bootstrap_dictionary:
+            raise EvaluatorNotRegistered(name)
+        return bootstrap_dictionary[name].filter_allowed(**kwargs)
+    else:
+        # since we are preloading evaluators manually, we can check to see which one to call
+        # based on the kwargs
+        if "urls" in kwargs:
+            return bootstrap_dictionary["preprocess"].filter_allowed(**kwargs)
         else:
             raise DefaultEvaluatorNotFound(list(kwargs.keys()))
 
 
 load_defaults()
```

### Comparing `datadiligence-0.1.1/src/datadiligence/evaluators/base.py` & `datadiligence-0.1.2/src/datadiligence/evaluators/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,7 +27,11 @@
         Returns:
             bool: True if the content is allowed, False otherwise.
         """
         for rule in self.rules:
             if rule.is_ready() and not rule.is_allowed(**kwargs):
                 return False
         return True
+
+    def filter_allowed(self, **kwargs):
+        """Filter a list of entries based on the rules in this evaluator."""
+        raise NotImplementedError
```

### Comparing `datadiligence-0.1.1/src/datadiligence/evaluators/postprocess.py` & `datadiligence-0.1.2/src/datadiligence/evaluators/postprocess.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/src/datadiligence/exceptions.py` & `datadiligence-0.1.2/src/datadiligence/exceptions.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/src/datadiligence/rules/base.py` & `datadiligence-0.1.2/src/datadiligence/rules/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     def is_ready(self):
         """Check if the rule is ready to be used."""
         raise NotImplementedError
 
 
 class BulkRule(Rule):
     """
-    Base class for bulk rules. get_allowed and is_ready must be implemented.
+    Base class for bulk rules. filter_allowed and is_ready must be implemented.
     """
 
-    def get_allowed(self, **kwargs):
+    def filter_allowed(self, **kwargs):
         """Filter a list of entries based on the rules in this evaluator."""
         raise NotImplementedError
 
 
 class HttpRule(Rule):
     def __init__(self, user_agent=None):
         """Initialize the rule with a user agent.
```

### Comparing `datadiligence-0.1.1/src/datadiligence/rules/http.py` & `datadiligence-0.1.2/src/datadiligence/rules/http.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/src/datadiligence/rules/spawning.py` & `datadiligence-0.1.2/src/datadiligence/rules/spawning.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,21 +67,21 @@
 
         if max_concurrent_requests <= 0 \
                 or max_concurrent_requests > self.MAX_CONCURRENT_REQUESTS \
                 or max_concurrent_requests is None:
             max_concurrent_requests = self.MAX_CONCURRENT_REQUESTS
         self.max_concurrent_requests = max_concurrent_requests
 
-    def get_allowed(self, urls=None, url=None, **kwargs):
+    def filter_allowed(self, urls=None, url=None, **kwargs):
         """Submit a list of URLs to the Spawning AI API.
         Args:
             urls (list): A list of URLs to submit.
             url (str): A single URL to submit.
         Returns:
-            list: A list containing the result dicts of the submission.
+            list: A list containing the allowed urls of the submission.
         """
         if urls is None:
             if url is not None:
                 urls = [url]
             else:
                 raise SpawningNoParam()
 
@@ -93,48 +93,81 @@
             wait(futures)
 
             for future in futures:
                 results.extend([response_url["url"] for response_url in future.result() if not response_url["optOut"]])
 
         return results
 
-    async def get_allowed_async(self, urls=None, url=None, **kwargs):
+    def is_allowed(self, urls=None, url=None, **kwargs):
+        """Submit a list of URLs to the Spawning AI API.
+        Args:
+            urls (list): A list of URLs to submit.
+            url (str): A single URL to submit.
+        Returns:
+            list: A list containing booleans, indicating if a respective URL is allowed.
+        """
+        if urls is None:
+            if url is not None:
+                urls = [url]
+            else:
+                raise SpawningNoParam()
+
+        results = []
+
+        # thread pool executor to submit chunks in parallel
+        with ThreadPoolExecutor(max_workers=self.max_concurrent_requests) as executor:
+            futures = [executor.submit(self._submit_chunk, chunk) for chunk in self._chunk(urls)]
+            wait(futures)
+
+            for future in futures:
+                results.extend([not response_url["optOut"] for response_url in future.result()])
+
+        return results
+
+    async def filter_allowed_async(self, urls=None, url=None, **kwargs):
         """Submit a list of URLs to the Spawning AI API.
 
         Args:
             urls (list): A list of URLs to submit.
             url (str): A single URL to submit.
 
         Returns:
-            list: A list containing the result dicts of the submission.
+            list: A list containing the allowed URLs.
 
         """
         if urls is None:
             if url is not None:
                 urls = [url]
             else:
                 raise SpawningNoParam()
 
         results = await self._submit_chunks_async(urls)
+        results = [response_url["url"] for response_url in results if not response_url["optOut"]]
         return results
 
-    def is_allowed(self, url=None, **kwargs):
-        """
-        Check if a URL is allowed based on the Spawning AI API.
+    async def is_allowed_async(self, urls=None, url=None, **kwargs):
+        """Submit a list of URLs to the Spawning AI API.
 
         Args:
-            url (str): The URL to check.
+            urls (list): A list of URLs to submit.
+            url (str): A single URL to submit.
 
         Returns:
-            bool: True if the URL is allowed, False otherwise.
+            list: A list of boolean values indicating if a URL is allowed to be used or not.
+
         """
-        if url is None:
-            return True
+        if urls is None:
+            if url is not None:
+                urls = [url]
+            else:
+                raise SpawningNoParam()
 
-        return len(self.get_allowed(url=url)) >= 1
+        results = await self._submit_chunks_async(urls)
+        results = [not response_url["optOut"] for response_url in results]
+        return results
 
     def is_ready(self):
         """Check if the Spawning AI API is ready to be used. This is determined by whether or not the API key is set.
         Returns:
             bool: True if the API key is set, False otherwise.
         """
         return bool(self.api_key)
@@ -181,15 +214,15 @@
             else:
                 for chunk in self._chunk(urls):
                     tasks.append(asyncio.create_task(self._submit_chunk_async(session, semaphore, chunk)))
 
             results = await asyncio.gather(*tasks)
 
         # flatten
-        return [response_url["url"] for response_url in itertools.chain(*results) if not response_url["optOut"]]
+        return [response_url for response_url in itertools.chain(*results)]
 
     async def _submit_chunk_async(self, session, semaphore, urls):
         """Submit a chunk of URLs to the Spawning AI API asynchronously.
 
         Args:
             session (aiohttp.ClientSession): The aiohttp session to use.
             urls (list): A list of URLs to submit.
```

### Comparing `datadiligence-0.1.1/src/datadiligence/utils.py` & `datadiligence-0.1.2/src/datadiligence/utils.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/src/datadiligence.egg-info/PKG-INFO` & `datadiligence-0.1.2/src/datadiligence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadiligence
-Version: 0.1.1
+Version: 0.1.2
 Summary: Respect generative AI opt-outs in your ML and training pipeline.
 Home-page: https://github.com/Spawning-Inc/datadiligence/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://datadiligence.readthedocs.io/en/latest/quickstart.html
 Project-URL: Source, https://github.com/Spawning-Inc/datadiligence/
@@ -65,16 +65,19 @@
 
    pip install datadiligence
 
 Add bulk pre-processing for URLs in your pipeline (requires Spawning API Key)::
 
    >>> import datadiligence as dd
    >>> urls = ["https://www.example.com/art-123456789.jpg", "https://www.example.com/art-987654321.jpg"]
+   >>> dd.filter_allowed(urls=urls)
+    ["https://www.example.com/art-123456789.jpg"]
    >>> dd.is_allowed(urls=urls)
-   ["https://www.example.com/art-123456789.jpg"]
+    [True, False]
+
 
 Check HTTP responses in post-processing::
 
    >>> response = requests.get("https://www.example.com/art-123456789.jpg")
    >>> is_allowed = dd.is_allowed(response=response)
    True
    >>> if is_allowed:
```

### Comparing `datadiligence-0.1.1/src/datadiligence.egg-info/SOURCES.txt` & `datadiligence-0.1.2/src/datadiligence.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/python-package.yml
 docs/Makefile
 docs/advanced.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
```

### Comparing `datadiligence-0.1.1/tests/samples/custom.py` & `datadiligence-0.1.2/tests/samples/custom.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/tests/server/app.py` & `datadiligence-0.1.2/tests/server/app.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/tests/test_evaluators.py` & `datadiligence-0.1.2/tests/test_evaluators.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import os
 from samples.custom import CustomEvaluator, NotReadyRule, CustomRule2
 
 # starting local server to echo back headers
 from werkzeug.serving import make_server
 from server.app import app
 import threading
+import datadiligence.exceptions
 
 
 class EvaluatorTests(TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.server = make_server('localhost', 5001, app)
@@ -36,15 +37,15 @@
             self.assertFalse(http_evaluator.is_allowed(response=response))
             self.assertFalse(http_evaluator.is_allowed(headers=response.headers))
 
         response = requests.get("http://localhost:5001/ai")
         self.assertTrue(http_evaluator.is_allowed(response=response))
         self.assertTrue(http_evaluator.is_allowed(headers=response.headers))
 
-        http_evaluator_2 = HttpEvaluator(respect_robots=False, respect_spawning=False)
+        http_evaluator_2 = HttpEvaluator(respect_robots=False)
         self.assertEqual(len(http_evaluator_2.rules), 0)
 
     def test_custom_evaluator(self):
         # custom evaluator
         custom_evaluator = CustomEvaluator()
         custom_rule = CustomRule2()
         not_ready_rule = NotReadyRule()
@@ -67,25 +68,25 @@
         spawning_api = SpawningAPI(user_agent="spawningbot")
         spawning_api.SPAWNING_AI_API_URL = "http://localhost:5001/opts"
 
         self.assertEqual(len(bulk_evaluator.rules), 0)
         bulk_evaluator.add_rule(spawning_api)
         self.assertEqual(len(bulk_evaluator.rules), 1)
 
-        urls = bulk_evaluator.get_allowed([
+        urls = bulk_evaluator.filter_allowed([
             "https://www.spawning.ai",
             "https://www.shutterstock.com",
             "https://open.ai",
             "https://www.google.com",
             "https://laion.ai",
             "https://www.youtube.com",
         ])
         self.assertEqual(len(urls), 3)
 
-        urls = bulk_evaluator.is_allowed(urls=[
+        urls = bulk_evaluator.filter_allowed(urls=[
             "https://www.spawning.ai",
             "https://www.shutterstock.com",
             "https://open.ai",
             "https://www.google.com",
             "https://laion.ai",
             "https://www.youtube.com",
         ])
@@ -94,28 +95,30 @@
         self.assertEqual(len(bulk_evaluator.rules), 1)
         bulk_evaluator.add_rule(None)
         self.assertEqual(len(bulk_evaluator.rules), 1)
 
         bulk_evaluator = PreprocessEvaluator()
         self.assertTrue(len(bulk_evaluator.rules) > 0)
 
-        self.assertEqual(bulk_evaluator.get_allowed([]), [])
-        self.assertEqual(bulk_evaluator.get_allowed(None), [])
+        self.assertEqual(bulk_evaluator.filter_allowed([]), [])
+        self.assertEqual(bulk_evaluator.filter_allowed(None), [])
+
+        self.assertEqual(bulk_evaluator.is_allowed(), [])
 
     def test_bulk_evaluator_ready_state(self):
         b = PreprocessEvaluator()
         b.rules = []
         del os.environ[SpawningAPI.API_KEY_ENV_VAR]
         spawning_rule = SpawningAPI()
 
         self.assertFalse(spawning_rule.is_ready())
 
         b.add_rule(spawning_rule)
 
-        urls = b.get_allowed([
+        urls = b.filter_allowed([
             "https://www.spawning.ai",
             "https://www.shutterstock.com",
             "https://open.ai",
             "https://www.google.com",
             "https://laion.ai",
             "https://www.youtube.com",
         ])
@@ -151,33 +154,58 @@
         evaluator = dd.get_evaluator("preprocess")
         evaluator.rules = []
         evaluator.add_rule(XRobotsTagHeader())
         evaluator.add_rule(spawning_api)
         dd.register_evaluator(evaluator, name="preprocess", overwrite=True)
 
         # urls defaults
-        urls = dd.is_allowed(urls=[
+        urls = dd.filter_allowed(urls=[
             "https://www.spawning.ai",
             "https://www.shutterstock.com",
             "https://open.ai",
             "https://www.google.com",
             "https://laion.ai",
             "https://www.youtube.com",
         ])
         self.assertEqual(len(urls), 3)
 
+        bool_urls = dd.is_allowed(urls=[
+            "https://www.spawning.ai",
+            "https://www.shutterstock.com",
+            "https://open.ai",
+            "https://www.google.com",
+            "https://laion.ai",
+            "https://www.youtube.com",
+        ])
+        self.assertFalse(bool_urls[0])
+        self.assertTrue(bool_urls[1])
+        self.assertTrue(bool_urls[2])
+        self.assertFalse(bool_urls[3])
+        self.assertFalse(bool_urls[4])
+        self.assertTrue(bool_urls[5])
+
         # response and headers defaults
         response = requests.get("http://localhost:5001/noai")
         self.assertFalse(dd.is_allowed(response=response))
         self.assertFalse(dd.is_allowed(headers=response.headers))
 
         response = requests.get("http://localhost:5001/ai")
         self.assertTrue(dd.is_allowed(response=response))
         self.assertTrue(dd.is_allowed(headers=response.headers))
 
+        urls = dd.filter_allowed(name="preprocess", urls=[
+            "https://www.spawning.ai",
+            "https://www.shutterstock.com",
+            "https://open.ai",
+            "https://www.google.com",
+            "https://laion.ai",
+            "https://www.youtube.com",
+        ])
+        self.assertEqual(len(urls), 3)
+
         # reload standard evaluators
         dd.load_defaults()
 
     @classmethod
     def tearDownClass(cls):
         cls.server.shutdown()
         cls.server_thread.join()
```

### Comparing `datadiligence-0.1.1/tests/test_xrobotsheader.py` & `datadiligence-0.1.2/tests/test_xrobotsheader.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.1/tox.ini` & `datadiligence-0.1.2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tox configuration file
 # Read more under https://tox.wiki/
 
 [tox]
 minversion = 3.24
-envlist = py36,py37,py38,py39,py310,py311
+envlist = py37,py38,py39,py310,py311
 isolated_build = True
 
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
```

