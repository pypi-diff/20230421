# Comparing `tmp/lovehim-0.1.tar.gz` & `tmp/lovehim-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.1.tar", last modified: Fri Apr 21 06:30:32 2023, max compression
+gzip compressed data, was "lovehim-0.2.tar", last modified: Fri Apr 21 07:08:30 2023, max compression
```

## Comparing `lovehim-0.1.tar` & `lovehim-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 06:30:32.223258 lovehim-0.1/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 06:30:32.223141 lovehim-0.1/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 06:30:32.222979 lovehim-0.1/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      196 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 06:30:32.000000 lovehim-0.1/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 06:30:32.223294 lovehim-0.1/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 06:25:16.000000 lovehim-0.1/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:08:30.832627 lovehim-0.2/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:08:30.832502 lovehim-0.2/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:08:30.832331 lovehim-0.2/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      196 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:08:30.000000 lovehim-0.2/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 07:08:30.832669 lovehim-0.2/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 07:08:20.000000 lovehim-0.2/setup.py
```

