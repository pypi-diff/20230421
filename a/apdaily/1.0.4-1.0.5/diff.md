# Comparing `tmp/apdaily-1.0.4.tar.gz` & `tmp/apdaily-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apdaily-1.0.4.tar", last modified: Fri Apr 21 00:28:21 2023, max compression
+gzip compressed data, was "apdaily-1.0.5.tar", last modified: Fri Apr 21 00:42:27 2023, max compression
```

## Comparing `apdaily-1.0.4.tar` & `apdaily-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:21.682764 apdaily-1.0.4/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:28:21.684762 apdaily-1.0.4/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      505 2023-04-20 17:56:45.000000 apdaily-1.0.4/README.md
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      103 2023-04-20 17:56:45.000000 apdaily-1.0.4/pyproject.toml
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      712 2023-04-21 00:28:21.701850 apdaily-1.0.4/setup.cfg
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:20.375411 apdaily-1.0.4/src/
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:20.813315 apdaily-1.0.4/src/apdaily/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.4/src/apdaily/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      143 2023-04-20 17:56:45.000000 apdaily-1.0.4/src/apdaily/main.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:21.145974 apdaily-1.0.4/src/apdaily.egg-info/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:28:19.000000 apdaily-1.0.4/src/apdaily.egg-info/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      428 2023-04-21 00:28:20.000000 apdaily-1.0.4/src/apdaily.egg-info/SOURCES.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        1 2023-04-21 00:28:19.000000 apdaily-1.0.4/src/apdaily.egg-info/dependency_links.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       12 2023-04-21 00:28:19.000000 apdaily-1.0.4/src/apdaily.egg-info/requires.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       40 2023-04-21 00:28:19.000000 apdaily-1.0.4/src/apdaily.egg-info/top_level.txt
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:21.362199 apdaily-1.0.4/src/apdaily_methods/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.4/src/apdaily_methods/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     3487 2023-04-21 00:14:47.000000 apdaily-1.0.4/src/apdaily_methods/apdaily_m1.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      335 2023-04-20 17:56:45.000000 apdaily-1.0.4/src/apdaily_methods/mouse_util.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:28:21.571890 apdaily-1.0.4/src/apdaily_startup/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.4/src/apdaily_startup/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     4567 2023-04-21 00:27:23.000000 apdaily-1.0.4/src/apdaily_startup/apdaily_startup_main.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.363017 apdaily-1.0.5/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     1162 2023-04-21 00:42:27.363017 apdaily-1.0.5/PKG-INFO
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      839 2023-04-21 00:39:50.000000 apdaily-1.0.5/README.md
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      103 2023-04-20 17:56:45.000000 apdaily-1.0.5/pyproject.toml
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      712 2023-04-21 00:42:27.372343 apdaily-1.0.5/setup.cfg
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.409519 apdaily-1.0.5/src/
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.620464 apdaily-1.0.5/src/apdaily/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      143 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily/main.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.943417 apdaily-1.0.5/src/apdaily.egg-info/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     1162 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/PKG-INFO
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      428 2023-04-21 00:42:26.000000 apdaily-1.0.5/src/apdaily.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        1 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)       12 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/requires.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)       40 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/top_level.txt
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.186131 apdaily-1.0.5/src/apdaily_methods/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily_methods/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     3487 2023-04-21 00:42:10.000000 apdaily-1.0.5/src/apdaily_methods/apdaily_m1.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      334 2023-04-21 00:42:02.000000 apdaily-1.0.5/src/apdaily_methods/mouse_util.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.310748 apdaily-1.0.5/src/apdaily_startup/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily_startup/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     4567 2023-04-21 00:27:23.000000 apdaily-1.0.5/src/apdaily_startup/apdaily_startup_main.py
```

### Comparing `apdaily-1.0.4/setup.cfg` & `apdaily-1.0.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apdaily
-version = 1.0.4
+version = 1.0.5
 author = Saranga Rajagopalan
 author_email = sarnga.raj@gmail.com
 description = A package that allows you to watch AP Classroom Daily videos automatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SarangaR/APDaily-Dev
 project_urls =
```

### Comparing `apdaily-1.0.4/src/apdaily_methods/apdaily_m1.py` & `apdaily-1.0.5/src/apdaily_methods/apdaily_m1.py`

 * *Files identical despite different names*

### Comparing `apdaily-1.0.4/src/apdaily_startup/apdaily_startup_main.py` & `apdaily-1.0.5/src/apdaily_startup/apdaily_startup_main.py`

 * *Files identical despite different names*

