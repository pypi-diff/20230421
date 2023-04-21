# Comparing `tmp/har2jicase-0.1.4.tar.gz` & `tmp/har2jicase-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.1.4.tar", last modified: Fri Apr 21 09:07:00 2023, max compression
+gzip compressed data, was "har2jicase-0.1.5.tar", last modified: Fri Apr 21 09:07:28 2023, max compression
```

## Comparing `har2jicase-0.1.4.tar` & `har2jicase-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:07:00.544073 har2jicase-0.1.4/
--rw-rw-rw-   0        0        0      512 2023-04-21 09:07:00.544073 har2jicase-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:07:00.540064 har2jicase-0.1.4/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      512 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.4/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 09:07:00.542069 har2jicase-0.1.4/har_to_case/
--rw-rw-rw-   0        0        0      254 2023-04-21 09:07:00.000000 har2jicase-0.1.4/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:07:00.543064 har2jicase-0.1.4/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.4/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.4/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.4/har_to_case/main.py
--rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.4/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 09:07:00.544073 har2jicase-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3917 2023-04-21 09:06:59.000000 har2jicase-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:07:28.037988 har2jicase-0.1.5/
+-rw-rw-rw-   0        0        0      512 2023-04-21 09:07:28.036988 har2jicase-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:07:28.032987 har2jicase-0.1.5/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.5/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 09:07:28.034988 har2jicase-0.1.5/har_to_case/
+-rw-rw-rw-   0        0        0      254 2023-04-21 09:07:27.000000 har2jicase-0.1.5/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:07:28.035988 har2jicase-0.1.5/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.5/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.5/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.5/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.5/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:07:28.037988 har2jicase-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3917 2023-04-21 09:07:26.000000 har2jicase-0.1.5/setup.py
```

### Comparing `har2jicase-0.1.4/PKG-INFO` & `har2jicase-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.4
+Version: 0.1.5
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.4/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.5/har2jicase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.4
+Version: 0.1.5
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.4/har_to_case/common/tools.py` & `har2jicase-0.1.5/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.4/har_to_case/main.py` & `har2jicase-0.1.5/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.4/har_to_case/parse_har.py` & `har2jicase-0.1.5/har_to_case/parse_har.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.4/setup.py` & `har2jicase-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 AUTHOR = 'Captain Ji'
 EMAIL = 'qing.ji@extremevision.com.cn'
 URL = ''  # 项目git地址
 LICENSE = 'MIT'  # 项目license
 PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude为排除的包
 REQUIRES_PYTHON = '>=3.6.13'
 PROJECT_PATH = 'har_to_case'
-VERSION = '0.1.4'  # 为项目指定目前的版本号
+VERSION = '0.1.5'  # 为项目指定目前的版本号
 pypi_username = 'jiqing19861123'
 pypi_password = 'CJ2938cj'
 # 项目依赖的库
 REQUIRED = ['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0']
 # 项目入口文件
 ENTRY_POINTS = {
     'console_scripts': [
```

