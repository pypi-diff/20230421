# Comparing `tmp/har2jicase-0.0.4.tar.gz` & `tmp/har2jicase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.4.tar", last modified: Fri Apr 21 04:46:21 2023, max compression
+gzip compressed data, was "har2jicase-0.0.5.tar", last modified: Fri Apr 21 04:57:38 2023, max compression
```

## Comparing `har2jicase-0.0.4.tar` & `har2jicase-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.606712 har2jicase-0.0.4/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:46:21.606712 har2jicase-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.601694 har2jicase-0.0.4/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.603816 har2jicase-0.0.4/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 04:46:15.000000 har2jicase-0.0.4/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.605758 har2jicase-0.0.4/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.4/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.4/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.4/har_to_case/main.py
--rw-rw-rw-   0        0        0     8408 2023-04-21 04:46:14.000000 har2jicase-0.0.4/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 04:46:21.606712 har2jicase-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:57:38.554894 har2jicase-0.0.5/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:57:38.554894 har2jicase-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 04:57:38.548895 har2jicase-0.0.5/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.5/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 04:57:38.551905 har2jicase-0.0.5/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 04:57:33.000000 har2jicase-0.0.5/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:57:38.553894 har2jicase-0.0.5/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.5/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.5/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.5/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8408 2023-04-21 04:46:14.000000 har2jicase-0.0.5/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:57:38.554894 har2jicase-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.5/setup.py
```

### Comparing `har2jicase-0.0.4/har_to_case/common/tools.py` & `har2jicase-0.0.5/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.4/har_to_case/main.py` & `har2jicase-0.0.5/har_to_case/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 Date      : 2023/4/19 14:15
 FileName  : main.py
 Software  : PyCharm
 Desc      : 项目主入口
 """
 import sys
 import argparse
+import time
 
 from loguru import logger
 from har_to_case.parse_har import ParseHar
 from har_to_case import __description__
 
 try:
     from har_to_case import __version__ as version
 except ImportError:
     version = None
 
 if len(sys.argv) == 1:
     sys.argv.append('--help')
-
+now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
 parser = argparse.ArgumentParser(description=__description__)
 parser.add_argument('-v', '--version', help=f"显示版本;当前版本：{version}", action="store_true")
 parser.add_argument('-i', '--input', type=str, help='har文件路径（必填）')
-parser.add_argument('-o', '--output', default=r'./', type=str, help='指定输出文件名')
+parser.add_argument('-o', '--output', default=f"test_record_{now}.yaml", type=str, help='指定输出文件名')
 
 
 def main():
     args = parser.parse_args()
     if args.version:
         logger.info(f"当前版本：{version}")
         exit(0)
```

### Comparing `har2jicase-0.0.4/har_to_case/parse_har.py` & `har2jicase-0.0.5/har_to_case/parse_har.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.4/setup.py` & `har2jicase-0.0.5/setup.py`

 * *Files identical despite different names*

