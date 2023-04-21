# Comparing `tmp/citecheck-0.1.2.tar.gz` & `tmp/citecheck-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citecheck-0.1.2.tar", last modified: Wed Mar 29 13:33:47 2023, max compression
+gzip compressed data, was "citecheck-0.2.0.tar", last modified: Fri Apr 21 10:30:43 2023, max compression
```

## Comparing `citecheck-0.1.2.tar` & `citecheck-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.544994 citecheck-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-29 13:33:25.000000 citecheck-0.1.2/.env.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.536994 citecheck-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-29 13:33:25.000000 citecheck-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.536994 citecheck-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-29 13:33:25.000000 citecheck-0.1.2/.github/workflows/build_lint_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-29 13:33:25.000000 citecheck-0.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-29 13:33:25.000000 citecheck-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-29 13:33:25.000000 citecheck-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 13:33:25.000000 citecheck-0.1.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-29 13:33:25.000000 citecheck-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-29 13:33:25.000000 citecheck-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-29 13:33:47.544994 citecheck-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-29 13:33:25.000000 citecheck-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.536994 citecheck-0.1.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.536994 citecheck-0.1.2/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/doc/source/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/source/whatsnew/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-29 13:33:25.000000 citecheck-0.1.2/doc/source/whatsnew/releasenotes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-29 13:33:25.000000 citecheck-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-29 13:33:25.000000 citecheck-0.1.2/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-03-29 13:33:25.000000 citecheck-0.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-29 13:33:25.000000 citecheck-0.1.2/scripts/compile-requirements.sh
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-29 13:33:25.000000 citecheck-0.1.2/scripts/dev-setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:33:47.544994 citecheck-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.536994 citecheck-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/src/citecheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/src/citecheck/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/check_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/citeas.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/cited.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/src/citecheck/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/types/citand.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-29 13:33:25.000000 citecheck-0.1.2/src/citecheck/core/types/citation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/src/citecheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 13:33:47.000000 citecheck-0.1.2/src/citecheck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.540994 citecheck-0.1.2/tests/citecheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:47.544994 citecheck-0.1.2/tests/citecheck/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/core/test_check_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/core/test_citeas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/core/test_cited.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-29 13:33:25.000000 citecheck-0.1.2/tests/citecheck/core/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 10:30:20.000000 citecheck-0.2.0/.env.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/workflows/build_lint_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-21 10:30:20.000000 citecheck-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 10:30:20.000000 citecheck-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:30:20.000000 citecheck-0.2.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-21 10:30:20.000000 citecheck-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-21 10:30:20.000000 citecheck-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 10:30:43.275886 citecheck-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-21 10:30:20.000000 citecheck-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.267886 citecheck-0.2.0/doc/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/full_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/full_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/whatsnew/releasenotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-21 10:30:20.000000 citecheck-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 10:30:20.000000 citecheck-0.2.0/scripts/compile-requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-21 10:30:20.000000 citecheck-0.2.0/scripts/dev-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:30:43.275886 citecheck-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.267886 citecheck-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/src/citecheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/cite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/citeas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/cited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/citedmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/citable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/decorate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/decorate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/decorate/check_citations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/test_citeas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/decorate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/decorate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/decorate/test_check_citations.py
```

### Comparing `citecheck-0.1.2/.github/workflows/pypi-publish.yml` & `citecheck-0.2.0/.github/workflows/pypi-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       uses: actions/setup-python@v2
       with:
         python-version: '3.8'
 
     - name: Install dependencies
       run: |
         pip install --upgrade pip
-        pip install -r requirements-ci.txt
+        pip install -r requirements/ci-requirements.txt
         pip install build twine
 
     - name: Build and publish
       env:
         TWINE_USERNAME: __token__
         TWINE_PASSWORD: ${{secrets.PYPI_TOKEN}}
       run: |
