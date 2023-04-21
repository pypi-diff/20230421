# Comparing `tmp/pycodata-0.4.0.tar.gz` & `tmp/pycodata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-0.4.0.tar", last modified: Sun Apr  2 05:50:28 2023, max compression
+gzip compressed data, was "pycodata-0.5.0.tar", last modified: Fri Apr 21 13:29:25 2023, max compression
```

## Comparing `pycodata-0.4.0.tar` & `pycodata-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,20 @@
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.748825 pycodata-0.4.0/
--rw-r--r--   0 milan      (501) staff       (20)       20 2023-03-30 04:39:27.000000 pycodata-0.4.0/INSTALL.TXT
--rw-r--r--   0 milan      (501) staff       (20)    35823 2023-03-30 04:39:27.000000 pycodata-0.4.0/LICENSE.TXT
--rw-r--r--   0 milan      (501) staff       (20)      261 2023-03-30 05:02:52.000000 pycodata-0.4.0/MANIFEST.in
--rw-r--r--   0 milan      (501) staff       (20)     2221 2023-04-02 05:50:28.738859 pycodata-0.4.0/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)     1210 2023-03-30 04:39:27.000000 pycodata-0.4.0/README.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.625103 pycodata-0.4.0/pycodata/
--rw-r--r--   0 milan      (501) staff       (20)     1056 2023-03-30 04:39:27.000000 pycodata-0.4.0/pycodata/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)     4559 2023-03-30 04:39:27.000000 pycodata-0.4.0/pycodata/_codata.c
--rw-r--r--   0 milan      (501) staff       (20)      555 2023-03-30 04:39:27.000000 pycodata-0.4.0/pycodata/version.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.636764 pycodata-0.4.0/pycodata.egg-info/
--rw-r--r--   0 milan      (501) staff       (20)     2221 2023-04-02 05:50:28.000000 pycodata-0.4.0/pycodata.egg-info/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)      951 2023-04-02 05:50:28.000000 pycodata-0.4.0/pycodata.egg-info/SOURCES.txt
--rw-r--r--   0 milan      (501) staff       (20)        1 2023-04-02 05:50:28.000000 pycodata-0.4.0/pycodata.egg-info/dependency_links.txt
--rw-r--r--   0 milan      (501) staff       (20)        9 2023-04-02 05:50:28.000000 pycodata-0.4.0/pycodata.egg-info/top_level.txt
--rw-r--r--   0 milan      (501) staff       (20)        0 2023-03-30 04:39:27.000000 pycodata-0.4.0/requirements.txt
--rw-r--r--   0 milan      (501) staff       (20)       38 2023-04-02 05:50:28.759609 pycodata-0.4.0/setup.cfg
--rw-r--r--   0 milan      (501) staff       (20)     5380 2023-03-30 04:39:27.000000 pycodata-0.4.0/setup.py
--rw-r--r--   0 milan      (501) staff       (20)      334 2023-03-30 04:39:27.000000 pycodata-0.4.0/site.cfg.example
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.640633 pycodata-0.4.0/sphinx/
--rw-r--r--   0 milan      (501) staff       (20)     6148 2023-03-30 05:09:42.000000 pycodata-0.4.0/sphinx/.DS_Store
--rw-r--r--   0 milan      (501) staff       (20)      638 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/Makefile
--rw-r--r--   0 milan      (501) staff       (20)      799 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/make.bat
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.643041 pycodata-0.4.0/sphinx/source/
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.652977 pycodata-0.4.0/sphinx/source/api/
--rw-r--r--   0 milan      (501) staff       (20)      312 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/api/codedoc.rst
--rw-r--r--   0 milan      (501) staff       (20)      116 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/api/index.rst
--rw-r--r--   0 milan      (501) staff       (20)     5332 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/conf.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.662267 pycodata-0.4.0/sphinx/source/getting_started/
--rw-r--r--   0 milan      (501) staff       (20)       88 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/getting_started/index.rst
--rw-r--r--   0 milan      (501) staff       (20)      612 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/getting_started/introduction.rst
--rw-r--r--   0 milan      (501) staff       (20)      525 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/index.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-02 05:50:28.701589 pycodata-0.4.0/sphinx/source/releases/
--rw-r--r--   0 milan      (501) staff       (20)      374 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      330 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.1-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      334 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.2-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      372 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.3-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      372 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.4-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      372 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.5-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      387 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.2.6-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      410 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/0.3.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      401 2023-03-31 05:05:42.000000 pycodata-0.4.0/sphinx/source/releases/0.4.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      241 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/index.rst
--rw-r--r--   0 milan      (501) staff       (20)      427 2023-03-30 04:39:27.000000 pycodata-0.4.0/sphinx/source/releases/template.txt
+drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:29:25.007377 pycodata-0.5.0/
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)    35823 2022-12-23 14:14:18.000000 pycodata-0.5.0/LICENSE.txt
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      173 2023-04-18 09:06:17.000000 pycodata-0.5.0/MANIFEST.in
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      724 2023-04-21 13:29:25.007377 pycodata-0.5.0/PKG-INFO
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      257 2023-04-21 12:39:44.000000 pycodata-0.5.0/README.rst
+drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:29:25.003378 pycodata-0.5.0/pycodata/
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)       97 2023-04-18 08:58:24.000000 pycodata-0.5.0/pycodata/__init__.py
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)    94888 2023-04-21 12:47:49.000000 pycodata-0.5.0/pycodata/cpycodata.c
+drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:29:25.007377 pycodata-0.5.0/pycodata/tests/
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)        0 2023-04-12 09:50:16.000000 pycodata-0.5.0/pycodata/tests/__init__.py
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      250 2023-04-21 12:43:29.000000 pycodata-0.5.0/pycodata/tests/test_lib.py
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      555 2023-04-21 12:36:09.000000 pycodata-0.5.0/pycodata/version.py
+drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:29:25.007377 pycodata-0.5.0/pycodata.egg-info/
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      724 2023-04-21 13:29:24.000000 pycodata-0.5.0/pycodata.egg-info/PKG-INFO
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)      306 2023-04-21 13:29:24.000000 pycodata-0.5.0/pycodata.egg-info/SOURCES.txt
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)        1 2023-04-21 13:29:24.000000 pycodata-0.5.0/pycodata.egg-info/dependency_links.txt
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)        9 2023-04-21 13:29:24.000000 pycodata-0.5.0/pycodata.egg-info/top_level.txt
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)        0 2023-02-20 07:43:52.000000 pycodata-0.5.0/requirements.txt
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)       38 2023-04-21 13:29:25.007377 pycodata-0.5.0/setup.cfg
+-rw-r--r--   0 mskocic   (1000) mskocic   (1000)     1641 2023-04-21 12:49:32.000000 pycodata-0.5.0/setup.py
```

### Comparing `pycodata-0.4.0/LICENSE.TXT` & `pycodata-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycodata-0.4.0/pycodata/version.py` & `pycodata-0.5.0/pycodata/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
            '__author_email__',
            '__maintainer__',
            '__maintainer_email__',
            '__copyright__',
            '__license__']
 
 __package_name__ = "pycodata"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "Milan Skocic"
 __author_email__ = "milan.skocic@icloud.com"
 __maintainer__ = __author__
 __maintainer_email__ = __author_email__
 __copyright__ = 'Copyright (C) 2023 ' + __author__
 __license__ = 'GNU General Public License v3 (GPLv3)'
```

