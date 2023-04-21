# Comparing `tmp/nlpie-0.1.tar.gz` & `tmp/nlpie-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nlpie-0.1.tar", last modified: Thu Apr 13 13:41:39 2023, max compression
+gzip compressed data, was "nlpie-0.2.tar", last modified: Fri Apr 21 21:32:59 2023, max compression
```

## Comparing `nlpie-0.1.tar` & `nlpie-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 omid       (501) staff       (20)        0 2023-04-13 13:41:39.000000 nlpie-0.1/
--rw-r--r--   0 omid       (501) staff       (20)      252 2023-04-13 13:41:39.000000 nlpie-0.1/PKG-INFO
-drwxr-xr-x   0 omid       (501) staff       (20)        0 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie/
--rw-r--r--   0 omid       (501) staff       (20)        0 2023-04-13 13:37:47.000000 nlpie-0.1/nlpie/__init__.py
-drwxr-xr-x   0 omid       (501) staff       (20)        0 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie.egg-info/
--rw-r--r--   0 omid       (501) staff       (20)      252 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie.egg-info/PKG-INFO
--rw-r--r--   0 omid       (501) staff       (20)      142 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie.egg-info/SOURCES.txt
--rw-r--r--   0 omid       (501) staff       (20)        1 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie.egg-info/dependency_links.txt
--rw-r--r--   0 omid       (501) staff       (20)        6 2023-04-13 13:41:39.000000 nlpie-0.1/nlpie.egg-info/top_level.txt
--rw-r--r--   0 omid       (501) staff       (20)       38 2023-04-13 13:41:39.000000 nlpie-0.1/setup.cfg
--rw-r--r--   0 omid       (501) staff       (20)      359 2023-04-13 13:40:36.000000 nlpie-0.1/setup.py
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-21 21:32:59.302145 nlpie-0.2/
+-rw-r--r--   0 omid       (502) staff       (20)       47 2023-04-21 21:32:59.300844 nlpie-0.2/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)     1587 2023-04-21 21:19:38.000000 nlpie-0.2/README.md
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-21 21:32:59.299507 nlpie-0.2/nlpie.egg-info/
+-rw-r--r--   0 omid       (502) staff       (20)       47 2023-04-21 21:32:59.000000 nlpie-0.2/nlpie.egg-info/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)      162 2023-04-21 21:32:59.000000 nlpie-0.2/nlpie.egg-info/SOURCES.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-21 21:32:59.000000 nlpie-0.2/nlpie.egg-info/dependency_links.txt
+-rw-r--r--   0 omid       (502) staff       (20)       50 2023-04-21 21:32:59.000000 nlpie-0.2/nlpie.egg-info/requires.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-21 21:32:59.000000 nlpie-0.2/nlpie.egg-info/top_level.txt
+-rw-r--r--   0 omid       (502) staff       (20)       38 2023-04-21 21:32:59.302426 nlpie-0.2/setup.cfg
+-rw-r--r--   0 omid       (502) staff       (20)      266 2023-04-21 21:31:14.000000 nlpie-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

