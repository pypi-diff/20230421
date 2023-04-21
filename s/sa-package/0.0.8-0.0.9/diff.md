# Comparing `tmp/sa_package-0.0.8.tar.gz` & `tmp/sa_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_package-0.0.8.tar", last modified: Sun Nov 20 07:51:35 2022, max compression
+gzip compressed data, was "sa_package-0.0.9.tar", last modified: Sun Nov 20 08:40:08 2022, max compression
```

## Comparing `sa_package-0.0.8.tar` & `sa_package-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-20 07:51:35.632455 sa_package-0.0.8/
--rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      261 2022-11-20 07:51:35.630382 sa_package-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       17 2022-11-14 08:11:02.000000 sa_package-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-20 07:51:35.568519 sa_package-0.0.8/sa_package/
-drwxrwxrwx   0        0        0        0 2022-11-20 07:51:35.593923 sa_package-0.0.8/sa_package/calendar/
--rw-rw-rw-   0        0        0        0 2022-11-20 07:19:46.000000 sa_package-0.0.8/sa_package/calendar/__init__.py
--rw-rw-rw-   0        0        0      842 2022-11-14 08:11:02.000000 sa_package-0.0.8/sa_package/calendar/calculate_date.py
-drwxrwxrwx   0        0        0        0 2022-11-20 07:51:35.625366 sa_package-0.0.8/sa_package/sa_package.egg-info/
--rw-rw-rw-   0        0        0      261 2022-11-20 07:51:35.000000 sa_package-0.0.8/sa_package/sa_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2022-11-20 07:51:35.000000 sa_package-0.0.8/sa_package/sa_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-20 07:51:35.000000 sa_package-0.0.8/sa_package/sa_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2022-11-20 07:51:35.000000 sa_package-0.0.8/sa_package/sa_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-20 07:51:35.000000 sa_package-0.0.8/sa_package/sa_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-20 07:51:35.634105 sa_package-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      741 2022-11-20 07:51:31.000000 sa_package-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.477459 sa_package-0.0.9/
+-rw-rw-rw-   0        0        0        0 2022-11-14 08:11:02.000000 sa_package-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      261 2022-11-20 08:40:08.475464 sa_package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2022-11-14 08:11:02.000000 sa_package-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.438564 sa_package-0.0.9/sa_package/
+-rw-rw-rw-   0        0        0        0 2022-11-20 08:34:44.000000 sa_package-0.0.9/sa_package/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.472474 sa_package-0.0.9/sa_package/calendar/
+-rw-rw-rw-   0        0        0        0 2022-11-20 07:19:46.000000 sa_package-0.0.9/sa_package/calendar/__init__.py
+-rw-rw-rw-   0        0        0      842 2022-11-14 08:11:02.000000 sa_package-0.0.9/sa_package/calendar/calculate_date.py
+drwxrwxrwx   0        0        0        0 2022-11-20 08:40:08.464496 sa_package-0.0.9/sa_package.egg-info/
+-rw-rw-rw-   0        0        0      261 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-11-20 08:40:08.000000 sa_package-0.0.9/sa_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-20 08:40:08.478457 sa_package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      669 2022-11-20 08:40:04.000000 sa_package-0.0.9/setup.py
```

### Comparing `sa_package-0.0.8/sa_package/calendar/calculate_date.py` & `sa_package-0.0.9/sa_package/calendar/calculate_date.py`

 * *Files identical despite different names*

