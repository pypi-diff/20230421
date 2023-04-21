# Comparing `tmp/python-ote-0.1.0.tar.gz` & `tmp/python-ote-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ote-0.1.0.tar", last modified: Tue Dec 14 21:14:41 2021, max compression
+gzip compressed data, was "python-ote-0.1.1.tar", last modified: Fri Apr 21 14:47:03 2023, max compression
```

## Comparing `python-ote-0.1.0.tar` & `python-ote-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 21:14:41.736274 python-ote-0.1.0/
--rw-r--r--   0 dan       (1000) dan       (1000)    11357 2021-09-23 12:05:33.000000 python-ote-0.1.0/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     1774 2021-12-14 21:14:41.736274 python-ote-0.1.0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     1272 2021-09-24 15:46:27.000000 python-ote-0.1.0/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 21:14:41.735274 python-ote-0.1.0/ote/
--rw-r--r--   0 dan       (1000) dan       (1000)     1776 2021-12-14 21:00:03.000000 python-ote-0.1.0/ote/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      747 2021-09-24 14:41:55.000000 python-ote-0.1.0/ote/items.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3263 2021-09-23 13:45:44.000000 python-ote-0.1.0/ote/settings.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 21:14:41.735274 python-ote-0.1.0/ote/spiders/
--rw-r--r--   0 dan       (1000) dan       (1000)      161 2021-09-23 12:05:33.000000 python-ote-0.1.0/ote/spiders/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2688 2021-12-14 20:31:30.000000 python-ote-0.1.0/ote/spiders/ote_electricity.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 21:14:41.736274 python-ote-0.1.0/python_ote.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     1774 2021-12-14 21:14:41.000000 python-ote-0.1.0/python_ote.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      295 2021-12-14 21:14:41.000000 python-ote-0.1.0/python_ote.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-12-14 21:14:41.000000 python-ote-0.1.0/python_ote.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)      566 2021-12-14 21:14:41.000000 python-ote-0.1.0/python_ote.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        4 2021-12-14 21:14:41.000000 python-ote-0.1.0/python_ote.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2021-12-14 21:14:41.736274 python-ote-0.1.0/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)      829 2021-12-14 21:05:56.000000 python-ote-0.1.0/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-21 14:47:03.766740 python-ote-0.1.1/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11357 2021-09-23 12:05:33.000000 python-ote-0.1.1/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     3234 2023-04-21 14:47:03.766740 python-ote-0.1.1/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2769 2022-01-04 14:23:57.000000 python-ote-0.1.1/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-21 14:47:03.764740 python-ote-0.1.1/ote/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1776 2021-12-14 21:00:03.000000 python-ote-0.1.1/ote/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      747 2021-09-24 14:41:55.000000 python-ote-0.1.1/ote/items.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3263 2021-09-23 13:45:44.000000 python-ote-0.1.1/ote/settings.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-21 14:47:03.765740 python-ote-0.1.1/ote/spiders/
+-rw-r--r--   0 dan       (1000) dan       (1000)      161 2021-09-23 12:05:33.000000 python-ote-0.1.1/ote/spiders/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2688 2021-12-14 20:31:30.000000 python-ote-0.1.1/ote/spiders/ote_electricity.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-21 14:47:03.766740 python-ote-0.1.1/python_ote.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3234 2023-04-21 14:47:03.000000 python-ote-0.1.1/python_ote.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      295 2023-04-21 14:47:03.000000 python-ote-0.1.1/python_ote.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-04-21 14:47:03.000000 python-ote-0.1.1/python_ote.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2023-04-21 14:47:03.000000 python-ote-0.1.1/python_ote.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        4 2023-04-21 14:47:03.000000 python-ote-0.1.1/python_ote.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-04-21 14:47:03.766740 python-ote-0.1.1/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)      829 2023-04-21 14:45:53.000000 python-ote-0.1.1/setup.py
```

### Comparing `python-ote-0.1.0/LICENSE` & `python-ote-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ote-0.1.0/ote/__init__.py` & `python-ote-0.1.1/ote/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ote-0.1.0/ote/items.py` & `python-ote-0.1.1/ote/items.py`

 * *Files identical despite different names*

### Comparing `python-ote-0.1.0/ote/settings.py` & `python-ote-0.1.1/ote/settings.py`

 * *Files identical despite different names*

### Comparing `python-ote-0.1.0/ote/spiders/ote_electricity.py` & `python-ote-0.1.1/ote/spiders/ote_electricity.py`

 * *Files identical despite different names*

### Comparing `python-ote-0.1.0/setup.py` & `python-ote-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as fh:
     install_requires = [line for line in fh if line and line[0] not in "#-"]
 
 setuptools.setup(
     name="python-ote",
-    version="0.1.0",
+    version="0.1.1",
     author="Dan Keder",
     author_email="dan.keder@protonmail.com",
     description="Python library for scraping daily electricity prices from OTE (ote-cr.cz)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dankeder/python-ote",
     packages=setuptools.find_packages(),
```

