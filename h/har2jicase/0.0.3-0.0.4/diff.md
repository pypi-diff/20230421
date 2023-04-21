# Comparing `tmp/har2jicase-0.0.3.tar.gz` & `tmp/har2jicase-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.3.tar", last modified: Fri Apr 21 04:42:45 2023, max compression
+gzip compressed data, was "har2jicase-0.0.4.tar", last modified: Fri Apr 21 04:46:21 2023, max compression
```

## Comparing `har2jicase-0.0.3.tar` & `har2jicase-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.639100 har2jicase-0.0.3/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:42:45.638101 har2jicase-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.634090 har2jicase-0.0.3/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:42:45.000000 har2jicase-0.0.3/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.636090 har2jicase-0.0.3/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 04:42:43.000000 har2jicase-0.0.3/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:42:45.638101 har2jicase-0.0.3/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.3/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.3/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.3/har_to_case/main.py
--rw-rw-rw-   0        0        0     8379 2023-04-21 04:40:08.000000 har2jicase-0.0.3/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 04:42:45.639100 har2jicase-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.606712 har2jicase-0.0.4/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:46:21.606712 har2jicase-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.601694 har2jicase-0.0.4/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:46:21.000000 har2jicase-0.0.4/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.603816 har2jicase-0.0.4/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 04:46:15.000000 har2jicase-0.0.4/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:46:21.605758 har2jicase-0.0.4/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.4/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.4/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1286 2023-04-21 02:30:51.000000 har2jicase-0.0.4/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8408 2023-04-21 04:46:14.000000 har2jicase-0.0.4/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:46:21.606712 har2jicase-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.4/setup.py
```

### Comparing `har2jicase-0.0.3/har_to_case/common/tools.py` & `har2jicase-0.0.4/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.3/har_to_case/main.py` & `har2jicase-0.0.4/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.3/har_to_case/parse_har.py` & `har2jicase-0.0.4/har_to_case/parse_har.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 from haralyzer import HarParser
 from loguru import logger
 
 from har_to_case.common.tools import dump_yaml
 
 logger.remove()  # 删去import logger之后自动产生的handler，不删除的话会出现重复输出的现象
-handler_id = logger.add(sys.stderr, level="INFO")  # 添加一个可以修改控制的handler
+handler_id = logger.add(sys.stderr, level="DEBUG")  # 添加一个可以修改控制的handler
 
 
 class ParseHar:
     regex_resource = re.compile(r"\/[^\/?\/]*\.(css|ico|jpg|png|gif|bmp|wav|js|jpeg|woff2)(\?.*)?")
     regex_name = re.compile(r"(?<=/api\/)(.*)(?=\?)|(?<=/api\/)(.*)")
     regex_api = re.compile(r"(\/api\/.*)")
 
@@ -194,14 +194,15 @@
 
     def generate_yaml_case(self):
         now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
         if self.output_file_path is None:
             file = f"test_record_{now}.yaml"
         else:
             file = self.output_file_path
+        logger.debug(file)
         test_case = self._generate_case_list()
         dump_yaml(test_case, file)
 
 
 if __name__ == '__main__':
     case = ParseHar('../192.168.1.117.har', '123.yaml')
     case.generate_yaml_case()
```

### Comparing `har2jicase-0.0.3/setup.py` & `har2jicase-0.0.4/setup.py`

 * *Files identical despite different names*

