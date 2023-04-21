# Comparing `tmp/python-filter-1.0.1.tar.gz` & `tmp/python-filter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-filter-1.0.1.tar", last modified: Fri Apr 21 00:56:49 2023, max compression
+gzip compressed data, was "python-filter-1.0.2.tar", last modified: Fri Apr 21 01:00:27 2023, max compression
```

## Comparing `python-filter-1.0.1.tar` & `python-filter-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.835456 python-filter-1.0.1/
--rw-rw-rw-   0        0        0      239 2023-04-21 00:56:49.832449 python-filter-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.800450 python-filter-1.0.1/pyfilter/
--rw-rw-rw-   0        0        0       93 2023-04-21 00:53:22.000000 python-filter-1.0.1/pyfilter/__init__.py
--rw-rw-rw-   0        0        0     2515 2023-04-21 00:46:51.000000 python-filter-1.0.1/pyfilter/dict_list.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.829451 python-filter-1.0.1/python_filter.egg-info/
--rw-rw-rw-   0        0        0      239 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 00:56:49.835456 python-filter-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-21 00:56:32.000000 python-filter-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.360016 python-filter-1.0.2/
+-rw-rw-rw-   0        0        0      239 2023-04-21 01:00:27.358006 python-filter-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.330011 python-filter-1.0.2/pyfilter/
+-rw-rw-rw-   0        0        0       67 2023-04-21 01:00:16.000000 python-filter-1.0.2/pyfilter/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-04-21 00:46:51.000000 python-filter-1.0.2/pyfilter/dict_list.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.356007 python-filter-1.0.2/python_filter.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:00:27.360016 python-filter-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-21 01:00:22.000000 python-filter-1.0.2/setup.py
```

### Comparing `python-filter-1.0.1/pyfilter/dict_list.py` & `python-filter-1.0.2/pyfilter/dict_list.py`

 * *Files identical despite different names*

