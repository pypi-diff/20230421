# Comparing `tmp/geomm-0.2.0.dev0.tar.gz` & `tmp/geomm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geomm-0.2.0.dev0.tar", last modified: Thu Feb 13 02:05:14 2020, max compression
+gzip compressed data, was "geomm-0.2.1.tar", last modified: Mon Apr 17 20:59:41 2023, max compression
```

## Comparing `geomm-0.2.0.dev0.tar` & `geomm-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,71 @@
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/
--rw-r--r--   0 salotz    (1000) salotz    (1000)       90 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/AUTHORS.org
--rw-r--r--   0 salotz    (1000) salotz    (1000)     1072 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/LICENSE
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      359 2020-02-12 22:45:30.000000 geomm-0.2.0.dev0/MANIFEST.in
--rw-r--r--   0 salotz    (1000) salotz    (1000)      535 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/PKG-INFO
--rw-rw-r--   0 salotz    (1000) salotz    (1000)     1142 2020-02-12 22:46:26.000000 geomm-0.2.0.dev0/README.org
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/envs/
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/envs/base/
--rw-r--r--   0 salotz    (1000) salotz    (1000)       65 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/envs/base/env.yaml
--rw-r--r--   0 salotz    (1000) salotz    (1000)      161 2020-02-13 00:24:51.000000 geomm-0.2.0.dev0/envs/base/requirements.in
--rw-r--r--   0 salotz    (1000) salotz    (1000)      145 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/envs/base/requirements.in~
--rw-------   0 salotz    (1000) salotz    (1000)      328 2020-02-13 00:25:49.000000 geomm-0.2.0.dev0/envs/base/requirements.txt
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      250 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/envs/base/self.requirements.txt
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/envs/dev/
--rw-r--r--   0 salotz    (1000) salotz    (1000)       97 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/envs/dev/env.yaml
--rw-r--r--   0 salotz    (1000) salotz    (1000)      612 2020-02-13 00:24:41.000000 geomm-0.2.0.dev0/envs/dev/requirements.in
--rw-r--r--   0 salotz    (1000) salotz    (1000)      572 2020-02-12 22:49:05.000000 geomm-0.2.0.dev0/envs/dev/requirements.in~
--rw-------   0 salotz    (1000) salotz    (1000)     5004 2020-02-13 00:25:34.000000 geomm-0.2.0.dev0/envs/dev/requirements.txt
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      234 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/envs/dev/self.requirements.txt
--rw-r--r--   0 salotz    (1000) salotz    (1000)       87 2020-02-12 22:45:54.000000 geomm-0.2.0.dev0/pyproject.toml
--rw-rw-r--   0 salotz    (1000) salotz    (1000)       46 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/requirements.in
--rw-r--r--   0 salotz    (1000) salotz    (1000)      184 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/setup.cfg
--rw-r--r--   0 salotz    (1000) salotz    (1000)     2426 2020-02-13 01:44:09.000000 geomm-0.2.0.dev0/setup.py
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/sphinx/
--rw-r--r--   0 salotz    (1000) salotz    (1000)      581 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/sphinx/Makefile
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/sphinx/_build/
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/sphinx/_build/html/
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/sphinx/_build/html/_static/
--rw-r--r--   0 salotz    (1000) salotz    (1000)      286 2020-02-12 23:42:13.000000 geomm-0.2.0.dev0/sphinx/_build/html/_static/file.png
--rw-r--r--   0 salotz    (1000) salotz    (1000)       90 2020-02-12 23:42:13.000000 geomm-0.2.0.dev0/sphinx/_build/html/_static/minus.png
--rw-r--r--   0 salotz    (1000) salotz    (1000)       90 2020-02-12 23:42:13.000000 geomm-0.2.0.dev0/sphinx/_build/html/_static/plus.png
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/sphinx/api/
--rw-r--r--   0 salotz    (1000) salotz    (1000)      173 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm._print_version.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      153 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm._version.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      154 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.arrhenius.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      162 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.box_vectors.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      154 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.centering.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      151 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.centroid.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      151 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.distance.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      166 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.elements.data.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      214 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.elements.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      162 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.free_energy.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      151 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.grouping.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      171 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.kinetic_energy.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      151 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.pyqcprot.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      139 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.rmsd.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      529 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      139 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.sasa.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      160 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.superimpose.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      165 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/geomm.theobald_qcp.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       52 2020-02-13 00:46:33.000000 geomm-0.2.0.dev0/sphinx/api/modules.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)     6897 2020-02-13 01:44:49.000000 geomm-0.2.0.dev0/sphinx/conf.py
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      696 2020-02-13 00:42:03.000000 geomm-0.2.0.dev0/sphinx/index.rst
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/sphinx/source/
--rw-r--r--   0 salotz    (1000) salotz    (1000)      544 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/changelog.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)     8192 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/dev_guide.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      284 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/general_info.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      141 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/glossary.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      567 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/installation.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)      635 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/introduction.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       34 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/news.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       24 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/quick_start.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       47 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/reference.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       41 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/troubleshooting.rst
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/sphinx/source/tutorials/
--rw-r--r--   0 salotz    (1000) salotz    (1000)       34 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/tutorials/example.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       77 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/tutorials/index.rst
--rw-r--r--   0 salotz    (1000) salotz    (1000)       81 2020-02-13 00:46:32.000000 geomm-0.2.0.dev0/sphinx/source/users_guide.rst
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.314063 geomm-0.2.0.dev0/src/
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/src/geomm/
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      154 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/src/geomm/__init__.py
--rw-rw-r--   0 salotz    (1000) salotz    (1000)       86 2020-02-12 21:35:09.000000 geomm-0.2.0.dev0/src/geomm/_print_version.py
--rw-rw-r--   0 salotz    (1000) salotz    (1000)      616 2020-02-13 01:44:31.000000 geomm-0.2.0.dev0/src/geomm/_version.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)      954 2020-02-13 00:23:50.000000 geomm-0.2.0.dev0/src/geomm/arrhenius.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     3867 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/box_vectors.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     5877 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/centering.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)      683 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/centroid.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)       90 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/distance.py
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/src/geomm/elements/
--rw-r--r--   0 salotz    (1000) salotz    (1000)        0 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/elements/__init__.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     7301 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/elements/data.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     2666 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/free_energy.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     3774 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/grouping.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)      373 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/kinetic_energy.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)   475448 2020-02-12 23:42:33.000000 geomm-0.2.0.dev0/src/geomm/pyqcprot.c
--rw-r--r--   0 salotz    (1000) salotz    (1000)    16054 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/pyqcprot.pyx
--rw-r--r--   0 salotz    (1000) salotz    (1000)     1083 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/rmsd.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     4505 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/sasa.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     5851 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/superimpose.py
--rw-r--r--   0 salotz    (1000) salotz    (1000)     2592 2019-09-25 15:39:27.000000 geomm-0.2.0.dev0/src/geomm/theobald_qcp.py
-drwxr-xr-x   0 salotz    (1000) salotz    (1000)        0 2020-02-13 02:05:14.318063 geomm-0.2.0.dev0/src/geomm.egg-info/
--rw-r--r--   0 salotz    (1000) salotz    (1000)      535 2020-02-13 02:05:14.000000 geomm-0.2.0.dev0/src/geomm.egg-info/PKG-INFO
--rw-r--r--   0 salotz    (1000) salotz    (1000)     2090 2020-02-13 02:05:14.000000 geomm-0.2.0.dev0/src/geomm.egg-info/SOURCES.txt
--rw-r--r--   0 salotz    (1000) salotz    (1000)        1 2020-02-13 02:05:14.000000 geomm-0.2.0.dev0/src/geomm.egg-info/dependency_links.txt
--rw-r--r--   0 salotz    (1000) salotz    (1000)       24 2020-02-13 02:05:14.000000 geomm-0.2.0.dev0/src/geomm.egg-info/requires.txt
--rw-r--r--   0 salotz    (1000) salotz    (1000)        6 2020-02-13 02:05:14.000000 geomm-0.2.0.dev0/src/geomm.egg-info/top_level.txt
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.987165 geomm-0.2.1/
+-rw-r--r--   0 alexrd     (501) staff       (20)       90 2023-04-17 20:58:25.000000 geomm-0.2.1/AUTHORS.org
+-rw-r--r--   0 alexrd     (501) staff       (20)     1072 2023-04-17 20:58:25.000000 geomm-0.2.1/LICENSE
+-rw-r--r--   0 alexrd     (501) staff       (20)      451 2023-04-17 20:58:25.000000 geomm-0.2.1/MANIFEST.in
+-rw-r--r--   0 alexrd     (501) staff       (20)      539 2023-04-17 20:59:41.987338 geomm-0.2.1/PKG-INFO
+-rw-r--r--   0 alexrd     (501) staff       (20)     1408 2023-04-17 20:58:25.000000 geomm-0.2.1/README.org
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.955797 geomm-0.2.1/envs/
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.963344 geomm-0.2.1/envs/base/
+-rw-r--r--   0 alexrd     (501) staff       (20)       65 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/base/env.yaml
+-rw-r--r--   0 alexrd     (501) staff       (20)      161 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/base/requirements.in
+-rw-r--r--   0 alexrd     (501) staff       (20)      328 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/base/requirements.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)      250 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/base/self.requirements.txt
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.965344 geomm-0.2.1/envs/dev/
+-rw-r--r--   0 alexrd     (501) staff       (20)       40 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/dev/dev.requirements.list
+-rw-r--r--   0 alexrd     (501) staff       (20)      572 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/dev/requirements.in
+-rw-r--r--   0 alexrd     (501) staff       (20)     7837 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/dev/requirements.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)      234 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/dev/self.requirements.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)        3 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/dev/tools.requirements.txt
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.965819 geomm-0.2.1/envs/test_install/
+-rw-r--r--   0 alexrd     (501) staff       (20)        3 2023-04-17 20:58:25.000000 geomm-0.2.1/envs/test_install/tools.requirements.txt
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.969176 geomm-0.2.1/info/
+-rw-r--r--   0 alexrd     (501) staff       (20)      934 2023-04-17 20:58:25.000000 geomm-0.2.1/info/README.org
+-rw-r--r--   0 alexrd     (501) staff       (20)     1042 2023-04-17 20:58:25.000000 geomm-0.2.1/info/changelog.org
+-rw-r--r--   0 alexrd     (501) staff       (20)     9689 2023-04-17 20:58:25.000000 geomm-0.2.1/info/dev_guide.org
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.969848 geomm-0.2.1/info/examples/
+-rw-r--r--   0 alexrd     (501) staff       (20)        0 2023-04-17 20:58:25.000000 geomm-0.2.1/info/examples/.keep
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.970933 geomm-0.2.1/info/examples/format_conversion/
+-rw-r--r--   0 alexrd     (501) staff       (20)       42 2023-04-17 20:58:25.000000 geomm-0.2.1/info/examples/format_conversion/conversion.requirements.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)     2602 2023-04-17 20:58:25.000000 geomm-0.2.1/info/examples/format_conversion/convert_pdb.py
+-rw-r--r--   0 alexrd     (501) staff       (20)   212871 2023-04-17 20:58:25.000000 geomm-0.2.1/info/examples/lysozyme_pxylene.pdb
+-rw-r--r--   0 alexrd     (501) staff       (20)      602 2023-04-17 20:58:25.000000 geomm-0.2.1/info/general_info.org
+-rw-r--r--   0 alexrd     (501) staff       (20)      586 2023-04-17 20:58:25.000000 geomm-0.2.1/info/installation.org
+-rw-r--r--   0 alexrd     (501) staff       (20)    17638 2023-04-17 20:58:25.000000 geomm-0.2.1/info/introduction.org
+-rw-r--r--   0 alexrd     (501) staff       (20)     1688 2023-04-17 20:58:25.000000 geomm-0.2.1/info/news.org
+-rw-r--r--   0 alexrd     (501) staff       (20)      733 2023-04-17 20:58:25.000000 geomm-0.2.1/info/reference.rst
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.971885 geomm-0.2.1/info/tutorials/
+-rw-r--r--   0 alexrd     (501) staff       (20)       20 2023-04-17 20:58:25.000000 geomm-0.2.1/info/tutorials/example.org
+-rw-r--r--   0 alexrd     (501) staff       (20)       77 2023-04-17 20:58:25.000000 geomm-0.2.1/info/tutorials/index.rst
+-rw-r--r--   0 alexrd     (501) staff       (20)       87 2023-04-17 20:58:25.000000 geomm-0.2.1/pyproject.toml
+-rw-r--r--   0 alexrd     (501) staff       (20)       75 2023-04-17 20:58:25.000000 geomm-0.2.1/requirements.in
+-rw-r--r--   0 alexrd     (501) staff       (20)      339 2023-04-17 20:59:41.988237 geomm-0.2.1/setup.cfg
+-rw-r--r--   0 alexrd     (501) staff       (20)     2517 2023-04-17 20:58:25.000000 geomm-0.2.1/setup.py
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.957120 geomm-0.2.1/src/
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.988661 geomm-0.2.1/src/geomm/
+-rw-r--r--   0 alexrd     (501) staff       (20)      212 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/__init__.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      104 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/_print_version.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      497 2023-04-17 20:59:41.988747 geomm-0.2.1/src/geomm/_version.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      954 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/arrhenius.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     3867 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/box_vectors.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     5877 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/centering.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      683 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/centroid.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      769 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/distance.py
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.986828 geomm-0.2.1/src/geomm/elements/
+-rw-r--r--   0 alexrd     (501) staff       (20)        0 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/elements/__init__.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     7301 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/elements/data.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     2666 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/free_energy.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     3774 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/grouping.py
+-rw-r--r--   0 alexrd     (501) staff       (20)      373 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/kinetic_energy.py
+-rw-r--r--   0 alexrd     (501) staff       (20)   402883 2023-04-17 20:59:40.000000 geomm-0.2.1/src/geomm/pyqcprot.c
+-rw-r--r--   0 alexrd     (501) staff       (20)    16054 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/pyqcprot.pyx
+-rw-r--r--   0 alexrd     (501) staff       (20)     1083 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/rmsd.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     4505 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/sasa.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     5851 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/superimpose.py
+-rw-r--r--   0 alexrd     (501) staff       (20)     2592 2023-04-17 20:58:25.000000 geomm-0.2.1/src/geomm/theobald_qcp.py
+drwxr-xr-x   0 alexrd     (501) staff       (20)        0 2023-04-17 20:59:41.986137 geomm-0.2.1/src/geomm.egg-info/
+-rw-r--r--   0 alexrd     (501) staff       (20)      539 2023-04-17 20:59:41.000000 geomm-0.2.1/src/geomm.egg-info/PKG-INFO
+-rw-r--r--   0 alexrd     (501) staff       (20)     1378 2023-04-17 20:59:41.000000 geomm-0.2.1/src/geomm.egg-info/SOURCES.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)        1 2023-04-17 20:59:41.000000 geomm-0.2.1/src/geomm.egg-info/dependency_links.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)       37 2023-04-17 20:59:41.000000 geomm-0.2.1/src/geomm.egg-info/requires.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)        6 2023-04-17 20:59:41.000000 geomm-0.2.1/src/geomm.egg-info/top_level.txt
+-rw-r--r--   0 alexrd     (501) staff       (20)    68611 2023-04-17 20:58:25.000000 geomm-0.2.1/versioneer.py
```

### Comparing `geomm-0.2.0.dev0/LICENSE` & `geomm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/PKG-INFO` & `geomm-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: geomm
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: A simple no-nonsense library for computing common geometry on macromolecular systems.
 Home-page: https://github.com/ADicksonLab/geomm
 Author: Samuel D. Lotz
 Author-email: samuel.lotz@salotz.info
 License: MIT
