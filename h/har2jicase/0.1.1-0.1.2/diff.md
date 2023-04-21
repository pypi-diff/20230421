# Comparing `tmp/har2jicase-0.1.1.tar.gz` & `tmp/har2jicase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.1.1.tar", last modified: Fri Apr 21 08:38:06 2023, max compression
+gzip compressed data, was "har2jicase-0.1.2.tar", last modified: Fri Apr 21 09:01:56 2023, max compression
```

## Comparing `har2jicase-0.1.1.tar` & `har2jicase-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.397973 har2jicase-0.1.1/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:38:06.396971 har2jicase-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.392576 har2jicase-0.1.1/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      512 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 08:38:06.000000 har2jicase-0.1.1/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.1/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.394592 har2jicase-0.1.1/har_to_case/
--rw-rw-rw-   0        0        0      204 2023-04-21 08:27:53.000000 har2jicase-0.1.1/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:38:06.396971 har2jicase-0.1.1/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.1/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.1/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.1.1/har_to_case/main.py
--rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.1/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 08:38:06.397973 har2jicase-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3461 2023-04-21 08:38:04.000000 har2jicase-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:01:56.429146 har2jicase-0.1.2/
+-rw-rw-rw-   0        0        0      512 2023-04-21 09:01:56.429146 har2jicase-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:01:56.415742 har2jicase-0.1.2/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.2/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 09:01:56.424144 har2jicase-0.1.2/har_to_case/
+-rw-rw-rw-   0        0        0      245 2023-04-21 09:01:56.000000 har2jicase-0.1.2/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:01:56.427154 har2jicase-0.1.2/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.2/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.2/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1385 2023-04-21 08:47:16.000000 har2jicase-0.1.2/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.2/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:01:56.429146 har2jicase-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3930 2023-04-21 09:01:52.000000 har2jicase-0.1.2/setup.py
```

### Comparing `har2jicase-0.1.1/PKG-INFO` & `har2jicase-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.1
+Version: 0.1.2
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.1/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.2/har2jicase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.1
+Version: 0.1.2
 Summary: 将浏览器录制的har文件为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.1/har_to_case/common/tools.py` & `har2jicase-0.1.2/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.1/har_to_case/main.py` & `har2jicase-0.1.2/har_to_case/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 except ImportError:
     version = None
 
 if len(sys.argv) == 1:
     sys.argv.append('--help')
 now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
 parser = argparse.ArgumentParser(description=__description__)
-parser.add_argument('-v', '--version', help=f"显示版本;当前版本：{version}", action="store_true")
+# parser.add_argument('-v', '--version', help=f"显示版本;当前版本：{version}", action="store_true")
 parser.add_argument('-i', '--input', type=str, help='har文件路径（必填）')
 parser.add_argument('-o', '--output', default=f"record_{now}.yaml", type=str, help='指定输出文件名')
 
 
 def main():
     args = parser.parse_args()
     if args.version:
```

### Comparing `har2jicase-0.1.1/har_to_case/parse_har.py` & `har2jicase-0.1.2/har_to_case/parse_har.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.1/setup.py` & `har2jicase-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,42 +28,53 @@
 KEYWORDS = 'har json compare comparison case yaml yml'
 AUTHOR = 'Captain Ji'
 EMAIL = 'qing.ji@extremevision.com.cn'
 URL = ''  # 项目git地址
 LICENSE = 'MIT'  # 项目license
 PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude为排除的包
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.1.1'  # 为项目指定目前的版本号
+PROJECT_PATH = 'har_to_case'
+VERSION = '0.1.2'  # 为项目指定目前的版本号
 pypi_username = 'jiqing19861123'
 pypi_password = 'CJ2938cj'
 # 项目依赖的库
 REQUIRED = ['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0']
 # 项目入口文件
 ENTRY_POINTS = {
     'console_scripts': [
-        'har2case = har_to_case.main:main'
+        f'har2case = {PROJECT_PATH}.main:main'
     ]
 }
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         LONG_DESC = '\n' + f.read()
 except FileNotFoundError:
     LONG_DESC = DESCRIPTION
 
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(f"{here}/{PROJECT_PATH}", project_slug, '__version__.py')) as f:
         exec(f.read(), about)
 else:
     about['__version__'] = VERSION
 
+with open(os.path.join(f"{here}/{PROJECT_PATH}", '__init__.py'), 'w', encoding='utf-8') as f:
+    f.write(f'__version__ = {VERSION}')
+    f.write(f'__title__ = {NAME}'
+            f'__description__ = {DESCRIPTION}'
+            f'__url__ = {URL}'
+            f'__version__ = {VERSION}'
+            f'__author__ = {AUTHOR}'
+            f'__author_email__ = {EMAIL}'
+            f'__license__ = {LICENSE}')
+
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
```

