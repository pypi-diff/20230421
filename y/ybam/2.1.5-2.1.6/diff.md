# Comparing `tmp/ybam-2.1.5.tar.gz` & `tmp/ybam-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ybam-2.1.5.tar", last modified: Fri Apr 21 08:18:32 2023, max compression
+gzip compressed data, was "ybam-2.1.6.tar", last modified: Fri Apr 21 08:32:30 2023, max compression
```

## Comparing `ybam-2.1.5.tar` & `ybam-2.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.921729 ybam-2.1.5/
--rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.5/LICENSE
--rw-rw-rw-   0        0        0      707 2023-04-21 08:18:32.920732 ybam-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-21 08:18:32.921729 ybam-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     4052 2023-04-21 08:18:16.000000 ybam-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.840947 ybam-2.1.5/ybam/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.5/ybam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.888820 ybam-2.1.5/ybam/bin/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.5/ybam/bin/__init__.py
--rw-rw-rw-   0        0        0      837 2023-04-21 08:14:06.000000 ybam-2.1.5/ybam/bin/bam.py
--rw-rw-rw-   0        0        0      356 2023-04-21 06:36:47.000000 ybam-2.1.5/ybam/bin/base_commond.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.892808 ybam-2.1.5/ybam/cmds/
--rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.5/ybam/cmds/__init__.py
--rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.5/ybam/cmds/clean.py
--rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.5/ybam/cmds/config.py
--rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.5/ybam/cmds/install.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.914749 ybam-2.1.5/ybam/conf/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.5/ybam/conf/__init__.py
--rw-rw-rw-   0        0        0     1170 2023-04-21 06:34:52.000000 ybam-2.1.5/ybam/conf/config.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.919735 ybam-2.1.5/ybam/lib/
--rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.5/ybam/lib/__init__.py
--rw-rw-rw-   0        0        0     1756 2023-04-21 06:36:27.000000 ybam-2.1.5/ybam/lib/cache.py
--rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.5/ybam/lib/common.py
--rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.5/ybam/lib/countdown_latch.py
--rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.5/ybam/lib/log.py
--rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.5/ybam/test.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:18:32.885827 ybam-2.1.5/ybam.egg-info/
--rw-rw-rw-   0        0        0      707 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 08:18:32.000000 ybam-2.1.5/ybam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.768932 ybam-2.1.6/
+-rw-rw-rw-   0        0        0        0 2023-04-21 06:43:13.000000 ybam-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:32:30.768932 ybam-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2023-04-21 06:44:28.000000 ybam-2.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:32:30.769929 ybam-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     4057 2023-04-21 08:32:04.000000 ybam-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.725051 ybam-2.1.6/ybam/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.6/ybam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.743999 ybam-2.1.6/ybam/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:29:19.000000 ybam-2.1.6/ybam/bin/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-21 08:31:30.000000 ybam-2.1.6/ybam/bin/bam.py
+-rw-rw-rw-   0        0        0      356 2023-04-21 06:36:47.000000 ybam-2.1.6/ybam/bin/base_commond.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.751977 ybam-2.1.6/ybam/cmds/
+-rw-rw-rw-   0        0        0     1054 2023-04-21 06:16:24.000000 ybam-2.1.6/ybam/cmds/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-04-21 06:48:30.000000 ybam-2.1.6/ybam/cmds/clean.py
+-rw-rw-rw-   0        0        0     1387 2023-04-21 05:52:57.000000 ybam-2.1.6/ybam/cmds/config.py
+-rw-rw-rw-   0        0        0     5760 2023-04-20 11:21:00.000000 ybam-2.1.6/ybam/cmds/install.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.754970 ybam-2.1.6/ybam/conf/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.6/ybam/conf/__init__.py
+-rw-rw-rw-   0        0        0     1170 2023-04-21 08:26:32.000000 ybam-2.1.6/ybam/conf/config.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.762951 ybam-2.1.6/ybam/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:28:58.000000 ybam-2.1.6/ybam/lib/__init__.py
+-rw-rw-rw-   0        0        0     1756 2023-04-21 06:36:27.000000 ybam-2.1.6/ybam/lib/cache.py
+-rw-rw-rw-   0        0        0     3813 2023-04-21 01:36:04.000000 ybam-2.1.6/ybam/lib/common.py
+-rw-rw-rw-   0        0        0      614 2023-04-20 07:17:05.000000 ybam-2.1.6/ybam/lib/countdown_latch.py
+-rw-rw-rw-   0        0        0      911 2023-04-21 03:39:04.000000 ybam-2.1.6/ybam/lib/log.py
+-rw-rw-rw-   0        0        0     1015 2023-04-21 06:36:09.000000 ybam-2.1.6/ybam/test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:30.739014 ybam-2.1.6/ybam.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 08:32:30.000000 ybam-2.1.6/ybam.egg-info/top_level.txt
```

### Comparing `ybam-2.1.5/PKG-INFO` & `ybam-2.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.5
+Version: 2.1.6
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ybam-2.1.5/setup.py` & `ybam-2.1.6/setup.py`

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
-VERSION = '2.1.5'
+VERSION = '2.1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'requests', 'urllib3' ,'PyYAML','filelock' , 'zipp'
 ]
 
 # What packages are optional?
@@ -122,15 +122,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     entry_points={
       'console_scripts': [
-            'ybam=ybam.bin.bam'
+            'ybam=ybam.bin.bam:main'
         ]
     },
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
 )
```