-Description: UNKNOWN
 Keywords: geometry chemistry macromolecules protein structural-informatics
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
+License-File: LICENSE
+License-File: AUTHORS.org
```

### Comparing `geomm-0.2.0.dev0/envs/dev/requirements.in~` & `geomm-0.2.1/envs/dev/requirements.in`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/setup.py` & `geomm-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 from os.path import join
 from os.path import splitext
 
 from setuptools import setup, find_packages
 
 import itertools as it
 
+import versioneer
+
 # package specific imports
 from Cython.Build import cythonize
 import numpy as np
 
 # the basic needed requirements for a package
 base_requirements = [
     'numpy',
     'scipy',
     'pint',
+    'scikit-learn'
 ]
 
 # extras requirements list
 
 # SNIPPET: example extra requirement
 # example_extra_requirements = ['requests']
 # extras = [example_extra_requirements,]
@@ -39,15 +42,15 @@
 
 # combination of all the extras requirements
 _all_requirements = [[base_requirements]] + extras
 all_requirements = it.chain.from_iterable(_all_requirements)
 
 setup(
     name='geomm',
-    version='0.2.0.dev0',
+    version=versioneer.get_version(),
     author="Samuel D. Lotz",
     author_email="samuel.lotz@salotz.info",
     description="A simple no-nonsense library for computing common geometry on macromolecular systems.",
     #long_description=open('README.org').read(),
     license="MIT",
     url="https://github.com/ADicksonLab/geomm",
     classifiers=[
@@ -61,14 +64,16 @@
     setup_requires=[
         'pytest-runner',
         'numpy',
         'cython',
     ],
     tests_require=['pytest', 'tox'],
 
+    cmdclass=versioneer.get_cmdclass(),
+
     include_dirs=[np.get_include()],
     ext_modules = cythonize("src/geomm/pyqcprot.pyx"),
 
 
     # package
     packages=find_packages(where='src'),
```

### Comparing `geomm-0.2.0.dev0/src/geomm/arrhenius.py` & `geomm-0.2.1/src/geomm/arrhenius.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/box_vectors.py` & `geomm-0.2.1/src/geomm/box_vectors.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/centering.py` & `geomm-0.2.1/src/geomm/centering.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/centroid.py` & `geomm-0.2.1/src/geomm/centroid.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/elements/data.py` & `geomm-0.2.1/src/geomm/elements/data.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/free_energy.py` & `geomm-0.2.1/src/geomm/free_energy.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/grouping.py` & `geomm-0.2.1/src/geomm/grouping.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/pyqcprot.c` & `geomm-0.2.1/src/geomm/pyqcprot.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-/* Generated by Cython 0.29.15 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "geomm.pyqcprot",
         "sources": [
             "src/geomm/pyqcprot.pyx"
         ]
     },
     "module_name": "geomm.pyqcprot"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_15"
-#define CYTHON_HEX_VERSION 0x001D0FF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -56,14 +58,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -92,18 +95,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -133,18 +140,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -156,61 +212,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -319,17 +386,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -435,24 +561,36 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #else
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -493,26 +631,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -538,21 +685,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -566,16 +713,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -585,19 +734,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -605,15 +753,21 @@
 
 #define __PYX_HAVE__geomm__pyqcprot
 #define __PYX_HAVE_API__geomm__pyqcprot
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include "math.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -703,14 +857,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -878,195 +1033,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":779
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":786
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":791
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":802
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":806
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":809
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":813
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1093,42 +1248,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":817
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":819
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1308,26 +1463,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1351,21 +1506,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
@@ -1381,37 +1544,14 @@
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1436,23 +1576,34 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -1499,16 +1650,18 @@
     static void __Pyx_ReleaseBuffer(Py_buffer *view);
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
@@ -1600,20 +1753,20 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
@@ -1661,29 +1814,36 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'geomm.pyqcprot' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "geomm.pyqcprot"
 extern int __pyx_module_is_main_geomm__pyqcprot;
 int __pyx_module_is_main_geomm__pyqcprot = 0;
 
 /* Implementation of 'geomm.pyqcprot' */
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_A[] = "A";
 static const char __pyx_k_C[] = "C";
 static const char __pyx_k_N[] = "N";
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_i[] = "i";
@@ -1771,61 +1931,49 @@
 static const char __pyx_k_coords1[] = "coords1";
 static const char __pyx_k_coords2[] = "coords2";
 static const char __pyx_k_float64[] = "float64";
 static const char __pyx_k_weights[] = "weights";
 static const char __pyx_k_evalprec[] = "evalprec";
 static const char __pyx_k_evecprec[] = "evecprec";
 static const char __pyx_k_mxEigenV[] = "mxEigenV";
-static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_a1122_1221[] = "a1122_1221";
 static const char __pyx_k_a1123_1321[] = "a1123_1321";
 static const char __pyx_k_a1124_1421[] = "a1124_1421";
 static const char __pyx_k_a1223_1322[] = "a1223_1322";
 static const char __pyx_k_a1224_1422[] = "a1224_1422";
 static const char __pyx_k_a1324_1423[] = "a1324_1423";
 static const char __pyx_k_a3142_4132[] = "a3142_4132";
 static const char __pyx_k_a3143_4133[] = "a3143_4133";
 static const char __pyx_k_a3144_4134[] = "a3144_4134";
 static const char __pyx_k_a3243_4233[] = "a3243_4233";
 static const char __pyx_k_a3244_4234[] = "a3244_4234";
 static const char __pyx_k_a3344_4334[] = "a3344_4334";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_InnerProduct[] = "InnerProduct";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_SyzSzymSyySzz2[] = "SyzSzymSyySzz2";
 static const char __pyx_k_geomm_pyqcprot[] = "geomm.pyqcprot";
 static const char __pyx_k_Sxy2Sxz2Syx2Szx2[] = "Sxy2Sxz2Syx2Szx2";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Sxx2Syy2Szz2Syz2Szy2[] = "Sxx2Syy2Szz2Syz2Szy2";
 static const char __pyx_k_src_geomm_pyqcprot_pyx[] = "src/geomm/pyqcprot.pyx";
 static const char __pyx_k_FastCalcRMSDAndRotation[] = "FastCalcRMSDAndRotation";
 static const char __pyx_k_CalcRMSDRotationalMatrix[] = "CalcRMSDRotationalMatrix";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_Fast_QCP_RMSD_structure_alignme[] = "\nFast QCP RMSD structure alignment --- :mod:`MDAnalysis.lib.qcprot`\n==================================================================\n\n:Author:   Joshua L. Adelman, University of Pittsburgh\n:Author:   Robert R. Delgado, Cornell University and Arizona State University\n:Contact:  jla65@pitt.edu\n:Year:     2011, 2016\n:Licence:  BSD\n\nPyQCPROT_ is a python/cython implementation of Douglas Theobald's QCP\nmethod for calculating the minimum RMSD between two structures\n[Theobald2005]_ and determining the optimal least-squares rotation\nmatrix [Liu2010]_.\n\nA full description of the method, along with the original C implementation can\nbe found at http://theobald.brandeis.edu/qcp/\n\nSee Also\n--------\nMDAnalysis.analysis.align:\n    Align structures using :func:`CalcRMSDRotationalMatrix`\nMDAnalysis.analysis.rms.rmsd:\n    Calculate the RMSD between two structures using\n    :func:`CalcRMSDRotationalMatrix`\n\n\n.. versionchanged:: 0.16.0\n   Call signatures were changed to directly interface with MDAnalysis\n   coordinate arrays: shape (N, 3)\n\nReferences\n----------\n\nIf you use this QCP rotation calculation method in a publication, please\nreference:\n\n.. [Theobald2005] Douglas L. Theobald (2005)\n   \"Rapid calculation of RMSD using a quaternion-based characteristic\n   polynomial.\"  Acta Crystallographica A 61(4):478-480.\n\n.. [Liu2010] Pu Liu, Dmitris K. Agrafiotis, and Douglas L. Theobald (2010)\n   \"Fast determination of the optimal rotational matrix for macromolecular\n   superpositions.\"  J. Comput. Chem. 31, 1561-1563.\n\n.. _PyQCPROT: https://github.com/synapticarbors/pyqcprot\n\n\nFunctions\n---------\n\nUsers will typically use the :func:`CalcRMSDRotationalMatrix` function.\n\n.. autofunction:: CalcRMSDRotationalMatrix\n\n.. autofunction:: InnerProduct\n\n.. autofunction:: FastCalcRMSDAndRotation\n\n";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_n_s_A;
 static PyObject *__pyx_n_s_C;
 static PyObject *__pyx_n_s_CalcRMSDRotationalMatrix;
 static PyObject *__pyx_n_s_E0;
 static PyObject *__pyx_n_s_FastCalcRMSDAndRotation;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_G1;
 static PyObject *__pyx_n_s_G2;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_n_s_InnerProduct;
 static PyObject *__pyx_n_s_N;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_Sxx;
 static PyObject *__pyx_n_s_Sxx2;
 static PyObject *__pyx_n_s_Sxx2Syy2Szz2Syz2Szy2;
 static PyObject *__pyx_n_s_SxxmSyy;
 static PyObject *__pyx_n_s_SxxpSyy;
 static PyObject *__pyx_n_s_Sxy;
 static PyObject *__pyx_n_s_Sxy2;
@@ -1847,15 +1995,14 @@
 static PyObject *__pyx_n_s_SyzpSzy;
 static PyObject *__pyx_n_s_Szx;
 static PyObject *__pyx_n_s_Szx2;
 static PyObject *__pyx_n_s_Szy;
 static PyObject *__pyx_n_s_Szy2;
 static PyObject *__pyx_n_s_Szz;
 static PyObject *__pyx_n_s_Szz2;
-static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_a11;
 static PyObject *__pyx_n_s_a1122_1221;
 static PyObject *__pyx_n_s_a1123_1321;
 static PyObject *__pyx_n_s_a1124_1421;
 static PyObject *__pyx_n_s_a12;
 static PyObject *__pyx_n_s_a1223_1322;
@@ -1897,16 +2044,14 @@
 static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_geomm_pyqcprot;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_mxEigenV;
 static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
 static PyObject *__pyx_n_s_normq;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_oldg;
 static PyObject *__pyx_n_s_q1;
@@ -1917,15 +2062,14 @@
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_ref;
 static PyObject *__pyx_n_s_rms;
 static PyObject *__pyx_n_s_rmsd;
 static PyObject *__pyx_n_s_rot;
 static PyObject *__pyx_kp_s_src_geomm_pyqcprot_pyx;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_weight;
 static PyObject *__pyx_n_s_weights;
 static PyObject *__pyx_n_s_x1;
 static PyObject *__pyx_n_s_x2;
 static PyObject *__pyx_n_s_xy;
 static PyObject *__pyx_n_s_y1;
 static PyObject *__pyx_n_s_y2;
@@ -1933,32 +2077,25 @@
 static PyObject *__pyx_n_s_z1;
 static PyObject *__pyx_n_s_z2;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_n_s_zx;
 static PyObject *__pyx_pf_5geomm_8pyqcprot_InnerProduct(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_A, PyArrayObject *__pyx_v_coords1, PyArrayObject *__pyx_v_coords2, int __pyx_v_N, PyArrayObject *__pyx_v_weight); /* proto */
 static PyObject *__pyx_pf_5geomm_8pyqcprot_2CalcRMSDRotationalMatrix(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_ref, PyArrayObject *__pyx_v_conf, int __pyx_v_N, PyArrayObject *__pyx_v_rot, PyArrayObject *__pyx_v_weights); /* proto */
 static PyObject *__pyx_pf_5geomm_8pyqcprot_4FastCalcRMSDAndRotation(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rot, PyArrayObject *__pyx_v_A, double __pyx_v_E0, int __pyx_v_N); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_9;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_codeobj__10;
