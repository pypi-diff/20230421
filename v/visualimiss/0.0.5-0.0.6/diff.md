# Comparing `tmp/visualimiss-0.0.5.tar.gz` & `tmp/visualimiss-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualimiss-0.0.5.tar", last modified: Fri Apr 14 16:41:13 2023, max compression
+gzip compressed data, was "visualimiss-0.0.6.tar", last modified: Fri Apr 21 11:58:34 2023, max compression
```

## Comparing `visualimiss-0.0.5.tar` & `visualimiss-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.574809 visualimiss-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      835 2023-04-14 16:41:13.572796 visualimiss-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-14 16:40:40.000000 visualimiss-0.0.5/README.md
--rw-rw-rw-   0        0        0      514 2023-04-14 16:39:01.000000 visualimiss-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 16:41:13.575816 visualimiss-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.558163 visualimiss-0.0.5/visualimiss/
--rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.5/visualimiss/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.5/visualimiss/utils.py
--rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.5/visualimiss/visualimiss.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.571282 visualimiss-0.0.5/visualimiss.egg-info/
--rw-rw-rw-   0        0        0      835 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.904872 visualimiss-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2646 2023-04-21 11:58:34.903861 visualimiss-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-04-15 15:24:07.000000 visualimiss-0.0.6/README.md
+-rw-rw-rw-   0        0        0      533 2023-04-15 17:38:10.000000 visualimiss-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:58:34.904872 visualimiss-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.875172 visualimiss-0.0.6/visualimiss/
+-rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.6/visualimiss/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.6/visualimiss/utils.py
+-rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.6/visualimiss/visualimiss.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.902884 visualimiss-0.0.6/visualimiss.egg-info/
+-rw-rw-rw-   0        0        0     2646 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/top_level.txt
```

### Comparing `visualimiss-0.0.5/LICENSE` & `visualimiss-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `visualimiss-0.0.5/visualimiss/visualimiss.py` & `visualimiss-0.0.6/visualimiss/visualimiss.py`

 * *Files identical despite different names*

