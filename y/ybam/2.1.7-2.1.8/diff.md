# Comparing `tmp/ybam-2.1.7.tar.gz` & `tmp/ybam-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ybam-2.1.7.tar", last modified: Fri Apr 21 08:40:51 2023, max compression
+gzip compressed data, was "ybam-2.1.8.tar", last modified: Fri Apr 21 08:42:52 2023, max compression
```

## Comparing `ybam-2.1.7.tar` & `ybam-2.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.730420 ybam-2.1.7/
--rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.7/LICENSE
--rw-rw-rw-   0        0        0      707 2023-04-21 08:40:51.730420 ybam-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-21 08:40:51.730420 ybam-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     4057 2023-04-21 08:40:42.000000 ybam-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.700503 ybam-2.1.7/ybam/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.7/ybam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.713466 ybam-2.1.7/ybam/bin/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.7/ybam/bin/__init__.py
--rw-rw-rw-   0        0        0      873 2023-04-21 08:39:44.000000 ybam-2.1.7/ybam/bin/bam.py
--rw-rw-rw-   0        0        0      361 2023-04-21 08:36:47.000000 ybam-2.1.7/ybam/bin/base_commond.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.717456 ybam-2.1.7/ybam/cmds/
--rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.7/ybam/cmds/__init__.py
--rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.7/ybam/cmds/clean.py
--rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.7/ybam/cmds/config.py
--rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.7/ybam/cmds/install.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.721447 ybam-2.1.7/ybam/conf/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.7/ybam/conf/__init__.py
--rw-rw-rw-   0        0        0     1170 2023-04-21 08:26:32.000000 ybam-2.1.7/ybam/conf/config.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.729423 ybam-2.1.7/ybam/lib/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.7/ybam/lib/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-04-21 08:36:52.000000 ybam-2.1.7/ybam/lib/cache.py
--rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.7/ybam/lib/common.py
--rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.7/ybam/lib/countdown_latch.py
--rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.7/ybam/lib/log.py
--rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.7/ybam/test.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:40:51.710538 ybam-2.1.7/ybam.egg-info/
--rw-rw-rw-   0        0        0      707 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 08:40:51.000000 ybam-2.1.7/ybam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.805047 ybam-2.1.8/
+-rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:42:52.804050 ybam-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:42:52.805047 ybam-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     4057 2023-04-21 08:42:40.000000 ybam-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.763159 ybam-2.1.8/ybam/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.8/ybam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.782110 ybam-2.1.8/ybam/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.8/ybam/bin/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-04-21 08:41:57.000000 ybam-2.1.8/ybam/bin/bam.py
+-rw-rw-rw-   0        0        0      361 2023-04-21 08:36:47.000000 ybam-2.1.8/ybam/bin/base_commond.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.788094 ybam-2.1.8/ybam/cmds/
+-rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.8/ybam/cmds/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.8/ybam/cmds/clean.py
+-rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.8/ybam/cmds/config.py
+-rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.8/ybam/cmds/install.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.790088 ybam-2.1.8/ybam/conf/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.8/ybam/conf/__init__.py
+-rw-rw-rw-   0        0        0     1170 2023-04-21 08:26:32.000000 ybam-2.1.8/ybam/conf/config.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.801057 ybam-2.1.8/ybam/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.8/ybam/lib/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-04-21 08:36:52.000000 ybam-2.1.8/ybam/lib/cache.py
+-rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.8/ybam/lib/common.py
+-rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.8/ybam/lib/countdown_latch.py
+-rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.8/ybam/lib/log.py
+-rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.8/ybam/test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:42:52.776127 ybam-2.1.8/ybam.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 08:42:52.000000 ybam-2.1.8/ybam.egg-info/top_level.txt
```

### Comparing `ybam-2.1.7/PKG-INFO` & `ybam-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.7
+Version: 2.1.8
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ybam-2.1.7/setup.py` & `ybam-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'ybam'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/kennethreitz/setup.py/blob/master/setup.py'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.1.7'
+VERSION = '2.1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'requests', 'urllib3' ,'PyYAML','filelock' , 'zipp'
 ]
 
 # What packages are optional?
```

### Comparing `ybam-2.1.7/ybam/bin/bam.py` & `ybam-2.1.8/ybam/bin/bam.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.append(BATH_DIR)
 from cmds import create_command
 from lib.log import *
 from conf.config import *
 
 def main()->None: 
     args = sys.argv[1:]
-    args = ['install', 'install' , '-1logLevel', '20', 'sdfsf']
+    # args = ['install', 'install' , '-1logLevel', '20', 'sdfsf']
     # 使用argparse解析命令行参数  
     parser = argparse.ArgumentParser()  
     parser.add_argument('-logLevel', type=int, help='log Level')  
     args, argsElse= parser.parse_known_args(args)
     config = Config('ybam\config.yaml')
     if args.logLevel:
         configLoging(args.logLevel)
```

### Comparing `ybam-2.1.7/ybam/cmds/__init__.py` & `ybam-2.1.8/ybam/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/cmds/clean.py` & `ybam-2.1.8/ybam/cmds/clean.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/cmds/config.py` & `ybam-2.1.8/ybam/cmds/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/cmds/install.py` & `ybam-2.1.8/ybam/cmds/install.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/conf/config.py` & `ybam-2.1.8/ybam/conf/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/lib/cache.py` & `ybam-2.1.8/ybam/lib/cache.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/lib/common.py` & `ybam-2.1.8/ybam/lib/common.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/lib/countdown_latch.py` & `ybam-2.1.8/ybam/lib/countdown_latch.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/lib/log.py` & `ybam-2.1.8/ybam/lib/log.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam/test.py` & `ybam-2.1.8/ybam/test.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.7/ybam.egg-info/PKG-INFO` & `ybam-2.1.8/ybam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.7
+Version: 2.1.8
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ybam-2.1.7/ybam.egg-info/SOURCES.txt` & `ybam-2.1.8/ybam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