-static PyObject *__pyx_codeobj__12;
-static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
 /* Late includes */
 
 /* "geomm/pyqcprot.pyx":150
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def InnerProduct(np.ndarray[np.float64_t, ndim=1] A,             # <<<<<<<<<<<<<<
  *                  np.ndarray[np.float64_t, ndim=2] coords1,
@@ -1971,14 +2108,17 @@
 static PyMethodDef __pyx_mdef_5geomm_8pyqcprot_1InnerProduct = {"InnerProduct", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5geomm_8pyqcprot_1InnerProduct, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5geomm_8pyqcprot_InnerProduct};
 static PyObject *__pyx_pw_5geomm_8pyqcprot_1InnerProduct(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_A = 0;
   PyArrayObject *__pyx_v_coords1 = 0;
   PyArrayObject *__pyx_v_coords2 = 0;
   int __pyx_v_N;
   PyArrayObject *__pyx_v_weight = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("InnerProduct (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_A,&__pyx_n_s_coords1,&__pyx_n_s_coords2,&__pyx_n_s_N,&__pyx_n_s_weight,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2086,80 +2226,28 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_coords2;
   __Pyx_Buffer __pyx_pybuffer_coords2;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_weight;
   __Pyx_Buffer __pyx_pybuffer_weight;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
-  Py_ssize_t __pyx_t_2;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  Py_ssize_t __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  unsigned int __pyx_t_6;
+  size_t __pyx_t_7;
+  size_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  int __pyx_t_10;
-  int __pyx_t_11;
-  int __pyx_t_12;
-  int __pyx_t_13;
-  unsigned int __pyx_t_14;
-  size_t __pyx_t_15;
-  size_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  size_t __pyx_t_18;
-  size_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
-  size_t __pyx_t_21;
-  size_t __pyx_t_22;
-  Py_ssize_t __pyx_t_23;
-  size_t __pyx_t_24;
-  Py_ssize_t __pyx_t_25;
-  size_t __pyx_t_26;
-  Py_ssize_t __pyx_t_27;
-  size_t __pyx_t_28;
-  Py_ssize_t __pyx_t_29;
-  size_t __pyx_t_30;
-  Py_ssize_t __pyx_t_31;
-  size_t __pyx_t_32;
-  Py_ssize_t __pyx_t_33;
-  size_t __pyx_t_34;
-  Py_ssize_t __pyx_t_35;
-  size_t __pyx_t_36;
-  Py_ssize_t __pyx_t_37;
-  Py_ssize_t __pyx_t_38;
-  Py_ssize_t __pyx_t_39;
-  Py_ssize_t __pyx_t_40;
-  Py_ssize_t __pyx_t_41;
-  Py_ssize_t __pyx_t_42;
-  Py_ssize_t __pyx_t_43;
-  Py_ssize_t __pyx_t_44;
-  Py_ssize_t __pyx_t_45;
-  size_t __pyx_t_46;
-  Py_ssize_t __pyx_t_47;
-  size_t __pyx_t_48;
-  Py_ssize_t __pyx_t_49;
-  size_t __pyx_t_50;
-  Py_ssize_t __pyx_t_51;
-  size_t __pyx_t_52;
-  Py_ssize_t __pyx_t_53;
-  size_t __pyx_t_54;
-  Py_ssize_t __pyx_t_55;
-  size_t __pyx_t_56;
-  Py_ssize_t __pyx_t_57;
-  Py_ssize_t __pyx_t_58;
-  Py_ssize_t __pyx_t_59;
-  Py_ssize_t __pyx_t_60;
-  Py_ssize_t __pyx_t_61;
-  Py_ssize_t __pyx_t_62;
-  Py_ssize_t __pyx_t_63;
-  Py_ssize_t __pyx_t_64;
-  Py_ssize_t __pyx_t_65;
-  Py_ssize_t __pyx_t_66;
-  PyObject *__pyx_t_67 = NULL;
+  size_t __pyx_t_10;
+  Py_ssize_t __pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("InnerProduct", 0);
   __pyx_pybuffer_A.pybuffer.buf = NULL;
   __pyx_pybuffer_A.refcount = 0;
   __pyx_pybuffernd_A.data = NULL;
   __pyx_pybuffernd_A.rcbuffer = &__pyx_pybuffer_A;
   __pyx_pybuffer_coords1.pybuffer.buf = NULL;
   __pyx_pybuffer_coords1.refcount = 0;
@@ -2217,237 +2305,237 @@
  * 
  *     A[0] = A[1] = A[2] = A[3] = A[4] = A[5] = A[6] = A[7] = A[8] = 0.0             # <<<<<<<<<<<<<<
  * 
  *     if (weight is not None):
  */
   __pyx_t_1 = 0;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_2 = 1;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_2, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_3 = 2;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_4 = 3;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_5 = 4;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_6 = 5;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_7 = 6;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_8 = 7;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
-  __pyx_t_9 = 8;
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 1;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 2;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 3;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 4;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 5;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 6;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 7;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
+  __pyx_t_1 = 8;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_A.diminfo[0].strides) = 0.0;
 
   /* "geomm/pyqcprot.pyx":197
  *     A[0] = A[1] = A[2] = A[3] = A[4] = A[5] = A[6] = A[7] = A[8] = 0.0
  * 
  *     if (weight is not None):             # <<<<<<<<<<<<<<
  *         for i in range(N):
  *             x1 = weight[i] * coords1[i, 0]
  */
-  __pyx_t_10 = (((PyObject *)__pyx_v_weight) != Py_None);
-  __pyx_t_11 = (__pyx_t_10 != 0);
-  if (__pyx_t_11) {
+  __pyx_t_2 = (((PyObject *)__pyx_v_weight) != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "geomm/pyqcprot.pyx":198
  * 
  *     if (weight is not None):
  *         for i in range(N):             # <<<<<<<<<<<<<<
  *             x1 = weight[i] * coords1[i, 0]
  *             y1 = weight[i] * coords1[i, 1]
  */
-    __pyx_t_12 = __pyx_v_N;
-    __pyx_t_13 = __pyx_t_12;
-    for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-      __pyx_v_i = __pyx_t_14;
+    __pyx_t_4 = __pyx_v_N;
+    __pyx_t_5 = __pyx_t_4;
+    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
+      __pyx_v_i = __pyx_t_6;
 
       /* "geomm/pyqcprot.pyx":199
  *     if (weight is not None):
  *         for i in range(N):
  *             x1 = weight[i] * coords1[i, 0]             # <<<<<<<<<<<<<<
  *             y1 = weight[i] * coords1[i, 1]
  *             z1 = weight[i] * coords1[i, 2]
  */
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_16 = __pyx_v_i;
-      __pyx_t_17 = 0;
-      __pyx_v_x1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_coords1.diminfo[1].strides)));
+      __pyx_t_7 = __pyx_v_i;
+      __pyx_t_8 = __pyx_v_i;
+      __pyx_t_1 = 0;
+      __pyx_v_x1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_1, __pyx_pybuffernd_coords1.diminfo[1].strides)));
 
       /* "geomm/pyqcprot.pyx":200
  *         for i in range(N):
  *             x1 = weight[i] * coords1[i, 0]
  *             y1 = weight[i] * coords1[i, 1]             # <<<<<<<<<<<<<<
  *             z1 = weight[i] * coords1[i, 2]
  * 
  */
-      __pyx_t_18 = __pyx_v_i;
-      __pyx_t_19 = __pyx_v_i;
-      __pyx_t_20 = 1;
-      __pyx_v_y1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_20, __pyx_pybuffernd_coords1.diminfo[1].strides)));
+      __pyx_t_8 = __pyx_v_i;
+      __pyx_t_7 = __pyx_v_i;
+      __pyx_t_1 = 1;
+      __pyx_v_y1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_1, __pyx_pybuffernd_coords1.diminfo[1].strides)));
 
       /* "geomm/pyqcprot.pyx":201
  *             x1 = weight[i] * coords1[i, 0]
  *             y1 = weight[i] * coords1[i, 1]
  *             z1 = weight[i] * coords1[i, 2]             # <<<<<<<<<<<<<<
  * 
  *             G1 += x1 * coords1[i, 0] + y1 * coords1[i, 1] + z1 * coords1[i, 2]
  */
-      __pyx_t_21 = __pyx_v_i;
-      __pyx_t_22 = __pyx_v_i;
-      __pyx_t_23 = 2;
-      __pyx_v_z1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_coords1.diminfo[1].strides)));
+      __pyx_t_7 = __pyx_v_i;
+      __pyx_t_8 = __pyx_v_i;
+      __pyx_t_1 = 2;
+      __pyx_v_z1 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_weight.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_1, __pyx_pybuffernd_coords1.diminfo[1].strides)));
 
       /* "geomm/pyqcprot.pyx":203
  *             z1 = weight[i] * coords1[i, 2]
  * 
  *             G1 += x1 * coords1[i, 0] + y1 * coords1[i, 1] + z1 * coords1[i, 2]             # <<<<<<<<<<<<<<
  * 
  *             x2 = coords2[i, 0]
  */
-      __pyx_t_24 = __pyx_v_i;
-      __pyx_t_25 = 0;
-      __pyx_t_26 = __pyx_v_i;
-      __pyx_t_27 = 1;
-      __pyx_t_28 = __pyx_v_i;
-      __pyx_t_29 = 2;
-      __pyx_v_G1 = (__pyx_v_G1 + (((__pyx_v_x1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_25, __pyx_pybuffernd_coords1.diminfo[1].strides))) + (__pyx_v_y1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_coords1.diminfo[1].strides)))) + (__pyx_v_z1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_coords1.diminfo[1].strides)))));
+      __pyx_t_8 = __pyx_v_i;
+      __pyx_t_1 = 0;
+      __pyx_t_7 = __pyx_v_i;
+      __pyx_t_9 = 1;
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 2;
+      __pyx_v_G1 = (__pyx_v_G1 + (((__pyx_v_x1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_1, __pyx_pybuffernd_coords1.diminfo[1].strides))) + (__pyx_v_y1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_coords1.diminfo[1].strides)))) + (__pyx_v_z1 * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords1.diminfo[1].strides)))));
 
       /* "geomm/pyqcprot.pyx":205
  *             G1 += x1 * coords1[i, 0] + y1 * coords1[i, 1] + z1 * coords1[i, 2]
  * 
  *             x2 = coords2[i, 0]             # <<<<<<<<<<<<<<
  *             y2 = coords2[i, 1]
  *             z2 = coords2[i, 2]
  */
-      __pyx_t_30 = __pyx_v_i;
-      __pyx_t_31 = 0;
-      __pyx_v_x2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_31, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 0;
+      __pyx_v_x2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":206
  * 
  *             x2 = coords2[i, 0]
  *             y2 = coords2[i, 1]             # <<<<<<<<<<<<<<
  *             z2 = coords2[i, 2]
  * 
  */
-      __pyx_t_32 = __pyx_v_i;
-      __pyx_t_33 = 1;
-      __pyx_v_y2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 1;
+      __pyx_v_y2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":207
  *             x2 = coords2[i, 0]
  *             y2 = coords2[i, 1]
  *             z2 = coords2[i, 2]             # <<<<<<<<<<<<<<
  * 
  *             G2 += weight[i] * (x2 * x2 + y2 * y2 + z2 * z2)
  */
-      __pyx_t_34 = __pyx_v_i;
-      __pyx_t_35 = 2;
-      __pyx_v_z2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 2;
+      __pyx_v_z2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":209
  *             z2 = coords2[i, 2]
  * 
  *             G2 += weight[i] * (x2 * x2 + y2 * y2 + z2 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[0] +=  (x1 * x2)
  */
-      __pyx_t_36 = __pyx_v_i;
-      __pyx_v_G2 = (__pyx_v_G2 + ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_weight.diminfo[0].strides)) * (((__pyx_v_x2 * __pyx_v_x2) + (__pyx_v_y2 * __pyx_v_y2)) + (__pyx_v_z2 * __pyx_v_z2))));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_v_G2 = (__pyx_v_G2 + ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_weight.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_weight.diminfo[0].strides)) * (((__pyx_v_x2 * __pyx_v_x2) + (__pyx_v_y2 * __pyx_v_y2)) + (__pyx_v_z2 * __pyx_v_z2))));
 
       /* "geomm/pyqcprot.pyx":211
  *             G2 += weight[i] * (x2 * x2 + y2 * y2 + z2 * z2)
  * 
  *             A[0] +=  (x1 * x2)             # <<<<<<<<<<<<<<
  *             A[1] +=  (x1 * y2)
  *             A[2] +=  (x1 * z2)
  */
-      __pyx_t_37 = 0;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_x2);
+      __pyx_t_11 = 0;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":212
  * 
  *             A[0] +=  (x1 * x2)
  *             A[1] +=  (x1 * y2)             # <<<<<<<<<<<<<<
  *             A[2] +=  (x1 * z2)
  * 
  */
-      __pyx_t_38 = 1;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_y2);
+      __pyx_t_11 = 1;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":213
  *             A[0] +=  (x1 * x2)
  *             A[1] +=  (x1 * y2)
  *             A[2] +=  (x1 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[3] +=  (y1 * x2)
  */
-      __pyx_t_39 = 2;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_z2);
+      __pyx_t_11 = 2;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_z2);
 
       /* "geomm/pyqcprot.pyx":215
  *             A[2] +=  (x1 * z2)
  * 
  *             A[3] +=  (y1 * x2)             # <<<<<<<<<<<<<<
  *             A[4] +=  (y1 * y2)
  *             A[5] +=  (y1 * z2)
  */
-      __pyx_t_40 = 3;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_x2);
+      __pyx_t_11 = 3;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":216
  * 
  *             A[3] +=  (y1 * x2)
  *             A[4] +=  (y1 * y2)             # <<<<<<<<<<<<<<
  *             A[5] +=  (y1 * z2)
  * 
  */
-      __pyx_t_41 = 4;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_y2);
+      __pyx_t_11 = 4;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":217
  *             A[3] +=  (y1 * x2)
  *             A[4] +=  (y1 * y2)
  *             A[5] +=  (y1 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[6] +=  (z1 * x2)
  */
-      __pyx_t_42 = 5;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_42, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_z2);
+      __pyx_t_11 = 5;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_z2);
 
       /* "geomm/pyqcprot.pyx":219
  *             A[5] +=  (y1 * z2)
  * 
  *             A[6] +=  (z1 * x2)             # <<<<<<<<<<<<<<
  *             A[7] +=  (z1 * y2)
  *             A[8] +=  (z1 * z2)
  */
-      __pyx_t_43 = 6;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_43, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_x2);
+      __pyx_t_11 = 6;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":220
  * 
  *             A[6] +=  (z1 * x2)
  *             A[7] +=  (z1 * y2)             # <<<<<<<<<<<<<<
  *             A[8] +=  (z1 * z2)
  * 
  */
-      __pyx_t_44 = 7;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_44, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_y2);
+      __pyx_t_11 = 7;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":221
  *             A[6] +=  (z1 * x2)
  *             A[7] +=  (z1 * y2)
  *             A[8] +=  (z1 * z2)             # <<<<<<<<<<<<<<
  * 
  *     else:
  */
