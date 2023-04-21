# Comparing `tmp/OMGITSLACKO-0.1.tar.gz` & `tmp/OMGITSLACKO-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMGITSLACKO-0.1.tar", last modified: Fri Apr 21 11:54:32 2023, max compression
+gzip compressed data, was "OMGITSLACKO-0.1.1.tar", last modified: Fri Apr 21 15:11:25 2023, max compression
```

## Comparing `OMGITSLACKO-0.1.tar` & `OMGITSLACKO-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:54:32.117760 OMGITSLACKO-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-21 11:54:32.108719 OMGITSLACKO-0.1/OMGITSLACKO/
--rw-rw-rw-   0        0        0       34 2023-04-21 10:51:23.000000 OMGITSLACKO-0.1/OMGITSLACKO/__init__.py
--rw-rw-rw-   0        0        0      924 2023-04-21 10:50:51.000000 OMGITSLACKO-0.1/OMGITSLACKO/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:54:32.115738 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/
--rw-rw-rw-   0        0        0      233 2023-04-21 11:54:31.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-21 11:54:32.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:54:31.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-21 11:54:31.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 11:54:31.000000 OMGITSLACKO-0.1/OMGITSLACKO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      233 2023-04-21 11:54:32.116740 OMGITSLACKO-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 11:54:32.117760 OMGITSLACKO-0.1/setup.cfg
--rw-rw-rw-   0        0        0      397 2023-04-21 11:52:01.000000 OMGITSLACKO-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:11:25.168764 OMGITSLACKO-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-04-21 15:11:25.160896 OMGITSLACKO-0.1.1/OMGITSLACKO/
+-rw-rw-rw-   0        0        0       34 2023-04-21 10:51:23.000000 OMGITSLACKO-0.1.1/OMGITSLACKO/__init__.py
+-rw-rw-rw-   0        0        0     5090 2023-04-21 15:10:10.000000 OMGITSLACKO-0.1.1/OMGITSLACKO/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:11:25.166759 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-04-21 15:11:24.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-21 15:11:25.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:11:24.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-21 15:11:24.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 15:11:24.000000 OMGITSLACKO-0.1.1/OMGITSLACKO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-21 15:11:25.167762 OMGITSLACKO-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:11:25.168764 OMGITSLACKO-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-04-21 15:10:49.000000 OMGITSLACKO-0.1.1/setup.py
```

