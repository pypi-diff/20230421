# Comparing `tmp/kfactory-0.6.2.tar.gz` & `tmp/kfactory-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.6.2.tar", last modified: Tue Apr 18 19:12:09 2023, max compression
+gzip compressed data, was "kfactory-0.6.3.tar", last modified: Fri Apr 21 19:57:59 2023, max compression
```

## Comparing `kfactory-0.6.2.tar` & `kfactory-0.6.3.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 19:11:53.000000 kfactory-0.6.2/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.054337 kfactory-0.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 19:11:53.000000 kfactory-0.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.054337 kfactory-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 19:11:53.000000 kfactory-0.6.2/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 19:11:53.000000 kfactory-0.6.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-18 19:11:53.000000 kfactory-0.6.2/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 19:11:53.000000 kfactory-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-18 19:11:53.000000 kfactory-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 19:11:53.000000 kfactory-0.6.2/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 19:11:53.000000 kfactory-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 19:11:53.000000 kfactory-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 19:11:53.000000 kfactory-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 19:12:09.062337 kfactory-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 19:11:53.000000 kfactory-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.054337 kfactory-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/klive.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 19:11:53.000000 kfactory-0.6.2/docs/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 19:11:53.000000 kfactory-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:12:09.062337 kfactory-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.054337 kfactory-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/generic_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)    80302 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/kcell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/src/kfactory/pcells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/src/kfactory/pcells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/pcells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/src/kfactory/utils/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22912 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/geo/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/geo/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/geo/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-18 19:11:53.000000 kfactory-0.6.2/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.058337 kfactory-0.6.2/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 19:12:09.000000 kfactory-0.6.2/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 19:12:09.000000 kfactory-0.6.2/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:12:09.000000 kfactory-0.6.2/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 19:12:09.000000 kfactory-0.6.2/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 19:12:09.000000 kfactory-0.6.2/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:12:09.062337 kfactory-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-18 19:11:53.000000 kfactory-0.6.2/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 19:57:41.000000 kfactory-0.6.3/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 19:57:41.000000 kfactory-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-21 19:57:41.000000 kfactory-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 19:57:41.000000 kfactory-0.6.3/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 19:57:41.000000 kfactory-0.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 19:57:41.000000 kfactory-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 19:57:41.000000 kfactory-0.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-21 19:57:59.395300 kfactory-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 19:57:41.000000 kfactory-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/klive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-21 19:57:41.000000 kfactory-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:57:59.395300 kfactory-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/generic_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81247 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/kcell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/pcells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/pcells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_spiral.py
```

### Comparing `kfactory-0.6.2/.github/workflows/pages.yml` & `kfactory-0.6.3/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/.github/workflows/release.yml` & `kfactory-0.6.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/.github/workflows/test_code.yml` & `kfactory-0.6.3/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/.pre-commit-config.yaml` & `kfactory-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/LICENSE` & `kfactory-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/Makefile` & `kfactory-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/PKG-INFO` & `kfactory-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.2
+Version: 0.6.3
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.2
+# KFactory 0.6.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.2/README.md` & `kfactory-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.6.2
+# KFactory 0.6.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.2/docs/Makefile` & `kfactory-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/README.md` & `kfactory-0.6.3/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.6.2
+# KFactory 0.6.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.2/docs/_static/complex.png` & `kfactory-0.6.3/docs/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/_static/klive.webm` & `kfactory-0.6.3/docs/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/_static/waveguide.png` & `kfactory-0.6.3/docs/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/complex_cell.py` & `kfactory-0.6.3/docs/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/conf.py` & `kfactory-0.6.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project = "kfactory"
-version = "0.6.2"
+version = "0.6.3"
 copyright = "2022"
 # author = "kfactory"
 
 # html_theme = "furo"
 # html_theme = "sphinx_rtd_theme"
 html_theme = "sphinx_book_theme"
```

### Comparing `kfactory-0.6.2/docs/index.rst` & `kfactory-0.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/intro.rst` & `kfactory-0.6.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/make.bat` & `kfactory-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/notebooks/00_geometry.py` & `kfactory-0.6.3/docs/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/notebooks/01_references.py` & `kfactory-0.6.3/docs/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/notebooks/02_DRC.py` & `kfactory-0.6.3/docs/notebooks/02_DRC.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,14 +62,55 @@
 d3 = datetime.now()
 
 print(f"time to draw: {d2-d1}")
 print(f"time to clean: {d3-d2}")
 print(f"total time: {d3-d1}")
 
 c