-      __pyx_t_45 = 8;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_45, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_z2);
+      __pyx_t_11 = 8;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_z2);
     }
 
     /* "geomm/pyqcprot.pyx":197
  *     A[0] = A[1] = A[2] = A[3] = A[4] = A[5] = A[6] = A[7] = A[8] = 0.0
  * 
  *     if (weight is not None):             # <<<<<<<<<<<<<<
  *         for i in range(N):
@@ -2460,51 +2548,51 @@
  * 
  *     else:
  *         for i in range(N):             # <<<<<<<<<<<<<<
  *             x1 = coords1[i, 0]
  *             y1 = coords1[i, 1]
  */
   /*else*/ {
-    __pyx_t_12 = __pyx_v_N;
-    __pyx_t_13 = __pyx_t_12;
-    for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-      __pyx_v_i = __pyx_t_14;
+    __pyx_t_4 = __pyx_v_N;
+    __pyx_t_5 = __pyx_t_4;
+    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
+      __pyx_v_i = __pyx_t_6;
 
       /* "geomm/pyqcprot.pyx":225
  *     else:
  *         for i in range(N):
  *             x1 = coords1[i, 0]             # <<<<<<<<<<<<<<
  *             y1 = coords1[i, 1]
  *             z1 = coords1[i, 2]
  */
-      __pyx_t_46 = __pyx_v_i;
-      __pyx_t_47 = 0;
-      __pyx_v_x1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_47, __pyx_pybuffernd_coords1.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 0;
+      __pyx_v_x1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords1.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":226
  *         for i in range(N):
  *             x1 = coords1[i, 0]
  *             y1 = coords1[i, 1]             # <<<<<<<<<<<<<<
  *             z1 = coords1[i, 2]
  * 
  */
-      __pyx_t_48 = __pyx_v_i;
-      __pyx_t_49 = 1;
-      __pyx_v_y1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_48, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_49, __pyx_pybuffernd_coords1.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 1;
+      __pyx_v_y1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords1.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":227
  *             x1 = coords1[i, 0]
  *             y1 = coords1[i, 1]
  *             z1 = coords1[i, 2]             # <<<<<<<<<<<<<<
  * 
  *             G1 += (x1 * x1 + y1 * y1 + z1 * z1)
  */
-      __pyx_t_50 = __pyx_v_i;
-      __pyx_t_51 = 2;
-      __pyx_v_z1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_50, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_51, __pyx_pybuffernd_coords1.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 2;
+      __pyx_v_z1 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords1.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords1.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords1.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":229
  *             z1 = coords1[i, 2]
  * 
  *             G1 += (x1 * x1 + y1 * y1 + z1 * z1)             # <<<<<<<<<<<<<<
  * 
  *             x2 = coords2[i, 0]
@@ -2514,39 +2602,39 @@
       /* "geomm/pyqcprot.pyx":231
  *             G1 += (x1 * x1 + y1 * y1 + z1 * z1)
  * 
  *             x2 = coords2[i, 0]             # <<<<<<<<<<<<<<
  *             y2 = coords2[i, 1]
  *             z2 = coords2[i, 2]
  */
-      __pyx_t_52 = __pyx_v_i;
-      __pyx_t_53 = 0;
-      __pyx_v_x2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_52, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_53, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 0;
+      __pyx_v_x2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":232
  * 
  *             x2 = coords2[i, 0]
  *             y2 = coords2[i, 1]             # <<<<<<<<<<<<<<
  *             z2 = coords2[i, 2]
  * 
  */
-      __pyx_t_54 = __pyx_v_i;
-      __pyx_t_55 = 1;
-      __pyx_v_y2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_54, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_55, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 1;
+      __pyx_v_y2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":233
  *             x2 = coords2[i, 0]
  *             y2 = coords2[i, 1]
  *             z2 = coords2[i, 2]             # <<<<<<<<<<<<<<
  * 
  *             G2 += (x2 * x2 + y2 * y2 + z2 * z2)
  */
-      __pyx_t_56 = __pyx_v_i;
-      __pyx_t_57 = 2;
-      __pyx_v_z2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_56, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_57, __pyx_pybuffernd_coords2.diminfo[1].strides));
+      __pyx_t_10 = __pyx_v_i;
+      __pyx_t_11 = 2;
+      __pyx_v_z2 = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_coords2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_coords2.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_coords2.diminfo[1].strides));
 
       /* "geomm/pyqcprot.pyx":235
  *             z2 = coords2[i, 2]
  * 
  *             G2 += (x2 * x2 + y2 * y2 + z2 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[0] +=  (x1 * x2)
@@ -2556,125 +2644,125 @@
       /* "geomm/pyqcprot.pyx":237
  *             G2 += (x2 * x2 + y2 * y2 + z2 * z2)
  * 
  *             A[0] +=  (x1 * x2)             # <<<<<<<<<<<<<<
  *             A[1] +=  (x1 * y2)
  *             A[2] +=  (x1 * z2)
  */
-      __pyx_t_58 = 0;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_58, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_x2);
+      __pyx_t_11 = 0;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":238
  * 
  *             A[0] +=  (x1 * x2)
  *             A[1] +=  (x1 * y2)             # <<<<<<<<<<<<<<
  *             A[2] +=  (x1 * z2)
  * 
  */
-      __pyx_t_59 = 1;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_59, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_y2);
+      __pyx_t_11 = 1;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":239
  *             A[0] +=  (x1 * x2)
  *             A[1] +=  (x1 * y2)
  *             A[2] +=  (x1 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[3] +=  (y1 * x2)
  */
-      __pyx_t_60 = 2;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_60, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_z2);
+      __pyx_t_11 = 2;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_x1 * __pyx_v_z2);
 
       /* "geomm/pyqcprot.pyx":241
  *             A[2] +=  (x1 * z2)
  * 
  *             A[3] +=  (y1 * x2)             # <<<<<<<<<<<<<<
  *             A[4] +=  (y1 * y2)
  *             A[5] +=  (y1 * z2)
  */
-      __pyx_t_61 = 3;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_61, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_x2);
+      __pyx_t_11 = 3;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":242
  * 
  *             A[3] +=  (y1 * x2)
  *             A[4] +=  (y1 * y2)             # <<<<<<<<<<<<<<
  *             A[5] +=  (y1 * z2)
  * 
  */
-      __pyx_t_62 = 4;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_62, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_y2);
+      __pyx_t_11 = 4;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":243
  *             A[3] +=  (y1 * x2)
  *             A[4] +=  (y1 * y2)
  *             A[5] +=  (y1 * z2)             # <<<<<<<<<<<<<<
  * 
  *             A[6] +=  (z1 * x2)
  */
-      __pyx_t_63 = 5;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_63, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_z2);
+      __pyx_t_11 = 5;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_y1 * __pyx_v_z2);
 
       /* "geomm/pyqcprot.pyx":245
  *             A[5] +=  (y1 * z2)
  * 
  *             A[6] +=  (z1 * x2)             # <<<<<<<<<<<<<<
  *             A[7] +=  (z1 * y2)
  *             A[8] +=  (z1 * z2)
  */
-      __pyx_t_64 = 6;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_64, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_x2);
+      __pyx_t_11 = 6;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_x2);
 
       /* "geomm/pyqcprot.pyx":246
  * 
  *             A[6] +=  (z1 * x2)
  *             A[7] +=  (z1 * y2)             # <<<<<<<<<<<<<<
  *             A[8] +=  (z1 * z2)
  * 
  */
-      __pyx_t_65 = 7;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_65, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_y2);
+      __pyx_t_11 = 7;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_y2);
 
       /* "geomm/pyqcprot.pyx":247
  *             A[6] +=  (z1 * x2)
  *             A[7] +=  (z1 * y2)
  *             A[8] +=  (z1 * z2)             # <<<<<<<<<<<<<<
  * 
  *     return (G1 + G2) * 0.5
  */
-      __pyx_t_66 = 8;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_66, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_z2);
+      __pyx_t_11 = 8;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides) += (__pyx_v_z1 * __pyx_v_z2);
     }
   }
   __pyx_L3:;
 
   /* "geomm/pyqcprot.pyx":249
  *             A[8] +=  (z1 * z2)
  * 
  *     return (G1 + G2) * 0.5             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_67 = PyFloat_FromDouble(((__pyx_v_G1 + __pyx_v_G2) * 0.5)); if (unlikely(!__pyx_t_67)) __PYX_ERR(0, 249, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_67);
-  __pyx_r = __pyx_t_67;
-  __pyx_t_67 = 0;
+  __pyx_t_12 = PyFloat_FromDouble(((__pyx_v_G1 + __pyx_v_G2) * 0.5)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_r = __pyx_t_12;
+  __pyx_t_12 = 0;
   goto __pyx_L0;
 
   /* "geomm/pyqcprot.pyx":150
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def InnerProduct(np.ndarray[np.float64_t, ndim=1] A,             # <<<<<<<<<<<<<<
  *                  np.ndarray[np.float64_t, ndim=2] coords1,
  *                  np.ndarray[np.float64_t, ndim=2] coords2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_67);
+  __Pyx_XDECREF(__pyx_t_12);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_A.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_coords1.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_coords2.rcbuffer->pybuffer);
@@ -2708,14 +2796,17 @@
 static PyMethodDef __pyx_mdef_5geomm_8pyqcprot_3CalcRMSDRotationalMatrix = {"CalcRMSDRotationalMatrix", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5geomm_8pyqcprot_3CalcRMSDRotationalMatrix, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5geomm_8pyqcprot_2CalcRMSDRotationalMatrix};
 static PyObject *__pyx_pw_5geomm_8pyqcprot_3CalcRMSDRotationalMatrix(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_ref = 0;
   PyArrayObject *__pyx_v_conf = 0;
   int __pyx_v_N;
   PyArrayObject *__pyx_v_rot = 0;
   PyArrayObject *__pyx_v_weights = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("CalcRMSDRotationalMatrix (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ref,&__pyx_n_s_conf,&__pyx_n_s_N,&__pyx_n_s_rot,&__pyx_n_s_weights,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2826,14 +2917,17 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   double __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CalcRMSDRotationalMatrix", 0);
   __pyx_pybuffer_A.pybuffer.buf = NULL;
   __pyx_pybuffer_A.refcount = 0;
   __pyx_pybuffernd_A.data = NULL;
   __pyx_pybuffernd_A.rcbuffer = &__pyx_pybuffer_A;
   __pyx_pybuffer_ref.pybuffer.buf = NULL;
   __pyx_pybuffer_ref.refcount = 0;
@@ -3110,14 +3204,17 @@
 static char __pyx_doc_5geomm_8pyqcprot_4FastCalcRMSDAndRotation[] = "\n    Calculate the RMSD, and/or the optimal rotation matrix.\n\n    Parameters\n    ----------\n    rot : ndarray np.float64_t\n        result rotation matrix, modified inplace\n    A : ndarray np.float64_t\n        the inner product of two structures\n    E0 : float64\n        0.5 * (G1 + G2)\n    N : int\n        size of the system\n\n    Returns\n    -------\n    rmsd : float\n        RMSD value for two structures\n\n\n    .. versionchanged:: 0.16.0\n       Array sized changed from 3xN to Nx3.\n    ";
 static PyMethodDef __pyx_mdef_5geomm_8pyqcprot_5FastCalcRMSDAndRotation = {"FastCalcRMSDAndRotation", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5geomm_8pyqcprot_5FastCalcRMSDAndRotation, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5geomm_8pyqcprot_4FastCalcRMSDAndRotation};
 static PyObject *__pyx_pw_5geomm_8pyqcprot_5FastCalcRMSDAndRotation(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_rot = 0;
   PyArrayObject *__pyx_v_A = 0;
   double __pyx_v_E0;
   int __pyx_v_N;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("FastCalcRMSDAndRotation (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_rot,&__pyx_n_s_A,&__pyx_n_s_E0,&__pyx_n_s_N,0};
     PyObject* values[4] = {0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -3290,51 +3387,22 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyArrayObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
-  Py_ssize_t __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
-  Py_ssize_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  unsigned int __pyx_t_18;
-  Py_ssize_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
-  Py_ssize_t __pyx_t_21;
-  __pyx_t_5numpy_float64_t __pyx_t_22;
-  double __pyx_t_23;
-  int __pyx_t_24;
-  int __pyx_t_25;
-  Py_ssize_t __pyx_t_26;
-  Py_ssize_t __pyx_t_27;
-  Py_ssize_t __pyx_t_28;
-  Py_ssize_t __pyx_t_29;
-  Py_ssize_t __pyx_t_30;
-  Py_ssize_t __pyx_t_31;
-  Py_ssize_t __pyx_t_32;
-  Py_ssize_t __pyx_t_33;
-  Py_ssize_t __pyx_t_34;
-  Py_ssize_t __pyx_t_35;
-  Py_ssize_t __pyx_t_36;
-  Py_ssize_t __pyx_t_37;
-  Py_ssize_t __pyx_t_38;
-  Py_ssize_t __pyx_t_39;
-  Py_ssize_t __pyx_t_40;
-  Py_ssize_t __pyx_t_41;
-  Py_ssize_t __pyx_t_42;
-  Py_ssize_t __pyx_t_43;
+  unsigned int __pyx_t_7;
+  __pyx_t_5numpy_float64_t __pyx_t_8;
+  double __pyx_t_9;
+  int __pyx_t_10;
+  int __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("FastCalcRMSDAndRotation", 0);
   __pyx_pybuffer_C.pybuffer.buf = NULL;
   __pyx_pybuffer_C.refcount = 0;
   __pyx_pybuffernd_C.data = NULL;
   __pyx_pybuffernd_C.rcbuffer = &__pyx_pybuffer_C;
   __pyx_pybuffer_rot.pybuffer.buf = NULL;
   __pyx_pybuffer_rot.refcount = 0;
@@ -3445,158 +3513,158 @@
   /* "geomm/pyqcprot.pyx":337
  *     cdef double a1324_1423, a1224_1422, a1223_1322, a1124_1421, a1123_1321, a1122_1221
  *     Sxx = A[0]
  *     Sxy = A[1]             # <<<<<<<<<<<<<<
  *     Sxz = A[2]
  *     Syx = A[3]
  */
-  __pyx_t_7 = 1;
+  __pyx_t_5 = 1;
   __pyx_t_6 = -1;
