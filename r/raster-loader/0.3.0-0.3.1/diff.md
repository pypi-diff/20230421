# Comparing `tmp/raster-loader-0.3.0.tar.gz` & `tmp/raster-loader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-loader-0.3.0.tar", last modified: Tue Mar  7 13:48:22 2023, max compression
+gzip compressed data, was "raster-loader-0.3.1.tar", last modified: Fri Apr 21 10:43:06 2023, max compression
```

## Comparing `raster-loader-0.3.0.tar` & `raster-loader-0.3.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.119041 raster-loader-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.103041 raster-loader-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.103041 raster-loader-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1577 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3201 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-07 13:48:00.000000 raster-loader-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-03-07 13:48:00.000000 raster-loader-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     7999 2023-03-07 13:48:00.000000 raster-loader-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-03-07 13:48:00.000000 raster-loader-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-03-07 13:48:00.000000 raster-loader-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     6123 2023-03-07 13:48:22.119041 raster-loader-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5246 2023-03-07 13:48:00.000000 raster-loader-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-03-07 13:48:00.000000 raster-loader-0.3.0/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-03-07 13:48:00.000000 raster-loader-0.3.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.099041 raster-loader-0.3.0/docker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docker/raster_loader/
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docker/raster_loader/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/.pages
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/_static/carto-logo.png
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/developer_guide/contribute.md
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/developer_guide/roadmap.md
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/source/user_guide/
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/user_guide/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.107041 raster-loader-0.3.0/docs/source/user_guide/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/user_guide/modules/raster_loader.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-03-07 13:48:00.000000 raster-loader-0.3.0/docs/source/user_guide/use_with_python.rst
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-07 13:48:00.000000 raster-loader-0.3.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.111041 raster-loader-0.3.0/raster_loader/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.111041 raster-loader-0.3.0/raster_loader/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/cli/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/cli/info.py
--rw-r--r--   0 runner    (1001) docker     (122)    45068 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.111041 raster-loader-0.3.0/raster_loader/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/.env.sample
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.115041 raster-loader-0.3.0/raster_loader/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)   729781 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/fixtures/mosaic.tif
--rw-r--r--   0 runner    (1001) docker     (122)   729822 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/fixtures/mosaic_wm.tif
--rw-r--r--   0 runner    (1001) docker     (122)  1265082 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/fixtures/quadbin_raster.tif
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    15556 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-03-07 13:48:00.000000 raster-loader-0.3.0/raster_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 13:48:22.111041 raster-loader-0.3.0/raster_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6123 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-07 13:48:22.000000 raster-loader-0.3.0/raster_loader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-03-07 13:48:00.000000 raster-loader-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-03-07 13:48:00.000000 raster-loader-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-03-07 13:48:22.119041 raster-loader-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-07 13:48:00.000000 raster-loader-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:06.012883 raster-loader-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.980883 raster-loader-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.980883 raster-loader-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.980883 raster-loader-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1577 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3201 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-21 10:42:48.000000 raster-loader-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-04-21 10:42:48.000000 raster-loader-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7999 2023-04-21 10:42:48.000000 raster-loader-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-04-21 10:42:48.000000 raster-loader-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-21 10:42:48.000000 raster-loader-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     6123 2023-04-21 10:43:06.012883 raster-loader-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5246 2023-04-21 10:42:48.000000 raster-loader-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-04-21 10:42:48.000000 raster-loader-0.3.1/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-04-21 10:42:48.000000 raster-loader-0.3.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.976883 raster-loader-0.3.1/docker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.980883 raster-loader-0.3.1/docker/raster_loader/
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docker/raster_loader/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/.pages
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/_static/carto-logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/developer_guide/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/developer_guide/roadmap.md
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/source/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/user_guide/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/docs/source/user_guide/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/user_guide/modules/raster_loader.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-04-21 10:42:48.000000 raster-loader-0.3.1/docs/source/user_guide/use_with_python.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-21 10:42:48.000000 raster-loader-0.3.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.984883 raster-loader-0.3.1/raster_loader/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.988883 raster-loader-0.3.1/raster_loader/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/cli/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45659 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.988883 raster-loader-0.3.1/raster_loader/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/.env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:06.012883 raster-loader-0.3.1/raster_loader/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122) 13073267 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/fixtures/fuji.tif
+-rw-r--r--   0 runner    (1001) docker     (122)   729781 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/fixtures/mosaic.tif
+-rw-r--r--   0 runner    (1001) docker     (122)   729822 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/fixtures/mosaic_wm.tif
+-rw-r--r--   0 runner    (1001) docker     (122)  1265082 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/fixtures/quadbin_raster.tif
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16722 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-21 10:42:48.000000 raster-loader-0.3.1/raster_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 10:43:05.988883 raster-loader-0.3.1/raster_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6123 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-21 10:43:05.000000 raster-loader-0.3.1/raster_loader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-04-21 10:42:48.000000 raster-loader-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-04-21 10:42:48.000000 raster-loader-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-04-21 10:43:06.016883 raster-loader-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-21 10:42:48.000000 raster-loader-0.3.1/setup.py
```

### Comparing `raster-loader-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `raster-loader-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `raster-loader-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.github/pull_request_template.md` & `raster-loader-0.3.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.github/workflows/ci.yml` & `raster-loader-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.github/workflows/pypi-publish.yml` & `raster-loader-0.3.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.gitignore` & `raster-loader-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/.readthedocs.yml` & `raster-loader-0.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/CHANGELOG.md` & `raster-loader-0.3.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.1] - 2023-04-21
+
+### Enhancements
+- Store raster nodata value in table metadata (#111)
+- Add level to raster metadata (#110)
+
+### Bug Fixes
+- Fixed issue in metadata when updating table (#112)
+
 ## [0.3.0] - 2023-03-07
 
 ### Enhancements
 - Create raster tables with geography and metadata (#105)
 
 ### Bug Fixes
 - Fixed band in field name (#102)
```

### Comparing `raster-loader-0.3.0/CONTRIBUTING.md` & `raster-loader-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/LICENSE` & `raster-loader-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/Makefile` & `raster-loader-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/PKG-INFO` & `raster-loader-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-loader
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for loading GIS raster data to standard cloud-based data warehouses that don't natively support raster data.
 Home-page: https://github.com/cartodb/raster-loader
 Author: CARTO
 License: BSD 3-Clause
 Keywords: carto,raster,gis,data warehouse,bigquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `raster-loader-0.3.0/README.md` & `raster-loader-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/ROADMAP.md` & `raster-loader-0.3.1/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/conftest.py` & `raster-loader-0.3.1/conftest.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docker/raster_loader/Dockerfile` & `raster-loader-0.3.1/docker/raster_loader/Dockerfile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/Makefile` & `raster-loader-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/make.bat` & `raster-loader-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/_static/carto-logo.png` & `raster-loader-0.3.1/docs/source/_static/carto-logo.png`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/conf.py` & `raster-loader-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/index.rst` & `raster-loader-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/user_guide/cli.rst` & `raster-loader-0.3.1/docs/source/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/user_guide/installation.rst` & `raster-loader-0.3.1/docs/source/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/docs/source/user_guide/use_with_python.rst` & `raster-loader-0.3.1/docs/source/user_guide/use_with_python.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/cli/bigquery.py` & `raster-loader-0.3.1/raster_loader/cli/bigquery.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/cli/info.py` & `raster-loader-0.3.1/raster_loader/cli/info.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/io.py` & `raster-loader-0.3.1/raster_loader/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,15 @@
 
 def band_field_name(band: int, band_type: str, base_name: str = "band") -> str:
     return "_".join([base_name, str(band), band_type])
 
 
 def array_to_record(
     arr: np.ndarray,
+    nodata: float,
     band: int,
     value_field: str,
     dtype_str: str,
     transformer: pyproj.Transformer,
     geotransform: Affine,
     row_off: int = 0,
     col_off: int = 0,
@@ -279,14 +280,15 @@
         pseudo_planar,
     )
 
     attrs = {
         "band": band,
         "value_field": value_field,
         "dtype": dtype_str,
+        "nodata": nodata,
         "crs": crs,
         "gdal_transform": geotransform.to_gdal(),
         "row_off": row_off,
         "col_off": col_off,
     }
 
     if should_swap[arr.dtype.byteorder]:
@@ -311,14 +313,15 @@
     }
 
     return record
 
 
 def array_to_quadbin_record(
     arr: np.ndarray,
+    nodata: float,
     band: int,
     value_field: str,
     dtype_str: str,
     transformer: pyproj.Transformer,
     geotransform: Affine,
     resolution: int,
     row_off: int = 0,
@@ -338,14 +341,15 @@
     block_quadbin = quadbin.point_to_cell(x, y, resolution)
     tile_x, tile_y, tile_z = quadbin.cell_to_tile(block_quadbin)
 
     attrs = {
         "band": band,
         "value_field": value_field,
         "dtype": dtype_str,
+        "nodata": nodata,
         "crs": crs,
         "gdal_transform": geotransform.to_gdal(),
         "row_off": row_off,
         "col_off": col_off,
         "block_area": quadbin.cell_area(block_quadbin),
         "z": tile_z,
         "x": tile_x,
@@ -527,14 +531,15 @@
                 "gdalwarp your_raster.tif -of COG "
                 "-co TILING_SCHEME=GoogleMapsCompatible -co COMPRESS=DEFLATE "
                 "your_compatible_raster.tif"
             )
             raise ValueError(msg)
 
         resolution = raster_info["GEO"]["MaxZoom"]
+        metadata["resolution"] = resolution
 
     """Requires rasterio."""
     if not _has_rasterio:  # pragma: no cover
         import_error_rasterio()
 
     """Open a raster file with rasterio."""
     with rasterio.open(file_path) as raster_dataset:
@@ -580,28 +585,30 @@
         metadata["irregular_pixel_block_shape"] = False
 
         for _, window in raster_dataset.block_windows():
 
             if output_quadbin:
                 rec = array_to_quadbin_record(
                     raster_dataset.read(band, window=window),
+                    raster_dataset.nodata,
                     band,
                     band_name,
                     str(band_type),
                     transformer,
                     raster_dataset.transform,
                     resolution,
                     window.row_off,
                     window.col_off,
                     crs=input_crs,
                 )
 
             else:
                 rec = array_to_record(
                     raster_dataset.read(band, window=window),
+                    raster_dataset.nodata,
                     band,
                     band_name,
                     str(band_type),
                     transformer,
                     raster_dataset.transform,
                     window.row_off,
                     window.col_off,
@@ -1151,14 +1158,23 @@
     dataset_id,
     table_id,
     client=None,
 ):
     if append_records:
         table_ref = f"{project_id}.{dataset_id}.{table_id}"
         location = "quadbin" if is_quadbin else "geog"
+        get_resolution = ""
+        fetch_resolution = ""
+        if is_quadbin:
+            get_resolution = """
+                ,INT64(
+                    JSON_QUERY(attrs, '$.resolution')
+                ) AS resolution"""
+            fetch_resolution = """
+                ,ANY_VALUE(resolution) AS resolution"""
         query = f"""
             UPDATE `{table_ref}`
             SET attrs = (
                 WITH parsed_meta AS (
                     SELECT PARSE_JSON(attrs) AS attrs
                     FROM `{table_ref}`
                     WHERE {location} IS NULL
@@ -1180,15 +1196,16 @@
                     INT64(
                         JSON_QUERY(attrs, '$.max_pixel_block_height_in_pixel')
                         ) AS max_pixel_block_height_in_pixel,
                     INT64(
                         JSON_QUERY(attrs, '$.max_pixel_block_width_in_pixel')
                     ) AS max_pixel_block_width_in_pixel,
                     JSON_VALUE(attrs, '$.crs') AS crs,
-                    JSON_QUERY_ARRAY(attrs, '$.gdal_transform') AS gdal_transform,
+                    JSON_QUERY_ARRAY(attrs, '$.gdal_transform') AS gdal_transform
+                    {get_resolution}
                   FROM parsed_meta
                 ),
                 meta2 AS (
                   SELECT
                     JSON_VALUE_ARRAY(attrs, '$.bands') AS bands,
                     SAFE.ST_GEOGFROMTEXT(
                         JSON_VALUE(attrs, '$.raster_boundary')
@@ -1204,29 +1221,29 @@
                     INT64(
                         JSON_QUERY(attrs, '$.max_pixel_block_height_in_pixel')
                         ) AS max_pixel_block_height_in_pixel,
                     INT64(
                         JSON_QUERY(attrs, '$.max_pixel_block_width_in_pixel')
                     ) AS max_pixel_block_width_in_pixel,
                     JSON_VALUE(attrs, '$.crs') AS crs,
-                    JSON_QUERY_ARRAY(attrs, '$.gdal_transform') AS gdal_transform,
+                    JSON_QUERY_ARRAY(attrs, '$.gdal_transform') AS gdal_transform
+                    {get_resolution}
                   FROM
                     (SELECT PARSE_JSON({sql_quote(json.dumps(metadata))}) AS attrs)
                 ),
                 united AS (
                     SELECT * FROM meta1
                     UNION ALL
                     SELECT * FROM meta2
-                ),
-                bands AS (
-                    SELECT ARRAY_AGG(DISTINCT band) AS bands
-                    FROM united, UNNEST(bands) AS band
                 )
                 SELECT TO_JSON_STRING(TO_JSON(STRUCT(
-                    (SELECT bands FROM bands) AS bands,
+                    (
+                        SELECT ARRAY_AGG(DISTINCT b)
+                        FROM united, UNNEST(bands) b
+                    ) AS bands,
                     ST_ASTEXT(ST_UNION_AGG(raster_boundary)) AS raster_boundary,
                     SUM(nb_pixel) AS nb_pixel,
                     SUM(nb_pixel_blocks) AS nb_pixel_blocks,
                     MAX(max_pixel_block_height_in_pixel)
                       AS max_pixel_block_height_in_pixel,
                     MIN(min_pixel_block_height_in_pixel)
                       AS min_pixel_block_height_in_pixel,
@@ -1247,14 +1264,15 @@
                     IF(
                         ARRAY_LENGTH(
                             ARRAY_AGG(DISTINCT TO_JSON_STRING(gdal_transform))
                         ) = 1,
                         ANY_VALUE(gdal_transform),
                         NULL
                     ) AS gdal_transform
+                    {fetch_resolution}
                 )))
                 FROM united
             ) WHERE {location} IS NULL
         """
 
         """Requires bigquery."""
         if not _has_bigquery:  # pragma: no cover
```

### Comparing `raster-loader-0.3.0/raster_loader/tests/fixtures/mosaic.tif` & `raster-loader-0.3.1/raster_loader/tests/fixtures/mosaic.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/tests/fixtures/mosaic_wm.tif` & `raster-loader-0.3.1/raster_loader/tests/fixtures/mosaic_wm.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/tests/fixtures/quadbin_raster.tif` & `raster-loader-0.3.1/raster_loader/tests/fixtures/quadbin_raster.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/tests/mocks.py` & `raster-loader-0.3.1/raster_loader/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/tests/test_cli.py` & `raster-loader-0.3.1/raster_loader/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.3.0/raster_loader/tests/test_io.py` & `raster-loader-0.3.1/raster_loader/tests/test_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,19 @@
 
 def test_array_to_record():
     arr = np.linspace(0, 100, 180 * 360).reshape(180, 360)
     crs = "EPSG:4326"
     transformer = pyproj.Transformer.from_crs(crs, "EPSG:4326", always_xy=True)
     geotransform = Affine.from_gdal(-180.0, 1.0, 0.0, 90.0, 0.0, -1.0)
     band = 1
+    nodata = -1
     value_field = "band_1_float64"
     dtype_str = "float64"
     record = io.array_to_record(
-        arr, band, value_field, dtype_str, transformer, geotransform, crs=crs
+        arr, nodata, band, value_field, dtype_str, transformer, geotransform, crs=crs
     )
 
     if should_swap[arr.dtype.byteorder]:
         arr_bytes = np.ascontiguousarray(arr.byteswap()).tobytes()
     else:
         arr_bytes = np.ascontiguousarray(arr).tobytes()
 
@@ -69,14 +70,15 @@
     assert record["block_width"] == 360
     assert record["band_1_float64"] == arr_bytes
 
     expected_attrs = {
         "band": band,
         "value_field": "band_1_float64",
         "dtype": "float64",
+        "nodata": nodata,
         "crs": crs,
         "gdal_transform": list(geotransform.to_gdal()),
         "row_off": 0,
         "col_off": 0,
     }
 
     for key, value in expected_attrs.items():
@@ -86,14 +88,15 @@
 def test_array_to_record_offset():
     arr = np.linspace(0, 100, 160 * 340).reshape(160, 340)
     transformer = pyproj.Transformer.from_crs("EPSG:4326", "EPSG:4326", always_xy=True)
     geotransform = Affine.from_gdal(-180.0, 1.0, 0.0, 90.0, 0.0, -1.0)
 
     record = io.array_to_record(
         arr,
+        -1,
         1,
         "band_1_float64",
         "float64",
         transformer,
         geotransform,
         row_off=20,
         col_off=20,
@@ -132,14 +135,15 @@
 
 def test_array_to_quadbin_record():
     arr = np.linspace(0, 100, 160 * 340).reshape(160, 340)
     transformer = pyproj.Transformer.from_crs("EPSG:4326", "EPSG:4326", always_xy=True)
     geotransform = Affine.from_gdal(-180.0, 1.0, 0.0, 90.0, 0.0, -1.0)
     record = io.array_to_quadbin_record(
         arr,
+        -1,
         1,
         "band_1_float64",
         "float64",
         transformer,
         geotransform,
         resolution=4,
         row_off=20,
@@ -156,14 +160,15 @@
     assert record["block_width"] == 340
     assert record["band_1_float64"] == arr_bytes
 
     expected_attrs = {
         "band": 1,
         "value_field": "band_1_float64",
         "dtype": "float64",
+        "nodata": -1,
         "crs": "EPSG:4326",
         "gdal_transform": list(geotransform.to_gdal()),
         "row_off": 20,
         "col_off": 20,
     }
 
     for key, value in expected_attrs.items():
@@ -173,35 +178,37 @@
 def test_record_to_array():
     arr = np.linspace(0, 100, 180 * 360).reshape(180, 360)
     crs = "EPSG:4326"
     transformer = pyproj.Transformer.from_crs(crs, "EPSG:4326", always_xy=True)
     geotransform = Affine.from_gdal(-180.0, 1.0, 0.0, 90.0, 0.0, -1.0)
     crs = "EPSG:4326"
     band = 1
+    nodata = 1
     value_field = "band_1_float64"
     dtype_str = "float64"
     record = io.array_to_record(
-        arr, band, value_field, dtype_str, transformer, geotransform, crs=crs
+        arr, nodata, band, value_field, dtype_str, transformer, geotransform, crs=crs
     )
     arr2 = io.record_to_array(record)
     assert np.allclose(arr, arr2)
     assert arr.dtype.name == arr2.dtype.name
     assert arr.shape == arr2.shape
 
 
 def test_record_to_array_invalid_dtype():
     arr = np.linspace(0, 100, 180 * 360).reshape(180, 360)
     crs = "EPSG:4326"
     transformer = pyproj.Transformer.from_crs(crs, "EPSG:4326", always_xy=True)
     geotransform = Affine.from_gdal(-180.0, 1.0, 0.0, 90.0, 0.0, -1.0)
     band = 1
+    nodata = 1
     value_field = "band_1_dtype"
     dtype_str = "dtype"
     record = io.array_to_record(
-        arr, band, value_field, dtype_str, transformer, geotransform, crs=crs
+        arr, nodata, band, value_field, dtype_str, transformer, geotransform, crs=crs
     )
 
     with pytest.raises(TypeError):
         io.record_to_array(record, "band_1_dtype")
 
 
 def test_rasterio_to_record():
@@ -213,14 +220,15 @@
     value_field = "band_1_uint8"
     dtype_str = "uint8"
     transformer = pyproj.Transformer.from_crs("EPSG:4326", "EPSG:4326", always_xy=True)
 
     with rasterio.open(test_file) as src:
         record = io.array_to_record(
             src.read(band),
+            src.nodata,
             band,
             value_field,
             dtype_str,
             transformer,
             src.transform,
             crs=src.crs.to_string(),
         )
@@ -235,14 +243,53 @@
         "gdal_transform": list(src.transform.to_gdal()),
         "row_off": 0,
         "col_off": 0,
     }
 
     for key, value in expected_attrs.items():
         assert json.loads(record["attrs"])[key] == value
+
+
+def test_rasterio_to_record_with_nodata():
+    import rasterio
+    import os
+
+    test_file = os.path.join(fixtures_dir, "fuji.tif")
+    band = 1
+    value_field = "band_1_uint8"
+    dtype_str = "uint8"
+    transformer = pyproj.Transformer.from_crs("EPSG:4326", "EPSG:4326", always_xy=True)
+
+    with rasterio.open(test_file) as src:
+        record = io.array_to_record(
+            src.read(band),
+            src.nodata,
+            band,
+            value_field,
+            dtype_str,
+            transformer,
+            src.transform,
+            crs=src.crs.to_string(),
+        )
+
+    assert isinstance(record, dict)
+
+    expected_attrs = {
+        "band": 1,
+        "value_field": "band_1_uint8",
+        "dtype": "uint8",
+        "nodata": -32767,
+        "crs": "EPSG:8692",
+        "gdal_transform": list(src.transform.to_gdal()),
+        "row_off": 0,
+        "col_off": 0,
+    }
+
+    for key, value in expected_attrs.items():
+        assert json.loads(record["attrs"])[key] == value
 
 
 @pytest.mark.integration_test
 def test_rasterio_to_bigquery_with_generic_raster():
     from raster_loader.io import rasterio_to_bigquery
     from raster_loader.io import bigquery_to_records
```

### Comparing `raster-loader-0.3.0/raster_loader.egg-info/PKG-INFO` & `raster-loader-0.3.1/raster_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-loader
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for loading GIS raster data to standard cloud-based data warehouses that don't natively support raster data.
 Home-page: https://github.com/cartodb/raster-loader
 Author: CARTO
 License: BSD 3-Clause
 Keywords: carto,raster,gis,data warehouse,bigquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `raster-loader-0.3.0/raster_loader.egg-info/SOURCES.txt` & `raster-loader-0.3.1/raster_loader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,10 +51,11 @@
 raster_loader/cli/info.py
 raster_loader/tests/.env.sample
 raster_loader/tests/__init__.py
 raster_loader/tests/mocks.py
 raster_loader/tests/test_cli.py
 raster_loader/tests/test_io.py
 raster_loader/tests/test_utils.py
+raster_loader/tests/fixtures/fuji.tif
 raster_loader/tests/fixtures/mosaic.tif
 raster_loader/tests/fixtures/mosaic_wm.tif
 raster_loader/tests/fixtures/quadbin_raster.tif
```

### Comparing `raster-loader-0.3.0/setup.cfg` & `raster-loader-0.3.1/setup.cfg`

 * *Files identical despite different names*

