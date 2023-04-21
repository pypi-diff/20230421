# Comparing `tmp/ybam-2.1.2.tar.gz` & `tmp/ybam-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ybam-2.1.2.tar", last modified: Fri Apr 21 07:32:53 2023, max compression
+gzip compressed data, was "ybam-2.1.3.tar", last modified: Fri Apr 21 08:11:09 2023, max compression
```

## Comparing `ybam-2.1.2.tar` & `ybam-2.1.3.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.212850 ybam-2.1.2/
--rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      707 2023-04-21 07:32:53.202864 ybam-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-21 07:32:53.212850 ybam-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3952 2023-04-21 07:32:34.000000 ybam-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.171950 ybam-2.1.2/ybam/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.2/ybam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.184919 ybam-2.1.2/ybam/bin/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.2/ybam/bin/__init__.py
--rw-rw-rw-   0        0        0      838 2023-04-21 06:36:37.000000 ybam-2.1.2/ybam/bin/bam.py
--rw-rw-rw-   0        0        0      356 2023-04-21 06:36:47.000000 ybam-2.1.2/ybam/bin/base_commond.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.188901 ybam-2.1.2/ybam/cmds/
--rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.2/ybam/cmds/__init__.py
--rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.2/ybam/cmds/clean.py
--rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.2/ybam/cmds/config.py
--rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.2/ybam/cmds/install.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.192902 ybam-2.1.2/ybam/conf/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.2/ybam/conf/__init__.py
--rw-rw-rw-   0        0        0     1170 2023-04-21 06:34:52.000000 ybam-2.1.2/ybam/conf/config.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.201867 ybam-2.1.2/ybam/lib/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.2/ybam/lib/__init__.py
--rw-rw-rw-   0        0        0     1756 2023-04-21 06:36:27.000000 ybam-2.1.2/ybam/lib/cache.py
--rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.2/ybam/lib/common.py
--rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.2/ybam/lib/countdown_latch.py
--rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.2/ybam/lib/log.py
--rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.2/ybam/test.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:53.180923 ybam-2.1.2/ybam.egg-info/
--rw-rw-rw-   0        0        0      707 2023-04-21 07:32:53.000000 ybam-2.1.2/ybam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-04-21 07:32:53.000000 ybam-2.1.2/ybam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 07:32:53.000000 ybam-2.1.2/ybam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 07:32:53.000000 ybam-2.1.2/ybam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 07:32:53.000000 ybam-2.1.2/ybam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.687833 ybam-2.1.3/
+-rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:11:09.686837 ybam-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:11:09.687833 ybam-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4058 2023-04-21 08:10:07.000000 ybam-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.656916 ybam-2.1.3/ybam/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.3/ybam/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-04-21 08:11:02.000000 ybam-2.1.3/ybam/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.670879 ybam-2.1.3/ybam/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.3/ybam/bin/__init__.py
+-rw-rw-rw-   0        0        0      838 2023-04-21 06:36:37.000000 ybam-2.1.3/ybam/bin/bam.py
+-rw-rw-rw-   0        0        0      356 2023-04-21 06:36:47.000000 ybam-2.1.3/ybam/bin/base_commond.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.674868 ybam-2.1.3/ybam/cmds/
+-rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.3/ybam/cmds/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.3/ybam/cmds/clean.py
+-rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.3/ybam/cmds/config.py
+-rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.3/ybam/cmds/install.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.676863 ybam-2.1.3/ybam/conf/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.3/ybam/conf/__init__.py
+-rw-rw-rw-   0        0        0     1170 2023-04-21 06:34:52.000000 ybam-2.1.3/ybam/conf/config.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.685839 ybam-2.1.3/ybam/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.3/ybam/lib/__init__.py
+-rw-rw-rw-   0        0        0     1756 2023-04-21 06:36:27.000000 ybam-2.1.3/ybam/lib/cache.py
+-rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.3/ybam/lib/common.py
+-rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.3/ybam/lib/countdown_latch.py
+-rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.3/ybam/lib/log.py
+-rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.3/ybam/test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:09.667888 ybam-2.1.3/ybam.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 08:11:09.000000 ybam-2.1.3/ybam.egg-info/top_level.txt
```

### Comparing `ybam-2.1.2/PKG-INFO` & `ybam-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.2
+Version: 2.1.3
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ybam-2.1.2/setup.py` & `ybam-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'ybam'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/kennethreitz/setup.py/blob/master/setup.py'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.1.2'
+VERSION = '2.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'requests', 'urllib3' ,'PyYAML','filelock' , 'zipp'
 ]
 
 # What packages are optional?
@@ -120,12 +120,17 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
+    entry_points={
+      'console_scripts': [
+            'ybam=ybam.__main__:main'
+        ]
+    },
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
 )
```

### Comparing `ybam-2.1.2/ybam/bin/bam.py` & `ybam-2.1.3/ybam/bin/bam.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/cmds/__init__.py` & `ybam-2.1.3/ybam/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/cmds/clean.py` & `ybam-2.1.3/ybam/cmds/clean.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/cmds/config.py` & `ybam-2.1.3/ybam/cmds/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/cmds/install.py` & `ybam-2.1.3/ybam/cmds/install.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/conf/config.py` & `ybam-2.1.3/ybam/conf/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/lib/cache.py` & `ybam-2.1.3/ybam/lib/cache.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/lib/common.py` & `ybam-2.1.3/ybam/lib/common.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/lib/countdown_latch.py` & `ybam-2.1.3/ybam/lib/countdown_latch.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/lib/log.py` & `ybam-2.1.3/ybam/lib/log.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam/test.py` & `ybam-2.1.3/ybam/test.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.2/ybam.egg-info/PKG-INFO` & `ybam-2.1.3/ybam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.2
+Version: 2.1.3
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