-  if (__pyx_t_7 < 0) {
-    __pyx_t_7 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_7 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_7 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 337, __pyx_L1_error)
   }
-  __pyx_v_Sxy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Sxy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":338
  *     Sxx = A[0]
  *     Sxy = A[1]
  *     Sxz = A[2]             # <<<<<<<<<<<<<<
  *     Syx = A[3]
  *     Syy = A[4]
  */
-  __pyx_t_8 = 2;
+  __pyx_t_5 = 2;
   __pyx_t_6 = -1;
-  if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_8 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 338, __pyx_L1_error)
   }
-  __pyx_v_Sxz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Sxz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":339
  *     Sxy = A[1]
  *     Sxz = A[2]
  *     Syx = A[3]             # <<<<<<<<<<<<<<
  *     Syy = A[4]
  *     Syz = A[5]
  */
-  __pyx_t_9 = 3;
+  __pyx_t_5 = 3;
   __pyx_t_6 = -1;
-  if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 339, __pyx_L1_error)
   }
-  __pyx_v_Syx = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Syx = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":340
  *     Sxz = A[2]
  *     Syx = A[3]
  *     Syy = A[4]             # <<<<<<<<<<<<<<
  *     Syz = A[5]
  *     Szx = A[6]
  */
-  __pyx_t_10 = 4;
+  __pyx_t_5 = 4;
   __pyx_t_6 = -1;
-  if (__pyx_t_10 < 0) {
-    __pyx_t_10 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 340, __pyx_L1_error)
   }
-  __pyx_v_Syy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Syy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":341
  *     Syx = A[3]
  *     Syy = A[4]
  *     Syz = A[5]             # <<<<<<<<<<<<<<
  *     Szx = A[6]
  *     Szy = A[7]
  */
-  __pyx_t_11 = 5;
+  __pyx_t_5 = 5;
   __pyx_t_6 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 341, __pyx_L1_error)
   }
-  __pyx_v_Syz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Syz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":342
  *     Syy = A[4]
  *     Syz = A[5]
  *     Szx = A[6]             # <<<<<<<<<<<<<<
  *     Szy = A[7]
  *     Szz = A[8]
  */
-  __pyx_t_12 = 6;
+  __pyx_t_5 = 6;
   __pyx_t_6 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 342, __pyx_L1_error)
   }
-  __pyx_v_Szx = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Szx = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":343
  *     Syz = A[5]
  *     Szx = A[6]
  *     Szy = A[7]             # <<<<<<<<<<<<<<
  *     Szz = A[8]
  * 
  */
-  __pyx_t_13 = 7;
+  __pyx_t_5 = 7;
   __pyx_t_6 = -1;
-  if (__pyx_t_13 < 0) {
-    __pyx_t_13 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_13 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 343, __pyx_L1_error)
   }
-  __pyx_v_Szy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Szy = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":344
  *     Szx = A[6]
  *     Szy = A[7]
  *     Szz = A[8]             # <<<<<<<<<<<<<<
  * 
  *     Sxx2 = Sxx * Sxx
  */
-  __pyx_t_14 = 8;
+  __pyx_t_5 = 8;
   __pyx_t_6 = -1;
-  if (__pyx_t_14 < 0) {
-    __pyx_t_14 += __pyx_pybuffernd_A.diminfo[0].shape;
-    if (unlikely(__pyx_t_14 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_A.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_A.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 344, __pyx_L1_error)
   }
-  __pyx_v_Szz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_A.diminfo[0].strides));
+  __pyx_v_Szz = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_A.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_A.diminfo[0].strides));
 
   /* "geomm/pyqcprot.pyx":346
  *     Szz = A[8]
  * 
  *     Sxx2 = Sxx * Sxx             # <<<<<<<<<<<<<<
  *     Syy2 = Syy * Syy
  *     Szz2 = Szz * Szz
@@ -3696,44 +3764,44 @@
   /* "geomm/pyqcprot.pyx":361
  *     Sxx2Syy2Szz2Syz2Szy2 = Syy2 + Szz2 - Sxx2 + Syz2 + Szy2
  * 
  *     C[2] = -2.0 * (Sxx2 + Syy2 + Szz2 + Sxy2 + Syx2 + Sxz2 + Szx2 + Syz2 + Szy2)             # <<<<<<<<<<<<<<
  *     C[1] = 8.0 * (Sxx*Syz*Szy + Syy*Szx*Sxz + Szz*Sxy*Syx - Sxx*Syy*Szz - Syz*Szx*Sxy - Szy*Syx*Sxz)
  * 
  */
-  __pyx_t_15 = 2;
+  __pyx_t_5 = 2;
   __pyx_t_6 = -1;
-  if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_pybuffernd_C.diminfo[0].shape;
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 361, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_C.diminfo[0].strides) = (-2.0 * ((((((((__pyx_v_Sxx2 + __pyx_v_Syy2) + __pyx_v_Szz2) + __pyx_v_Sxy2) + __pyx_v_Syx2) + __pyx_v_Sxz2) + __pyx_v_Szx2) + __pyx_v_Syz2) + __pyx_v_Szy2));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides) = (-2.0 * ((((((((__pyx_v_Sxx2 + __pyx_v_Syy2) + __pyx_v_Szz2) + __pyx_v_Sxy2) + __pyx_v_Syx2) + __pyx_v_Sxz2) + __pyx_v_Szx2) + __pyx_v_Syz2) + __pyx_v_Szy2));
 
   /* "geomm/pyqcprot.pyx":362
  * 
  *     C[2] = -2.0 * (Sxx2 + Syy2 + Szz2 + Sxy2 + Syx2 + Sxz2 + Szx2 + Syz2 + Szy2)
  *     C[1] = 8.0 * (Sxx*Syz*Szy + Syy*Szx*Sxz + Szz*Sxy*Syx - Sxx*Syy*Szz - Syz*Szx*Sxy - Szy*Syx*Sxz)             # <<<<<<<<<<<<<<
  * 
  *     SxzpSzx = Sxz + Szx
  */
-  __pyx_t_16 = 1;
+  __pyx_t_5 = 1;
   __pyx_t_6 = -1;
-  if (__pyx_t_16 < 0) {
-    __pyx_t_16 += __pyx_pybuffernd_C.diminfo[0].shape;
-    if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_16 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 362, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_C.diminfo[0].strides) = (8.0 * (((((((__pyx_v_Sxx * __pyx_v_Syz) * __pyx_v_Szy) + ((__pyx_v_Syy * __pyx_v_Szx) * __pyx_v_Sxz)) + ((__pyx_v_Szz * __pyx_v_Sxy) * __pyx_v_Syx)) - ((__pyx_v_Sxx * __pyx_v_Syy) * __pyx_v_Szz)) - ((__pyx_v_Syz * __pyx_v_Szx) * __pyx_v_Sxy)) - ((__pyx_v_Szy * __pyx_v_Syx) * __pyx_v_Sxz)));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides) = (8.0 * (((((((__pyx_v_Sxx * __pyx_v_Syz) * __pyx_v_Szy) + ((__pyx_v_Syy * __pyx_v_Szx) * __pyx_v_Sxz)) + ((__pyx_v_Szz * __pyx_v_Sxy) * __pyx_v_Syx)) - ((__pyx_v_Sxx * __pyx_v_Syy) * __pyx_v_Szz)) - ((__pyx_v_Syz * __pyx_v_Szx) * __pyx_v_Sxy)) - ((__pyx_v_Szy * __pyx_v_Syx) * __pyx_v_Sxz)));
 
   /* "geomm/pyqcprot.pyx":364
  *     C[1] = 8.0 * (Sxx*Syz*Szy + Syy*Szx*Sxz + Szz*Sxy*Syx - Sxx*Syy*Szz - Syz*Szx*Sxy - Szy*Syx*Sxz)
  * 
  *     SxzpSzx = Sxz + Szx             # <<<<<<<<<<<<<<
  *     SyzpSzy = Syz + Szy
  *     SxypSyx = Sxy + Syx
@@ -3815,25 +3883,25 @@
   /* "geomm/pyqcprot.pyx":374
  *     Sxy2Sxz2Syx2Szx2 = Sxy2 + Sxz2 - Syx2 - Szx2
  * 
  *     C[0] = (Sxy2Sxz2Syx2Szx2 * Sxy2Sxz2Syx2Szx2             # <<<<<<<<<<<<<<
  *          + (Sxx2Syy2Szz2Syz2Szy2 + SyzSzymSyySzz2) * (Sxx2Syy2Szz2Syz2Szy2 - SyzSzymSyySzz2)
  *          + (-(SxzpSzx)*(SyzmSzy)+(SxymSyx)*(SxxmSyy-Szz)) * (-(SxzmSzx)*(SyzpSzy)+(SxymSyx)*(SxxmSyy+Szz))
  */
-  __pyx_t_17 = 0;
+  __pyx_t_5 = 0;
   __pyx_t_6 = -1;
-  if (__pyx_t_17 < 0) {
-    __pyx_t_17 += __pyx_pybuffernd_C.diminfo[0].shape;
-    if (unlikely(__pyx_t_17 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_17 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 374, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_C.diminfo[0].strides) = ((((((__pyx_v_Sxy2Sxz2Syx2Szx2 * __pyx_v_Sxy2Sxz2Syx2Szx2) + ((__pyx_v_Sxx2Syy2Szz2Syz2Szy2 + __pyx_v_SyzSzymSyySzz2) * (__pyx_v_Sxx2Syy2Szz2Syz2Szy2 - __pyx_v_SyzSzymSyySzz2))) + ((((-__pyx_v_SxzpSzx) * __pyx_v_SyzmSzy) + (__pyx_v_SxymSyx * (__pyx_v_SxxmSyy - __pyx_v_Szz))) * (((-__pyx_v_SxzmSzx) * __pyx_v_SyzpSzy) + (__pyx_v_SxymSyx * (__pyx_v_SxxmSyy + __pyx_v_Szz))))) + ((((-__pyx_v_SxzpSzx) * __pyx_v_SyzpSzy) - (__pyx_v_SxypSyx * (__pyx_v_SxxpSyy - __pyx_v_Szz))) * (((-__pyx_v_SxzmSzx) * __pyx_v_SyzmSzy) - (__pyx_v_SxypSyx * (__pyx_v_SxxpSyy + __pyx_v_Szz))))) + (((__pyx_v_SxypSyx * __pyx_v_SyzpSzy) + (__pyx_v_SxzpSzx * (__pyx_v_SxxmSyy + __pyx_v_Szz))) * (((-__pyx_v_SxymSyx) * __pyx_v_SyzmSzy) + (__pyx_v_SxzpSzx * (__pyx_v_SxxpSyy + __pyx_v_Szz))))) + (((__pyx_v_SxypSyx * __pyx_v_SyzmSzy) + (__pyx_v_SxzmSzx * (__pyx_v_SxxmSyy - __pyx_v_Szz))) * (((-__pyx_v_SxymSyx) * __pyx_v_SyzpSzy) + (__pyx_v_SxzmSzx * (__pyx_v_SxxpSyy - __pyx_v_Szz)))));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides) = ((((((__pyx_v_Sxy2Sxz2Syx2Szx2 * __pyx_v_Sxy2Sxz2Syx2Szx2) + ((__pyx_v_Sxx2Syy2Szz2Syz2Szy2 + __pyx_v_SyzSzymSyySzz2) * (__pyx_v_Sxx2Syy2Szz2Syz2Szy2 - __pyx_v_SyzSzymSyySzz2))) + ((((-__pyx_v_SxzpSzx) * __pyx_v_SyzmSzy) + (__pyx_v_SxymSyx * (__pyx_v_SxxmSyy - __pyx_v_Szz))) * (((-__pyx_v_SxzmSzx) * __pyx_v_SyzpSzy) + (__pyx_v_SxymSyx * (__pyx_v_SxxmSyy + __pyx_v_Szz))))) + ((((-__pyx_v_SxzpSzx) * __pyx_v_SyzpSzy) - (__pyx_v_SxypSyx * (__pyx_v_SxxpSyy - __pyx_v_Szz))) * (((-__pyx_v_SxzmSzx) * __pyx_v_SyzmSzy) - (__pyx_v_SxypSyx * (__pyx_v_SxxpSyy + __pyx_v_Szz))))) + (((__pyx_v_SxypSyx * __pyx_v_SyzpSzy) + (__pyx_v_SxzpSzx * (__pyx_v_SxxmSyy + __pyx_v_Szz))) * (((-__pyx_v_SxymSyx) * __pyx_v_SyzmSzy) + (__pyx_v_SxzpSzx * (__pyx_v_SxxpSyy + __pyx_v_Szz))))) + (((__pyx_v_SxypSyx * __pyx_v_SyzmSzy) + (__pyx_v_SxzmSzx * (__pyx_v_SxxmSyy - __pyx_v_Szz))) * (((-__pyx_v_SxymSyx) * __pyx_v_SyzpSzy) + (__pyx_v_SxzmSzx * (__pyx_v_SxxpSyy - __pyx_v_Szz)))));
 
   /* "geomm/pyqcprot.pyx":381
  *          + (+(SxypSyx)*(SyzmSzy)+(SxzmSzx)*(SxxmSyy-Szz)) * (-(SxymSyx)*(SyzpSzy)+(SxzmSzx)*(SxxpSyy-Szz)))
  * 
  *     mxEigenV = E0             # <<<<<<<<<<<<<<
  *     for i in range(50):
  *         oldg = mxEigenV
@@ -3843,16 +3911,16 @@
   /* "geomm/pyqcprot.pyx":382
  * 
  *     mxEigenV = E0
  *     for i in range(50):             # <<<<<<<<<<<<<<
  *         oldg = mxEigenV
  *         x2 = mxEigenV*mxEigenV
  */
-  for (__pyx_t_18 = 0; __pyx_t_18 < 50; __pyx_t_18+=1) {
-    __pyx_v_i = __pyx_t_18;
+  for (__pyx_t_7 = 0; __pyx_t_7 < 50; __pyx_t_7+=1) {
+    __pyx_v_i = __pyx_t_7;
 
     /* "geomm/pyqcprot.pyx":383
  *     mxEigenV = E0
  *     for i in range(50):
  *         oldg = mxEigenV             # <<<<<<<<<<<<<<
  *         x2 = mxEigenV*mxEigenV
  *         b = (x2 + C[2])*mxEigenV
@@ -3871,69 +3939,69 @@
     /* "geomm/pyqcprot.pyx":385
  *         oldg = mxEigenV
  *         x2 = mxEigenV*mxEigenV
  *         b = (x2 + C[2])*mxEigenV             # <<<<<<<<<<<<<<
  *         a = b + C[1]
  *         delta = ((a*mxEigenV + C[0])/(2.0*x2*mxEigenV + b + a))
  */
-    __pyx_t_19 = 2;
+    __pyx_t_5 = 2;
     __pyx_t_6 = -1;
-    if (__pyx_t_19 < 0) {
-      __pyx_t_19 += __pyx_pybuffernd_C.diminfo[0].shape;
-      if (unlikely(__pyx_t_19 < 0)) __pyx_t_6 = 0;
-    } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (__pyx_t_5 < 0) {
+      __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+      if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+    } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
     if (unlikely(__pyx_t_6 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_6);
       __PYX_ERR(0, 385, __pyx_L1_error)
     }
-    __pyx_v_b = ((__pyx_v_x2 + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_C.diminfo[0].strides))) * __pyx_v_mxEigenV);
+    __pyx_v_b = ((__pyx_v_x2 + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides))) * __pyx_v_mxEigenV);
 
     /* "geomm/pyqcprot.pyx":386
  *         x2 = mxEigenV*mxEigenV
  *         b = (x2 + C[2])*mxEigenV
  *         a = b + C[1]             # <<<<<<<<<<<<<<
  *         delta = ((a*mxEigenV + C[0])/(2.0*x2*mxEigenV + b + a))
  *         mxEigenV -= delta
  */
