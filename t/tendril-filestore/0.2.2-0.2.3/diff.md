# Comparing `tmp/tendril-filestore-0.2.2.tar.gz` & `tmp/tendril-filestore-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.2.2.tar", last modified: Fri Apr 21 08:12:11 2023, max compression
+gzip compressed data, was "tendril-filestore-0.2.3.tar", last modified: Fri Apr 21 12:48:54 2023, max compression
```

## Comparing `tendril-filestore-0.2.2.tar` & `tendril-filestore-0.2.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.318102 tendril-filestore-0.2.2/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-21 08:12:11.318102 tendril-filestore-0.2.2/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-21 08:12:11.318102 tendril-filestore-0.2.2/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.2.2/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.310102 tendril-filestore-0.2.2/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.2/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.2/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6100 2023-04-21 08:02:15.000000 tendril-filestore-0.2.2/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.2.2/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.2.2/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.2.2/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.2.2/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/common/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.2.2/src/tendril/common/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1646 2023-04-19 17:38:08.000000 tendril-filestore-0.2.2/src/tendril/common/filestore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.2.2/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3458 2023-04-20 12:32:52.000000 tendril-filestore-0.2.2/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.2.2/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6765 2023-04-21 06:02:17.000000 tendril-filestore-0.2.2/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1575 2023-04-21 05:38:37.000000 tendril-filestore-0.2.2/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2977 2023-04-20 15:56:35.000000 tendril-filestore-0.2.2/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.314102 tendril-filestore-0.2.2/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.2.2/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6250 2023-04-19 17:30:49.000000 tendril-filestore-0.2.2/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1426 2023-04-11 18:49:23.000000 tendril-filestore-0.2.2/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1886 2023-04-21 08:09:25.000000 tendril-filestore-0.2.2/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.318102 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-21 08:12:11.000000 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-04-21 08:12:11.000000 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-21 08:12:11.000000 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2023-04-21 08:12:11.000000 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-21 08:12:11.000000 tendril-filestore-0.2.2/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:12:11.318102 tendril-filestore-0.2.2/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.2.2/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.587120 tendril-filestore-0.2.3/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-21 12:48:54.595120 tendril-filestore-0.2.3/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.2.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.587120 tendril-filestore-0.2.3/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.3/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.3/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6100 2023-04-21 08:02:15.000000 tendril-filestore-0.2.3/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.2.3/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.2.3/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.2.3/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.2.3/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/common/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.2.3/src/tendril/common/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1646 2023-04-19 17:38:08.000000 tendril-filestore-0.2.3/src/tendril/common/filestore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.2.3/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3458 2023-04-20 12:32:52.000000 tendril-filestore-0.2.3/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.2.3/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6765 2023-04-21 12:45:53.000000 tendril-filestore-0.2.3/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1576 2023-04-21 12:45:53.000000 tendril-filestore-0.2.3/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2977 2023-04-20 15:56:35.000000 tendril-filestore-0.2.3/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.2.3/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6250 2023-04-19 17:30:49.000000 tendril-filestore-0.2.3/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1426 2023-04-11 18:49:23.000000 tendril-filestore-0.2.3/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2750 2023-04-21 12:45:53.000000 tendril-filestore-0.2.3/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-21 12:48:54.000000 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-04-21 12:48:54.000000 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-21 12:48:54.000000 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2023-04-21 12:48:54.000000 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-21 12:48:54.000000 tendril-filestore-0.2.3/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 12:48:54.591120 tendril-filestore-0.2.3/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.2.3/tox.ini
```

### Comparing `tendril-filestore-0.2.2/.gitignore` & `tendril-filestore-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/.readthedocs.yml` & `tendril-filestore-0.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/.travis.yml` & `tendril-filestore-0.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/LICENSE` & `tendril-filestore-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/PKG-INFO` & `tendril-filestore-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.2.2
+Version: 0.2.3
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.2.2/README.rst` & `tendril-filestore-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/Makefile` & `tendril-filestore-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/_static/custom.css` & `tendril-filestore-0.2.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/_static/favicon.ico` & `tendril-filestore-0.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/_static/logo.png` & `tendril-filestore-0.2.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/_static/logo_packed.png` & `tendril-filestore-0.2.3/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/_templates/about.html` & `tendril-filestore-0.2.3/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/conf.py` & `tendril-filestore-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/index.rst` & `tendril-filestore-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/docs/installation.rst` & `tendril-filestore-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/setup.py` & `tendril-filestore-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/apiserver/routers/filestore.py` & `tendril-filestore-0.2.3/src/tendril/apiserver/routers/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/common/filestore/formats.py` & `tendril-filestore-0.2.3/src/tendril/common/filestore/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/config/__init__.py` & `tendril-filestore-0.2.3/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/config/filestore.py` & `tendril-filestore-0.2.3/src/tendril/config/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/config/filestore_core.py` & `tendril-filestore-0.2.3/src/tendril/config/filestore_core.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/filestore/actual.py` & `tendril-filestore-0.2.3/src/tendril/filestore/actual.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,30 +117,14 @@
 
         self._prep_for_upload(target_bucket, filename, user, overwrite)
 
         logger.debug(f"Moving file {filename} from bucket {self.name} to {target_bucket.name}")
         move.move_file(self.fs, filename, target_bucket.fs, filename)
         return change_file_bucket(filename, self.id, target_bucket.id, user, session=session)
 
