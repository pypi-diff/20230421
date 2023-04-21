# Comparing `tmp/har2jicase-0.0.8.tar.gz` & `tmp/har2jicase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.8.tar", last modified: Fri Apr 21 05:42:13 2023, max compression
+gzip compressed data, was "har2jicase-0.0.9.tar", last modified: Fri Apr 21 08:22:52 2023, max compression
```

## Comparing `har2jicase-0.0.8.tar` & `har2jicase-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.310704 har2jicase-0.0.8/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:42:13.310704 har2jicase-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.303709 har2jicase-0.0.8/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.8/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.307704 har2jicase-0.0.8/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 05:42:05.000000 har2jicase-0.0.8/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.308704 har2jicase-0.0.8/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.8/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.8/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.8/har_to_case/main.py
--rw-rw-rw-   0        0        0     8608 2023-04-21 05:42:05.000000 har2jicase-0.0.8/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 05:42:13.310704 har2jicase-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.850682 har2jicase-0.0.9/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:22:52.850682 har2jicase-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.843683 har2jicase-0.0.9/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 08:22:52.000000 har2jicase-0.0.9/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.9/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.846682 har2jicase-0.0.9/har_to_case/
+-rw-rw-rw-   0        0        0      499 2023-04-21 07:27:11.000000 har2jicase-0.0.9/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:22:52.849682 har2jicase-0.0.9/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.9/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.9/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 06:55:19.000000 har2jicase-0.0.9/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8742 2023-04-21 07:22:54.000000 har2jicase-0.0.9/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:22:52.851682 har2jicase-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3397 2023-04-21 08:22:51.000000 har2jicase-0.0.9/setup.py
```

### Comparing `har2jicase-0.0.8/har_to_case/common/tools.py` & `har2jicase-0.0.9/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.8/har_to_case/main.py` & `har2jicase-0.0.9/har_to_case/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if len(sys.argv) == 1:
     sys.argv.append('--help')
 now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
 parser = argparse.ArgumentParser(description=__description__)
 parser.add_argument('-v', '--version', help=f"显示版本;当前版本：{version}", action="store_true")
 parser.add_argument('-i', '--input', type=str, help='har文件路径（必填）')
-parser.add_argument('-o', '--output', default=f"test_record_{now}.yaml", type=str, help='指定输出文件名')
+parser.add_argument('-o', '--output', default=f"record_{now}.yaml", type=str, help='指定输出文件名')
 
 
 def main():
     args = parser.parse_args()
     if args.version:
         logger.info(f"当前版本：{version}")
         exit(0)
```

### Comparing `har2jicase-0.0.8/har_to_case/parse_har.py` & `har2jicase-0.0.9/har_to_case/parse_har.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 
 import yaml
 import re
 from haralyzer import HarParser
 from loguru import logger
 
-from har_to_case.common.tools import dump_yaml
+from common.tools import dump_yaml
 
 logger.remove()  # 删去import logger之后自动产生的handler，不删除的话会出现重复输出的现象
 handler_id = logger.add(sys.stderr, level="INFO")  # 添加一个可以修改控制的handler
 
 
 class ParseHar:
     regex_resource = re.compile(r"\/[^\/?\/]*\.(css|ico|jpg|png|gif|bmp|wav|js|jpeg|woff2)(\?.*)?")
@@ -139,15 +139,15 @@
                     else:
                         if validate_contains == '':
                             validate_contains = item
                         else:
                             logger.debug(item)
                             validate_contains = validate_contains + '-' + item
             request_dict['validate']['contains'] = validate_contains
-            logger.info('已成功解析返回体')
+            logger.info('成功解析返回体')
         except KeyError as e:
             logger.debug(e)
 
     def _generate_case_dict(self, entry, test_case_dict, request_dict):
         '''
         生成用例字典的函数,将
         :param entry:
@@ -160,15 +160,14 @@
         self._make_request_method(entry, request_dict)
         self._make_request_params(entry, request_dict)
         self._make_request_header(request_dict)
         self._make_respone_validate(entry, request_dict)
         self._make_respone_valiade_contains(entry, request_dict)
 
     def _generate_case_list(self) -> list:
-        logger.info('拼装用例')
         # 遍历har文件中的每个请求
         test_case_list = []
         for page in self.har_parser.pages:
             for entry in page.entries:
                 # 提取需要的信息
                 if self.regex_resource.search(entry["request"]["url"]) is None:
                     request_dict = {
@@ -183,29 +182,33 @@
                             },
                             'contains': ''
                         }
                     }
                     test_case_dict = {"name": '',
                                       "requests": request_dict}
                     # 构建框架用例格式字典
+                    logger.info(
+                        '---------------------------------------构建用例--------------------- -----------------')
                     self._generate_case_dict(entry, test_case_dict, request_dict)
                     if test_case_dict['name'] == '':
                         pass
                     else:
                         test_case_list.append(test_case_dict)
             return test_case_list
 
     def generate_yaml_case(self):
+        '''
+        生成yaml格式用例
+        '''
         now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
         if '.yaml' in self.output_file_path or '.yml' in self.output_file_path:
             file = self.output_file_path
 
         else:
-            file = self.output_file_path + f"/test_record_{now}.yaml"
-        print(file)
+            file = self.output_file_path + f"/record_{now}.yaml"
         test_case = self._generate_case_list()
         dump_yaml(test_case, file)
 
 
 if __name__ == '__main__':
-    case = ParseHar('../192.168.1.117.har', './common')
+    case = ParseHar('./192.168.1.117.har', './casefile')
     case.generate_yaml_case()
```