```

### Comparing `citecheck-0.1.2/.gitignore` & `citecheck-0.2.0/.gitignore`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# Profiling output
-*.prof
-
-# Black formatter temp files
-*.py.*.tmp
-
-# Draw.io temp files
-~drawio~*~*.drawio.tmp
-
-# VS Code config
-.vscode/
-
-# Windows thumbnail cache files
-Thumbs.db
-
-# Project Configuration file
-.config.yaml
-
-# Cached datasets
-.datasetcache
-
-# Microsoft Office lock files
-~$*.xlsx
-
-# Automatically generated setuptools_scm version file
-src/**/_version.py
-
-# Automatically generated Sphinx API documentation
-doc/source/_apidoc/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# Profiling output
+*.prof
+
+# Black formatter temp files
+*.py.*.tmp
+
+# Draw.io temp files
+~drawio~*~*.drawio.tmp
+
+# VS Code config
+.vscode/
+
+# Windows thumbnail cache files
+Thumbs.db
+
+# Project Configuration file
+.config.yaml
+
+# Cached datasets
+.datasetcache
+
+# Microsoft Office lock files
+~$*.xlsx
+
+# Automatically generated setuptools_scm version file
+src/**/_version.py
+
+# Automatically generated Sphinx API documentation
+doc/source/_apidoc/
```