-    @with_db
-    def delete(self, filename, user, session=None):
-        if not self._fs.exists(filename):
-            raise FileNotFoundError(f"Delete of nonexisting file {filename} "
-                                    f"from bucket {self.name} requested.")
-
-        if not self._allow_delete:
-            owner = get_storedfile_owner(filename, self._id, session=session)
-            if owner.puid != user:
-                raise PermissionError(f"Deletion of file {filename} "
-                                      f"not permitted from bucket {self.name}")
-
-        logger.info(f"Deleting {filename} from bucket {self.name}")
-        self.fs.remove(filename)
-        delete_stored_file(filename, self.id, user, session=session)
-
     def _list(self, page=None):
         for f in self.fs.filterdir('/', page=page,
                                    exclude_files=self._exclude_filenames,
                                    exclude_dirs=self._exclude_directories):
             yield f.name
 
     def list(self, page=None):
@@ -153,14 +137,30 @@
             kwargs['filenames'] = filenames
         return get_paginated_stored_files(
             pagination_params=pagination_params,
             bucket=self.id, include_owner=include_owner,
             **kwargs
         )
 
+    @with_db
+    def delete(self, filename, user, session=None):
+        if not self._fs.exists(filename):
+            raise FileNotFoundError(f"Delete of nonexisting file {filename} "
+                                    f"from bucket {self.name} requested.")
+
+        if not self._allow_delete:
+            owner = get_storedfile_owner(filename, self._id, session=session)
+            if owner.puid != user:
+                raise PermissionError(f"Deletion of file {filename} "
+                                      f"not permitted from bucket {self.name}")
+
+        logger.info(f"Deleting {filename} from bucket {self.name}")
+        self.fs.remove(filename)
+        delete_stored_file(filename, self.id, user, session=session)
+
     def purge(self, user):
         if not self._allow_delete:
             raise PermissionError(f"Deletion of files from bucket {self.name} "
                                   f"is not permitted")
         logger.warning(f"Purging all files from bucket {self.name}")
         for filename in self.list():
             with get_session() as session:
```

### Comparing `tendril-filestore-0.2.2/src/tendril/filestore/base.py` & `tendril-filestore-0.2.3/src/tendril/filestore/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,24 +44,24 @@
 
     def upload(self, file, user, overwrite=False):
         raise NotImplementedError
 
     def move(self, filename, target_bucket, user, overwrite=False):
         raise NotImplementedError
 
-    def delete(self, filename, user):
-        raise NotImplementedError
-
     def list(self, page=None):
         raise NotImplementedError
 
     def list_info(self, include_owner=False, filenames=None):
         raise NotImplementedError
 
+    def find(self, spec):
+        raise NotImplementedError
+
+    def delete(self, filename, user):
+        raise NotImplementedError
+
     def purge(self, user):
         raise NotImplementedError
 
     def prune(self, user):
         raise NotImplementedError
-
-    def find(self, spec):
-        raise NotImplementedError
```

### Comparing `tendril-filestore-0.2.2/src/tendril/filestore/buckets.py` & `tendril-filestore-0.2.3/src/tendril/filestore/buckets.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/filestore/db/controller.py` & `tendril-filestore-0.2.3/src/tendril/filestore/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril/filestore/db/model.py` & `tendril-filestore-0.2.3/src/tendril/filestore/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril_filestore.egg-info/PKG-INFO` & `tendril-filestore-0.2.3/src/tendril_filestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.2.2
+Version: 0.2.3
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.2.2/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril-filestore-0.2.3/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/src/tendril_filestore.egg-info/requires.txt` & `tendril-filestore-0.2.3/src/tendril_filestore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/tests/coveralls.py` & `tendril-filestore-0.2.3/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.2/tox.ini` & `tendril-filestore-0.2.3/tox.ini`

 * *Files identical despite different names*

