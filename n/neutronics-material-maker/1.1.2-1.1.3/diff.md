# Comparing `tmp/neutronics_material_maker-1.1.2.tar.gz` & `tmp/neutronics_material_maker-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutronics_material_maker-1.1.2.tar", last modified: Mon Jan  9 10:42:05 2023, max compression
+gzip compressed data, was "neutronics_material_maker-1.1.3.tar", last modified: Fri Apr 21 12:45:01 2023, max compression
```

## Comparing `neutronics_material_maker-1.1.2.tar` & `neutronics_material_maker-1.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.061841 neutronics_material_maker-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.053841 neutronics_material_maker-1.1.2/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.053841 neutronics_material_maker-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.053841 neutronics_material_maker-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/.github/workflows/python-publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-01-09 10:42:05.061841 neutronics_material_maker-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/make_docs_from_rst.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/example_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/example_material_from_library.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/example_material_from_mixture.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/docs/source/material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 10:42:05.061841 neutronics_material_maker-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 10:42:04.000000 neutronics_material_maker-1.1.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/src/neutronics_material_maker/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/breeder_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/coolant_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/insulators.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/magnet_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/moderators.json
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/multiplier_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/plasma_material.json
--rw-r--r--   0 runner    (1001) docker     (123)   144857 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/pnnl_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/scintillators.json
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/structural_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)    37032 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/material.py
--rw-r--r--   0 runner    (1001) docker     (123)    17074 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-01-09 10:42:05.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-09 10:42:05.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 10:42:05.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-09 10:42:05.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-09 10:42:05.000000 neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 10:42:05.057841 neutronics_material_maker-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40050 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/tests/test_Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/tests/test_Material_from_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-09 10:41:49.000000 neutronics_material_maker-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.671106 neutronics_material_maker-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/python-publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/make_docs_from_rst.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material_from_library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material_from_mixture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/neutronics_material_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/coolant_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/insulators.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/magnet_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/moderators.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/plasma_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)   144857 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/pnnl_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/scintillators.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/structural_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40030 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_Material_from_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tox.ini
```

### Comparing `neutronics_material_maker-1.1.2/.circleci/config.yml` & `neutronics_material_maker-1.1.3/.circleci/config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     working_directory: ~/repo
 
     steps:
       - checkout
       - run:
           name: install
           command: |
-            conda install -c conda-forge openmc==0.13.2
+            conda install -c conda-forge openmc==0.13.3=*nompi*
             pip install .[density,tests]
  
       # run tests!
       - run:
           name: run tests
           command:
             pytest tests -v --cov=neutronics_material_maker --cov-report term --cov-report html:htmlcov --cov-report xml --junitxml=test-reports/junit.xml
```

### Comparing `neutronics_material_maker-1.1.2/.github/workflows/black.yml` & `neutronics_material_maker-1.1.3/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/.github/workflows/python-publish-testpypi.yml` & `neutronics_material_maker-1.1.3/.github/workflows/python-publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/.github/workflows/python-publish.yml` & `neutronics_material_maker-1.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/.gitignore` & `neutronics_material_maker-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/CITATION.cff` & `neutronics_material_maker-1.1.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/Dockerfile` & `neutronics_material_maker-1.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/LICENSE.txt` & `neutronics_material_maker-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/PKG-INFO` & `neutronics_material_maker-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutronics_material_maker
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for making reproducible materials and standardizing use across several neutronics codes
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2020 UKAEA and neutronics-material-maker contributors
         Copyright (c) 2021 neutronics-material-maker contributors
