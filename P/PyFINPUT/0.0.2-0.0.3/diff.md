# Comparing `tmp/PyFINPUT-0.0.2.tar.gz` & `tmp/PyFINPUT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFINPUT-0.0.2.tar", last modified: Wed Apr 19 00:27:32 2023, max compression
+gzip compressed data, was "PyFINPUT-0.0.3.tar", last modified: Thu Apr 20 19:31:52 2023, max compression
```

## Comparing `PyFINPUT-0.0.2.tar` & `PyFINPUT-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 00:27:32.724636 PyFINPUT-0.0.2/
--rw-r--r--   0 ben       (1000) ben       (1000)    35149 2023-04-17 15:44:18.000000 PyFINPUT-0.0.2/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-19 00:27:32.724636 PyFINPUT-0.0.2/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      131 2023-04-17 15:50:43.000000 PyFINPUT-0.0.2/README.md
--rw-r--r--   0 ben       (1000) ben       (1000)      103 2023-04-19 00:27:32.724636 PyFINPUT-0.0.2/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)      664 2023-04-19 00:26:52.000000 PyFINPUT-0.0.2/setup.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 00:27:32.713802 PyFINPUT-0.0.2/src/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 00:27:32.724636 PyFINPUT-0.0.2/src/PyFINPUT/
--rw-r--r--   0 ben       (1000) ben       (1000)     4631 2023-04-18 23:11:45.000000 PyFINPUT-0.0.2/src/PyFINPUT/PyFINPUT.py
--rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-04-19 00:26:22.000000 PyFINPUT-0.0.2/src/PyFINPUT/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)      964 2023-04-18 19:15:02.000000 PyFINPUT-0.0.2/src/PyFINPUT/utils.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 00:27:32.724636 PyFINPUT-0.0.2/src/PyFINPUT.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-19 00:27:32.000000 PyFINPUT-0.0.2/src/PyFINPUT.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      252 2023-04-19 00:27:32.000000 PyFINPUT-0.0.2/src/PyFINPUT.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-19 00:27:32.000000 PyFINPUT-0.0.2/src/PyFINPUT.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        9 2023-04-19 00:27:32.000000 PyFINPUT-0.0.2/src/PyFINPUT.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/
+-rw-r--r--   0 ben       (1000) ben       (1000)    35149 2023-04-17 15:44:18.000000 PyFINPUT-0.0.3/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1493 2023-04-19 00:30:49.000000 PyFINPUT-0.0.3/README.md
+-rw-r--r--   0 ben       (1000) ben       (1000)      103 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)      664 2023-04-20 19:29:41.000000 PyFINPUT-0.0.3/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.975690 PyFINPUT-0.0.3/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.986523 PyFINPUT-0.0.3/src/PyFINPUT/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9062 2023-04-20 19:26:14.000000 PyFINPUT-0.0.3/src/PyFINPUT/PyFINPUT.py
+-rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-04-19 00:26:22.000000 PyFINPUT-0.0.3/src/PyFINPUT/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      964 2023-04-18 19:15:02.000000 PyFINPUT-0.0.3/src/PyFINPUT/utils.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      252 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        9 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/top_level.txt
```

### Comparing `PyFINPUT-0.0.2/LICENSE` & `PyFINPUT-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFINPUT-0.0.2/setup.py` & `PyFINPUT-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyFINPUT',
-    version='0.0.2',
+    version='0.0.3',
     license='GNU General Public License v3.0',
     author="Benedict Saunders",
     author_email='benedictsaunders@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/benedictsaunders/PyFINPUT',
     keywords='input, file, keywords',
```

### Comparing `PyFINPUT-0.0.2/src/PyFINPUT/utils.py` & `PyFINPUT-0.0.3/src/PyFINPUT/utils.py`

 * *Files identical despite different names*