### Comparing `citecheck-0.1.2/.pre-commit-config.yaml` & `citecheck-0.2.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,71 @@
-default_stages:
-  [
-    commit,
-    merge-commit,
-    push,
-    prepare-commit-msg,
-    commit-msg,
-    post-checkout,
-    post-commit,
-    post-merge,
-    post-rewrite,
-    manual,
-  ]
-ci:
-  autofix_prs: false
-repos:
-  - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
-    hooks:
-      - id: validate-pyproject
-
-  - repo: https://github.com/MarcoGorelli/absolufy-imports
-    rev: v0.3.1
-    hooks:
-      - id: absolufy-imports
-        files: ^src/
-
-  - repo: https://github.com/python/black
-    rev: 23.1.0
-    hooks:
-      - id: black
-
-  - repo: https://github.com/lk16/detect-missing-init
-    rev: v0.1.6
-    hooks:
-      - id: detect-missing-init
-        args: ["--create", "--python-folders", "src/citecheck,tests"]
-
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
-    hooks:
-      - id: debug-statements
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.259"
-    hooks:
-      - id: ruff
-
-  - repo: https://github.com/pycqa/pylint
-    rev: v2.17.0
-    hooks:
-      - id: pylint
-        args: ["--disable", "fixme"]
-
-  - repo: local
-    hooks:
-      - id: setuptools_scm
-        name: setuptools_scm
-        entry: python -m setuptools_scm -c
-        additional_dependencies: [setuptools_scm]
-        language: python
-        files: ^pyproject.toml$
+default_stages:
+  [
+    commit,
+    merge-commit,
+    push,
+    prepare-commit-msg,
+    commit-msg,
+    post-checkout,
+    post-commit,
+    post-merge,
+    post-rewrite,
+    manual,
+  ]
+ci:
+  autofix_prs: false
+repos:
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.12.2
+    hooks:
+      - id: validate-pyproject
+
+  - repo: https://github.com/MarcoGorelli/absolufy-imports
+    rev: v0.3.1
+    hooks:
+      - id: absolufy-imports
+        files: ^src/
+
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+
+  - repo: https://github.com/lk16/detect-missing-init
+    rev: v0.1.6
+    hooks:
+      - id: detect-missing-init
+        args: ["--create", "--python-folders", "src/citecheck,tests"]
+
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: debug-statements
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.262
+    hooks:
+      - id: ruff
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.2.0
+    hooks:
+    -   id: mypy
+        args: ["."]
+        pass_filenames: false
+
+  - repo: https://github.com/pycqa/pylint
+    rev: v3.0.0a6
+    hooks:
+      - id: pylint
+        args: ["--disable", "fixme"]
+
+  - repo: local
+    hooks:
+      - id: setuptools_scm
+        name: setuptools_scm
+        entry: python -m setuptools_scm -c
+        additional_dependencies: [setuptools_scm]
+        language: python
+        files: ^pyproject.toml$
```

### Comparing `citecheck-0.1.2/LICENSE.txt` & `citecheck-0.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Nathan McDougall
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Nathan McDougall
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `citecheck-0.1.2/PKG-INFO` & `citecheck-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-Metadata-Version: 2.1
-Name: citecheck
-Version: 0.1.2
-Summary: Run-time protection of citation chains
-Author-email: Nathan McDougall <nathan.j.mcdougall@gmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, Nathan McDougall
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: dev
-Provides-Extra: check
-Provides-Extra: test
-Provides-Extra: notebook
-License-File: LICENSE.txt
+<div align="center">
+  <img src="doc/source/_static/logo/full_dark.svg#gh-dark-mode-only"><br>
+  <img src="doc/source/_static/logo/full_light.svg#gh-light-mode-only"><br>
+</div>
 
-# citecheck
+# citecheck: like typechecks, but for citations 📖⛓️
 
 <!-- badges: start -->
-![Python Version](https://img.shields.io/badge/python-3.10.8-green)
 [![License](https://img.shields.io/github/license/nathanjmcdougall/citecheck)](https://github.com/nathanjmcdougall/citecheck/blob/main/LICENSE.txt)
+[![PyPI version](https://badge.fury.io/py/citecheck.svg)](https://badge.fury.io/py/citecheck)
 [![Documentation Status](https://readthedocs.org/projects/citecheck/badge/?version=latest)](https://citecheck.readthedocs.io/en/latest/?badge=latest)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Linting: Ruff](https://img.shields.io/badge/linting-ruff-yellowgreen)](https://github.com/charliermarsh/ruff)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nathanjmcdougall/citecheck/main.svg)](https://results.pre-commit.ci/latest/github/nathanjmcdougall/citecheck/main)
+[![codecov](https://codecov.io/gh/nathanjmcdougall/citecheck/branch/develop/graph/badge.svg?token=OUHWT2NL8O)](https://codecov.io/gh/nathanjmcdougall/citecheck)
+<!-- [![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck) -->
 <!-- badges: end -->
 
-Run-time protection of citation chains in Python
+## Quick example
+Consider this example (all authors and quantities are fictitious):
+
+- Doe (2021) published a method for estimating $V_t$ as a function of $q_p$ and $t$.
+- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and $\rho$, with the explicit requirement that $V_t$ be estimated using the method of Doe (2021) in particular.
+
+The goal for citecheck is that you could implement this as follows:
+```Python
+@enforcecite
+def calc_vt_doe2021(
+  qt: float,
+  t: float
+) -> Annotated[float, Cite("doe2021")]:
+    ...
+
+@enforcecite
+def calc_rm_bloggs2023(
+  vt: CiteAs[float, "doe2021"],
+  rho: float
+) -> Annotated[float, Cite("bloggs2023")]:
+    ...
+```
+
+Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe (2021), we would get an error:
+
+```Python
+calc_rm_bloggs2023(vt=1.0, rho=1.0) # Error
+calc_rm_bloggs2023(vt=calc_vt_doe2021(1.0, 1.0), rho=1.0) # OK
+```
+
+citecheck is still in development, but this is the general idea.
+
+## When to use citecheck
+
+You should consider using citecheck when you are implementing functions corresponding to equations or methodologies in multiple papers which refer to one another.
 
 ## Getting Started with Development
 
+Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup script:
+
 ```bash
 source .\scripts\dev-setup.sh
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `citecheck-0.1.2/doc/Makefile` & `citecheck-0.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `citecheck-0.1.2/doc/source/conf.py` & `citecheck-0.2.0/doc/source/conf.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""Configuration file for the Sphinx documentation builder."""
-
-from pathlib import Path
-
-import tomli
-
-# Sphinx expects some non-pylint compliant names
-# pylint: disable=invalid-name
-ROOT_PATH = Path(__file__).parent.parent.parent
-
-with open(ROOT_PATH / "pyproject.toml", mode="rb") as f:
-    _pyproject = tomli.load(f)
-
-_project = _pyproject["project"]
-_name = _project["name"]
-_authors = _project["authors"]
-_first_author = _authors[0]["name"]
-_description = _project["description"]
-language = "en"
-source_suffix = [".rst"]
-source_encoding = "utf-8"
-
-
-extensions = [
-    "sphinx_copybutton",
-    "sphinx_design",
-    "sphinx_toggleprompt",
-    "sphinx_favicon",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.coverage",
-    "sphinx.ext.doctest",
-    "sphinx.ext.extlinks",
-    "sphinx.ext.ifconfig",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.linkcode",
-    "sphinx.ext.mathjax",
-    "sphinx.ext.todo",
-]
-
-name = _name
-author = _first_author
-description = _description
-
-templates_path = ["_templates"]
-exclude_patterns = []
-
-intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
-
-napoleon_google_docstring = True
-
-html_theme = "pydata_sphinx_theme"
-html_static_path = ["_static"]
-html_theme_options = {
-    "github_url": "https://github.com/nathanjmcdougall/citecheck",
-    "pygment_light_style": "tango",
-    "pygment_dark_style": "monokai",
-    "logo": {
-        "image_light": "logo-light.png",
-        "image_dark": "logo-dark.png",
-        "alt_text": "Documentation - Index",
-    },
-}
-favicons = [{"href": "favicon.ico"}]
-
-
-def linkcode_resolve(domain, info):
-    """Determine the URL corresponding to Python object."""
-    if domain != "py":
-        return None
-    if not info["module"]:
-        return None
-    filename = info["module"].replace(".", "/")
-    return f"https://github.com/nathanjmcdougall/citecheck/{filename}.py"
+"""Configuration file for the Sphinx documentation builder."""
+
+from pathlib import Path
+
+import tomli
+
+# Sphinx expects some non-pylint compliant names
+# pylint: disable=invalid-name
+ROOT_PATH = Path(__file__).parent.parent.parent
+
+with open(ROOT_PATH / "pyproject.toml", mode="rb") as f:
+    _pyproject = tomli.load(f)
+
+_project = _pyproject["project"]
+_name = _project["name"]
+_authors = _project["authors"]
+_first_author = _authors[0]["name"]
+_description = _project["description"]
+language = "en"
+source_suffix = [".rst"]
+source_encoding = "utf-8"
+
+
+extensions = [
+    "sphinx_copybutton",
+    "sphinx_design",
+    "sphinx_toggleprompt",
+    "sphinx_favicon",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.linkcode",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.todo",
+]
+
+name = _name
+author = _first_author
+description = _description
+
+templates_path = ["_templates"]
+exclude_patterns = []
+
+intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
+
+napoleon_google_docstring = True
+
+html_theme = "pydata_sphinx_theme"
+html_static_path = ["_static"]
+html_theme_options = {
+    "github_url": "https://github.com/nathanjmcdougall/citecheck",
+    "pygment_light_style": "tango",
+    "pygment_dark_style": "monokai",
+    "logo": {
+        "image_light": "logo-light.png",
+        "image_dark": "logo-dark.png",
+        "alt_text": "Documentation - Index",
+    },
+}
+favicons = [{"href": "favicon.ico"}]
+
+
+def linkcode_resolve(domain, info):
+    """Determine the URL corresponding to Python object."""
+    if domain != "py":
+        return None
+    if not info["module"]:
+        return None
+    filename = info["module"].replace(".", "/")
+    return f"https://github.com/nathanjmcdougall/citecheck/{filename}.py"
```

### Comparing `citecheck-0.1.2/requirements-ci.txt` & `citecheck-0.2.0/requirements/ci-requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-#
-# This file is autogenerated by pip-compile with Python 3.10
-# by the following command:
-#
-#    pip-compile --extra=check --extra=test --output-file=requirements-ci.txt --resolver=backtracking pyproject.toml
-#
-attrs==22.2.0
-    # via pytest
-cfgv==3.3.1
-    # via pre-commit
-coverage[toml]==7.2.2
-    # via
-    #   citecheck (pyproject.toml)
-    #   pytest-cov
-distlib==0.3.6
-    # via virtualenv
-exceptiongroup==1.1.1
-    # via pytest
-filelock==3.10.7
-    # via virtualenv
-identify==2.5.22
-    # via pre-commit
-iniconfig==2.0.0
-    # via pytest
-nodeenv==1.7.0
-    # via pre-commit
-packaging==23.0
-    # via pytest
-platformdirs==3.2.0
-    # via virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==3.2.1
-    # via citecheck (pyproject.toml)
-pytest==7.2.2
-    # via
-    #   citecheck (pyproject.toml)
-    #   pytest-cov
-pytest-cov==4.0.0
-    # via citecheck (pyproject.toml)
-pyyaml==6.0
-    # via pre-commit
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-virtualenv==20.21.0
-    # via pre-commit
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --extra=check --extra=test --output-file=requirements/ci-requirements.txt --resolver=backtracking pyproject.toml
+#
+attrs==22.2.0
+    # via pytest
+cfgv==3.3.1
+    # via pre-commit
+coverage[toml]==7.2.2
+    # via
+    #   citecheck (pyproject.toml)
+    #   pytest-cov
+distlib==0.3.6
+    # via virtualenv
+exceptiongroup==1.1.1
+    # via pytest
+filelock==3.10.7
+    # via virtualenv
+identify==2.5.22
+    # via pre-commit
+iniconfig==2.0.0
+    # via pytest
+mypy==1.2.0
+    # via citecheck (pyproject.toml)
+mypy-extensions==1.0.0
+    # via mypy
+nodeenv==1.7.0
+    # via pre-commit
+packaging==23.0
+    # via pytest
+platformdirs==3.2.0
+    # via virtualenv
+pluggy==1.0.0
+    # via pytest
+pre-commit==3.2.1
+    # via citecheck (pyproject.toml)
+pytest==7.2.2
+    # via
+    #   citecheck (pyproject.toml)
+    #   pytest-cov
+pytest-cov==4.0.0
+    # via citecheck (pyproject.toml)
+pyyaml==6.0
+    # via pre-commit
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
+typing-extensions==4.5.0
+    # via mypy
+virtualenv==20.21.0
+    # via pre-commit
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `citecheck-0.1.2/src/citecheck/core/check_citations.py` & `citecheck-0.2.0/src/citecheck/decorate/check_citations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,85 @@
 """A decorator to check citations of Cited objects in function annotations."""
 import inspect
-from typing import Any, Callable, TypeVar
+from typing import Annotated, Any, Callable, get_args, get_origin
 
-from citecheck.core.citeas import _BaseCiteAs
-from citecheck.core.cited import _BaseCited
+from citecheck.core.cite import Cite
+from citecheck.core.citedmixin import _CitedMixin
 from citecheck.core.errors import CitationError, CitationWarning
+from citecheck.core.types.citation import Citation, _CitationT
 
-C = TypeVar("C", bound=Any)
 
-
-def _eq_compare(citation1: C, citation2: C) -> bool:
+def _eq_compare(citation1: _CitationT, citation2: _CitationT) -> bool:
     return citation1 == citation2
 
 
+def _get_compare_func(
+    compare_func: Callable[[Citation, Citation], bool] | None
+) -> Callable[[Citation, Citation], bool]:
+    if compare_func is None:
+        return _eq_compare
+    return compare_func
+
+
 def check_citations(
-    warn: bool = False, compare_func: Callable[[C, C], bool] | None = None
-):
+    warn: bool = False,
+    compare_func: Callable[[Citation, Citation], bool] | None = None,
+) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
     """A decorator to check citations of Cited objects in function annotations."""
 
-    if compare_func is None:
-        compare_func = _eq_compare
+    _compare_func = _get_compare_func(compare_func)
 
     raiser = CitationWarning if warn else CitationError
 
-    def decorator(func):
+    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
         # Get the function signature
         sig = inspect.signature(func)
 
         # Get the function annotations
         anns = func.__annotations__
 
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             # Get the function arguments
             bound_args = sig.bind(*args, **kwargs)
 
             # Iterate over the function arguments
             for arg_name, arg_value in bound_args.arguments.items():
                 # Check if the argument is cited
-                if isinstance(arg_value, _BaseCited):
+                if isinstance(arg_value, _CitedMixin):
                     # Check if the argument is annotated
                     if arg_name in anns:
                         ann = anns[arg_name]
 
-                        # Check if the annotation is a Cited object
-                        if isinstance(ann, _BaseCiteAs):
-                            # Check if the annotation matches the citation of the
-                            # argument
-                            # pylint: disable=protected-access
-                            if not compare_func(ann._citation, arg_value._citation):
+                        # Check if the annotation is typing.Annotated
+                        if get_origin(ann) is Annotated:
+                            # Get the annotation arguments which are Cite type
+                            ann_args = [
+                                arg for arg in get_args(ann) if isinstance(arg, Cite)
+                            ]
+
+                            # Iterate over the annotation arguments
+                            any_match = False
+                            for ann_arg in ann_args:
+                                # pylint: disable=protected-access
+                                citation = arg_value._citation
+                                # pylint: enable=protected-access
+
+                                match = _compare_func(citation, ann_arg.citation)
+                                any_match = any_match or match
+
+                            # Check if the citation matches
+                            if not any_match:
+                                annotated_citations = [arg.citation for arg in ann_args]
                                 raise raiser(
-                                    f"Function {func.__name__} was called with an "
-                                    f"argument {arg_name} which has a "
-                                    f"citation {arg_value._citation} which does not "
-                                    f"match the annotation {ann._citation}"
+                                    f"Function {func.__name__} was called with "
+                                    f"an argument {arg_name} which has a "
+                                    f"citation {citation} which "
+                                    f"does not match any of the annotated citations "
+                                    f"{annotated_citations}"
                                 )
-                            # pylint: enable=protected-access
 
             # Call the function
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `citecheck-0.1.2/src/citecheck.egg-info/SOURCES.txt` & `citecheck-0.2.0/src/citecheck.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,43 +2,49 @@
 .gitignore
 .pre-commit-config.yaml
 .python-version
 .readthedocs.yaml
 LICENSE.txt
 README.md
 pyproject.toml
-requirements-ci.txt
-requirements.txt
+requirements.in
 .github/dependabot.yml
 .github/workflows/build_lint_test.yml
 .github/workflows/pypi-publish.yml
 doc/Makefile
 doc/make.bat
 doc/source/conf.py
 doc/source/index.rst
-doc/source/_static/.gitkeep
+doc/source/_static/logo/full_dark.svg
+doc/source/_static/logo/full_light.svg
+doc/source/_static/logo/icon_light.svg
 doc/source/whatsnew/index.rst
 doc/source/whatsnew/releasenotes.rst
+requirements/ci-requirements.txt
+requirements/requirements.txt
 scripts/compile-requirements.sh
 scripts/dev-setup.sh
 src/citecheck/__init__.py
 src/citecheck/_version.py
 src/citecheck.egg-info/PKG-INFO
 src/citecheck.egg-info/SOURCES.txt
 src/citecheck.egg-info/dependency_links.txt
 src/citecheck.egg-info/requires.txt
 src/citecheck.egg-info/top_level.txt
 src/citecheck/core/__init__.py
-src/citecheck/core/check_citations.py
+src/citecheck/core/cite.py
 src/citecheck/core/citeas.py
 src/citecheck/core/cited.py
+src/citecheck/core/citedmixin.py
 src/citecheck/core/errors.py
 src/citecheck/core/types/__init__.py
-src/citecheck/core/types/citand.py
+src/citecheck/core/types/citable.py
 src/citecheck/core/types/citation.py
+src/citecheck/decorate/__init__.py
+src/citecheck/decorate/check_citations.py
 tests/__init__.py
 tests/citecheck/__init__.py
 tests/citecheck/core/__init__.py
-tests/citecheck/core/test_check_citations.py
 tests/citecheck/core/test_citeas.py
-tests/citecheck/core/test_cited.py
-tests/citecheck/core/test_errors.py
+tests/citecheck/core/test_errors.py
+tests/citecheck/decorate/__init__.py
+tests/citecheck/decorate/test_check_citations.py
```

### Comparing `citecheck-0.1.2/tests/citecheck/core/test_errors.py` & `citecheck-0.2.0/tests/citecheck/core/test_errors.py`

 * *Files identical despite different names*

