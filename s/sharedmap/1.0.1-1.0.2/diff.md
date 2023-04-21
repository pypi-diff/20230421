# Comparing `tmp/sharedmap-1.0.1.tar.gz` & `tmp/sharedmap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedmap-1.0.1.tar", last modified: Fri Apr 21 07:08:14 2023, max compression
+gzip compressed data, was "sharedmap-1.0.2.tar", last modified: Fri Apr 21 08:03:56 2023, max compression
```

## Comparing `sharedmap-1.0.1.tar` & `sharedmap-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 07:08:14.281279 sharedmap-1.0.1/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.1/LICENSE
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 07:08:14.281279 sharedmap-1.0.1/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3853 2023-04-21 07:04:13.000000 sharedmap-1.0.1/README.md
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 07:08:14.277279 sharedmap-1.0.1/native/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.1/native/avltree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1551 2023-04-21 03:58:52.000000 sharedmap-1.0.1/native/pynative.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7178 2023-04-21 04:09:15.000000 sharedmap-1.0.1/native/pyrbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4340 2023-04-21 03:37:21.000000 sharedmap-1.0.1/native/pyshareabledict.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.1/native/rbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.1/native/stringbox.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.1/native/tree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-04-21 07:08:14.281279 sharedmap-1.0.1/setup.cfg
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1518 2023-04-21 07:07:56.000000 sharedmap-1.0.1/setup.py
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 07:08:14.281279 sharedmap-1.0.1/sharedmap.egg-info/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 07:08:14.000000 sharedmap-1.0.1/sharedmap.egg-info/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      299 2023-04-21 07:08:14.000000 sharedmap-1.0.1/sharedmap.egg-info/SOURCES.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-04-21 07:08:14.000000 sharedmap-1.0.1/sharedmap.egg-info/dependency_links.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-04-21 07:08:14.000000 sharedmap-1.0.1/sharedmap.egg-info/top_level.txt
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.2/LICENSE
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 08:03:56.920754 sharedmap-1.0.2/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3853 2023-04-21 07:04:13.000000 sharedmap-1.0.2/README.md
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/native/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.2/native/avltree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.2/native/avltree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1551 2023-04-21 03:58:52.000000 sharedmap-1.0.2/native/pynative.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      288 2023-04-20 09:22:52.000000 sharedmap-1.0.2/native/pynative.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7178 2023-04-21 04:09:15.000000 sharedmap-1.0.2/native/pyrbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4340 2023-04-21 03:37:21.000000 sharedmap-1.0.2/native/pyshareabledict.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3441 2023-04-20 13:10:17.000000 sharedmap-1.0.2/native/pytree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.2/native/rbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.2/native/rbtree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.2/native/stringbox.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.2/native/stringbox.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.2/native/tree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.2/native/tree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-04-21 08:03:56.920754 sharedmap-1.0.2/setup.cfg
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1888 2023-04-21 08:03:51.000000 sharedmap-1.0.2/setup.py
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-21 08:03:56.920754 sharedmap-1.0.2/sharedmap.egg-info/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4309 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      399 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-04-21 08:03:56.000000 sharedmap-1.0.2/sharedmap.egg-info/top_level.txt
```

### Comparing `sharedmap-1.0.1/LICENSE` & `sharedmap-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/PKG-INFO` & `sharedmap-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.1
+Version: 1.0.2
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

### Comparing `sharedmap-1.0.1/README.md` & `sharedmap-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/avltree.cpp` & `sharedmap-1.0.2/native/avltree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/pynative.cpp` & `sharedmap-1.0.2/native/pynative.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/pyrbtree.cpp` & `sharedmap-1.0.2/native/pyrbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/pyshareabledict.cpp` & `sharedmap-1.0.2/native/pyshareabledict.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/rbtree.cpp` & `sharedmap-1.0.2/native/rbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/stringbox.cpp` & `sharedmap-1.0.2/native/stringbox.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/native/tree.cpp` & `sharedmap-1.0.2/native/tree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.1/setup.py` & `sharedmap-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 	"native/avltree.cpp",
 	"native/rbtree.cpp",
 	"native/pyshareabledict.cpp",
 	"native/pyrbtree.cpp",
 	"native/pynative.cpp",
 ]
 
+include_files = [
+	"native/avltree.h",
+	"native/pynative.h",
+	"native/pytree.h",
+	"native/rbtree.h",
+	"native/stringbox.h",
+	"native/tree.h",
+]
+
 if version >= (2,0) and version < (3,0):
 	module1 = Extension('sharedmap',sources = other_sources,include_dirs=['./native'],libraries = ['rt'],extra_compile_args=["-DNDEBUG"],extra_link_args=["-s"])
 elif version >= (3,0) and version < (4,0):
 	module1 = Extension('sharedmap',sources = other_sources,include_dirs=['./native'],libraries = ['rt'],extra_compile_args=["-DNDEBUG"],extra_link_args=["-s"])
 
 
 
@@ -29,21 +38,22 @@
 	with open("README.md", "r") as fh:
 		long_description = fh.read()
 except Exception as e:
 	long_description = "";
 
 
 setup (name = projname,
-	version = '1.0.1',
+	version = '1.0.2',
 	description = projname,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "lyramilk",
 	packages=[],
 	ext_modules = [module1],
+	data_files=include_files,
 	install_requires = [],
 	author_email='lyramilk@qq.com',
 	license='Apache License 2.0',
 	url='', 
 	classifiers=[
 		"Intended Audience :: Developers",
 		"Operating System :: OS Independent",
@@ -52,7 +62,18 @@
 		'Programming Language :: Python :: 3',
 		'Topic :: Utilities'
 	],
 	keywords = 'sharedmap,sharememory,rbtree,avltree',
 )
 
 
+'''
+
+	"native/stringbox.cpp",
+	"native/tree.cpp",
+	"native/avltree.cpp",
+	"native/rbtree.cpp",
+	"native/pyshareabledict.cpp",
+	"native/pyrbtree.cpp",
+	"native/pynative.cpp",
+
+'''
```

### Comparing `sharedmap-1.0.1/sharedmap.egg-info/PKG-INFO` & `sharedmap-1.0.2/sharedmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.1
+Version: 1.0.2
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