+
+# +
+c = kf.KCell("minkowski_tiled_test")
+
+
+d1 = datetime.now()
+
+for i in range(50):
+    ellipse = kf.kdb.Polygon.ellipse(kf.kdb.Box(10000, 20000), i * 2)
+
+    x0 = 0
+    for j in range(5000, 30000, 500):
+        c.shapes(c.klib.layer(1, 0)).insert(
+            ellipse.transformed(kf.kdb.Trans(x0, i * 30000))
+        )
+        c.shapes(c.klib.layer(1, 0)).insert(
+            ellipse.transformed(kf.kdb.Trans(x0 + j, i * 30000))
+        )
+
+        x0 += 15000
+
+d2 = datetime.now()
+
+c.shapes(c.klib.layer(2, 0)).insert(
+    kf.utils.fix_spacing_minkowski_tiled(
+        c,
+        1000,
+        c.klib.layer(1, 0),
+        n_threads=32,
+        tile_size=(250, 250),
+        smooth=5,
+    )
+)
+
+d3 = datetime.now()
+
+print(f"time to draw: {d2-d1}")
+print(f"time to clean: {d3-d2}")
+print(f"total time: {d3-d1}")
+
+c
 # -
 
 c = kf.KCell("ToFill")
 c.shapes(kf.klib.layer(1, 0)).insert(
     kf.kdb.DPolygon.ellipse(kf.kdb.DBox(5000, 3000), 512)
 )
 c.shapes(kf.klib.layer(10, 0)).insert(
@@ -80,15 +121,15 @@
 c
 
 fc = kf.KCell("fill")
 fc.shapes(fc.klib.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
 fc.shapes(fc.klib.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
 fc
 
-import kfactory.utils.geo.fill as fill
+import kfactory.utils.fill as fill
 
 # fill.fill_tiled(c, fc, [(kf.klib.layer(1,0), 0)], exclude_layers = [(kf.klib.layer(10,0), 100), (kf.klib.layer(2,0), 0), (kf.klib.layer(3,0),0)], x_space=5, y_space=5)
 fill.fill_tiled(
     c,
     fc,
     [(kf.klib.layer(1, 0), 0)],
     exclude_layers=[
```

### Comparing `kfactory-0.6.2/docs/star.py` & `kfactory-0.6.3/docs/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/docs/waveguide.py` & `kfactory-0.6.3/docs/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/pyproject.toml` & `kfactory-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.6.2"
+version = "0.6.3"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
```

### Comparing `kfactory-0.6.2/src/kfactory/__init__.py` & `kfactory-0.6.3/src/kfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     LayerEnum,
     show,
 )
 from . import pcells, placer, routing, utils, port
 from .config import logger
 
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
     "Ports",
```

### Comparing `kfactory-0.6.2/src/kfactory/config.py` & `kfactory-0.6.3/src/kfactory/config.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/generic_tech.py` & `kfactory-0.6.3/src/kfactory/generic_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/kcell.py` & `kfactory-0.6.3/src/kfactory/kcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -949,34 +949,42 @@
         c._locked = False
         return c
 
     def __copy__(self) -> "KCell":
         """Enables use of :py:func:`copy.copy` and :py:func:`copy.deep_copy`."""
         return self.dup()
 
-    def add_port(self, port: Port, name: str | None = None) -> None:
+    def add_port(
+        self, port: Port, name: str | None = None, keep_mirror: bool = False
+    ) -> None:
         """Add an existing port. E.g. from an instance to propagate the port.
 
         Args:
             port: The port to add. Port should either be a :py:class:`~Port`,
                 or will be converted to an integer based port with 90° increment
             name: Overwrite the name of the port
+            keep_mirror: Keep the mirror part of the transformation of a port if
+                `True`, else set the mirror flag to `False`.
         """
         self.ports.add_port(port=port, name=name)
 
-    def add_ports(self, ports: Iterable[Port], prefix: str = "") -> None:
+    def add_ports(
+        self, ports: Iterable[Port], prefix: str = "", keep_mirror: bool = False
+    ) -> None:
         """Add a sequence of ports to the cells.
 
         Can be useful to add all ports of a instance for example.
 
         Args:
             ports: list/tuple (anything iterable) of ports.
             prefix: string to add in front of all the port names
+            keep_mirror: Keep the mirror part of the transformation of a port if
+                `True`, else set the mirror flag to `False`.
         """
-        self.ports.add_ports(ports=ports, prefix=prefix)
+        self.ports.add_ports(ports=ports, prefix=prefix, keep_mirror=keep_mirror)
 
     @classmethod
     def from_yaml(
         cls: "Callable[..., KCell]",
         constructor: Any,
         node: Any,
         verbose: bool = False,
@@ -1176,27 +1184,27 @@
     def ports(self, new_ports: "InstancePorts | Ports") -> None:
         self._ports = new_ports.copy()
 
     @overload
     def create_port(
         self,
         *,
-        name: str,
+        name: str | None = None,
         trans: kdb.Trans,
         width: int,
         layer: LayerEnum | int,
         port_type: str = "optical",
     ) -> None:
         ...
 
     @overload
     def create_port(
         self,
         *,
-        name: str,
+        name: str | None = None,
         dcplx_trans: kdb.DCplxTrans,
         dwidth: float,
         layer: LayerEnum | int,
         port_type: str = "optical",
     ) -> None:
         ...
 
@@ -1209,26 +1217,26 @@
     ) -> None:
         ...
 
     @overload
     def create_port(
         self,
         *,
-        name: str,
+        name: str | None = None,
         width: int,
         position: tuple[int, int],
         angle: int,
         layer: LayerEnum | int,
         port_type: str = "optical",
         mirror_x: bool = False,
     ) -> None:
         ...
 
     def create_port(self, **kwargs: Any) -> None:
-        """Create a new port. Equivalent to :py:attr:`~add_port(Port(...))`."""
+        """Proxy for :py:func:`Ports.create_port`."""
         self.ports.create_port(**kwargs)
 
     @overload
     def create_inst(
         self,
         cell: "KCell | int",
         trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector = kdb.Trans(),
@@ -1919,27 +1927,39 @@
         """Check whether a port is already in the list."""
         return port.hash() in [v.hash() for v in self._ports]
 
     def __iter__(self) -> Iterator[Port]:
         """Iterator, that allows for loops etc to directly access the object."""
         yield from self._ports
 
-    def add_port(self, port: Port, name: str | None = None) -> None:
+    def add_port(
+        self, port: Port, name: str | None = None, keep_mirror: bool = False
+    ) -> None:
         """Add a port object.
 
         Args:
             port: The port to add
             name: Overwrite the name of the port
+            keep_mirror: Keep the mirror flag from the original port if `True`,
+                else set :py:attr:~`Port.trans.mirror` (or the complex equivalent)
+                to `False`.
         """
         _port = port.copy()
+        if not keep_mirror:
+            if port._trans:
+                port._trans.mirror = False
+            elif port._dcplx_trans:
+                port._dcplx_trans.mirror = False
         if name is not None:
             _port.name = name
         self._ports.append(_port)
 
-    def add_ports(self, ports: Iterable[Port], prefix: str = "") -> None:
+    def add_ports(
+        self, ports: Iterable[Port], prefix: str = "", keep_mirror: bool = False
+    ) -> None:
         """Append a list of ports."""
         for p in ports:
             name = p.name or ""
             self.add_port(port=p, name=prefix + name)
 
     @overload
     def create_port(
@@ -2051,16 +2071,18 @@
         self._ports.append(port)
         return port
 
     def get_all_named(self) -> dict[str, Port]:
         """Get all ports in a dictionary with names as keys."""
         return {v.name: v for v in self._ports if v.name is not None}
 
-    def __getitem__(self, key: str | None) -> Port:
+    def __getitem__(self, key: int | str | None) -> Port:
         """Get a specific port by name."""
+        if isinstance(key, int):
+            return self._ports[key]
         try:
             return next(filter(lambda port: port.name == key, self._ports))
         except StopIteration:
             raise ValueError(
                 f"{key} is not a port. Available ports: {[v.name for v in self._ports]}"
             )
 
@@ -2114,15 +2136,15 @@
 
         Args:
             instance: The related instance
         """
         self.cell_ports = instance.cell.ports
         self.instance = instance
 
-    def __getitem__(self, key: str | None) -> Port:
+    def __getitem__(self, key: int | str | None) -> Port:
         """Get a port by name."""
         p = self.cell_ports[key]
         if self.instance.is_complex():
             return p.copy(self.instance.dcplx_trans)
         else:
             return p.copy(self.instance.trans)
```

### Comparing `kfactory-0.6.2/src/kfactory/pcells/bezier.py` & `kfactory-0.6.3/src/kfactory/pcells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/pcells/circular.py` & `kfactory-0.6.3/src/kfactory/pcells/circular.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 A circular bend has a constant radius.
 """
 
 import numpy as np
 
 from .. import kdb
 from ..kcell import KCell, LayerEnum, autocell
-from ..utils import Enclosure
-from ..utils.geo import extrude_path
+from ..utils import Enclosure, extrude_path
 
 __all__ = ["bend_circular"]
 
 
 @autocell
 def bend_circular(
     width: float,
```

### Comparing `kfactory-0.6.2/src/kfactory/pcells/dbu/taper.py` & `kfactory-0.6.3/src/kfactory/pcells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/pcells/dbu/waveguide.py` & `kfactory-0.6.3/src/kfactory/pcells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/pcells/euler.py` & `kfactory-0.6.3/src/kfactory/pcells/euler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 import numpy as np
 from scipy.optimize import brentq  # type: ignore[import]
 from scipy.special import fresnel  # type: ignore[import]
 
 from .. import kdb
 from ..kcell import KCell, LayerEnum, autocell
-from ..utils import Enclosure
-from ..utils.geo import extrude_path
+from ..utils import Enclosure, extrude_path
 
 __all__ = [
     "euler_bend_points",
     "euler_sbend_points",
     "bend_euler",
     "bend_s_euler",
 ]
@@ -190,39 +189,35 @@
         enclosure=enclosure,
         start_angle=0,
         end_angle=theta,
     )
 
     if theta == 90:
         c.create_port(
-            name="W0",
             layer=layer,
             width=int(width / c.klib.dbu),
             trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
         )
         c.create_port(
-            name="N0",
             layer=layer,
             width=int(width / c.klib.dbu),
             trans=kdb.Trans(1, False, backbone[-1].to_itype(dbu).to_v()),
         )
     elif theta == 180:
         c.create_port(
-            name="W0",
             layer=layer,
             width=int(width / c.klib.dbu),
             trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
         )
         c.create_port(
-            name="W1",
             layer=layer,
             width=int(width / c.klib.dbu),
             trans=kdb.Trans(2, False, backbone[-1].to_itype(dbu).to_v()),
         )
-
+    c.autorename_ports()
     return c
 
 
 @autocell
 def bend_s_euler(
     offset: float,
     width: float,
```

### Comparing `kfactory-0.6.2/src/kfactory/pcells/taper.py` & `kfactory-0.6.3/src/kfactory/pcells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/pcells/waveguide.py` & `kfactory-0.6.3/src/kfactory/pcells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/placer.py` & `kfactory-0.6.3/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/port.py` & `kfactory-0.6.3/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/routing/electrical.py` & `kfactory-0.6.3/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/routing/manhattan.py` & `kfactory-0.6.3/src/kfactory/routing/manhattan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Can calculate manhattan routes based on ports/transformations."""
 
 import numpy as np
 
 from .. import kdb
 from ..config import logger
 from ..kcell import KLib, Port
-from ..utils.geo import clean_points
+from ..utils import clean_points
 
 __all__ = ["route_manhattan", "route_manhattan_180"]
 
 
 def droute_manhattan_180(
     port1: kdb.DTrans,
     port2: kdb.DTrans,
```

### Comparing `kfactory-0.6.2/src/kfactory/routing/optical.py` & `kfactory-0.6.3/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory/utils/__init__.py` & `kfactory-0.6.3/src/kfactory/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,29 @@
 :py:func:~`fill_tiled` provides a filling algorithm that can use the
 :py:class:~`klayout.db.TilingProcessor` to calculate the regions to fill.
 
 :py:func:~`fix_spacing` uses a region space check to calculate areas that violate
 min space violations. :py:func:~`fix_spacing_tiled` to fix it using a TilingProcessor.
 """
 
-from . import geo, violations
-from .geo import Direction, Enclosure, extrude_path, extrude_path_dynamic
-from .geo.fill import fill_tiled
-from .violations import fix_spacing_tiled
+from .enclosure import (
+    Direction,
+    Enclosure,
+    clean_points,
+    extrude_path,
+    extrude_path_dynamic,
+)
+from .fill import fill_tiled
+from .violations import fix_spacing_minkowski_tiled, fix_spacing_tiled
 
 __all__ = [
     "Enclosure",
     "violations",
     "Direction",
     "geo",
     "extrude_path",
     "extrude_path_dynamic",
     "fill_tiled",
     "fix_spacing_tiled",
+    "fix_spacing_minkowski_tiled",
+    "clean_points",
 ]
```

### Comparing `kfactory-0.6.2/src/kfactory/utils/geo/enclosure.py` & `kfactory-0.6.3/src/kfactory/utils/enclosure.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,82 @@
+"""Enclosure module.
+
+Enclosures allow to calculate slab/excludes and similar concepts to an arbitrary
+shape located on a main_layer or reference layer or region.
+"""
+
+import os
 from collections.abc import Callable, Sequence
 from enum import IntEnum
 from hashlib import sha1
 from typing import Any, Optional, TypeGuard
 
 import numpy as np
 from pydantic import BaseModel, Field, PrivateAttr
 
-from ... import kdb
-from ...kcell import KCell, LayerEnum
+from .. import kdb
+from ..config import logger
+from ..kcell import KCell, LayerEnum
 
 __all__ = [
     "Enclosure",
     "extrude_path",
     "extrude_path_points",
     "extrude_path_dynamic",
     "extrude_path_dynamic_points",
 ]
 
 
 class Direction(IntEnum):
+    """Direction for applying standard minkowski sums.
+
+    Attributes:
+        X: Only apply in x-direction.
+        Y: Only apply in y-direction.
+        BOTH: Apply in both x/y-direction. Equivalent to a
+            minkowski sum with a square.
+    """
+
     X = 1
     Y = 2
     BOTH = 3
 
 
 def is_callable_widths(
     widths: Callable[[float], float] | list[float]
 ) -> TypeGuard[Callable[[float], float]]:
+    """Determines whether a width object is callable or a list."""
     return callable(widths)
 
 
 def path_pts_to_polygon(
     pts_top: list[kdb.DPoint], pts_bot: list[kdb.DPoint]
 ) -> kdb.DPolygon:
+    """Convert a list of points to a polygon."""
     pts_bot.reverse()
     return kdb.DPolygon(pts_top + pts_bot)
 
 
-def is_Region(r: object) -> TypeGuard[kdb.Region]:
+def _is_Region(r: object) -> TypeGuard[kdb.Region]:
     return isinstance(r, kdb.Region)
 
 
-def is_int(r: object) -> TypeGuard[int]:
+def _is_int(r: object) -> TypeGuard[int]:
     return isinstance(r, int)
 
 
-def is_callable(r: object) -> TypeGuard[Callable[[float], float]]:
+def _is_callable(r: object) -> TypeGuard[Callable[[float], float]]:
     return callable(r)
 
 
 def clean_points(points: list[kdb.Point]) -> list[kdb.Point]:
+    """Remove useless points from a manhattan type of list.
+
+    This will remove the middle points that are on a straight line.
+    """
     if len(points) < 2:
         return points
     if len(points) == 2:
         return points if points[1] != points[0] else points[:1]
     p_p = points[0]
     p = points[1]
 
@@ -299,30 +322,38 @@
                 layer_list[layer].add_section(section)
     if is_callable_widths(widths):
         for layer, layer_sec in layer_list.items():
             reg = kdb.Region()
             for section in layer_sec.sections:
 
                 def w_max(x: float) -> float:
-                    return widths(x) + 2 * section.d_max * target.klib.dbu  # type: ignore[operator]
+                    return (
+                        widths(x)  # type: ignore[operator]
+                        + 2 * section.d_max * target.klib.dbu
+                    )
 
                 _r = kdb.Region(
                     path_pts_to_polygon(
                         *extrude_path_dynamic_points(
                             path,
                             w_max,
                             start_angle,
                             end_angle,
                         )
                     ).to_itype(target.klib.dbu)
                 )
                 if section.d_min is not None:
 
                     def w_min(x: float) -> float:
-                        return widths(x) + 2 * section.d_min * target.klib.dbu  # type: ignore[operator]
+                        return (
+                            widths(x)  # type: ignore[operator]
+                            + 2  # type: ignore[operator]
+                            * section.d_min
+                            * target.klib.dbu
+                        )
 
                     _r -= kdb.Region(
                         path_pts_to_polygon(
                             *extrude_path_dynamic_points(
                                 path,
                                 w_min,
                                 start_angle,
@@ -333,27 +364,33 @@
                 reg.insert(_r)
             target.shapes(layer).insert(reg.merge())
 
     else:
         for layer, layer_sec in layer_list.items():
             reg = kdb.Region()
             for section in layer_sec.sections:
-                max_widths = [w + 2 * section.d_max * target.klib.dbu for w in widths]  # type: ignore[union-attr]
+                max_widths = [
+                    w + 2 * section.d_max * target.klib.dbu
+                    for w in widths  # type: ignore[union-attr]
+                ]
                 _r = kdb.Region(
                     path_pts_to_polygon(
                         *extrude_path_dynamic_points(
                             path,
                             max_widths,
                             start_angle,
                             end_angle,
                         )
                     ).to_itype(target.klib.dbu)
                 )
                 if section.d_min is not None:
-                    min_widths = [w + 2 * section.d_min * target.klib.dbu for w in widths]  # type: ignore[union-attr]
+                    min_widths = [
+                        w + 2 * section.d_min * target.klib.dbu
+                        for w in widths  # type: ignore[union-attr]
+                    ]
                     _r -= kdb.Region(
                         path_pts_to_polygon(
                             *extrude_path_dynamic_points(
                                 path,
                                 min_widths,
                                 start_angle,
                                 end_angle,
@@ -361,107 +398,181 @@
                         ).to_itype(target.klib.dbu)
                     )
                 reg.insert(_r)
             target.shapes(layer).insert(reg.merge())
 
 
 class Section(BaseModel):
+    """Section of an Enclosure.
+
+    Visualization::
+
+        Maximum only Section:
+            ┌────────────────────────┐  ▲
+            │                        │  │
+            │  ┌──────────────────┐  │  │
+            │  │                  │  │  │
+            │  │    Reference     │  │  │ Section
+            │  │                  │  │  │ (d_max only)
+            │  └─────────────┬────┘  │  │
+            │                │d_max  │  │
+            └────────────────▼───────┘  ▼
+
+
+        Minimum & Maximum Section:
+            ┌─────────────────┐
+            │     Section     │
+            │  ┌───────────┐  │
+            │  │           │  │
+            │  │  ┌─────┐  │◄─┼──d_min
+            │  │  │ Ref │  │  │
+            │  │  └─────┘  │  │
+            │  │           │  │◄─d_max
+            │  └───────────┘  │
+            │                 │
+            └─────────────────┘
+
+    Attributes:
+        d_min: Start of the section. If `None`,
+            the section will span all the way between the maxes.
+        d_max: the maximum extent of the section from the reference.
+    """
+
     d_min: int | None = None
     d_max: int
 
     def __hash__(self) -> int:
+        """Hash of the section."""
         return hash((self.d_min, self.d_max))
 
 
 class LayerSection(BaseModel):
+    """A collection of sections intended for a layer.
+
+    Adding a section will trigger an evaluation to merge
+    touching or overlapping sections.
+    """
+
     sections: list[Section] = Field(default=[])
 
     def add_section(self, sec: Section) -> None:
+        """Add a new section.
+
+        Checks for overlaps after.
+        """
         if not self.sections:
             self.sections.append(sec)
         else:
             i = 0
             if sec.d_min is not None:
                 while i < len(self.sections) and sec.d_min > self.sections[i].d_max:
                     i += 1
-                while i < len(self.sections) and sec.d_max >= self.sections[i].d_min:  # type: ignore[operator]
+                while (
+                    i < len(self.sections)
+                    and sec.d_max >= self.sections[i].d_min  # type: ignore[operator]
+                ):
                     sec.d_max = max(self.sections[i].d_max, sec.d_max)
-                    sec.d_min = min(self.sections[i].d_min, sec.d_min)  # type: ignore[type-var]
+                    sec.d_min = min(
+                        self.sections[i].d_min, sec.d_min  # type: ignore[type-var]
+                    )
                     self.sections.pop(i)
                     if i == len(self.sections):
                         break
             self.sections.insert(i, sec)
 
     def __hash__(self) -> int:
+        """Unique hash of LayerSection."""
         return hash(tuple((s.d_min, s.d_max) for s in self.sections))
 
 
 class Enclosure(BaseModel):
+    """Definitions for calculation of enclosing (or smaller) shapes of a reference.
+
+    Attributes:
+        layer_sections: Mapping of layers to their :py:class;`LayerSection`
+
+    """
+
     layer_sections: dict[LayerEnum | int, LayerSection]
     _name: str | None = PrivateAttr(default=None)
     warn: bool = True
 
     main_layer: LayerEnum | int | None
 
     yaml_tag: str = "!Enclosure"
 
     class Config:
+        """pydantic config."""
+
         validate_assignment = True
 
     def __init__(
         self,
         sections: Sequence[
             tuple[LayerEnum | int, int] | tuple[LayerEnum | int, int, int]
         ] = [],
         name: str | None = None,
         warn: bool = True,
         main_layer: LayerEnum | int | None = None,
     ):
+        """Constructor of new enclosure."""
         super().__init__(
             warn=warn,
             layer_sections={},
             main_layer=main_layer,
         )
 
         self._name = name
+
+        self.layer_sections = {}
+
         for sec in sorted(sections, key=lambda sec: (sec[0], sec[1])):
             if sec[0] in self.layer_sections:
                 ls = self.layer_sections[sec[0]]
             else:
                 ls = LayerSection()
                 self.layer_sections[sec[0]] = ls
             ls.add_section(Section(d_max=sec[1])) if len(sec) < 3 else ls.add_section(
                 Section(d_max=sec[2], d_min=sec[1])  # type:ignore[misc]
             )
 
     def __hash__(self) -> int:  # make hashable BaseModel subclass
+        """Calculate a unique hash of the enclosure."""
         return hash(
             (str(self), self.main_layer, tuple(list(self.layer_sections.items())))
         )
 
     def __add__(self, other: "Enclosure") -> "Enclosure":
+        """Returns the merged enclosure of two enclosures."""
         enc = Enclosure()
 
         for layer, secs in self.layer_sections.items():
             for sec in secs.sections:
                 enc.add_section(layer, sec)
 
         for layer, secs in other.layer_sections.items():
             for sec in secs.sections:
                 enc.add_section(layer, sec)
 
         return enc
 
     def __iadd__(self, other: "Enclosure") -> "Enclosure":
+        """Allows merging another enclosure into this one."""
         for layer, secs in other.layer_sections.items():
             for sec in secs.sections:
                 self.add_section(layer, sec)
         return self
 
     def add_section(self, layer: LayerEnum | int, sec: Section) -> None:
+        """Add a new section to the the enclosure.
+
+        Args:
+            layer: Target layer.
+            sec: New section to add.
+        """
         d = self.layer_sections
 
         if layer in self.layer_sections:
             d[layer].add_section(sec)
         else:
             d[layer] = LayerSection(sections=[sec])
 
@@ -469,14 +580,24 @@
 
     def minkowski_region(
         self,
         r: kdb.Region,
         d: int | None,
         shape: Callable[[int], list[kdb.Point] | kdb.Box | kdb.Edge | kdb.Polygon],
     ) -> kdb.Region:
+        """Calculaste a region from a minkowski sum.
+
+        If the distance is negative, the function will take the inverse region and apply
+        the minkowski and take the inverse again.
+
+        Args:
+            r: Target region.
+            d: Distance to pass to the shape. Can be any integer. [dbu]
+            shape: Function returning a shape for the minkowski region.
+        """
         if d is None:
             return kdb.Region()
         elif d == 0:
             return r.dup()
         elif d > 0:
             return r.minkowski_sum(shape(d))
         else:
@@ -497,14 +618,25 @@
 
     def apply_minkowski_enc(
         self,
         c: KCell,
         ref: int | kdb.Region | None,  # layer index or the region
         direction: Direction = Direction.BOTH,
     ) -> None:
+        """Apply an enclosure with a vector in y-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            ref: Reference to use as a base for the enclosure.
+            direction: X/Y or both directions, see :py:class:~`DIRECTION`.
+                Uses a box if both directions are selected.
+        """
         match direction:
             case Direction.BOTH:
 
                 def box(d: int) -> kdb.Box:
                     return kdb.Box(-d, -d, d, d)
 
                 self.apply_minkowski_custom(c, ref=ref, shape=box)
@@ -523,57 +655,238 @@
 
                 self.apply_minkowski_custom(c, ref=ref, shape=edge)
 
             case _:
                 raise ValueError("Undefined direction")
 
     def apply_minkowski_y(self, c: KCell, ref: int | kdb.Region | None = None) -> None:
+        """Apply an enclosure with a vector in y-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            ref: Reference to use as a base for the enclosure.
+        """
         return self.apply_minkowski_enc(c, ref=ref, direction=Direction.Y)
 
     def apply_minkowski_x(self, c: KCell, ref: int | kdb.Region | None) -> None:
+        """Apply an enclosure with a vector in x-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            ref: Reference to use as a base for the enclosure.
+        """
         return self.apply_minkowski_enc(c, ref=ref, direction=Direction.X)
 
     def apply_minkowski_custom(
         self,
         c: KCell,
         shape: Callable[[int], kdb.Edge | kdb.Polygon | kdb.Box],
         ref: int | kdb.Region | None = None,
     ) -> None:
+        """Apply an enclosure with a custom shape.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            shape: A function that will return a shape which takes one argument
+                the size of the section in dbu.
+            ref: Reference to use as a base for the enclosure.
+        """
         if ref is None:
             ref = self.main_layer
 
-        if ref is None:
-            raise ValueError(
-                "The enclosure doesn't have  a reference `main_layer` defined. Therefore the layer must be defined in calls"
-            )
+            if ref is None:
+                raise ValueError(
+                    "The enclosure doesn't have  a reference `main_layer` defined."
+                    " Therefore the layer must be defined in calls"
+                )
         r = kdb.Region(c.begin_shapes_rec(ref)) if isinstance(ref, int) else ref.dup()
         r.merge()
 
-        for layer, layersec in self.layer_sections.items():
+        for layer, layersec in reversed(self.layer_sections.items()):
             for section in layersec.sections:
                 c.shapes(layer).insert(
                     self.minkowski_region(r, section.d_max, shape)
                     - self.minkowski_region(r, section.d_min, shape)
                 )
 
+    def apply_minkowski_tiled(
+        self,
+        c: KCell,
+        ref: int | kdb.Region | None = None,
+        tile_size: float | None = None,
+        n_pts: int = 64,
+        n_threads: int | None = None,
+    ) -> None:
+        """Minkowski regions with tiling processor.
+
+        Useful if the target is a big or complicated enclosure. Will split target ref
+        into tiles and calculate them in parallel. Uses a circle as a shape for the
+        minkowski sum.
+
+        Args:
+            c: Target KCell to apply the enclosures into.
+            ref: The reference shapes to apply the enclosures to.
+                Can be a layer or a region. If `None`, it will trey to use the
+                :py:attr:`main_layer`
+            tile_size: Tile size. This should be in the order off 10+ maximum size
+                of the maximum size of sections.
+            n_pts: Number of points in the circle. < 3 will create a triangle. 4 a
+                diamond, etc.
+            n_threads: Number o threads to use. By default (`None`) it will use as many
+                threads as are set to the process (usually all cores of the machine).
+        """
+        if ref is None:
+            ref = self.main_layer
+
+            if ref is None:
+                raise ValueError(
+                    "The enclosure doesn't have  a reference `main_layer` defined."
+                    " Therefore the layer must be defined in calls"
+                )
+        tp = kdb.TilingProcessor()
+        tp.frame = c.dbbox()  # type: ignore[misc]
+        tp.dbu = c.klib.dbu
+        tp.threads = n_threads or len(os.sched_getaffinity(0))
+        maxsize = 0
+        for layersection in self.layer_sections.values():
+            maxsize = max(
+                maxsize, *[section.d_max for section in layersection.sections]
+            )
+
+        min_tile_size_rec = 10 * maxsize * tp.dbu
+
+        if tile_size is None:
+            tile_size = min_tile_size_rec * 2
+
+        if float(tile_size) <= min_tile_size_rec:
+            logger.warning(
+                "Tile size should be larger than the maximum of "
+                "the enclosures (recommendation: {} / {})",
+                tile_size,
+                min_tile_size_rec,
+            )
+
+        tp.tile_border(maxsize * tp.dbu, maxsize * tp.dbu)
+
+        tp.tile_size(tile_size, tile_size)
+        if isinstance(ref, int):
+            tp.input("main_layer", c.klib, c.cell_index(), ref)
+        else:
+            tp.input("main_layer", ref)
+
+        operators = []
+
+        for layer, sections in self.layer_sections.items():
+            operator = RegionOperator(cell=c, layer=layer)
+            tp.output(f"target_{layer}", operator)
+            for i, section in enumerate(reversed(sections.sections)):
+                queue_str = f"var tile_reg = (_tile & _frame).sized({maxsize});"
+                queue_str += (
+                    "var max_shape = Polygon.ellipse("
+                    f"Box.new({section.d_max*2},{section.d_max*2}), {n_pts});"
+                )
+                match section.d_max:
+                    case d if d > 0:
+                        max_region = (
+                            "var max_reg = "
+                            "main_layer.minkowski_sum(max_shape).merged();"
+                        )
+                    case d if d < 0:
+                        max_region = (
+                            "var max_reg = tile_reg - " "(tile_reg - main_layer);"
+                        )
+                    case 0:
+                        max_region = "var max_reg = main_layer & tile_reg;"
+                queue_str += max_region
+                if section.d_min:
+                    queue_str += (
+                        "var min_shape = Polygon.ellipse("
+                        f"Box.new({section.d_min*2},{section.d_min*2}), 64);"
+                    )
+                    match section.d_min:
+                        case d if d > 0:
+                            min_region = (
+                                "var min_reg = main_layer.minkowski_sum(min_shape);"
+                            )
+                        case d if d < 0:
+                            min_region = (
+                                "var min_reg = tile_reg - "
+                                "(tile_reg - main_layer).minkowski_sum(min_shape);"
+                            )
+                        case 0:
+                            min_region = "var min_reg = main_layer & tile_reg;"
+                    queue_str += min_region
+                    queue_str += (
+                        f"_output(target_{layer}," "(max_reg - min_reg)& _tile, true);"
+                    )
+                else:
+                    queue_str += f"_output(target_{layer},max_reg & _tile, true);"
+
+                tp.queue(queue_str)
+                logger.debug(
+                    "String queued for {} on layer {}: {}", c.name, layer, queue_str
+                )
+
+            operators.append((layer, operator))
+
+        c.klib.start_changes()
+        logger.info("Starting minkowski on {}", c.name)
+        tp.execute(f"Minkowski {c.name}")
+        c.klib.end_changes()
+
+        for layer, operator in operators:
+            operator.insert()
+
     def apply_custom(
         self,
         c: KCell,
         shape: Callable[
             [int, int | None], kdb.Edge | kdb.Polygon | kdb.Box | kdb.Region
         ],
     ) -> None:
+        """Apply a custom shape based on the section size.
+
+        Args:
+            c: The cell to apply the enclosure to.
+            shape: A function taking the section size in dbu to calculate the
+                full enclosure.
+        """
         for layer, layersec in self.layer_sections.items():
             for sec in layersec.sections:
                 c.shapes(layer).insert(shape(sec.d_max, sec.d_min))
 
-    def apply_bbox(self, c: KCell, ref: int | kdb.Region) -> None:
-        if is_int(ref):
+    def apply_bbox(self, c: KCell, ref: int | kdb.Region | None = None) -> None:
+        """Apply an enclosure based on a bounding box.
+
+        Args:
+            c: Target cell.
+            ref: Reference layer or region (the bounding box). If `None` use
+                :py:attr:~`main_layer` if defined, else throw an error.
+        """
+        if ref is None:
+            ref = self.main_layer
+
+            if ref is None:
+                raise ValueError(
+                    "The enclosure doesn't have  a reference `main_layer` defined."
+                    " Therefore the layer must be defined in calls"
+                )
+
+        if _is_int(ref):
             _ref = c.bbox_per_layer(ref)
-        elif is_Region(ref):
+        elif _is_Region(ref):
             _ref = ref.bbox()
 
         def bbox_reg(d_max: int, d_min: int | None = None) -> kdb.Region:
             reg_max = kdb.Region(_ref)
             reg_max.size(d_max)
             if d_min is None:
                 return reg_max
@@ -581,18 +894,23 @@
             reg_min.size(d_min)
             return reg_max - reg_min
 
         self.apply_custom(c, bbox_reg)
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
+        """Get YAML representation of the enclosure."""
         d = dict(node.enclosures)
         return representer.represent_mapping(cls.yaml_tag, d)
 
     def __str__(self) -> str:
+        """String of enclosure. Use :py:attr:~`name`.
+
+        Use a hash of the sections and main_layer if the name is `None`.
+        """
         if self._name is not None:
             return self._name
         list_to_hash: Any = [
             self.main_layer,
         ]
         for layer, layer_section in self.layer_sections.items():
             list_to_hash.append([str(layer), str(layer_section.sections)])
@@ -643,7 +961,47 @@
             raise ValueError(
                 "The enclosure doesn't have  a reference `main_layer` defined."
                 " Therefore the layer must be defined in calls"
             )
         extrude_path_dynamic(
             target=c, layer=main_layer, path=path, widths=widths, enclosure=self
         )
+
+
+class RegionOperator(kdb.TileOutputReceiver):
+    """Region collector. Just getst the tile and inserts it into the target cell."""
+
+    def __init__(self, cell: KCell, layer: LayerEnum | int) -> None:
+        """Initialization.
+
+        Args:
+            cell: Target cell.
+            layer: Target layer.
+        """
+        self.kcell = cell
+        self.layer = layer
+        self.region = kdb.Region()
+
+    def put(
+        self,
+        ix: int,
+        iy: int,
+        tile: kdb.Box,
+        region: kdb.Region,
+        dbu: float,
+        clip: bool,
+    ) -> None:
+        """Tiling Processor output call.
+
+        Args:
+            ix: x-axis index of tile.
+            iy: y_axis index of tile.
+            tile: The bounding box of the tile.
+            region: The target object of the :py:class:~`klayout.db.TilingProcessor`
+            dbu: dbu used by the processor.
+            clip: Whether the target was clipped to the tile or not.
+        """
+        self.region.insert(region)
+
+    def insert(self) -> None:
+        """Insert the finished region into the cell."""
+        self.kcell.shapes(self.layer).insert(self.region)
```

### Comparing `kfactory-0.6.2/src/kfactory/utils/geo/fill.py` & `kfactory-0.6.3/src/kfactory/utils/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Iterable
 
-from ... import KCell, KLib, LayerEnum, kdb
-from ...config import logger
+from .. import KCell, KLib, LayerEnum, kdb
+from ..config import logger
 
 
 class FillOperator(kdb.TileOutputReceiver):
     def __init__(
         self,
         klib: KLib,
         top_cell: KCell,
```

### Comparing `kfactory-0.6.2/src/kfactory/utils/geo/simplify.py` & `kfactory-0.6.3/src/kfactory/utils/simplify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from ... import kdb
+from .. import kdb
 
 
 def simplify(points: list[kdb.Point], tolerance: float) -> list[kdb.Point]:
     [points[0]]
     if len(points) < 3:
         return points
```

### Comparing `kfactory-0.6.2/src/kfactory/utils/violations.py` & `kfactory-0.6.3/src/kfactory/utils/violations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Utilities to fix DRC violations.
 
 :py:func:~`fix_spacing_tiled` uses :py:func:~`kdb.Region.space_check` to detect
 minimum space violations and then applies a fix.
 """
 
+import os
 from typing import overload
 
 from .. import KCell, LayerEnum, kdb
+from ..config import logger
+
+__all__ = [
+    "fix_spacing_tiled",
+    "fix_spacing_sizing_tiled",
+    "fix_spacing_minkowski_tiled",
+]
 
 
 @overload
 def fix_spacing_tiled(
     c: KCell,
     min_space: int,
     layer: LayerEnum | int,
@@ -45,19 +53,20 @@
 def fix_spacing_tiled(
     c: KCell,
     min_space: int,
     layer: LayerEnum | int,
     metrics: kdb.Metrics = kdb.Metrics.Euclidian,
     ignore_angle: float = 80,
     size_space_check: int = 5,
-    n_threads: int = 4,
+    n_threads: int | None = None,
     tile_size: tuple[float, float] | None = None,
     overlap: float = 3,
     smooth_factor: float = 0.05,
     smooth_absolute: int | None = None,
+    smooth_keep_hv: bool = True,
 ) -> kdb.Region:
     """Fix minimum space violations.
 
     Fix min space issues by running a drc check on the input region and merging
     it with the affcted polygons.
 
     Args:
@@ -83,70 +92,68 @@
 
     """
     if tile_size is None:
         min(25 * min_space, 250)
         tile_size = (30 * min_space * c.klib.dbu, 30 * min_space * c.klib.dbu)
 
     tp = kdb.TilingProcessor()
-    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore
+    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore[misc]
     tp.dbu = c.klib.dbu
-    tp.threads = n_threads
     tp.tile_size(*tile_size)  # tile size in um
     tp.tile_border(min_space * overlap * tp.dbu, min_space * overlap * tp.dbu)
     tp.input("reg", c.klib, c.cell_index(), layer)
+    tp.threads = n_threads or len(os.sched_getaffinity(0))
 
-    fix_reg = kdb.Region()
-
+    fix_reg = RegionOperator()
     tp.output("fix_reg", fix_reg)
 
     if smooth_factor != 0 or smooth_absolute:
+        keep = "true" if smooth_keep_hv else "false"
         smooth = (
             min(int(smooth_factor * min_space), 1)
             if not smooth_absolute
             else smooth_absolute
         )
         queue_str = (
-            "var tile_reg = reg & (_tile & _frame); "
-            f"var sc = tile_reg.space_check({min_space},"
+            f"var sc = reg.space_check({min_space},"
             f" false, Metrics.{metrics.to_s()},"
             f" {ignore_angle}); "
             "var edges = sc.edges(); edges.merge(); "
             f"var r_int = (edges.extended(0, 0, 0, {size_space_check}, true)"
             " + sc.polygons()); r_int.merge();"
-            " r_int.insert(tile_reg.interacting(sc.polygons())); "
-            f"r_int.merge(); r_int.smooth({smooth}); "
+            " r_int.insert(reg.interacting(sc.polygons())); "
+            f"r_int.merge(); r_int.smooth({smooth}, {keep}); "
             f"_output(fix_reg, r_int)"
         )
     else:
         queue_str = (
-            "var tile_reg = reg & (_tile & _frame);"
-            f"var sc = tile_reg.space_check({min_space},"
+            f"var sc = reg.space_check({min_space},"
             f" false, Metrics.{metrics.to_s()},"
             f" {ignore_angle});"
             "var edges = sc.edges(); edges.merge();"
             f"var r_int = (edges.extended(0, 0, 0, {size_space_check}, true)"
             " + sc.polygons()); r_int.merge();"
-            " r_int.insert(tile_reg.interacting(sc.polygons()));"
+            " r_int.insert(reg.interacting(sc.polygons()));"
             "r_int.merge(); _output(fix_reg, r_int)"
         )
 
     tp.queue(queue_str)
 
     c.klib.start_changes()
     tp.execute("Min Space Fix")
     c.klib.end_changes()
 
-    return fix_reg
+    return fix_reg.region
 
 
 def fix_spacing_sizing_tiled(
     c: KCell,
     min_space: int,
     layer: LayerEnum,
-    n_threads: int = 4,
+    n_threads: int | None = None,
     tile_size: tuple[float, float] | None = None,
     overlap: int = 2,
 ) -> kdb.Region:
     """Fix min space issues by using a dilation & erosion.
 
     Args:
         c: Input cell
@@ -163,20 +170,20 @@
         kdb.Region: Region containing the fixes for the violations
 
     """
     tp = kdb.TilingProcessor()
     if tile_size is None:
         size = min_space * 20 * c.klib.dbu
         tile_size = (size, size)
-    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore
+    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore[misc]
     tp.dbu = c.klib.dbu
-    tp.threads = n_threads
     tp.tile_size(*tile_size)  # tile size in um
     tp.tile_border(min_space * overlap * tp.dbu, min_space * overlap * tp.dbu)
     tp.input("reg", c.klib, c.cell_index(), layer)
+    tp.threads = n_threads or len(os.sched_getaffinity(0))
 
     fix_reg = kdb.Region()
 
     tp.output("fix_reg", fix_reg)
 
     queue_str = (
         "var tile_reg= reg & (_tile & _frame);"
@@ -187,7 +194,101 @@
     tp.queue(queue_str)
 
     c.klib.start_changes()
     tp.execute("Min Space Fix")
     c.klib.end_changes()
 
     return fix_reg
+
+
+def fix_spacing_minkowski_tiled(
+    c: KCell,
+    min_space: int,
+    ref: LayerEnum | kdb.Region,
+    n_threads: int | None = None,
+    tile_size: tuple[float, float] | None = None,
+    overlap: int = 2,
+    smooth: int | None = None,
+) -> kdb.Region:
+    """Fix min space issues by using a dilation & erosion with a box.
+
+    Args:
+        c: Input cell
+        min_space: Minimum space rule [dbu]
+        ref: Input layer index or region
+        metrics: The metrics to use to determine the violation edges
+        n_threads: on how many threads to run the check simultaneously
+        tile_size: tuple determining the size of each sub tile (in um), should be big
+            compared to the violation size
+        overlap: how many times bigger to make the tile border in relation to the
+            violation size. Smaller than 1 can lead to errors
+        smooth: Apply smoothening (simplifying) at the end if > 0
+
+    Returns:
+        kdb.Region: Region containing the fixes for the violations
+    """
+    tp = kdb.TilingProcessor()
+    tp.frame = c.dbbox()  # type: ignore[misc]
+    tp.dbu = c.klib.dbu
+    tp.threads = n_threads or len(os.sched_getaffinity(0))
+
+    min_tile_size_rec = 10 * min_space * tp.dbu
+
+    if tile_size is None:
+        tile_size = (min_tile_size_rec * 2, min_tile_size_rec * 2)
+
+    tp.tile_border(min_space * tp.dbu, min_space * tp.dbu)
+
+    tp.tile_size(*tile_size)
+    if isinstance(ref, int):
+        tp.input("main_layer", c.klib, c.cell_index(), ref)
+    else:
+        tp.input("main_layer", ref)
+
+    operator = RegionOperator()
+    tp.output("target", operator)
+    queue_str = (
+        f"var tile_reg = (_tile & _frame).sized({min_space});"
+        f"var shape = Box.new({2*min_space},{2*min_space});"
+        "var reg = main_layer.minkowski_sum(shape).merged();"
+        "reg = tile_reg - (tile_reg - reg).minkowski_sum(shape);"
+        "_output(target, reg & _tile, true);"
+    )
+
+    tp.queue(queue_str)
+    logger.debug("String queued for {}:  {}", c.name, queue_str)
+
+    c.klib.start_changes()
+    logger.info("Starting minkowski on {}", c.name)
+    tp.execute(f"Minkowski {c.name}")
+    c.klib.end_changes()
+
+    return operator.region
+
+
+class RegionOperator(kdb.TileOutputReceiver):
+    """Region collector. Just getst the tile and inserts it into the target cell."""
+
+    def __init__(self) -> None:
+        """Initialization."""
+        self.region = kdb.Region()
+
+    def put(
+        self,
+        ix: int,
+        iy: int,
+        tile: kdb.Box,
+        region: kdb.Region,
+        dbu: float,
+        clip: bool,
+    ) -> None:
+        """Tiling Processor output call.
+
+        Args:
+            ix: x-axis index of tile.
+            iy: y_axis index of tile.
+            tile: The bounding box of the tile.
+            region: The target object of the :py:class:~`klayout.db.TilingProcessor`
+            dbu: dbu used by the processor.
+            clip: Whether the target was clipped to the tile or not.
+        """
+        self.region.insert(region)
```

### Comparing `kfactory-0.6.2/src/kfactory/widgets/interactive.py` & `kfactory-0.6.3/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.6.3/src/kfactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.2
+Version: 0.6.3
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.2
+# KFactory 0.6.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.2/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.6.3/src/kfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/waveguide.py
 docs/_static/complex.png
 docs/_static/klive.webm
 docs/_static/waveguide.png
 docs/notebooks/00_geometry.py
 docs/notebooks/01_references.py
 docs/notebooks/02_DRC.py
+docs/notebooks/03_Enclosures.py
 src/kfactory/__init__.py
 src/kfactory/config.py
 src/kfactory/generic_tech.py
 src/kfactory/kcell.py
 src/kfactory/placer.py
 src/kfactory/port.py
 src/kfactory/py.typed
@@ -53,19 +54,18 @@
 src/kfactory/pcells/dbu/taper.py
 src/kfactory/pcells/dbu/waveguide.py
 src/kfactory/routing/__init__.py
 src/kfactory/routing/electrical.py
 src/kfactory/routing/manhattan.py
 src/kfactory/routing/optical.py
 src/kfactory/utils/__init__.py
+src/kfactory/utils/enclosure.py
+src/kfactory/utils/fill.py
+src/kfactory/utils/simplify.py
 src/kfactory/utils/violations.py
-src/kfactory/utils/geo/__init__.py
-src/kfactory/utils/geo/enclosure.py
-src/kfactory/utils/geo/fill.py
-src/kfactory/utils/geo/simplify.py
 src/kfactory/widgets/__init__.py
 src/kfactory/widgets/interactive.py
 tests/conftest.py
 tests/test_cell.py
 tests/test_cplxcells.py
 tests/test_enclosure.py
 tests/test_extrude.py
```

### Comparing `kfactory-0.6.2/src/kfactory.egg-info/requires.txt` & `kfactory-0.6.3/src/kfactory.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/conftest.py` & `kfactory-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/test_cplxcells.py` & `kfactory-0.6.3/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/test_enclosure.py` & `kfactory-0.6.3/tests/test_enclosure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import kfactory as kf
-from kfactory.utils.geo import extrude_path, extrude_path_dynamic
-import numpy as np
 
 
 @kf.autocell
 def mmi_enc(layer: kf.kcell.LayerEnum, enclosure: kf.utils.Enclosure):
     c = kf.KCell()
     c.shapes(layer).insert(kf.kdb.Box(-10000, -6000, 10000, 6000))
```

### Comparing `kfactory-0.6.2/tests/test_extrude.py` & `kfactory-0.6.3/tests/test_extrude.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import kfactory as kf
-from kfactory.utils.geo import extrude_path, extrude_path_dynamic
+from kfactory.utils import extrude_path, extrude_path_dynamic
 import numpy as np
 
 
 @kf.autocell
 def taper_dyn(
     length: float, width: float, layer: kf.LayerEnum, enclosure: kf.utils.Enclosure
 ) -> kf.KCell:
```

### Comparing `kfactory-0.6.2/tests/test_ports.py` & `kfactory-0.6.3/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/test_rename.py` & `kfactory-0.6.3/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/test_routing.py` & `kfactory-0.6.3/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.2/tests/test_spiral.py` & `kfactory-0.6.3/tests/test_spiral.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
             for _theta in np.linspace(
                 0, theta, int(theta // theta_step + 0.5), endpoint=True
             )
         ]
     ]
 
-    kf.utils.geo.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
+    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
 
     c.create_port(
         name="W0", trans=kf.kdb.Trans(2, False, 0, 0), width=width, layer=layer
     )
 
     match theta:
         case 90:
@@ -87,15 +87,15 @@
         for x, y in [
             [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
             for _theta in np.linspace(
                 0, theta, int(theta // theta_step + 0.5), endpoint=True
             )
         ]
     ]
-    kf.utils.geo.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
+    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
     dp1 = kf.kcell.Port(
         dwidth=width, layer=layer, name="W0", dcplx_trans=kf.kdb.DCplxTrans.R180
     )
     warnings.filterwarnings("ignore")
     c.add_port(dp1)
 
     match theta:
```