-    __pyx_t_20 = 1;
+    __pyx_t_5 = 1;
     __pyx_t_6 = -1;
-    if (__pyx_t_20 < 0) {
-      __pyx_t_20 += __pyx_pybuffernd_C.diminfo[0].shape;
-      if (unlikely(__pyx_t_20 < 0)) __pyx_t_6 = 0;
-    } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (__pyx_t_5 < 0) {
+      __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+      if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+    } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
     if (unlikely(__pyx_t_6 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_6);
       __PYX_ERR(0, 386, __pyx_L1_error)
     }
-    __pyx_v_a = (__pyx_v_b + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_C.diminfo[0].strides)));
+    __pyx_v_a = (__pyx_v_b + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides)));
 
     /* "geomm/pyqcprot.pyx":387
  *         b = (x2 + C[2])*mxEigenV
  *         a = b + C[1]
  *         delta = ((a*mxEigenV + C[0])/(2.0*x2*mxEigenV + b + a))             # <<<<<<<<<<<<<<
  *         mxEigenV -= delta
  *         if (fabs(mxEigenV - oldg) < fabs((evalprec)*mxEigenV)):
  */
-    __pyx_t_21 = 0;
+    __pyx_t_5 = 0;
     __pyx_t_6 = -1;
-    if (__pyx_t_21 < 0) {
-      __pyx_t_21 += __pyx_pybuffernd_C.diminfo[0].shape;
-      if (unlikely(__pyx_t_21 < 0)) __pyx_t_6 = 0;
-    } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (__pyx_t_5 < 0) {
+      __pyx_t_5 += __pyx_pybuffernd_C.diminfo[0].shape;
+      if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+    } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_C.diminfo[0].shape)) __pyx_t_6 = 0;
     if (unlikely(__pyx_t_6 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_6);
       __PYX_ERR(0, 387, __pyx_L1_error)
     }
-    __pyx_t_22 = ((__pyx_v_a * __pyx_v_mxEigenV) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_C.diminfo[0].strides)));
-    __pyx_t_23 = ((((2.0 * __pyx_v_x2) * __pyx_v_mxEigenV) + __pyx_v_b) + __pyx_v_a);
-    if (unlikely(__pyx_t_23 == 0)) {
+    __pyx_t_8 = ((__pyx_v_a * __pyx_v_mxEigenV) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_C.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_C.diminfo[0].strides)));
+    __pyx_t_9 = ((((2.0 * __pyx_v_x2) * __pyx_v_mxEigenV) + __pyx_v_b) + __pyx_v_a);
+    if (unlikely(__pyx_t_9 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
       __PYX_ERR(0, 387, __pyx_L1_error)
     }
-    __pyx_v_delta = (__pyx_t_22 / __pyx_t_23);
+    __pyx_v_delta = (__pyx_t_8 / __pyx_t_9);
 
     /* "geomm/pyqcprot.pyx":388
  *         a = b + C[1]
  *         delta = ((a*mxEigenV + C[0])/(2.0*x2*mxEigenV + b + a))
  *         mxEigenV -= delta             # <<<<<<<<<<<<<<
  *         if (fabs(mxEigenV - oldg) < fabs((evalprec)*mxEigenV)):
  *             break
@@ -3943,16 +4011,16 @@
     /* "geomm/pyqcprot.pyx":389
  *         delta = ((a*mxEigenV + C[0])/(2.0*x2*mxEigenV + b + a))
  *         mxEigenV -= delta
  *         if (fabs(mxEigenV - oldg) < fabs((evalprec)*mxEigenV)):             # <<<<<<<<<<<<<<
  *             break
  * 
  */
-    __pyx_t_24 = ((fabs((__pyx_v_mxEigenV - __pyx_v_oldg)) < fabs((__pyx_v_evalprec * __pyx_v_mxEigenV))) != 0);
-    if (__pyx_t_24) {
+    __pyx_t_10 = ((fabs((__pyx_v_mxEigenV - __pyx_v_oldg)) < fabs((__pyx_v_evalprec * __pyx_v_mxEigenV))) != 0);
+    if (__pyx_t_10) {
 
       /* "geomm/pyqcprot.pyx":390
  *         mxEigenV -= delta
  *         if (fabs(mxEigenV - oldg) < fabs((evalprec)*mxEigenV)):
  *             break             # <<<<<<<<<<<<<<
  * 
  *     #if (i == 50):
@@ -3973,31 +4041,31 @@
   /* "geomm/pyqcprot.pyx":397
  *     # the fabs() is to guard against extremely small,
  *     # but *negative* numbers due to floating point error
  *     rms = sqrt(fabs(2.0 * (E0 - mxEigenV)/N))             # <<<<<<<<<<<<<<
  * 
  *     if (rot is None):
  */
-  __pyx_t_23 = (2.0 * (__pyx_v_E0 - __pyx_v_mxEigenV));
+  __pyx_t_9 = (2.0 * (__pyx_v_E0 - __pyx_v_mxEigenV));
   if (unlikely(__pyx_v_N == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
     __PYX_ERR(0, 397, __pyx_L1_error)
   }
-  __pyx_v_rms = sqrt(fabs((__pyx_t_23 / __pyx_v_N)));
+  __pyx_v_rms = sqrt(fabs((__pyx_t_9 / __pyx_v_N)));
 
   /* "geomm/pyqcprot.pyx":399
  *     rms = sqrt(fabs(2.0 * (E0 - mxEigenV)/N))
  * 
  *     if (rot is None):             # <<<<<<<<<<<<<<
  *         return rms # Don't bother with rotation.
  * 
  */
-  __pyx_t_24 = (((PyObject *)__pyx_v_rot) == Py_None);
-  __pyx_t_25 = (__pyx_t_24 != 0);
-  if (__pyx_t_25) {
+  __pyx_t_10 = (((PyObject *)__pyx_v_rot) == Py_None);
+  __pyx_t_11 = (__pyx_t_10 != 0);
+  if (__pyx_t_11) {
 
     /* "geomm/pyqcprot.pyx":400
  * 
  *     if (rot is None):
  *         return rms # Don't bother with rotation.             # <<<<<<<<<<<<<<
  * 
  *     a11 = SxxpSyy + Szz-mxEigenV
@@ -4264,16 +4332,16 @@
   /* "geomm/pyqcprot.pyx":436
  *     # uncommented, but it is most likely unnecessary.
  * 
  *     if (qsqr < evecprec):             # <<<<<<<<<<<<<<
  *         q1 =  a12*a3344_4334 - a13*a3244_4234 + a14*a3243_4233
  *         q2 = -a11*a3344_4334 + a13*a3144_4134 - a14*a3143_4133
  */
-  __pyx_t_25 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
-  if (__pyx_t_25) {
+  __pyx_t_11 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
+  if (__pyx_t_11) {
 
     /* "geomm/pyqcprot.pyx":437
  * 
  *     if (qsqr < evecprec):
  *         q1 =  a12*a3344_4334 - a13*a3244_4234 + a14*a3243_4233             # <<<<<<<<<<<<<<
  *         q2 = -a11*a3344_4334 + a13*a3144_4134 - a14*a3143_4133
  *         q3 =  a11*a3244_4234 - a12*a3144_4134 + a14*a3142_4132
@@ -4319,16 +4387,16 @@
     /* "geomm/pyqcprot.pyx":443
  *         qsqr = q1*q1 + q2 *q2 + q3*q3+q4*q4
  * 
  *         if (qsqr < evecprec):             # <<<<<<<<<<<<<<
  *             a1324_1423 = a13 * a24 - a14 * a23
  *             a1224_1422 = a12 * a24 - a14 * a22
  */
-    __pyx_t_25 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
-    if (__pyx_t_25) {
+    __pyx_t_11 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
+    if (__pyx_t_11) {
 
       /* "geomm/pyqcprot.pyx":444
  * 
  *         if (qsqr < evecprec):
  *             a1324_1423 = a13 * a24 - a14 * a23             # <<<<<<<<<<<<<<
  *             a1224_1422 = a12 * a24 - a14 * a22
  *             a1223_1322 = a12 * a23 - a13 * a22
@@ -4428,16 +4496,16 @@
       /* "geomm/pyqcprot.pyx":457
  *             qsqr = q1*q1 + q2 *q2 + q3*q3+q4*q4
  * 
  *             if (qsqr < evecprec):             # <<<<<<<<<<<<<<
  *                 q1 =  a32 * a1324_1423 - a33 * a1224_1422 + a34 * a1223_1322
  *                 q2 = -a31 * a1324_1423 + a33 * a1124_1421 - a34 * a1123_1321
  */
-      __pyx_t_25 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
-      if (__pyx_t_25) {
+      __pyx_t_11 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
+      if (__pyx_t_11) {
 
         /* "geomm/pyqcprot.pyx":458
  * 
  *             if (qsqr < evecprec):
  *                 q1 =  a32 * a1324_1423 - a33 * a1224_1422 + a34 * a1223_1322             # <<<<<<<<<<<<<<
  *                 q2 = -a31 * a1324_1423 + a33 * a1124_1421 - a34 * a1123_1321
  *                 q3 =  a31 * a1224_1422 - a32 * a1124_1421 + a34 * a1122_1221
@@ -4483,131 +4551,131 @@
         /* "geomm/pyqcprot.pyx":464
  *                 qsqr = q1*q1 + q2 *q2 + q3*q3 + q4*q4
  * 
  *                 if (qsqr < evecprec):             # <<<<<<<<<<<<<<
  *                     # if qsqr is still too small, return the identity matrix. #
  *                     rot[0] = rot[4] = rot[8] = 1.0
  */
-        __pyx_t_25 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
-        if (__pyx_t_25) {
+        __pyx_t_11 = ((__pyx_v_qsqr < __pyx_v_evecprec) != 0);
+        if (__pyx_t_11) {
 
           /* "geomm/pyqcprot.pyx":466
  *                 if (qsqr < evecprec):
  *                     # if qsqr is still too small, return the identity matrix. #
  *                     rot[0] = rot[4] = rot[8] = 1.0             # <<<<<<<<<<<<<<
  *                     rot[1] = rot[2] = rot[3] = rot[5] = rot[6] = rot[7] = 0.0
  * 
  */
-          __pyx_t_26 = 0;
+          __pyx_t_5 = 0;
           __pyx_t_6 = -1;
-          if (__pyx_t_26 < 0) {
-            __pyx_t_26 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_26 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_26 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 466, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
-          __pyx_t_27 = 4;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
+          __pyx_t_5 = 4;
           __pyx_t_6 = -1;
-          if (__pyx_t_27 < 0) {
-            __pyx_t_27 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_27 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_27 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 466, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_27, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
-          __pyx_t_28 = 8;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
+          __pyx_t_5 = 8;
           __pyx_t_6 = -1;
-          if (__pyx_t_28 < 0) {
-            __pyx_t_28 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_28 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_28 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 466, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 1.0;
 
           /* "geomm/pyqcprot.pyx":467
  *                     # if qsqr is still too small, return the identity matrix. #
  *                     rot[0] = rot[4] = rot[8] = 1.0
  *                     rot[1] = rot[2] = rot[3] = rot[5] = rot[6] = rot[7] = 0.0             # <<<<<<<<<<<<<<
  * 
  *                     return
  */
-          __pyx_t_29 = 1;
+          __pyx_t_5 = 1;
           __pyx_t_6 = -1;
-          if (__pyx_t_29 < 0) {
-            __pyx_t_29 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_29 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_29 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_29, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
-          __pyx_t_30 = 2;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          __pyx_t_5 = 2;
           __pyx_t_6 = -1;
-          if (__pyx_t_30 < 0) {
-            __pyx_t_30 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_30 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_30 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
-          __pyx_t_31 = 3;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          __pyx_t_5 = 3;
           __pyx_t_6 = -1;
-          if (__pyx_t_31 < 0) {
-            __pyx_t_31 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_31 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_31 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_31, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
-          __pyx_t_32 = 5;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          __pyx_t_5 = 5;
           __pyx_t_6 = -1;
-          if (__pyx_t_32 < 0) {
-            __pyx_t_32 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_32 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_32 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
-          __pyx_t_33 = 6;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          __pyx_t_5 = 6;
           __pyx_t_6 = -1;
-          if (__pyx_t_33 < 0) {
-            __pyx_t_33 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_33 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_33 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
-          __pyx_t_34 = 7;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          __pyx_t_5 = 7;
           __pyx_t_6 = -1;
-          if (__pyx_t_34 < 0) {
-            __pyx_t_34 += __pyx_pybuffernd_rot.diminfo[0].shape;
-            if (unlikely(__pyx_t_34 < 0)) __pyx_t_6 = 0;
-          } else if (unlikely(__pyx_t_34 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+          if (__pyx_t_5 < 0) {
+            __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+            if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+          } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
           if (unlikely(__pyx_t_6 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_6);
             __PYX_ERR(0, 467, __pyx_L1_error)
           }
-          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
+          *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = 0.0;
 
           /* "geomm/pyqcprot.pyx":469
  *                     rot[1] = rot[2] = rot[3] = rot[5] = rot[6] = rot[7] = 0.0
  * 
  *                     return             # <<<<<<<<<<<<<<
  * 
  * 
@@ -4806,177 +4874,177 @@
   /* "geomm/pyqcprot.pyx":490
  *     ax = q1 * q2
  * 
  *     rot[0] = a2 + x2 - y2 - z2             # <<<<<<<<<<<<<<
  *     rot[1] = 2 * (xy + az)
  *     rot[2] = 2 * (zx - ay)
  */
-  __pyx_t_35 = 0;
+  __pyx_t_5 = 0;
   __pyx_t_6 = -1;
-  if (__pyx_t_35 < 0) {
-    __pyx_t_35 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_35 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_35 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 490, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 + __pyx_v_x2) - __pyx_v_y2) - __pyx_v_z2);
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 + __pyx_v_x2) - __pyx_v_y2) - __pyx_v_z2);
 
   /* "geomm/pyqcprot.pyx":491
  * 
  *     rot[0] = a2 + x2 - y2 - z2
  *     rot[1] = 2 * (xy + az)             # <<<<<<<<<<<<<<
  *     rot[2] = 2 * (zx - ay)
  *     rot[3] = 2 * (xy - az)
  */
-  __pyx_t_36 = 1;
+  __pyx_t_5 = 1;
   __pyx_t_6 = -1;
-  if (__pyx_t_36 < 0) {
-    __pyx_t_36 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_36 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_36 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 491, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_xy + __pyx_v_az));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_xy + __pyx_v_az));
 
   /* "geomm/pyqcprot.pyx":492
  *     rot[0] = a2 + x2 - y2 - z2
  *     rot[1] = 2 * (xy + az)
  *     rot[2] = 2 * (zx - ay)             # <<<<<<<<<<<<<<
  *     rot[3] = 2 * (xy - az)
  *     rot[4] = a2 - x2 + y2 - z2
  */
-  __pyx_t_37 = 2;
+  __pyx_t_5 = 2;
   __pyx_t_6 = -1;
-  if (__pyx_t_37 < 0) {
-    __pyx_t_37 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_37 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_37 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 492, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_zx - __pyx_v_ay));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_zx - __pyx_v_ay));
 
   /* "geomm/pyqcprot.pyx":493
  *     rot[1] = 2 * (xy + az)
  *     rot[2] = 2 * (zx - ay)
  *     rot[3] = 2 * (xy - az)             # <<<<<<<<<<<<<<
  *     rot[4] = a2 - x2 + y2 - z2
  *     rot[5] = 2 * (yz + ax)
  */
-  __pyx_t_38 = 3;
+  __pyx_t_5 = 3;
   __pyx_t_6 = -1;
-  if (__pyx_t_38 < 0) {
-    __pyx_t_38 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_38 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_38 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 493, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_xy - __pyx_v_az));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_xy - __pyx_v_az));
 
   /* "geomm/pyqcprot.pyx":494
  *     rot[2] = 2 * (zx - ay)
  *     rot[3] = 2 * (xy - az)
  *     rot[4] = a2 - x2 + y2 - z2             # <<<<<<<<<<<<<<
  *     rot[5] = 2 * (yz + ax)
  *     rot[6] = 2 * (zx + ay)
  */
-  __pyx_t_39 = 4;
+  __pyx_t_5 = 4;
   __pyx_t_6 = -1;
-  if (__pyx_t_39 < 0) {
-    __pyx_t_39 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_39 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_39 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 494, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 - __pyx_v_x2) + __pyx_v_y2) - __pyx_v_z2);
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 - __pyx_v_x2) + __pyx_v_y2) - __pyx_v_z2);
 
   /* "geomm/pyqcprot.pyx":495
  *     rot[3] = 2 * (xy - az)
  *     rot[4] = a2 - x2 + y2 - z2
  *     rot[5] = 2 * (yz + ax)             # <<<<<<<<<<<<<<
  *     rot[6] = 2 * (zx + ay)
  *     rot[7] = 2 * (yz - ax)
  */
-  __pyx_t_40 = 5;
+  __pyx_t_5 = 5;
   __pyx_t_6 = -1;
-  if (__pyx_t_40 < 0) {
-    __pyx_t_40 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_40 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_40 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 495, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_yz + __pyx_v_ax));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_yz + __pyx_v_ax));
 
   /* "geomm/pyqcprot.pyx":496
  *     rot[4] = a2 - x2 + y2 - z2
  *     rot[5] = 2 * (yz + ax)
  *     rot[6] = 2 * (zx + ay)             # <<<<<<<<<<<<<<
  *     rot[7] = 2 * (yz - ax)
  *     rot[8] = a2 - x2 - y2 + z2
  */
-  __pyx_t_41 = 6;
+  __pyx_t_5 = 6;
   __pyx_t_6 = -1;
-  if (__pyx_t_41 < 0) {
-    __pyx_t_41 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_41 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_41 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 496, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_zx + __pyx_v_ay));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_zx + __pyx_v_ay));
 
   /* "geomm/pyqcprot.pyx":497
  *     rot[5] = 2 * (yz + ax)
  *     rot[6] = 2 * (zx + ay)
  *     rot[7] = 2 * (yz - ax)             # <<<<<<<<<<<<<<
  *     rot[8] = a2 - x2 - y2 + z2
  * 
  */
