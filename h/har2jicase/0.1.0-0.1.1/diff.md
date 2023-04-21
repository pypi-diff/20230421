# Comparing `tmp/har2jicase-0.1.0.tar.gz` & `tmp/har2jicase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.1.0.tar", last modified: Fri Apr 21 08:27:27 2023, max compression
+gzip compressed data, was "har2jicase-0.1.1.tar", last modified: Fri Apr 21 08:38:06 2023, max compression
```

## Comparing `har2jicase-0.1.0.tar` & `har2jicase-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.784453 har2jicase-0.1.0/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:27:27.784453 har2jicase-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.778561 har2jicase-0.1.0/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.0/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.781419 har2jicase-0.1.0/har_to_case/
--rw-rw-rw-   0        0        0      499 2023-04-21 07:27:11.000000 har2jicase-0.1.0/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.783450 har2jicase-0.1.0/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.0/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.0/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.1.0/har_to_case/main.py
--rw-rw-rw-   0        0        0     8742 2023-04-21 07:22:54.000000 har2jicase-0.1.0/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 08:27:27.784453 har2jicase-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3324 2023-04-21 08:26:03.000000 har2jicase-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.397973 har2jicase-0.1.1/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:38:06.396971 har2jicase-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.392576 har2jicase-0.1.1/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.1/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.394592 har2jicase-0.1.1/har_to_case/
+-rw-rw-rw-   0        0        0      204 2023-04-21 08:27:53.000000 har2jicase-0.1.1/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.396971 har2jicase-0.1.1/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.1/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.1/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.1.1/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.1/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:38:06.397973 har2jicase-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3461 2023-04-21 08:38:04.000000 har2jicase-0.1.1/setup.py
```

### Comparing `har2jicase-0.1.0/PKG-INFO` & `har2jicase-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.0
+Version: 0.1.1
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.0/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.1/har2jicase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.0
+Version: 0.1.1
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.0/har_to_case/common/tools.py` & `har2jicase-0.1.1/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.0/har_to_case/main.py` & `har2jicase-0.1.1/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.0/har_to_case/parse_har.py` & `har2jicase-0.1.1/har_to_case/parse_har.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 
 import yaml
 import re
 from haralyzer import HarParser
 from loguru import logger
 
-from common.tools import dump_yaml
+from har_to_case.common.tools import dump_yaml
 
 logger.remove()  # 删去import logger之后自动产生的handler，不删除的话会出现重复输出的现象
 handler_id = logger.add(sys.stderr, level="INFO")  # 添加一个可以修改控制的handler
 
 
 class ParseHar:
     regex_resource = re.compile(r"\/[^\/?\/]*\.(css|ico|jpg|png|gif|bmp|wav|js|jpeg|woff2)(\?.*)?")
```

### Comparing `har2jicase-0.1.0/setup.py` & `har2jicase-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 -*- coding: UTF-8 -*-
 Project   : pypi
 Author    : Captain
 Email     : qing.ji@extremevision.com.cn
 Date      : 2023/4/21 15:34
 FileName  : setup.py
 Software  : PyCharm
-Desc      : Note: To use the 'upload' functionality of this file, you must:
-            $ pipenv install twine --dev
+Desc      :
+            手动构建与上传pypi
+            python setup_backup.py sdist bdist_wheel
+            python -m twine upload dist/* -u jiqing19861123 -p CJ2938cj
+
+            自动构建与上传pypi
+            python setup.py upload
 """
 
 import io
 import os
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
@@ -23,15 +28,15 @@
 KEYWORDS = 'har json compare comparison case yaml yml'
 AUTHOR = 'Captain Ji'
 EMAIL = 'qing.ji@extremevision.com.cn'
 URL = ''  # 项目git地址
 LICENSE = 'MIT'  # 项目license
 PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude为排除的包
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.1.0'  # 为项目指定目前的版本号
+VERSION = '0.1.1'  # 为项目指定目前的版本号
 pypi_username = 'jiqing19861123'
 pypi_password = 'CJ2938cj'
 # 项目依赖的库
 REQUIRED = ['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0']
 # 项目入口文件
 ENTRY_POINTS = {
     'console_scripts': [
```

