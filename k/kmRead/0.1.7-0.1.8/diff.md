# Comparing `tmp/kmRead-0.1.7.tar.gz` & `tmp/kmRead-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kmRead-0.1.7.tar", last modified: Fri Apr 21 01:55:35 2023, max compression
+gzip compressed data, was "dist\kmRead-0.1.8.tar", last modified: Fri Apr 21 02:50:04 2023, max compression
```

## Comparing `kmRead-0.1.7.tar` & `kmRead-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/
--rw-rw-rw-   0        0        0      337 2023-04-21 01:55:35.000000 kmRead-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead/
--rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.7/kmRead/__init__.py
--rw-rw-rw-   0        0        0     9592 2023-04-21 01:54:47.000000 kmRead-0.1.7/kmRead/kmRead.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead.egg-info/
--rw-rw-rw-   0        0        0      337 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-21 01:55:35.000000 kmRead-0.1.7/kmRead.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 01:55:34.000000 kmRead-0.1.7/kmRead.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:55:35.000000 kmRead-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-04-21 01:55:07.000000 kmRead-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:50:04.000000 kmRead-0.1.8/
+-rw-rw-rw-   0        0        0      337 2023-04-21 02:50:04.000000 kmRead-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead/
+-rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.8/kmRead/__init__.py
+-rw-rw-rw-   0        0        0     9956 2023-04-21 02:47:12.000000 kmRead-0.1.8/kmRead/kmRead.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/
+-rw-rw-rw-   0        0        0      337 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 02:50:04.000000 kmRead-0.1.8/kmRead.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 02:50:04.000000 kmRead-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-04-21 02:49:42.000000 kmRead-0.1.8/setup.py
```

### Comparing `kmRead-0.1.7/kmRead/kmRead.py` & `kmRead-0.1.8/kmRead/kmRead.py`

 * *Files 7% similar despite different names*

```diff
@@ -220,18 +220,23 @@
     # print(*put())
     run(*put(),False)
 
         
 
    
 def mainInit():
-    print('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
-    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
-    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.zxm\shell\zxm2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
-    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.xmind\shell\xmind2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
+    print(sys.argv,sys.argv[0][:-3])
+#    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
+#    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.zxm\shell\zxm2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
+#    os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.xmind\shell\xmind2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
+    
+    os.system(r'''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\"{}kme.exe\" \"%1\""'''.format(sys.argv[0][:-3]))
+    os.system(r'''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.zxm\shell\zxm2Excel\command" /f /d "\"{}kme.exe\" \"%1\""'''.format(sys.argv[0][:-3]))
+    os.system(r'''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.xmind\shell\xmind2Excel\command" /f /d "\"{}kme.exe\" \"%1\""'''.format(sys.argv[0][:-3]))
+
 
     # pv=""
     # p=""
     # if os.environ.get('HOME') is not None:
     #     pv=os.path.join(os.environ.get('HOME'),".km")
     # elif os.environ.get('HOMEPATH') is not None:
     #     pv=os.path.join(os.environ.get('HOMEPATH'),".km")
```

### Comparing `kmRead-0.1.7/setup.py` & `kmRead-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
 name = "kmRead",
-version = "0.1.7",
+version = "0.1.8",
 keywords = ["pip", "km","mind","csv"],
 description = "把km、zxm和xmind文件转换成表格文件",
 long_description = "把km、zxm和xmind文件转换成表格文件",
 license = "MIT Licence",
 
 url = "https://gitee.com/tuboyou/km-read",
 author = "lixuecheng",
```

