# Comparing `tmp/har2jicase-0.0.2.tar.gz` & `tmp/har2jicase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.2.tar", last modified: Fri Apr 21 04:22:23 2023, max compression
+gzip compressed data, was "har2jicase-0.0.3.tar", last modified: Fri Apr 21 04:42:45 2023, max compression
```

## Comparing `har2jicase-0.0.2.tar` & `har2jicase-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.521029 har2jicase-0.0.2/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:22:23.521029 har2jicase-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.516029 har2jicase-0.0.2/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:22:23.000000 har2jicase-0.0.2/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.519037 har2jicase-0.0.2/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 04:19:33.000000 har2jicase-0.0.2/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:22:23.520029 har2jicase-0.0.2/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.2/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.2/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.2/har_to_case/main.py
--rw-rw-rw-   0        0        0     8170 2023-04-21 02:37:23.000000 har2jicase-0.0.2/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 04:22:23.521029 har2jicase-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1905 2023-04-21 04:22:19.000000 har2jicase-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.639100 har2jicase-0.0.3/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:42:45.638101 har2jicase-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.634090 har2jicase-0.0.3/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.636090 har2jicase-0.0.3/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 04:42:43.000000 har2jicase-0.0.3/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.638101 har2jicase-0.0.3/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.3/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.3/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.3/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8379 2023-04-21 04:40:08.000000 har2jicase-0.0.3/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:42:45.639100 har2jicase-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.3/setup.py
```

### Comparing `har2jicase-0.0.2/har_to_case/common/tools.py` & `har2jicase-0.0.3/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.2/har_to_case/main.py` & `har2jicase-0.0.3/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.2/har_to_case/parse_har.py` & `har2jicase-0.0.3/har_to_case/parse_har.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # 导入yaml和其他需要的库
 import json
 import time
+import sys
 
 import yaml
 import re
 from haralyzer import HarParser
 from loguru import logger
 
 from har_to_case.common.tools import dump_yaml
 
+logger.remove()  # 删去import logger之后自动产生的handler，不删除的话会出现重复输出的现象
+handler_id = logger.add(sys.stderr, level="INFO")  # 添加一个可以修改控制的handler
+
 
 class ParseHar:
     regex_resource = re.compile(r"\/[^\/?\/]*\.(css|ico|jpg|png|gif|bmp|wav|js|jpeg|woff2)(\?.*)?")
     regex_name = re.compile(r"(?<=/api\/)(.*)(?=\?)|(?<=/api\/)(.*)")
     regex_api = re.compile(r"(\/api\/.*)")
 
     def __init__(self, har_file_path, output_file_path=None):
@@ -186,18 +190,18 @@
         # 将案件字入yaml文件中
         with open(f"{self.output_file_path}/test_record_{now}.yaml", "w", encoding='utf-8') as f:
             yaml.dump(test_case, f, default_flow_style=False, allow_unicode=True)
         logger.info('用例生成成功')
 
     def generate_yaml_case(self):
         now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
-        if self.output_file_path is not None:
-            file = self.output_file_path
+        if self.output_file_path is None:
+            file = f"test_record_{now}.yaml"
         else:
-            file = f"./test_record_{now}.yaml"
+            file = self.output_file_path
         test_case = self._generate_case_list()
         dump_yaml(test_case, file)
 
 
 if __name__ == '__main__':
-    case = ParseHar('../192.168.1.117.har', './123/123/123.yaml')
+    case = ParseHar('../192.168.1.117.har', '123.yaml')
     case.generate_yaml_case()
```

### Comparing `har2jicase-0.0.2/setup.py` & `har2jicase-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,21 +32,21 @@
         os.system('git tag v{0}'.format(__version__))
         os.system('git push --tags')
 
         sys.exit(0)
 
 
 setup(
-    name=__title__,
-    version=__version__,
-    description=__description__,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    keywords='har json compare comparison case yaml yml',
-    author=__author__,
+    name=__title__,  # Replace with your own project title
+    version=__version__,  # Replace with your own version
+    description=__description__,  # Replace with your own description
+    long_description=long_description,  # Optiona
+    long_description_content_type="text/markdown",  # Optional (see note above)
+    keywords='har json compare comparison case yaml yml',  # Optional
+    author=__author__,  # Replace with
     author_email=__author_email__,
     url=__url__,
     license=__license__,
     packages=find_packages(include=('har*',)),
     include_package_data=True,
     zip_safe=True,
     install_requires=['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0'],
```