```

### Comparing `neutronics_material_maker-1.1.2/README.md` & `neutronics_material_maker-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/Makefile` & `neutronics_material_maker-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/conf.py` & `neutronics_material_maker-1.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/example_material.rst` & `neutronics_material_maker-1.1.3/docs/source/example_material.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/example_material_from_library.rst` & `neutronics_material_maker-1.1.3/docs/source/example_material_from_library.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/example_material_from_mixture.rst` & `neutronics_material_maker-1.1.3/docs/source/example_material_from_mixture.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/index.rst` & `neutronics_material_maker-1.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/docs/source/install.rst` & `neutronics_material_maker-1.1.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/pyproject.toml` & `neutronics_material_maker-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/__init__.py` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/breeder_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/coolant_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/coolant_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/magnet_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/magnet_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/multiplier_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/pnnl_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/pnnl_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/scintillators.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/scintillators.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/data/structural_materials.json` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/structural_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/material.py` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,14 @@
         comment: Optional[str] = None,
         zaid_suffix: Optional[str] = None,
         material_id: Optional[int] = None,
         decimal_places: Optional[int] = 8,
         volume_in_cm3: Optional[float] = None,
         additional_end_lines: Optional[Dict[str, List[str]]] = None,
     ):
-
         self.name = name
         self.temperature = temperature
         self.temperature_to_neutronics_code = temperature_to_neutronics_code
         self.pressure = pressure
         self.packing_fraction = packing_fraction
         self.elements = elements
         self.chemical_equation = chemical_equation
@@ -627,34 +626,34 @@
         else:
             openmc_material = openmc.Material(name=self.name)
 
         if self.temperature_to_neutronics_code is True:
             openmc_material.temperature = self.temperature
 
         if self.isotopes is not None:
-
             openmc_material = self._add_isotopes(openmc_material)
 
         if self.elements is not None:
-
             openmc_material = self._add_elements_from_dict(openmc_material)
 
         if self.chemical_equation is not None:
-
             openmc_material = self._add_elements_from_equation(openmc_material)
 
+        # sorts the materials to avoid differently ordered material xml files
+        # resulting in different neutronics results
+        openmc_material._nuclides = sorted(openmc_material._nuclides)
+
         openmc_material = self._add_density(openmc_material)
 
         if original_cross_sections is not None:
             os.environ["OPENMC_CROSS_SECTIONS"] = original_cross_sections
 
         return openmc_material
 
     def _check_enrichment_attributes(self):
-
         if self.enrichment is None:
             return None
 
         elif self.enrichment_type is not None and self.enrichment_target is not None:
             return re.split(r"(\d+)", self.enrichment_target)[0]
 
         elif (
@@ -695,15 +694,14 @@
         """
 
         enrichment_element = self._check_enrichment_attributes()
 
         for element_symbol, element_number in zip(
             self.elements.keys(), self.elements.values()
         ):
-
             if element_symbol == enrichment_element:
                 openmc_material.add_element(
                     element_symbol,
                     element_number,
                     percent_type=self.percent_type,
                     enrichment=self.enrichment,
                     enrichment_target=self.enrichment_target,
@@ -749,15 +747,14 @@
         """
 
         if isinstance(self.density, float):
             density = self.density
 
         # a density equation is being used
         elif isinstance(self.density, str):
-
             if self.density.startswith("PropsSI"):
                 from CoolProp.CoolProp import PropsSI
 
                 # Set any custom symbols for use in asteval
                 asteval_user_symbols = {"PropsSI": PropsSI}
 
                 aeval = asteval.Interpreter(usersyms=asteval_user_symbols)
@@ -786,15 +783,14 @@
             else:
                 self.density = density
 
         elif (
             self.atoms_per_unit_cell is not None
             and self.volume_of_unit_cell_cm3 is not None
         ):
-
             molar_mass = (
                 self._get_atoms_in_crystal() * openmc_material.average_molar_mass
             )
 
             mass = self.atoms_per_unit_cell * molar_mass * atomic_mass_unit_in_g
 
             self.density = mass / self.volume_of_unit_cell_cm3
@@ -827,15 +823,14 @@
                     list_of_fractions.append(float(tokens[counter + 1]))
                 else:
                     list_of_fractions.append(1)
         self.list_of_fractions = list_of_fractions
         return sum(list_of_fractions)
 
     def from_json_file(filename: str, name: str, **kwargs):
-
         with open(filename, "r") as file:
             new_data = json.load(file)
 
         print(new_data)
         print(new_data.keys())
 
         entry = new_data[name]
```

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker/utils.py` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,14 @@
         "c     "
         + name
         + " density "
         + f"{mat.openmc_material.get_mass_density():.{mat.decimal_places}e}"
         + " g/cm3"
     ]
     for i, isotope in enumerate(mat.openmc_material.nuclides):
-
         if i == 0:
             start = f"M{mat.material_id: <5}"
         else:
             start = "      "
 
         if isotope[2] == "ao":
             prefix = "  "
```

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/PKG-INFO` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutronics-material-maker
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for making reproducible materials and standardizing use across several neutronics codes
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2020 UKAEA and neutronics-material-maker contributors
         Copyright (c) 2021 neutronics-material-maker contributors
```