-  __pyx_t_42 = 7;
+  __pyx_t_5 = 7;
   __pyx_t_6 = -1;
-  if (__pyx_t_42 < 0) {
-    __pyx_t_42 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_42 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_42 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 497, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_42, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_yz - __pyx_v_ax));
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (2.0 * (__pyx_v_yz - __pyx_v_ax));
 
   /* "geomm/pyqcprot.pyx":498
  *     rot[6] = 2 * (zx + ay)
  *     rot[7] = 2 * (yz - ax)
  *     rot[8] = a2 - x2 - y2 + z2             # <<<<<<<<<<<<<<
  * 
  *     return rms
  */
-  __pyx_t_43 = 8;
+  __pyx_t_5 = 8;
   __pyx_t_6 = -1;
-  if (__pyx_t_43 < 0) {
-    __pyx_t_43 += __pyx_pybuffernd_rot.diminfo[0].shape;
-    if (unlikely(__pyx_t_43 < 0)) __pyx_t_6 = 0;
-  } else if (unlikely(__pyx_t_43 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
+  if (__pyx_t_5 < 0) {
+    __pyx_t_5 += __pyx_pybuffernd_rot.diminfo[0].shape;
+    if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+  } else if (unlikely(__pyx_t_5 >= __pyx_pybuffernd_rot.diminfo[0].shape)) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
     __PYX_ERR(0, 498, __pyx_L1_error)
   }
-  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_43, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 - __pyx_v_x2) - __pyx_v_y2) + __pyx_v_z2);
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rot.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_rot.diminfo[0].strides) = (((__pyx_v_a2 - __pyx_v_x2) - __pyx_v_y2) + __pyx_v_z2);
 
   /* "geomm/pyqcprot.pyx":500
  *     rot[8] = a2 - x2 - y2 + z2
  * 
  *     return rms             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5017,899 +5085,46 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_C);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 272, __pyx_L1_error)
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 276, __pyx_L1_error)
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 306, __pyx_L1_error)
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":822
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 822, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5920,43 +5135,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":825
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5967,43 +5185,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":828
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 828, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6014,43 +5235,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":831
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 831, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6061,43 +5285,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":834
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 834, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6108,1069 +5335,326 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":838
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":840
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":842
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":848
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 851, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 851, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 852, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":853
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 853, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 853, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 853, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 853, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 853, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 855, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 855, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":856
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 856, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 856, __pyx_L1_error)
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":860
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 860, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 860, __pyx_L1_error)
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 870, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 870, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 870, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":873
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":875
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 878, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":880
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 880, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 880, __pyx_L1_error)
-
-        /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":899
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 899, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 899, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 899, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 901, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 901, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 901, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":902
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 906, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":907
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":842
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1024
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1030
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1036, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1038
- *         _import_array()
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":944
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1038, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1038, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -7180,15 +5664,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7199,17 +5683,20 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7217,84 +5704,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1042, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1044, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1044, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7309,15 +5796,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7328,17 +5815,20 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7346,81 +5836,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1048, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1050
+      /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1050, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1050, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+    /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7435,14 +5928,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":966
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":978
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":966
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":981
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":993
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":981
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":996
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":996
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -7486,23 +6153,19 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_A, __pyx_k_A, sizeof(__pyx_k_A), 0, 0, 1, 1},
   {&__pyx_n_s_C, __pyx_k_C, sizeof(__pyx_k_C), 0, 0, 1, 1},
   {&__pyx_n_s_CalcRMSDRotationalMatrix, __pyx_k_CalcRMSDRotationalMatrix, sizeof(__pyx_k_CalcRMSDRotationalMatrix), 0, 0, 1, 1},
   {&__pyx_n_s_E0, __pyx_k_E0, sizeof(__pyx_k_E0), 0, 0, 1, 1},
   {&__pyx_n_s_FastCalcRMSDAndRotation, __pyx_k_FastCalcRMSDAndRotation, sizeof(__pyx_k_FastCalcRMSDAndRotation), 0, 0, 1, 1},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_G1, __pyx_k_G1, sizeof(__pyx_k_G1), 0, 0, 1, 1},
   {&__pyx_n_s_G2, __pyx_k_G2, sizeof(__pyx_k_G2), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_n_s_InnerProduct, __pyx_k_InnerProduct, sizeof(__pyx_k_InnerProduct), 0, 0, 1, 1},
   {&__pyx_n_s_N, __pyx_k_N, sizeof(__pyx_k_N), 0, 0, 1, 1},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_Sxx, __pyx_k_Sxx, sizeof(__pyx_k_Sxx), 0, 0, 1, 1},
   {&__pyx_n_s_Sxx2, __pyx_k_Sxx2, sizeof(__pyx_k_Sxx2), 0, 0, 1, 1},
   {&__pyx_n_s_Sxx2Syy2Szz2Syz2Szy2, __pyx_k_Sxx2Syy2Szz2Syz2Szy2, sizeof(__pyx_k_Sxx2Syy2Szz2Syz2Szy2), 0, 0, 1, 1},
   {&__pyx_n_s_SxxmSyy, __pyx_k_SxxmSyy, sizeof(__pyx_k_SxxmSyy), 0, 0, 1, 1},
   {&__pyx_n_s_SxxpSyy, __pyx_k_SxxpSyy, sizeof(__pyx_k_SxxpSyy), 0, 0, 1, 1},
   {&__pyx_n_s_Sxy, __pyx_k_Sxy, sizeof(__pyx_k_Sxy), 0, 0, 1, 1},
   {&__pyx_n_s_Sxy2, __pyx_k_Sxy2, sizeof(__pyx_k_Sxy2), 0, 0, 1, 1},
@@ -7524,15 +6187,14 @@
   {&__pyx_n_s_SyzpSzy, __pyx_k_SyzpSzy, sizeof(__pyx_k_SyzpSzy), 0, 0, 1, 1},
   {&__pyx_n_s_Szx, __pyx_k_Szx, sizeof(__pyx_k_Szx), 0, 0, 1, 1},
   {&__pyx_n_s_Szx2, __pyx_k_Szx2, sizeof(__pyx_k_Szx2), 0, 0, 1, 1},
   {&__pyx_n_s_Szy, __pyx_k_Szy, sizeof(__pyx_k_Szy), 0, 0, 1, 1},
   {&__pyx_n_s_Szy2, __pyx_k_Szy2, sizeof(__pyx_k_Szy2), 0, 0, 1, 1},
   {&__pyx_n_s_Szz, __pyx_k_Szz, sizeof(__pyx_k_Szz), 0, 0, 1, 1},
   {&__pyx_n_s_Szz2, __pyx_k_Szz2, sizeof(__pyx_k_Szz2), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_a11, __pyx_k_a11, sizeof(__pyx_k_a11), 0, 0, 1, 1},
   {&__pyx_n_s_a1122_1221, __pyx_k_a1122_1221, sizeof(__pyx_k_a1122_1221), 0, 0, 1, 1},
   {&__pyx_n_s_a1123_1321, __pyx_k_a1123_1321, sizeof(__pyx_k_a1123_1321), 0, 0, 1, 1},
   {&__pyx_n_s_a1124_1421, __pyx_k_a1124_1421, sizeof(__pyx_k_a1124_1421), 0, 0, 1, 1},
   {&__pyx_n_s_a12, __pyx_k_a12, sizeof(__pyx_k_a12), 0, 0, 1, 1},
   {&__pyx_n_s_a1223_1322, __pyx_k_a1223_1322, sizeof(__pyx_k_a1223_1322), 0, 0, 1, 1},
@@ -7574,16 +6236,14 @@
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_geomm_pyqcprot, __pyx_k_geomm_pyqcprot, sizeof(__pyx_k_geomm_pyqcprot), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_mxEigenV, __pyx_k_mxEigenV, sizeof(__pyx_k_mxEigenV), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
   {&__pyx_n_s_normq, __pyx_k_normq, sizeof(__pyx_k_normq), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
   {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
   {&__pyx_n_s_oldg, __pyx_k_oldg, sizeof(__pyx_k_oldg), 0, 0, 1, 1},
   {&__pyx_n_s_q1, __pyx_k_q1, sizeof(__pyx_k_q1), 0, 0, 1, 1},
@@ -7594,15 +6254,14 @@
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_ref, __pyx_k_ref, sizeof(__pyx_k_ref), 0, 0, 1, 1},
   {&__pyx_n_s_rms, __pyx_k_rms, sizeof(__pyx_k_rms), 0, 0, 1, 1},
   {&__pyx_n_s_rmsd, __pyx_k_rmsd, sizeof(__pyx_k_rmsd), 0, 0, 1, 1},
   {&__pyx_n_s_rot, __pyx_k_rot, sizeof(__pyx_k_rot), 0, 0, 1, 1},
   {&__pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_k_src_geomm_pyqcprot_pyx, sizeof(__pyx_k_src_geomm_pyqcprot_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_weight, __pyx_k_weight, sizeof(__pyx_k_weight), 0, 0, 1, 1},
   {&__pyx_n_s_weights, __pyx_k_weights, sizeof(__pyx_k_weights), 0, 0, 1, 1},
   {&__pyx_n_s_x1, __pyx_k_x1, sizeof(__pyx_k_x1), 0, 0, 1, 1},
   {&__pyx_n_s_x2, __pyx_k_x2, sizeof(__pyx_k_x2), 0, 0, 1, 1},
   {&__pyx_n_s_xy, __pyx_k_xy, sizeof(__pyx_k_xy), 0, 0, 1, 1},
   {&__pyx_n_s_y1, __pyx_k_y1, sizeof(__pyx_k_y1), 0, 0, 1, 1},
   {&__pyx_n_s_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 0, 1, 1},
@@ -7611,17 +6270,15 @@
   {&__pyx_n_s_z2, __pyx_k_z2, sizeof(__pyx_k_z2), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {&__pyx_n_s_zx, __pyx_k_zx, sizeof(__pyx_k_zx), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 198, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 856, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1038, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -7634,135 +6291,80 @@
  * 
  *     E0 = InnerProduct(A, conf, ref, N, weights)
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_int_9); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":856
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 856, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":880
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 880, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1038
- *         _import_array()
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":944
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1038, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1044, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "geomm/pyqcprot.pyx":150
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def InnerProduct(np.ndarray[np.float64_t, ndim=1] A,             # <<<<<<<<<<<<<<
  *                  np.ndarray[np.float64_t, ndim=2] coords1,
  *                  np.ndarray[np.float64_t, ndim=2] coords2,
  */
