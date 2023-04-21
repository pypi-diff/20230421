# Comparing `tmp/factorslib-1.0.tar.gz` & `tmp/factorslib-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorslib-1.0.tar", last modified: Fri Apr 21 01:23:28 2023, max compression
+gzip compressed data, was "factorslib-2.0.tar", last modified: Fri Apr 21 01:44:54 2023, max compression
```

## Comparing `factorslib-1.0.tar` & `factorslib-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:23:28.300903 factorslib-1.0/
--rw-rw-rw-   0        0        0     1038 2023-04-21 01:21:47.000000 factorslib-1.0/LICENCE.txt
--rw-rw-rw-   0        0        0      860 2023-04-21 01:23:28.300903 factorslib-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 08:49:22.000000 factorslib-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:23:28.288936 factorslib-1.0/factors/
--rw-rw-rw-   0        0        0        0 2023-04-21 00:17:05.000000 factorslib-1.0/factors/__init__.py
--rw-rw-rw-   0        0        0    39400 2023-03-01 06:35:33.000000 factorslib-1.0/factors/factors.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:23:28.299906 factorslib-1.0/factorslib.egg-info/
--rw-rw-rw-   0        0        0      860 2023-04-21 01:23:27.000000 factorslib-1.0/factorslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-21 01:23:28.000000 factorslib-1.0/factorslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:23:27.000000 factorslib-1.0/factorslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 01:23:28.000000 factorslib-1.0/factorslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:23:28.300903 factorslib-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-04-21 01:20:25.000000 factorslib-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.351450 factorslib-2.0/
+-rw-rw-rw-   0        0        0     1038 2023-04-21 01:21:47.000000 factorslib-2.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      325 2023-04-21 01:44:54.351450 factorslib-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:49:22.000000 factorslib-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.339168 factorslib-2.0/factors/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:29:23.000000 factorslib-2.0/factors/__init__.py
+-rw-rw-rw-   0        0        0    39400 2023-03-01 06:35:33.000000 factorslib-2.0/factors/factors.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:54.351450 factorslib-2.0/factorslib.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-04-21 01:44:53.000000 factorslib-2.0/factorslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-21 01:44:54.000000 factorslib-2.0/factorslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:44:53.000000 factorslib-2.0/factorslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 01:44:54.000000 factorslib-2.0/factorslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:44:54.352450 factorslib-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-04-21 01:44:31.000000 factorslib-2.0/setup.py
```

### Comparing `factorslib-1.0/LICENCE.txt` & `factorslib-2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `factorslib-1.0/factors/factors.py` & `factorslib-2.0/factors/factors.py`

 * *Files identical despite different names*

