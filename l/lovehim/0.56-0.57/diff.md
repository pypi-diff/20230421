# Comparing `tmp/lovehim-0.56.tar.gz` & `tmp/lovehim-0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.56.tar", last modified: Fri Apr 21 08:12:34 2023, max compression
+gzip compressed data, was "lovehim-0.57.tar", last modified: Fri Apr 21 08:14:38 2023, max compression
```

## Comparing `lovehim-0.56.tar` & `lovehim-0.57.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.829381 lovehim-0.56/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:12:34.829217 lovehim-0.56/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.828220 lovehim-0.56/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.56/lovehim/__init__.py
--rw-r--r--   0 gera       (501) staff       (20)      741 2023-04-21 08:12:24.000000 lovehim-0.56/lovehim/__main__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:11:21.000000 lovehim-0.56/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.829021 lovehim-0.56/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:12:34.829423 lovehim-0.56/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:12:28.000000 lovehim-0.56/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:14:38.555364 lovehim-0.57/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:14:38.555225 lovehim-0.57/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:14:38.554236 lovehim-0.57/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       60 2023-04-21 08:14:31.000000 lovehim-0.57/lovehim/__init__.py
+-rw-r--r--   0 gera       (501) staff       (20)      741 2023-04-21 08:12:24.000000 lovehim-0.57/lovehim/__main__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:11:21.000000 lovehim-0.57/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:14:38.555029 lovehim-0.57/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:14:38.000000 lovehim-0.57/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:14:38.555425 lovehim-0.57/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:14:29.000000 lovehim-0.57/setup.py
```

### Comparing `lovehim-0.56/lovehim/__main__.py` & `lovehim-0.57/lovehim/__main__.py`

 * *Files identical despite different names*

### Comparing `lovehim-0.56/lovehim/get_verse.py` & `lovehim-0.57/lovehim/get_verse.py`

 * *Files identical despite different names*