-  __pyx_tuple__9 = PyTuple_Pack(14, __pyx_n_s_A, __pyx_n_s_coords1, __pyx_n_s_coords2, __pyx_n_s_N, __pyx_n_s_weight, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_z1, __pyx_n_s_z2, __pyx_n_s_i, __pyx_n_s_G1, __pyx_n_s_G2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 150, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(5, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_InnerProduct, 150, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(14, __pyx_n_s_A, __pyx_n_s_coords1, __pyx_n_s_coords2, __pyx_n_s_N, __pyx_n_s_weight, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_z1, __pyx_n_s_z2, __pyx_n_s_i, __pyx_n_s_G1, __pyx_n_s_G2); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(5, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_InnerProduct, 150, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 150, __pyx_L1_error)
 
   /* "geomm/pyqcprot.pyx":253
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def CalcRMSDRotationalMatrix(np.ndarray[np.float64_t, ndim=2] ref,             # <<<<<<<<<<<<<<
  *                              np.ndarray[np.float64_t, ndim=2] conf,
  *                              int N,
  */
-  __pyx_tuple__11 = PyTuple_Pack(7, __pyx_n_s_ref, __pyx_n_s_conf, __pyx_n_s_N, __pyx_n_s_rot, __pyx_n_s_weights, __pyx_n_s_E0, __pyx_n_s_A); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 253, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_CalcRMSDRotationalMatrix, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(7, __pyx_n_s_ref, __pyx_n_s_conf, __pyx_n_s_N, __pyx_n_s_rot, __pyx_n_s_weights, __pyx_n_s_E0, __pyx_n_s_A); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_CalcRMSDRotationalMatrix, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 253, __pyx_L1_error)
 
   /* "geomm/pyqcprot.pyx":288
  *     return FastCalcRMSDAndRotation(rot, A, E0, N)
  * 
  * def FastCalcRMSDAndRotation(np.ndarray[np.float64_t, ndim=1] rot,             # <<<<<<<<<<<<<<
  *                             np.ndarray[np.float64_t, ndim=1] A,
  *                             double E0, int N):
  */
-  __pyx_tuple__13 = PyTuple_Pack(88, __pyx_n_s_rot, __pyx_n_s_A, __pyx_n_s_E0, __pyx_n_s_N, __pyx_n_s_rmsd, __pyx_n_s_Sxx, __pyx_n_s_Sxy, __pyx_n_s_Sxz, __pyx_n_s_Syx, __pyx_n_s_Syy, __pyx_n_s_Syz, __pyx_n_s_Szx, __pyx_n_s_Szy, __pyx_n_s_Szz, __pyx_n_s_Szz2, __pyx_n_s_Syy2, __pyx_n_s_Sxx2, __pyx_n_s_Sxy2, __pyx_n_s_Syz2, __pyx_n_s_Sxz2, __pyx_n_s_Syx2, __pyx_n_s_Szy2, __pyx_n_s_Szx2, __pyx_n_s_SyzSzymSyySzz2, __pyx_n_s_Sxx2Syy2Szz2Syz2Szy2, __pyx_n_s_Sxy2Sxz2Syx2Szx2, __pyx_n_s_SxzpSzx, __pyx_n_s_SyzpSzy, __pyx_n_s_SxypSyx, __pyx_n_s_SyzmSzy, __pyx_n_s_SxzmSzx, __pyx_n_s_SxymSyx, __pyx_n_s_SxxpSyy, __pyx_n_s_SxxmSyy, __pyx_n_s_C, __pyx_n_s_i, __pyx_n_s_mxEigenV, __pyx_n_s_oldg, __pyx_n_s_b, __pyx_n_s_a, __pyx_n_s_delta, __pyx_n_s_rms, __pyx_n_s_qsqr, __pyx_n_s_q1, __pyx_n_s_q2, __pyx_n_s_q3, __pyx_n_s_q4, __pyx_n_s_normq, __pyx_n_s_a11, __pyx_n_s_a12, __pyx_n_s_a13, __pyx_n_s_a14, __pyx_n_s_a21, __pyx_n_s_a22, __pyx_n_s_a23, __pyx_n_s_a24, __pyx_n_s_a31, __pyx_n_s_a32, __pyx_n_s_a33, __pyx_n_s_a34, __pyx_n_s_a41, __pyx_n_s_a42, __pyx_n_s_a43, __pyx_n_s_a44, __pyx_n_s_a2, __pyx_n_s_x2, __pyx_n_s_y2, __pyx_n_s_z2, __pyx_n_s_xy, __pyx_n_s_az, __pyx_n_s_zx, __pyx_n_s_ay, __pyx_n_s_yz, __pyx_n_s_ax, __pyx_n_s_a3344_4334, __pyx_n_s_a3244_4234, __pyx_n_s_a3243_4233, __pyx_n_s_a3143_4133, __pyx_n_s_a3144_4134, __pyx_n_s_a3142_4132, __pyx_n_s_evecprec, __pyx_n_s_evalprec, __pyx_n_s_a1324_1423, __pyx_n_s_a1224_1422, __pyx_n_s_a1223_1322, __pyx_n_s_a1124_1421, __pyx_n_s_a1123_1321, __pyx_n_s_a1122_1221); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(4, 0, 88, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_FastCalcRMSDAndRotation, 288, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(88, __pyx_n_s_rot, __pyx_n_s_A, __pyx_n_s_E0, __pyx_n_s_N, __pyx_n_s_rmsd, __pyx_n_s_Sxx, __pyx_n_s_Sxy, __pyx_n_s_Sxz, __pyx_n_s_Syx, __pyx_n_s_Syy, __pyx_n_s_Syz, __pyx_n_s_Szx, __pyx_n_s_Szy, __pyx_n_s_Szz, __pyx_n_s_Szz2, __pyx_n_s_Syy2, __pyx_n_s_Sxx2, __pyx_n_s_Sxy2, __pyx_n_s_Syz2, __pyx_n_s_Sxz2, __pyx_n_s_Syx2, __pyx_n_s_Szy2, __pyx_n_s_Szx2, __pyx_n_s_SyzSzymSyySzz2, __pyx_n_s_Sxx2Syy2Szz2Syz2Szy2, __pyx_n_s_Sxy2Sxz2Syx2Szx2, __pyx_n_s_SxzpSzx, __pyx_n_s_SyzpSzy, __pyx_n_s_SxypSyx, __pyx_n_s_SyzmSzy, __pyx_n_s_SxzmSzx, __pyx_n_s_SxymSyx, __pyx_n_s_SxxpSyy, __pyx_n_s_SxxmSyy, __pyx_n_s_C, __pyx_n_s_i, __pyx_n_s_mxEigenV, __pyx_n_s_oldg, __pyx_n_s_b, __pyx_n_s_a, __pyx_n_s_delta, __pyx_n_s_rms, __pyx_n_s_qsqr, __pyx_n_s_q1, __pyx_n_s_q2, __pyx_n_s_q3, __pyx_n_s_q4, __pyx_n_s_normq, __pyx_n_s_a11, __pyx_n_s_a12, __pyx_n_s_a13, __pyx_n_s_a14, __pyx_n_s_a21, __pyx_n_s_a22, __pyx_n_s_a23, __pyx_n_s_a24, __pyx_n_s_a31, __pyx_n_s_a32, __pyx_n_s_a33, __pyx_n_s_a34, __pyx_n_s_a41, __pyx_n_s_a42, __pyx_n_s_a43, __pyx_n_s_a44, __pyx_n_s_a2, __pyx_n_s_x2, __pyx_n_s_y2, __pyx_n_s_z2, __pyx_n_s_xy, __pyx_n_s_az, __pyx_n_s_zx, __pyx_n_s_ay, __pyx_n_s_yz, __pyx_n_s_ax, __pyx_n_s_a3344_4334, __pyx_n_s_a3244_4234, __pyx_n_s_a3243_4233, __pyx_n_s_a3143_4133, __pyx_n_s_a3144_4134, __pyx_n_s_a3142_4132, __pyx_n_s_evecprec, __pyx_n_s_evalprec, __pyx_n_s_a1324_1423, __pyx_n_s_a1224_1422, __pyx_n_s_a1223_1322, __pyx_n_s_a1124_1421, __pyx_n_s_a1123_1321, __pyx_n_s_a1122_1221); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 88, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_geomm_pyqcprot_pyx, __pyx_n_s_FastCalcRMSDAndRotation, 288, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_9 = PyInt_FromLong(9); if (unlikely(!__pyx_int_9)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -7805,39 +6407,77 @@
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 918, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7856,25 +6496,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initpyqcprot(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initpyqcprot(void)
@@ -7948,14 +6590,17 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_pyqcprot(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'pyqcprot' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -7995,19 +6640,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("pyqcprot", __pyx_methods, __pyx_k_Fast_QCP_RMSD_structure_alignme, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -8018,15 +6661,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_geomm__pyqcprot) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8036,23 +6679,23 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "geomm.pyqcprot")) {
       if (unlikely(PyDict_SetItemString(modules, "geomm.pyqcprot", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() != 0)) goto __pyx_L1_error;
+  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
@@ -8110,20 +6753,20 @@
  * #                  Douglas L. Theobald
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../tmp/pip-build-env-jxtwwji2/overlay/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../anaconda3/envs/wepy/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -8250,15 +6893,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -8277,15 +6920,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -8293,15 +6936,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -8689,24 +7332,23 @@
   ctx->is_complex = 0;
   return 0;
 }
 static PyObject *
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
-    int i = 0, number;
-    int ndim = ctx->head->field->type->ndim;
-;
+    int i = 0, number, ndim;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
         return NULL;
     }
     if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
         if (number == -1) return NULL;
@@ -8828,16 +7470,16 @@
           return NULL;
         }
         CYTHON_FALLTHROUGH;
       case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
       case 'l': case 'L': case 'q': case 'Q':
       case 'f': case 'd': case 'g':
       case 'O': case 'p':
-        if (ctx->enc_type == *ts && got_Z == ctx->is_complex &&
-            ctx->enc_packmode == ctx->new_packmode) {
+        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
+            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
           ctx->enc_count += ctx->new_count;
           ctx->new_count = 1;
           got_Z = 0;
           ++ts;
           break;
         }
         CYTHON_FALLTHROUGH;
@@ -9001,15 +7643,15 @@
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -9243,15 +7885,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -9267,215 +7909,14 @@
 
 /* BufferIndexError */
   static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* DictGetItem */
-  #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-  static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -9623,48 +8064,225 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
+/* RaiseException */
+  #if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -9714,15 +8332,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -9751,15 +8369,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -9781,15 +8399,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -9855,15 +8473,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -9875,41 +8493,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -9920,34 +8545,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -9959,27 +8599,25 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
   /* CIntFromPyVerify */
@@ -10000,45 +8638,14 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* Declarations */
   #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -10160,15 +8767,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -10314,15 +8921,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -10339,48 +8946,24 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) ((enum NPY_TYPES) 0 - (enum NPY_TYPES) 1), const_zero = (enum NPY_TYPES) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -10559,17 +9142,62 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
-    const unsigned int neg_one = (unsigned int) ((unsigned int) 0 - (unsigned int) 1), const_zero = (unsigned int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(unsigned int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(unsigned int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -10750,15 +9378,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned int");
     return (unsigned int) -1;
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -10781,15 +9416,22 @@
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -11070,19 +9712,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -11332,14 +9996,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `geomm-0.2.0.dev0/src/geomm/pyqcprot.pyx` & `geomm-0.2.1/src/geomm/pyqcprot.pyx`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/rmsd.py` & `geomm-0.2.1/src/geomm/rmsd.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/sasa.py` & `geomm-0.2.1/src/geomm/sasa.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/superimpose.py` & `geomm-0.2.1/src/geomm/superimpose.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm/theobald_qcp.py` & `geomm-0.2.1/src/geomm/theobald_qcp.py`

 * *Files identical despite different names*

### Comparing `geomm-0.2.0.dev0/src/geomm.egg-info/PKG-INFO` & `geomm-0.2.1/src/geomm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: geomm
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: A simple no-nonsense library for computing common geometry on macromolecular systems.
 Home-page: https://github.com/ADicksonLab/geomm
 Author: Samuel D. Lotz
 Author-email: samuel.lotz@salotz.info
 License: MIT
-Description: UNKNOWN
 Keywords: geometry chemistry macromolecules protein structural-informatics
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
+License-File: LICENSE
+License-File: AUTHORS.org
```

