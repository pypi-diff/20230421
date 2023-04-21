# Comparing `tmp/tggl-1.0.1.tar.gz` & `tmp/tggl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tggl-1.0.1.tar", last modified: Fri Apr 21 15:58:46 2023, max compression
+gzip compressed data, was "tggl-1.1.0.tar", last modified: Fri Apr 21 16:03:30 2023, max compression
```

## Comparing `tggl-1.0.1.tar` & `tggl-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-21 15:58:46.991504 tggl-1.0.1/
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-21 15:58:46.991379 tggl-1.0.1/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)       38 2023-04-21 15:58:46.991551 tggl-1.0.1/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)      223 2023-04-21 15:58:46.000000 tggl-1.0.1/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-21 15:58:46.991185 tggl-1.0.1/tggl.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-21 15:58:46.000000 tggl-1.0.1/tggl.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      120 2023-04-21 15:58:46.000000 tggl-1.0.1/tggl.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-21 15:58:46.000000 tggl-1.0.1/tggl.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-21 15:58:46.000000 tggl-1.0.1/tggl.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-21 16:03:30.014750 tggl-1.1.0/
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-21 16:03:30.014621 tggl-1.1.0/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)       38 2023-04-21 16:03:30.014791 tggl-1.1.0/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)      223 2023-04-21 16:03:29.000000 tggl-1.1.0/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-21 16:03:30.005286 tggl-1.1.0/tggl/
+-rw-r--r--   0 nick       (501) staff       (20)     1777 2023-04-21 15:45:14.000000 tggl-1.1.0/tggl/__init__.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-21 16:03:30.010541 tggl-1.1.0/tggl.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-21 16:03:29.000000 tggl-1.1.0/tggl.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      137 2023-04-21 16:03:29.000000 tggl-1.1.0/tggl.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-21 16:03:29.000000 tggl-1.1.0/tggl.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)        5 2023-04-21 16:03:29.000000 tggl-1.1.0/tggl.egg-info/top_level.txt
```

