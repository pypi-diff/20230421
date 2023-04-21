# Comparing `tmp/pynamer-0.0.2.tar.gz` & `tmp/pynamer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.0.2.tar", last modified: Sun Apr 16 15:12:10 2023, max compression
+gzip compressed data, was "pynamer-0.2.0.tar", last modified: Fri Apr 21 20:37:15 2023, max compression
```

## Comparing `pynamer-0.0.2.tar` & `pynamer-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:12:10.755890 pynamer-0.0.2/
--rw-rw-rw-   0        0        0      206 2023-04-16 15:12:10.755890 pynamer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-04-15 17:52:26.000000 pynamer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 15:12:10.724641 pynamer-0.0.2/pynamer/
--rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.0.2/pynamer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:12:10.755890 pynamer-0.0.2/pynamer.egg-info/
--rw-rw-rw-   0        0        0      206 2023-04-16 15:12:10.000000 pynamer-0.0.2/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-16 15:12:10.000000 pynamer-0.0.2/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:12:10.000000 pynamer-0.0.2/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 15:12:10.000000 pynamer-0.0.2/pynamer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-16 15:12:10.000000 pynamer-0.0.2/pynamer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:12:10.755890 pynamer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      395 2023-04-16 15:11:59.000000 pynamer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:15.010111 pynamer-0.2.0/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.2.0/AUTHORS.md
+-rw-rw-rw-   0        0        0      466 2023-04-21 20:36:59.000000 pynamer-0.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-21 17:08:24.000000 pynamer-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7484 2023-04-21 20:37:15.010111 pynamer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6279 2023-04-21 18:16:39.000000 pynamer-0.2.0/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1662 2023-04-21 20:37:15.010111 pynamer-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 17:08:24.000000 pynamer-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.925446 pynamer-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer/
+-rw-rw-rw-   0        0        0     1172 2023-04-21 20:37:00.000000 pynamer-0.2.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     1459 2023-04-21 20:34:11.000000 pynamer-0.2.0/src/pynamer/pynamer.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer/resources/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:08:24.000000 pynamer-0.2.0/src/pynamer/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0     7484 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.994467 pynamer-0.2.0/tests/
+-rw-rw-rw-   0        0        0      781 2023-04-21 18:16:35.000000 pynamer-0.2.0/tests/test_pynamer.py
+-rw-rw-rw-   0        0        0     1165 2023-04-21 18:15:58.000000 pynamer-0.2.0/tests/test_pynamer_cli.py
```

