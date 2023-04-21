# Comparing `tmp/ifunnygifmaker-0.1.5.tar.gz` & `tmp/ifunnygifmaker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.1.5.tar", last modified: Fri Apr 21 04:17:35 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.1.6.tar", last modified: Fri Apr 21 04:24:32 2023, max compression
```

## Comparing `ifunnygifmaker-0.1.5.tar` & `ifunnygifmaker-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.5/README.md
--rw-r--r--   0        0        0     6148 2023-04-21 04:15:30.948860 ifunnygifmaker-0.1.5/ifunnygifmaker/.DS_Store
--rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.5/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0     4492 2023-04-21 04:16:43.733682 ifunnygifmaker-0.1.5/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      416 2023-04-21 04:17:30.587395 ifunnygifmaker-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.6/README.md
+-rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.1.6/ifunnygifmaker/.DS_Store
+-rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.6/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.1.6/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0     4492 2023-04-21 04:24:24.239227 ifunnygifmaker-0.1.6/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      416 2023-04-21 04:24:28.604051 ifunnygifmaker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.6/PKG-INFO
```

### Comparing `ifunnygifmaker-0.1.5/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.1.6/ifunnygifmaker/mememaker.py`

 * *Files identical despite different names*

