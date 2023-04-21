# Comparing `tmp/factorslib-2.0.tar.gz` & `tmp/factorslib-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorslib-2.0.tar", last modified: Fri Apr 21 01:44:54 2023, max compression
+gzip compressed data, was "factorslib-3.0.tar", last modified: Fri Apr 21 01:50:53 2023, max compression
```

## Comparing `factorslib-2.0.tar` & `factorslib-3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.351450 factorslib-2.0/
--rw-rw-rw-   0        0        0     1038 2023-04-21 01:21:47.000000 factorslib-2.0/LICENCE.txt
--rw-rw-rw-   0        0        0      325 2023-04-21 01:44:54.351450 factorslib-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 08:49:22.000000 factorslib-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.339168 factorslib-2.0/factors/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:29:23.000000 factorslib-2.0/factors/__init__.py
--rw-rw-rw-   0        0        0    39400 2023-03-01 06:35:33.000000 factorslib-2.0/factors/factors.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.351450 factorslib-2.0/factorslib.egg-info/
--rw-rw-rw-   0        0        0      325 2023-04-21 01:44:53.000000 factorslib-2.0/factorslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-21 01:44:54.000000 factorslib-2.0/factorslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:44:53.000000 factorslib-2.0/factorslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 01:44:54.000000 factorslib-2.0/factorslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:44:54.352450 factorslib-2.0/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-04-21 01:44:31.000000 factorslib-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:50:53.562037 factorslib-3.0/
+-rw-rw-rw-   0        0        0     1038 2023-04-21 01:21:47.000000 factorslib-3.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      325 2023-04-21 01:50:53.562037 factorslib-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:49:22.000000 factorslib-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:50:53.548073 factorslib-3.0/factorslib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:29:23.000000 factorslib-3.0/factorslib/__init__.py
+-rw-rw-rw-   0        0        0    39400 2023-03-01 06:35:33.000000 factorslib-3.0/factorslib/factors.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:50:53.561039 factorslib-3.0/factorslib.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-04-21 01:50:52.000000 factorslib-3.0/factorslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-21 01:50:53.000000 factorslib-3.0/factorslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:50:53.000000 factorslib-3.0/factorslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 01:50:53.000000 factorslib-3.0/factorslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:50:53.563033 factorslib-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-04-21 01:50:27.000000 factorslib-3.0/setup.py
```

### Comparing `factorslib-2.0/LICENCE.txt` & `factorslib-3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `factorslib-2.0/factors/factors.py` & `factorslib-3.0/factorslib/factors.py`

 * *Files identical despite different names*

### Comparing `factorslib-2.0/setup.py` & `factorslib-3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="factorslib",
-    version="2.0",
+    version="3.0",
     author="wytxty",
     author_email="yvettewkkaa@gmail.com",
     description="financial factors calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wytxty/factorslib",
     packages=setuptools.find_packages(),
```

