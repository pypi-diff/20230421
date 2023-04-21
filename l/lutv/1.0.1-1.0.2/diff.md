# Comparing `tmp/lutv-1.0.1.tar.gz` & `tmp/lutv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lutv-1.0.1.tar", last modified: Sun Nov  6 09:04:11 2022, max compression
+gzip compressed data, was "lutv-1.0.2.tar", last modified: Fri Apr 21 11:42:59 2023, max compression
```

## Comparing `lutv-1.0.1.tar` & `lutv-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-06 09:04:11.704855 lutv-1.0.1/
--rw-rw-rw-   0        0        0     1075 2022-11-06 02:47:18.000000 lutv-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1445 2022-11-06 09:04:11.704855 lutv-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      734 2022-11-06 09:00:39.000000 lutv-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-06 09:04:11.689121 lutv-1.0.1/lutv/
--rw-rw-rw-   0        0        0        0 2022-11-06 08:49:22.000000 lutv-1.0.1/lutv/__init__.py
--rw-rw-rw-   0        0        0    17148 2022-11-06 08:49:06.000000 lutv-1.0.1/lutv/random.py
-drwxrwxrwx   0        0        0        0 2022-11-06 09:04:11.704855 lutv-1.0.1/lutv.egg-info/
--rw-rw-rw-   0        0        0     1445 2022-11-06 09:04:11.000000 lutv-1.0.1/lutv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2022-11-06 09:04:11.000000 lutv-1.0.1/lutv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-06 09:04:11.000000 lutv-1.0.1/lutv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-11-06 09:04:11.000000 lutv-1.0.1/lutv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-06 09:04:11.704855 lutv-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1095 2022-11-06 07:49:36.000000 lutv-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.350758 lutv-1.0.2/
+-rw-rw-rw-   0        0        0     1075 2022-11-06 02:47:18.000000 lutv-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1445 2023-04-21 11:42:59.348622 lutv-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2022-11-06 09:00:39.000000 lutv-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.346642 lutv-1.0.2/lutv/
+-rw-rw-rw-   0        0        0        0 2022-11-06 08:49:22.000000 lutv-1.0.2/lutv/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-04-21 11:33:56.000000 lutv-1.0.2/lutv/gpt.py
+-rw-rw-rw-   0        0        0    17148 2022-11-06 08:49:06.000000 lutv-1.0.2/lutv/random.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.348622 lutv-1.0.2/lutv.egg-info/
+-rw-rw-rw-   0        0        0     1445 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:42:59.350758 lutv-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-04-21 11:38:21.000000 lutv-1.0.2/setup.py
```

### Comparing `lutv-1.0.1/LICENSE` & `lutv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lutv-1.0.1/PKG-INFO` & `lutv-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lutv
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is my personal project
 Author: Trần Xuân Lợi
 Author-email: tranxuanloi2007@gmail.com
 Keywords: LuTV,lutv,random,random_uer,lutvrandom,LuTV Random User,Tranxuanloi,TranXuanLoi,tranxuanloi,tranxuanloi2007
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lutv-1.0.1/README.md` & `lutv-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lutv-1.0.1/lutv/random.py` & `lutv-1.0.2/lutv/random.py`

 * *Files identical despite different names*

### Comparing `lutv-1.0.1/lutv.egg-info/PKG-INFO` & `lutv-1.0.2/lutv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lutv
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is my personal project
 Author: Trần Xuân Lợi
 Author-email: tranxuanloi2007@gmail.com
 Keywords: LuTV,lutv,random,random_uer,lutvrandom,LuTV Random User,Tranxuanloi,TranXuanLoi,tranxuanloi,tranxuanloi2007
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lutv-1.0.1/setup.py` & `lutv-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'This is my personal project'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
```

