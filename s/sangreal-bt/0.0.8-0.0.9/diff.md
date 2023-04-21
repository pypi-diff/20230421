# Comparing `tmp/sangreal-bt-0.0.8.tar.gz` & `tmp/sangreal-bt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sangreal-bt-0.0.8.tar", last modified: Tue Feb 25 07:32:47 2020, max compression
+gzip compressed data, was "dist/sangreal-bt-0.0.9.tar", last modified: Tue Feb 25 08:36:32 2020, max compression
```

## Comparing `sangreal-bt-0.0.8.tar` & `sangreal-bt-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/
--rw-r--r--   0 liubola   (1000) liubola   (1001)      527 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1001)       36 2020-02-20 07:07:32.000000 sangreal-bt-0.0.8/README.md
-drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt/
--rw-r--r--   0 liubola   (1000) liubola   (1001)       50 2020-02-21 14:25:06.000000 sangreal-bt-0.0.8/sangreal_bt/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1001)      161 2020-02-22 00:58:37.000000 sangreal-bt-0.0.8/sangreal_bt/commons.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt/datafeed/
--rw-r--r--   0 liubola   (1000) liubola   (1001)       53 2020-02-21 02:00:38.000000 sangreal-bt-0.0.8/sangreal_bt/datafeed/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1001)      826 2020-02-21 05:39:18.000000 sangreal-bt-0.0.8/sangreal_bt/datafeed/datafeed.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt/strategy/
--rw-r--r--   0 liubola   (1000) liubola   (1001)        0 2020-02-21 14:24:50.000000 sangreal-bt-0.0.8/sangreal_bt/strategy/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1001)    11313 2020-02-25 00:22:05.000000 sangreal-bt-0.0.8/sangreal_bt/strategy/strategy.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/
--rw-r--r--   0 liubola   (1000) liubola   (1001)      527 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1001)      371 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/SOURCES.txt
--rw-r--r--   0 liubola   (1000) liubola   (1001)        1 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/dependency_links.txt
--rw-r--r--   0 liubola   (1000) liubola   (1001)       29 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/requires.txt
--rw-r--r--   0 liubola   (1000) liubola   (1001)       12 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/sangreal_bt.egg-info/top_level.txt
--rw-r--r--   0 liubola   (1000) liubola   (1001)       38 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/setup.cfg
--rw-r--r--   0 liubola   (1000) liubola   (1001)      890 2020-02-25 07:32:47.000000 sangreal-bt-0.0.8/setup.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      527 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       36 2020-02-20 07:07:32.000000 sangreal-bt-0.0.9/README.md
+drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt/
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       50 2020-02-21 14:25:06.000000 sangreal-bt-0.0.9/sangreal_bt/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      161 2020-02-22 00:58:37.000000 sangreal-bt-0.0.9/sangreal_bt/commons.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt/datafeed/
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       53 2020-02-21 02:00:38.000000 sangreal-bt-0.0.9/sangreal_bt/datafeed/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      826 2020-02-21 05:39:18.000000 sangreal-bt-0.0.9/sangreal_bt/datafeed/datafeed.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt/strategy/
+-rw-r--r--   0 liubola   (1000) liubola   (1001)        0 2020-02-21 14:24:50.000000 sangreal-bt-0.0.9/sangreal_bt/strategy/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1001)    11313 2020-02-25 00:22:05.000000 sangreal-bt-0.0.9/sangreal_bt/strategy/strategy.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1001)        0 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      527 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      371 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/SOURCES.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1001)        1 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/dependency_links.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       40 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/requires.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       12 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/sangreal_bt.egg-info/top_level.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1001)       38 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/setup.cfg
+-rw-r--r--   0 liubola   (1000) liubola   (1001)      912 2020-02-25 08:36:32.000000 sangreal-bt-0.0.9/setup.py
```

### Comparing `sangreal-bt-0.0.8/PKG-INFO` & `sangreal-bt-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sangreal-bt
-Version: 0.0.8
+Version: 0.0.9
 Summary: vector backtest
 Home-page: https://github.com/liubola/sangreal-bt
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `sangreal-bt-0.0.8/sangreal_bt/datafeed/datafeed.py` & `sangreal-bt-0.0.9/sangreal_bt/datafeed/datafeed.py`

 * *Files identical despite different names*

### Comparing `sangreal-bt-0.0.8/sangreal_bt/strategy/strategy.py` & `sangreal-bt-0.0.9/sangreal_bt/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `sangreal-bt-0.0.8/sangreal_bt.egg-info/PKG-INFO` & `sangreal-bt-0.0.9/sangreal_bt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sangreal-bt
-Version: 0.0.8
+Version: 0.0.9
 Summary: vector backtest
 Home-page: https://github.com/liubola/sangreal-bt
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `sangreal-bt-0.0.8/setup.py` & `sangreal-bt-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sangreal-bt',
-    version='0.0.8',
+    version='0.0.9',
     description=('vector backtest'),
     install_requires=[
         'attrs',
         'fastcache',
         'pandas',
         'numpy',
+        'matplotlib',
     ],
     # long_description=open('README.rst').read(),
     author='liubola',
     author_email='lby3523@gmail.com',
     # maintainer='<维护人员的名字>',
     # maintainer_email='<维护人员的邮件地址',
     license='GNU General Public License v3.0',
```

