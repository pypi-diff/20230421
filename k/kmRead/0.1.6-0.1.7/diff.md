# Comparing `tmp/kmRead-0.1.6.tar.gz` & `tmp/kmRead-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kmRead-0.1.6.tar", last modified: Fri Apr 14 12:18:54 2023, max compression
+gzip compressed data, was "dist\kmRead-0.1.7.tar", last modified: Fri Apr 21 01:55:35 2023, max compression
```

## Comparing `kmRead-0.1.6.tar` & `kmRead-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:18:54.000000 kmRead-0.1.6/
--rw-rw-rw-   0        0        0      337 2023-04-14 12:18:54.000000 kmRead-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead/
--rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.6/kmRead/__init__.py
--rw-rw-rw-   0        0        0     9590 2023-04-14 12:17:56.000000 kmRead-0.1.6/kmRead/kmRead.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/
--rw-rw-rw-   0        0        0      337 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 12:18:54.000000 kmRead-0.1.6/kmRead.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 12:18:54.000000 kmRead-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-04-14 12:18:44.000000 kmRead-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/
+-rw-rw-rw-   0        0        0      337 2023-04-21 01:55:35.000000 kmRead-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead/
+-rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.7/kmRead/__init__.py
+-rw-rw-rw-   0        0        0     9592 2023-04-21 01:54:47.000000 kmRead-0.1.7/kmRead/kmRead.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead.egg-info/
+-rw-rw-rw-   0        0        0      337 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:55:35.000000 kmRead-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-04-21 01:55:07.000000 kmRead-0.1.7/setup.py
```

### Comparing `kmRead-0.1.6/kmRead/kmRead.py` & `kmRead-0.1.7/kmRead/kmRead.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         
 
    
 def mainInit():
     print('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
     os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
     os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.zxm\shell\zxm2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
-    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.xmind\shell\zxm2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
+    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.xmind\shell\xmind2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
 
     # pv=""
     # p=""
     # if os.environ.get('HOME') is not None:
     #     pv=os.path.join(os.environ.get('HOME'),".km")
     # elif os.environ.get('HOMEPATH') is not None:
     #     pv=os.path.join(os.environ.get('HOMEPATH'),".km")
```

### Comparing `kmRead-0.1.6/setup.py` & `kmRead-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
 name = "kmRead",
-version = "0.1.6",
+version = "0.1.7",
 keywords = ["pip", "km","mind","csv"],
 description = "把km、zxm和xmind文件转换成表格文件",
 long_description = "把km、zxm和xmind文件转换成表格文件",
 license = "MIT Licence",
 
 url = "https://gitee.com/tuboyou/km-read",
 author = "lixuecheng",
```

