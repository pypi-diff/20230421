# Comparing `tmp/dkist_data_simulator-3.1.4.tar.gz` & `tmp/dkist_data_simulator-3.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_data_simulator-3.1.4.tar", last modified: Mon Apr 10 19:27:20 2023, max compression
+gzip compressed data, was "dkist_data_simulator-3.1.5rc1.tar", last modified: Fri Apr 21 17:38:55 2023, max compression
```

## Comparing `dkist_data_simulator-3.1.4.tar` & `dkist_data_simulator-3.1.5rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     3308 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    16806 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/dataset.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/vtf_crisp_5d.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10932 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7180 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec122.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26874 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/core.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/cryo.py
--rw-rw-rw-   0 root         (0) root         (0)     3446 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/dlnirsp.py
--rw-rw-rw-   0 root         (0) root         (0)     7627 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vbi.py
--rw-rw-rw-   0 root         (0) root         (0)     6602 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/visp.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vtf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     8380 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/util.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/examples/
--rwxrwxrwx   0 root         (0) root         (0)      908 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/examples/vtf_crisp_5d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2656 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      607 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.827862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/data/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/data/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16806 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/dataset.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/examples/vtf_crisp_5d.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10932 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7180 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec122.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26874 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    11479 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/cryo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3446 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/dlnirsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7627 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/vbi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6602 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/visp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/vtf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     8380 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_214_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-21 17:38:55.000000 dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/examples/
+-rwxrwxrwx   0 root         (0) root         (0)      908 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/examples/vtf_crisp_5d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 17:38:55.831862 dkist_data_simulator-3.1.5rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2023-04-21 17:38:55.835862 dkist_data_simulator-3.1.5rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      607 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-04-21 17:38:31.000000 dkist_data_simulator-3.1.5rc1/tox.ini
```

### Comparing `dkist_data_simulator-3.1.4/.gitignore` & `dkist_data_simulator-3.1.5rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/.pre-commit-config.yaml` & `dkist_data_simulator-3.1.5rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/PKG-INFO` & `dkist_data_simulator-3.1.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 3.1.4
+Version: 3.1.5rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.4/README.rst` & `dkist_data_simulator-3.1.5rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/bitbucket-pipelines.yml` & `dkist_data_simulator-3.1.5rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/dataset.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/expansions.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/schemas.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/schemas.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec122.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/core.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/core.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/cryo.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/cryo.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,19 +209,18 @@
         w.wcs.crval = self.linewave.to_value(u.nm), 0, 0
         w.wcs.cdelt = (
             self.spectral_scale.to_value(u.nm / u.pix),
             self.plate_scale.to_value(u.arcsec / u.pix),
             self.slit_width.to_value(u.arcsec),
         )
         w.wcs.cunit = "nm", "arcsec", "arcsec"
-        w.wcs.ctype = "WAVE", "HPLT-TAN", "HPLN-TAN"
+        w.wcs.ctype = "AWAV", "HPLT-TAN", "HPLN-TAN"
         w.wcs.pc = np.identity(self.array_ndim)
         return w
 
-
 class SimpleCryoCIDataset(BaseCryoCIDataset):
     """
     A five dimensional Cryo cube with regular raster spacing.
     """
 
     name = "cryo-ci-simple"
```

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/dlnirsp.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/dlnirsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,10 +106,10 @@
             self.array_shape[2] / 2,
             self.array_shape[1] / 2,
             self.array_shape[0] / 2,
         )
         w.wcs.crval = 0, 0, 0
         w.wcs.cdelt = [self.plate_scale[i].value for i in range(self.array_ndim)]
         w.wcs.cunit = "arcsec", "arcsec", "nm"
-        w.wcs.ctype = "HPLN-TAN", "HPLT-TAN", "WAVE"
+        w.wcs.ctype = "HPLN-TAN", "HPLT-TAN", "AWAV"
         w.wcs.pc = np.identity(self.array_ndim)
         return w
```

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vbi.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/vbi.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/visp.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/visp.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         w.wcs.crval = 0, self.linewave.to_value(u.nm), 0
         w.wcs.cdelt = (
             self.plate_scale.to_value(u.arcsec / u.pix),
             self.spectral_scale.to_value(u.nm / u.pix),
             self.slit_width.to_value(u.arcsec),
         )
         w.wcs.cunit = "arcsec", "nm", "arcsec"
-        w.wcs.ctype = "HPLT-TAN", "WAVE", "HPLN-TAN"
+        w.wcs.ctype = "HPLT-TAN", "AWAV", "HPLN-TAN"
         w.wcs.pc = np.identity(self.array_ndim)
         return w
 
 
 class TimeDependentVISPDataset(SimpleVISPDataset):
     """
     A version of the ViSP dataset where the CRVAL and PC matrix change with time.
```

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vtf.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/spec214/vtf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/conftest.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_122.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214_inventory.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_214_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_dataset.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator/util.py` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator/util.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/PKG-INFO` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-data-simulator
-Version: 3.1.4
+Version: 3.1.5rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/SOURCES.txt` & `dkist_data_simulator-3.1.5rc1/dkist_data_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/docs/Makefile` & `dkist_data_simulator-3.1.5rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/docs/conf.py` & `dkist_data_simulator-3.1.5rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/docs/make.bat` & `dkist_data_simulator-3.1.5rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.1.5rc1/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/licenses/LICENSE.rst` & `dkist_data_simulator-3.1.5rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/licenses/TEMPLATE_LICENSE.rst` & `dkist_data_simulator-3.1.5rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/setup.cfg` & `dkist_data_simulator-3.1.5rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/setup.py` & `dkist_data_simulator-3.1.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.4/tox.ini` & `dkist_data_simulator-3.1.5rc1/tox.ini`

 * *Files identical despite different names*

