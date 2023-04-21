# Comparing `tmp/har2jicase-0.0.9.tar.gz` & `tmp/har2jicase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.9.tar", last modified: Fri Apr 21 08:22:52 2023, max compression
+gzip compressed data, was "har2jicase-0.1.0.tar", last modified: Fri Apr 21 08:27:27 2023, max compression
```

## Comparing `har2jicase-0.0.9.tar` & `har2jicase-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.850682 har2jicase-0.0.9/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:22:52.850682 har2jicase-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.843683 har2jicase-0.0.9/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.9/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.846682 har2jicase-0.0.9/har_to_case/
--rw-rw-rw-   0        0        0      499 2023-04-21 07:27:11.000000 har2jicase-0.0.9/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.849682 har2jicase-0.0.9/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.9/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.9/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.0.9/har_to_case/main.py
--rw-rw-rw-   0        0        0     8742 2023-04-21 07:22:54.000000 har2jicase-0.0.9/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 08:22:52.851682 har2jicase-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3397 2023-04-21 08:22:51.000000 har2jicase-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.784453 har2jicase-0.1.0/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:27:27.784453 har2jicase-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.778561 har2jicase-0.1.0/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 08:27:27.000000 har2jicase-0.1.0/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.0/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.781419 har2jicase-0.1.0/har_to_case/
+-rw-rw-rw-   0        0        0      499 2023-04-21 07:27:11.000000 har2jicase-0.1.0/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:27:27.783450 har2jicase-0.1.0/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.0/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.0/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.1.0/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8742 2023-04-21 07:22:54.000000 har2jicase-0.1.0/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:27:27.784453 har2jicase-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3324 2023-04-21 08:26:03.000000 har2jicase-0.1.0/setup.py
```

### Comparing `har2jicase-0.0.9/PKG-INFO` & `har2jicase-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.0.9
+Version: 0.1.0
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.0.9/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.0/har2jicase.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.0.9
+Version: 0.1.0
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.0.9/har_to_case/common/tools.py` & `har2jicase-0.1.0/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.9/har_to_case/main.py` & `har2jicase-0.1.0/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.9/har_to_case/parse_har.py` & `har2jicase-0.1.0/har_to_case/parse_har.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.9/setup.py` & `har2jicase-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,37 @@
             $ pipenv install twine --dev
 """
 
 import io
 import os
 import sys
 from shutil import rmtree
-
 from setuptools import find_packages, setup, Command
 
-# 写入自己的内容 start——1
+# 写入自己的内容
 NAME = 'har2jicase'  # 项目名
 DESCRIPTION = '将浏览器录制的har文件为极星测试框架的YAML测试用例'
 KEYWORDS = 'har json compare comparison case yaml yml'
 AUTHOR = 'Captain Ji'
 EMAIL = 'qing.ji@extremevision.com.cn'
 URL = ''  # 项目git地址
 LICENSE = 'MIT'  # 项目license
 PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude为排除的包
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.0.9'  # 为项目指定目前的版本号
+VERSION = '0.1.0'  # 为项目指定目前的版本号
 pypi_username = 'jiqing19861123'
 pypi_password = 'CJ2938cj'
 # 项目依赖的库
 REQUIRED = ['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0']
+# 项目入口文件
 ENTRY_POINTS = {
     'console_scripts': [
         'har2case = har_to_case.main:main'
     ]
-},
+}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         LONG_DESC = '\n' + f.read()
 except FileNotFoundError:
@@ -82,17 +82,17 @@
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system(f'twine upload dist/* -u {pypi_username} -p {pypi_password}')
 
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        # self.status('Pushing git tags…')
+        # os.system('git tag v{0}'.format(about['__version__']))
+        # os.system('git push --tags')
 
         sys.exit()
 
 
 setup(
     name=NAME,  # 和前边的保持一致
     version=about['__version__'],
@@ -105,16 +105,12 @@
     python_requires=REQUIRES_PYTHON,
     url=URL,
     license=LICENSE,
     packages=PACKAGES,
     include_package_data=True,
     zip_safe=True,
     install_requires=REQUIRED,
-    entry_points={
-        'console_scripts': [
-            'har2case = har_to_case.main:main'
-        ]
-    },
+    entry_points=ENTRY_POINTS,
     cmdclass={
         'upload': UploadCommand,
     }
 )
```

