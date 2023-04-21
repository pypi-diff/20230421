# Comparing `tmp/har2jicase-0.0.1.tar.gz` & `tmp/har2jicase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.1.tar", last modified: Fri Apr 21 03:08:03 2023, max compression
+gzip compressed data, was "har2jicase-0.0.2.tar", last modified: Fri Apr 21 04:22:23 2023, max compression
```

## Comparing `har2jicase-0.0.1.tar` & `har2jicase-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.852098 har2jicase-0.0.1/
--rw-rw-rw-   0        0        0      484 2023-04-21 03:08:03.852098 har2jicase-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.827098 har2jicase-0.0.1/api_to_case/
--rw-rw-rw-   0        0        0      522 2022-10-31 02:55:00.000000 har2jicase-0.0.1/api_to_case/__init__.py
--rw-rw-rw-   0        0        0     1458 2022-10-31 02:56:36.000000 har2jicase-0.0.1/api_to_case/api2case.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.828098 har2jicase-0.0.1/api_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.1/api_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-04-20 03:11:57.000000 har2jicase-0.0.1/api_to_case/common/tools.py
--rw-rw-rw-   0        0        0     8883 2022-10-28 09:38:22.000000 har2jicase-0.0.1/api_to_case/main.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.841101 har2jicase-0.0.1/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 03:08:03.000000 har2jicase-0.0.1/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.843097 har2jicase-0.0.1/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 03:04:57.000000 har2jicase-0.0.1/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:08:03.846098 har2jicase-0.0.1/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.1/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.1/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.1/har_to_case/main.py
--rw-rw-rw-   0        0        0     8170 2023-04-21 02:37:23.000000 har2jicase-0.0.1/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 03:08:03.852098 har2jicase-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-04-21 03:08:02.000000 har2jicase-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.521029 har2jicase-0.0.2/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:22:23.521029 har2jicase-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.516029 har2jicase-0.0.2/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.519037 har2jicase-0.0.2/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 04:19:33.000000 har2jicase-0.0.2/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.520029 har2jicase-0.0.2/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.2/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.2/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.2/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8170 2023-04-21 02:37:23.000000 har2jicase-0.0.2/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:22:23.521029 har2jicase-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1905 2023-04-21 04:22:19.000000 har2jicase-0.0.2/setup.py
```

### Comparing `har2jicase-0.0.1/api_to_case/api2case.py` & `har2jicase-0.0.2/har_to_case/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-#!/usr/bin/env python
+#! /usr/bin/env python
 """
--*- coding: utf-8 -*-
-Author   : JiQing
-Email    : qing.ji@extremevision.com.cn
-Date     : 2022/10/26 9:38
-Desc     :
-FileName : api2case.py
-Software : PyCharm
+-*- coding: UTF-8 -*-
+Project   : har2case
+Author    : Captain
+Email     : qing.ji@extremevision.com.cn
+Date      : 2023/4/19 14:15
+FileName  : main.py
+Software  : PyCharm
+Desc      : 项目主入口
 """
 import sys
 import argparse
 
 from loguru import logger
-from api_to_case.main import SwaggerParser
-from api_to_case import __description__
+from har_to_case.parse_har import ParseHar
+from har_to_case import __description__
 
 try:
-    from api_to_case import __version__ as version
+    from har_to_case import __version__ as version
 except ImportError:
     version = None
 
 if len(sys.argv) == 1:
     sys.argv.append('--help')
 
 parser = argparse.ArgumentParser(description=__description__)
 parser.add_argument('-v', '--version', help=f"显示版本;当前版本：{version}", action="store_true")
-parser.add_argument('-u', '--url', type=str, help='swagger API接口文档地址（必填)')
-parser.add_argument('-n', '--username', default=None, type=str, help='swagger用户名')
-parser.add_argument('-w', '--password', default=None, type=str, help='swagger密码')
-parser.add_argument('-p', '--path', default=None, type=str, help='API路径，用于单独转换指定API')
+parser.add_argument('-i', '--input', type=str, help='har文件路径（必填）')
+parser.add_argument('-o', '--output', default=r'./', type=str, help='指定输出文件名')
 
 
 def main():
     args = parser.parse_args()
     if args.version:
         logger.info(f"当前版本：{version}")
         exit(0)
     arguments = parser.parse_args()
-    if not arguments.url:
-        logger.error("Swagger API地址为必填项")
-    SwaggerParser(arguments.url, arguments.username, arguments.password).gen_testcase(arguments.path)
+    if not arguments.input:
+        logger.error("har文件路径为必填项：-i {har file path}")
+    ParseHar(arguments.input, arguments.output).generate_yaml_case()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `har2jicase-0.0.1/api_to_case/common/tools.py` & `har2jicase-0.0.2/har_to_case/common/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,25 +53,28 @@
     if os.path.exists(yaml_file):
         logger.debug("文件存在，跳过解析")
         return
 
     logger.info("开始创建YAML格式文件")
     with io.open(yaml_file, 'w', encoding="utf-8") as outfile:
         yaml.dump(case, outfile, allow_unicode=True, default_flow_style=False, indent=4)
+
         logger.info(f"yaml文件:{yaml_file}创建成功")
 
 
 def dump_json(case, json_file):
     '''
     创建YAML格式文件
     :param case:
     :param json_file:
     :return:
     '''
     logger.info("开始创建json格式文件")
+    if not os.path.exists(json_file):
+        os.makedirs(json_file)
 
     with io.open(json_file, 'w', encoding="utf-8") as outfile:
         my_json_str = json.dumps(case, ensure_ascii=False, indent=4)
         if isinstance(my_json_str, bytes):
             my_json_str = my_json_str.decode("utf-8")
         outfile.write(my_json_str)
     logger.info(f"json文件: {json_file}创建成功")
```

### Comparing `har2jicase-0.0.1/har_to_case/parse_har.py` & `har2jicase-0.0.2/har_to_case/parse_har.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.1/setup.py` & `har2jicase-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,23 +42,23 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='har json compare comparison case yaml yml',
     author=__author__,
     author_email=__author_email__,
     url=__url__,
     license=__license__,
-    packages=find_packages(),
+    packages=find_packages(include=('har*',)),
     include_package_data=True,
     zip_safe=True,
     install_requires=['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0'],
     entry_points={
         'console_scripts': [
-            'har2case = har_to_case.parse_har:main'
+            'har2case = har_to_case.main:main'
         ]
     },
     cmdclass={
         'har2case': ParserCommand
     }
 )
 
 # python setup.py sdist bdist_wheel
-# python -m twine upload dist/*
+# python -m twine upload dist/* -u jiqing19861123 -p CJ2938cj
```

