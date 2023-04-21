# Comparing `tmp/pylogix-plc-3.9.19.tar.gz` & `tmp/pylogix-plc-3.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogix-plc-3.9.19.tar", last modified: Thu Apr 20 18:43:23 2023, max compression
+gzip compressed data, was "pylogix-plc-3.9.20.tar", last modified: Fri Apr 21 19:26:37 2023, max compression
```

## Comparing `pylogix-plc-3.9.19.tar` & `pylogix-plc-3.9.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.604359 pylogix-plc-3.9.19/
--rw-rw-rw-   0        0        0      351 2023-04-20 18:43:23.602362 pylogix-plc-3.9.19/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 18:39:38.000000 pylogix-plc-3.9.19/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.535357 pylogix-plc-3.9.19/empty/
--rw-rw-rw-   0        0        0       45 2023-03-07 06:02:06.000000 pylogix-plc-3.9.19/empty/__init__.py
--rw-rw-rw-   0        0        0     2007 2023-04-20 18:36:09.000000 pylogix-plc-3.9.19/empty/blank.py
--rw-rw-rw-   0        0        0       93 2023-04-20 18:34:57.000000 pylogix-plc-3.9.19/empty/empty.py
--rw-rw-rw-   0        0        0        3 2023-04-20 18:41:56.000000 pylogix-plc-3.9.19/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.594364 pylogix-plc-3.9.19/pylogix_plc.egg-info/
--rw-rw-rw-   0        0        0      351 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 18:43:23.604359 pylogix-plc-3.9.19/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-04-20 18:43:17.000000 pylogix-plc-3.9.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:26:37.882885 pylogix-plc-3.9.20/
+-rw-rw-rw-   0        0        0    32093 2023-04-21 19:26:37.881830 pylogix-plc-3.9.20/PKG-INFO
+-rw-rw-rw-   0        0        0    31285 2023-04-21 19:25:22.000000 pylogix-plc-3.9.20/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:26:37.833838 pylogix-plc-3.9.20/empty/
+-rw-rw-rw-   0        0        0       33 2023-04-21 19:19:03.000000 pylogix-plc-3.9.20/empty/__init__.py
+-rw-rw-rw-   0        0        0     2007 2023-04-20 18:36:09.000000 pylogix-plc-3.9.20/empty/blank.py
+-rw-rw-rw-   0        0        0       93 2023-04-20 18:34:57.000000 pylogix-plc-3.9.20/empty/empty.py
+-rw-rw-rw-   0        0        0        3 2023-04-20 18:41:56.000000 pylogix-plc-3.9.20/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 19:26:37.877905 pylogix-plc-3.9.20/pylogix_plc.egg-info/
+-rw-rw-rw-   0        0        0    32093 2023-04-21 19:26:37.000000 pylogix-plc-3.9.20/pylogix_plc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-21 19:26:37.000000 pylogix-plc-3.9.20/pylogix_plc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:26:37.000000 pylogix-plc-3.9.20/pylogix_plc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 19:26:37.000000 pylogix-plc-3.9.20/pylogix_plc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:26:37.882885 pylogix-plc-3.9.20/setup.cfg
+-rw-rw-rw-   0        0        0      992 2023-04-21 19:26:25.000000 pylogix-plc-3.9.20/setup.py
```

### Comparing `pylogix-plc-3.9.19/empty/blank.py` & `pylogix-plc-3.9.20/empty/blank.py`

 * *Files identical despite different names*