### Comparing `neutronics_material_maker-1.1.2/src/neutronics_material_maker.egg-info/SOURCES.txt` & `neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.2/tests/test_Material.py` & `neutronics_material_maker-1.1.3/tests/test_Material.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import neutronics_material_maker as nmm
 import pytest
 
 
 class test_object_properties(unittest.TestCase):
     def test_error_raised_when_enrichment_and_enrichment_target(self):
         def error_raised_correctly():
-
             test_material = nmm.Material.from_library(
                 name="WC", enrichment=90, enrichment_target=None
             )
             test_material.openmc_material
 
         self.assertRaises(ValueError, error_raised_correctly)
 
@@ -141,15 +140,15 @@
         assert float(fispact_density) == pytest.approx(7.874)
 
     def test_fispact_material(self):
         test_mat = nmm.Material.from_library("Li4SiO4", volume_in_cm3=1.0)
         line_by_line_material = test_mat.fispact_material.split("\n")
 
         assert len(line_by_line_material) == 10
-        assert line_by_line_material[0].startswith("DENSITY 2.31899993235464")
+        assert line_by_line_material[0].startswith("DENSITY 2.318999932")
         assert line_by_line_material[1] == "FUEL 8"
 
         dict_of_fispact_mats = {}
         for entry in line_by_line_material:
             isotope_and_fraction = entry.split()
             dict_of_fispact_mats[isotope_and_fraction[0]] = float(
                 isotope_and_fraction[1]
@@ -165,15 +164,15 @@
         assert dict_of_fispact_mats["O18"] == pytest.approx(9.324307302413e19)
 
     def test_fispact_material_with_volume(self):
         test_mat = nmm.Material.from_library("Li4SiO4", volume_in_cm3=2.0)
         line_by_line_material = test_mat.fispact_material.split("\n")
 
         assert len(line_by_line_material) == 10
-        assert line_by_line_material[0].startswith("DENSITY 2.31899993235464")
+        assert line_by_line_material[0].startswith("DENSITY 2.3189999")
         assert line_by_line_material[1] == "FUEL 8"
 
         dict_of_fispact_mats = {}
         for entry in line_by_line_material:
             isotope_and_fraction = entry.split()
             dict_of_fispact_mats[isotope_and_fraction[0]] = float(
                 isotope_and_fraction[1]
@@ -384,15 +383,14 @@
         assert "      050122.30c  1.1575e-02" in line_by_line_material
         assert "      050124.30c  1.4475e-02" in line_by_line_material
         assert "      050114.30c  1.6500e-03" in line_by_line_material
         assert "      050117.30c  1.9200e-02" in line_by_line_material
         assert "      050116.30c  3.6350e-02" in line_by_line_material
 
     def test_material_creation_from_chemical_formula_with_enrichment(self):
-
         pb_fraction = 3
         li_fraction = 7
         enrichment = 20
 
         lithium_lead_elements = "Li" + str(li_fraction) + "Pb" + str(pb_fraction)
         test_material = nmm.Material.from_library(
             "lithium-lead",
@@ -427,15 +425,14 @@
         )
         assert li7_atom_count == pytest.approx(
             ((100.0 - enrichment) / 100) * (li_fraction / (pb_fraction + li_fraction)),
             rel=0.01,
         )
 
     def test_material_creation_from_chemical_formula_with_enrichment2(self):
-
         pb_fraction = 3
         li_fraction = 7
         enrichment = 20
 
         lithium_lead_elements = "Li" + str(li_fraction) + "Pb" + str(pb_fraction)
         test_material = nmm.Material.from_library(
             "lithium-lead",
@@ -467,15 +464,14 @@
             enrichment * li_fraction / 1000, rel=0.01
         )
         assert li7_atom_count == pytest.approx(
             (100.0 - enrichment) * li_fraction / 1000, rel=0.01
         )
 
     def test_density_of_crystals(self):
-
         # these tests fail because the density value is too far away from calculated value
         # however, this could be becuase the density values are rounded to 2 dp
 
         test_mat = nmm.Material.from_library(name="Li4SiO4")
         assert test_mat.openmc_material.density == pytest.approx(2.32, rel=0.01)
 
         test_mat = nmm.Material.from_library(name="Li2SiO3")
@@ -504,39 +500,36 @@
 
         test_mat = nmm.Material.from_library(name="Zr5Pb3")
         assert test_mat.openmc_material.density == pytest.approx(8.23, rel=0.01)
 
         #  TODO extra checks for all the crystals needed here
 
     def test_density_of_enriched_crystals(self):
-
         test_mat = nmm.Material.from_library(name="Li4SiO4")
         test_mat_enriched = nmm.Material.from_library(
             name="Li4SiO4",
             enrichment=50.0,
             enrichment_target="Li6",
             enrichment_type="ao",
         )
         assert (
             test_mat.openmc_material.density > test_mat_enriched.openmc_material.density
         )
 
     def test_density_of_packed_crystals(self):
-
         test_mat = nmm.Material.from_library(name="Li4SiO4")
         test_mat_packed = nmm.Material.from_library(
             name="Li4SiO4", packing_fraction=0.35
         )
         assert (
             test_mat.openmc_material.density * 0.35
             == test_mat_packed.openmc_material.density
         )
 
     def test_material_creation_from_chemical_formula(self):
-
         pb_fraction = 3
         li_fraction = 7
 
         lithium_lead_elements = "Li" + str(li_fraction) + "Pb" + str(pb_fraction)
         test_material = nmm.Material.from_library(
             "lithium-lead",
             chemical_equation=lithium_lead_elements,
@@ -989,9 +982,8 @@
         with pytest.raises(NameError):
             nmm.Material.from_library(
                 name="Nb3Sn", temperature=373, pressure=1e6, density="os.system('ls')"
             )
 
 
 if __name__ == "__main__":
-
     unittest.main()
```

### Comparing `neutronics_material_maker-1.1.2/tests/test_Material_from_mixture.py` & `neutronics_material_maker-1.1.3/tests/test_Material_from_mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 import neutronics_material_maker as nmm
 import openmc
 import pytest
 
 
 class test_object_properties(unittest.TestCase):
     def test_serpent_from_mixture_type(self):
-
         test_material = nmm.Material.from_mixture(
             name="test_material",
             materials=[
                 nmm.Material.from_library("Li4SiO4"),
                 nmm.Material.from_library("Be12Ti"),
             ],
             fracs=[0.50, 0.50],
             percent_type="vo",
         )
 
         assert len(test_material.serpent_material) > 100
         assert isinstance(test_material.serpent_material, str)
 
     def test_mcnp_from_mixture_type(self):
-
         test_material = nmm.Material.from_mixture(
             name="test_material",
             materials=[
                 nmm.Material.from_library("Li4SiO4"),
                 nmm.Material.from_library("Be12Ti"),
             ],
             fracs=[0.50, 0.50],
@@ -40,15 +38,14 @@
             material_id=2,
         )
 
         assert len(test_material.mcnp_material) > 100
         assert isinstance(test_material.mcnp_material, str)
 
     def test_shift_from_mixture_type(self):
-
         test_material = nmm.Material.from_mixture(
             name="test_material",
             materials=[
                 nmm.Material.from_library("Li4SiO4"),
                 nmm.Material.from_library("Be12Ti"),
             ],
             fracs=[0.50, 0.50],
@@ -57,15 +54,14 @@
             material_id=2,
         )
 
         assert len(test_material.shift_material) > 100
         assert isinstance(test_material.shift_material, str)
 
     def test_fispact_from_mixture_type(self):
-
         test_material = nmm.Material.from_mixture(
             name="test_material",
             materials=[
                 nmm.Material.from_library("Li4SiO4"),
                 nmm.Material.from_library("Be12Ti"),
             ],
             fracs=[0.50, 0.50],
@@ -107,15 +103,14 @@
             percent_type="vo",
         )
 
         assert isinstance(test_material, openmc.Material) is False
         assert isinstance(test_material.openmc_material, openmc.Material)
 
     def test_mutliname_setting(self):
-
         test_material = nmm.Material.from_mixture(
             materials=[
                 nmm.Material.from_library("Pb842Li158", temperature=500),
                 nmm.Material.from_library("SiC"),
             ],
             fracs=[0.5, 0.5],
         )
@@ -165,15 +160,14 @@
             percent_type="vo",
         ).openmc_material
 
         assert test_material_1.density == test_material_2.density
         assert test_material_1.nuclides == test_material_2.nuclides
 
     def test_density_of_mixed_two_packed_crystals(self):
-
         test_material_1 = nmm.Material.from_library(name="Li4SiO4")
         test_material_packed_1 = nmm.Material.from_library(
             name="Li4SiO4", packing_fraction=0.65
         )
         assert (
             test_material_1.openmc_material.density * 0.65
             == test_material_packed_1.openmc_material.density
@@ -198,15 +192,14 @@
         assert mixed_packed_crystals.openmc_material.density == pytest.approx(
             (test_material_1.openmc_material.density * 0.65 * 0.75)
             + (test_material_2.openmc_material.density * 0.35 * 0.25),
             rel=0.01,
         )
 
     def test_density_of_mixed_two_packed_and_non_packed_crystals(self):
-
         test_material_1 = nmm.Material.from_library(name="Li4SiO4")
         test_material_1_packed = nmm.Material.from_library(
             name="Li4SiO4", packing_fraction=0.65
         )
 
         mixed_material = nmm.Material.from_mixture(
             name="mixed_material",
@@ -217,28 +210,26 @@
 
         assert mixed_material.openmc_material.density == pytest.approx(
             (test_material_1.openmc_material.density * 0.2)
             + (test_material_1.openmc_material.density * 0.65 * 0.8)
         )
 
     def test_density_of_mixed_materials_from_density(self):
-
         test_material = nmm.Material.from_library(
             "H2O", temperature=300, pressure=100000
         )
         test_mixed_material = nmm.Material.from_mixture(
             name="test_mixed_material", materials=[test_material], fracs=[1]
         )
 
         assert test_material.openmc_material.density == pytest.approx(
             test_mixed_material.openmc_material.density
         )
 
     def test_density_of_mixed_one_packed_crystal_and_one_non_crystal(self):
-
         test_material_1 = nmm.Material.from_library(
             name="H2O", temperature=300, pressure=100000
         )
 
         test_material_2 = nmm.Material.from_library(name="Li4SiO4")
         test_material_2_packed = nmm.Material.from_library(
             name="Li4SiO4", packing_fraction=0.65
@@ -256,15 +247,14 @@
             == pytest.approx(
                 (test_material_1.openmc_material.density * 0.5)
                 + (test_material_2.openmc_material.density * 0.65 * 0.5)
             )
         )
 
     def test_packing_fraction_for_single_materials(self):
-
         test_material_1 = nmm.Material.from_library("Li4SiO4").openmc_material
 
         test_material_2 = nmm.Material.from_library(
             "Li4SiO4", packing_fraction=1
         ).openmc_material
 
         assert test_material_1.density == test_material_2.density
@@ -278,15 +268,14 @@
         test_material_4 = nmm.Material.from_library(
             "Li4SiO4", packing_fraction=0.75
         ).openmc_material
 
         assert test_material_4.density == pytest.approx(test_material_1.density * 0.75)
 
     def test_packing_fraction_for_from_mixture_function(self):
-
         test_material_5 = nmm.Material.from_mixture(
             name="test_material_5",
             materials=[
                 nmm.Material.from_library("tungsten"),
                 nmm.Material.from_library("eurofer"),
             ],
             fracs=[0.5, 0.5],
@@ -311,15 +300,14 @@
             ],
             fracs=[0.5, 0.5],
         ).openmc_material
 
         assert test_material_7.density == pytest.approx(test_material_5.density * 0.5)
 
     def test_packing_fraction_of_a_from_mixture(self):
-
         test_material_6 = nmm.Material.from_mixture(
             name="test_material_6",
             materials=[
                 nmm.Material.from_library("tungsten", packing_fraction=0.34),
                 nmm.Material.from_library("eurofer", packing_fraction=0.60),
             ],
             fracs=[0.5, 0.5],
@@ -336,15 +324,14 @@
         ).openmc_material
 
         assert test_material_6.get_mass_density() * 0.25 == pytest.approx(
             test_material_7.get_mass_density()
         )
 
     def test_packing_fraction_for_mix_materials_function(self):
-
         test_material_8 = openmc.Material.mix_materials(
             name="test_material_8",
             materials=[
                 nmm.Material.from_library("tungsten").openmc_material,
                 nmm.Material.from_library("eurofer").openmc_material,
             ],
             fracs=[0.5, 0.5],
@@ -380,15 +367,14 @@
             fracs=[0.5, 0.5],
             percent_type="vo",
         )
 
         assert test_material_10.density == pytest.approx(test_material_8.density * 0.5)
 
     def test_from_mixture_vs_mix_materials(self):
-
         test_material_11 = nmm.Material.from_mixture(
             name="test_material_11",
             materials=[
                 nmm.Material.from_library("tungsten"),
                 nmm.Material.from_library("eurofer"),
             ],
             fracs=[0.5, 0.5],
```

### Comparing `neutronics_material_maker-1.1.2/tests/test_utils.py` & `neutronics_material_maker-1.1.3/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 if __name__ == "__main__":
     unittest.main()
 
 
 class test_object_properties(unittest.TestCase):
     def test_additional_lines_multimaterial_mcnp(self):
-
         test_mat1 = nmm.Material.from_library(
             "Li4SiO4", additional_end_lines={"mcnp": ["mat1_additional"]}
         )
         test_mat2 = nmm.Material.from_library(
             "Be12Ti", additional_end_lines={"mcnp": ["mat2_additional"]}
         )
 
@@ -42,15 +41,14 @@
 
         assert test_mat3.mcnp_material.split("\n")[-2] == "extra_mcnp_lin"
         assert test_mat3.serpent_material.split("\n")[-1] == "extra_serpent_lin"
         assert test_mat3.fispact_material.split("\n")[-1] == "extra_fispact_lin"
         assert test_mat3.shift_material.split("\n")[-1] == "extra_shift_lin"
 
     def test_additional_lines_mcnp(self):
-
         test_mat = nmm.Material.from_library(
             "H2O",
             pressure=1e6,
             temperature=393,
             material_id=1,
             additional_end_lines={"mcnp": ["        mt24 lwtr.01"]},
         )
@@ -219,53 +217,48 @@
 
     def test_number_of_materials_in_dict(self):
         import neutronics_material_maker as nmm_again
 
         assert len(nmm_again.AvailableMaterials().keys()) >= 418
 
     def test_dictionary_of_materials_makes_openmc_materials(self):
-
         for mat in nmm.AvailableMaterials().keys():
             print(mat)
             test_mat = nmm.Material.from_library(mat, temperature=300, pressure=5e6)
 
             assert isinstance(test_mat.openmc_material, openmc.Material)
 
     def test_dictionary_of_materials_makes_mcnp_materials(self):
-
         for mat in nmm.AvailableMaterials().keys():
             print(mat)
             test_mat = nmm.Material.from_library(
                 mat, temperature=300, pressure=5e6, material_id=1
             )
 
             assert isinstance(test_mat.mcnp_material, str)
 
     def test_dictionary_of_materials_makes_shift_materials(self):
-
         for mat in nmm.AvailableMaterials().keys():
             print(mat)
             test_mat = nmm.Material.from_library(
                 mat, temperature=300, pressure=5e6, material_id=1
             )
 
             assert isinstance(test_mat.shift_material, str)
 
     def test_dictionary_of_materials_makes_fispact_materials(self):
-
         for mat in nmm.AvailableMaterials().keys():
             print(mat)
             test_mat = nmm.Material.from_library(
                 mat, temperature=300, pressure=5e6, volume_in_cm3=1.5
             )
 
             assert isinstance(test_mat.fispact_material, str)
 
     def test_dictionary_of_materials_makes_serpent_materials(self):
-
         for mat in nmm.AvailableMaterials().keys():
             print(mat)
             test_mat = nmm.Material.from_library(mat, temperature=300, pressure=5e6)
 
             assert isinstance(test_mat.serpent_material, str)
 
     def test_adding_one_material_AddMaterialFromFile(self):
```