### Comparing `ybam-2.1.5/ybam/bin/bam.py` & `ybam-2.1.6/ybam/bin/bam.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 
 BATH_DIR = os.path.dirname(os.path.dirname(__file__))
 sys.path.append(BATH_DIR)
 from cmds import create_command
 from lib.log import *
 from conf.config import *
 
-if __name__ == '__main__':
+def main()->None: 
     args = sys.argv[1:]
     #args = ['install', 'install' , '-1logLevel', '20', 'sdfsf']
     # 使用argparse解析命令行参数  
     parser = argparse.ArgumentParser()  
     parser.add_argument('-logLevel', type=int, help='log Level')  
     args, argsElse= parser.parse_known_args(args)
-    config = Config('config.yaml')
+    config = Config('ybam\config.yaml')
     if args.logLevel:
         configLoging(args.logLevel)
     else:
         configLoging(config.get('LOG_LEVEL'))
     if not argsElse[0]:
         logging.error("please input command!")
     cmdName = argsElse[0]
 
     create_command(cmdName, args, argsElse)
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `ybam-2.1.5/ybam/cmds/__init__.py` & `ybam-2.1.6/ybam/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/cmds/clean.py` & `ybam-2.1.6/ybam/cmds/clean.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/cmds/config.py` & `ybam-2.1.6/ybam/cmds/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/cmds/install.py` & `ybam-2.1.6/ybam/cmds/install.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/conf/config.py` & `ybam-2.1.6/ybam/conf/config.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/lib/cache.py` & `ybam-2.1.6/ybam/lib/cache.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/lib/common.py` & `ybam-2.1.6/ybam/lib/common.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/lib/countdown_latch.py` & `ybam-2.1.6/ybam/lib/countdown_latch.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/lib/log.py` & `ybam-2.1.6/ybam/lib/log.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam/test.py` & `ybam-2.1.6/ybam/test.py`

 * *Files identical despite different names*

### Comparing `ybam-2.1.5/ybam.egg-info/PKG-INFO` & `ybam-2.1.6/ybam.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybam
-Version: 2.1.5
+Version: 2.1.6
 Summary: My short description for my project.
 Home-page: https://github.com/kennethreitz/setup.py/blob/master/setup.py
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ybam-2.1.5/ybam.egg-info/SOURCES.txt` & `ybam-2.1.6/ybam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

