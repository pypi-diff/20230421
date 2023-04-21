# Comparing `tmp/Zeraora-0.2.1.tar.gz` & `tmp/Zeraora-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.1.tar", last modified: Thu Apr 20 09:01:04 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.2.tar", last modified: Fri Apr 21 08:01:18 2023, max compression
```

## Comparing `Zeraora-0.2.1.tar` & `Zeraora-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 09:01:04.000000 Zeraora-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-20 09:00:44.000000 Zeraora-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 09:01:04.000000 Zeraora-0.2.1/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:01:04.000000 Zeraora-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-20 09:00:44.000000 Zeraora-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:01:04.000000 Zeraora-0.2.1/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-04-20 09:00:44.000000 Zeraora-0.2.1/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 08:01:18.000000 Zeraora-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 08:01:04.000000 Zeraora-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:01:18.000000 Zeraora-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 08:01:04.000000 Zeraora-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/typing.py
```

### Comparing `Zeraora-0.2.1/PKG-INFO` & `Zeraora-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.1
+Version: 0.2.2
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.1/README.md` & `Zeraora-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.1/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.2/Zeraora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.1
+Version: 0.2.2
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.1/setup.py` & `Zeraora-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("./zeraora/__init__.py") as f:
     for line in f.readlines():
         if line.startswith("version"):
             delim = '"' if '"' in line else "'"
             version = line.split(delim)[1]
             break
@@ -40,9 +40,9 @@
         "Typing :: Typed",
     ],
     project_urls={
         "Source": "https://github.com/aixcyi/zeraora",
         "Tracker": "https://github.com/aixcyi/zeraora/issues",
     },
     python_requires='>=3.7',
-    packages=['zeraora'],
+    packages=find_packages(where=".", exclude=['test*']),
 )
```

### Comparing `Zeraora-0.2.1/zeraora/charsets.py` & `Zeraora-0.2.2/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.1/zeraora/decorators.py` & `Zeraora-0.2.2/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.1/zeraora/generators.py` & `Zeraora-0.2.2/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.1/zeraora/time.py` & `Zeraora-0.2.2/zeraora/time.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.1/zeraora/typing.py` & `Zeraora-0.2.2/zeraora/typing.py`

 * *Files identical despite different names*

