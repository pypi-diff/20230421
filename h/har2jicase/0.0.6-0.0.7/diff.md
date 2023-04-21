# Comparing `tmp/har2jicase-0.0.6.tar.gz` & `tmp/har2jicase-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.6.tar", last modified: Fri Apr 21 05:19:44 2023, max compression
+gzip compressed data, was "har2jicase-0.0.7.tar", last modified: Fri Apr 21 05:30:25 2023, max compression
```

## Comparing `har2jicase-0.0.6.tar` & `har2jicase-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:19:44.092379 har2jicase-0.0.6/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:19:44.092379 har2jicase-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:19:44.082381 har2jicase-0.0.6/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 05:19:44.000000 har2jicase-0.0.6/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.6/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 05:19:44.087379 har2jicase-0.0.6/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 05:18:38.000000 har2jicase-0.0.6/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:19:44.090379 har2jicase-0.0.6/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.6/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.6/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.6/har_to_case/main.py
--rw-rw-rw-   0        0        0     8341 2023-04-21 05:16:13.000000 har2jicase-0.0.6/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 05:19:44.092379 har2jicase-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.787051 har2jicase-0.0.7/
+-rw-rw-rw-   0        0        0      484 2023-04-21 05:30:25.785979 har2jicase-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.775653 har2jicase-0.0.7/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.7/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.782203 har2jicase-0.0.7/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 05:30:17.000000 har2jicase-0.0.7/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.784974 har2jicase-0.0.7/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.7/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.7/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.7/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8568 2023-04-21 05:30:17.000000 har2jicase-0.0.7/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:30:25.787051 har2jicase-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.7/setup.py
```

### Comparing `har2jicase-0.0.6/har_to_case/common/tools.py` & `har2jicase-0.0.7/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.6/har_to_case/main.py` & `har2jicase-0.0.7/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.6/har_to_case/parse_har.py` & `har2jicase-0.0.7/har_to_case/parse_har.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,97 +32,97 @@
     def _make_request_name(self, entry: dict, test_case_dict: dict):
         '''
         解析har文件中entry项拼接出用例名，实际上是通过解析url后替换”/“为”-“生成用例名
         :param entry: har文件中entry项
         :return: 根据url拼接用例名
         '''
         global names
-        logger.info('解析用例名')
         if self.regex_resource.search(entry["request"]["url"]) is None:
             # 通过正则匹配url中的接口地址来取名
             names = self.regex_name.findall(entry["request"]["url"])
             try:
                 for i in names[0]:
                     if i != '':
                         name = i.replace("/", '-')
                         test_case_dict['name'] = name
+                        logger.info(f'成功解析用例名:{name}')
             except IndexError as e:
                 logger.debug(e)
                 logger.debug(names)
                 pass
 
     def _make_request_url(self, entry: dict, request_dict: dict):
         '''
         解析har文件获取接口请求地址
         :param entry: har文件得entry部分
         :param request_dict: 构造的request字典
         :return:
         '''
-        logger.info('解析请求地址')
         url = self.regex_api.findall(entry["request"]["url"])
         try:
             request_dict['url'] = url[0]
+            logger.info(f'成功解析请求地址:{url[0]}')
         except IndexError as e:
             logger.debug(e)
             logger.debug(url)
             pass
 
     def _make_request_method(self, entry: dict, request_dict: dict):
         '''
         解析har文件获取请求方法
         :param entry: har文件得entry部分
         :param request_dict: 构造的request字典
         :return:
         '''
-        logger.info('解析请求方法')
         request_dict['method'] = entry["request"]["method"]
+        logger.info(f"成功解析请求方法:{request_dict['method']}")
 
     def _make_request_header(self, request_dict: dict):
         '''
         构造request字典中headers部分;框架中有独立的请求头生成方法,所以此工具只负责生成固定的请求头,不解析entry获取请求头信息
         :param request_dict:
         :return:
         '''
-        logger.info('解析请求头')
+
         request_dict['headers'] = {'Authorization': "", "Content-Type": "application/json; charset=utf-8"}
+        logger.info(f"成功配置请求头:{request_dict['headers']}")
 
     def _make_request_params(self, entry: dict, request_dict: dict):
         '''
         解析har文件获取请求参数
         :param entry: har文件的entry部分
         :param request_dict: 构造的request字典
         :return:
         '''
-        logger.info('解析请求参数')
         if "postData" in entry["request"]:
             request_dict['params'] = json.loads(entry["request"]["postData"]["text"])
+            logger.info(f"成功解析请求参数:{request_dict['params']}")
         else:
             request_dict['params'] = None
 
     def _make_respone_validate(self, entry: dict, request_dict: dict):
         '''
         解析har文件respone部分,生成用例断言
         :param entry: har文件的entry部分
         :param request_dict: 构造的request字典
         '''
-        logger.info('解析返回状态码')
         try:
             data = json.loads(entry['response']['content']['text'])
             request_dict['validate']['equals']['status_code'] = data['status_code']
+            logger.info(f"成功解析返回状态码:{request_dict['validate']['equals']}")
         except KeyError as e:
             logger.debug(e)
 
     def _make_respone_valiade_contains(self, entry: dict, request_dict: dict):
         '''
         解析har文件respone部分,通过返回体中的key生成断言应包含的关键字
         :param entry: har文件的entry部分
         :param request_dict: 构造的request字典
         :return:
         '''
-        logger.info('解析返回体')
         try:
             data = json.loads(entry['response']['content']['text'])
             data = data['data']
             validate_contains = ''
             if isinstance(data, dict):
                 for key in data.keys():
                     if validate_contains == '':
@@ -139,14 +139,15 @@
                     else:
                         if validate_contains == '':
                             validate_contains = item
                         else:
                             logger.debug(item)
                             validate_contains = validate_contains + '-' + item
             request_dict['validate']['contains'] = validate_contains
+            logger.info('已成功解析返回体')
         except KeyError as e:
             logger.debug(e)
 
     def _generate_case_dict(self, entry, test_case_dict, request_dict):
         '''
         生成用例字典的函数,将
         :param entry:
@@ -191,19 +192,18 @@
                         pass
                     else:
                         test_case_list.append(test_case_dict)
             return test_case_list
 
     def generate_yaml_case(self):
         now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
-        if self.output_file_path is None:
-            file = f"test_record_{now}.yaml"
+        if '.yaml' or '.yml' not in self.output_file_path:
+            file = self.output_file_path + f"test_record_{now}.yaml"
         else:
             file = self.output_file_path
-        logger.debug(file)
         test_case = self._generate_case_list()
         dump_yaml(test_case, file)
 
 
 if __name__ == '__main__':
     case = ParseHar('../192.168.1.117.har', '123.yaml')
     case.generate_yaml_case()
```

### Comparing `har2jicase-0.0.6/setup.py` & `har2jicase-0.0.7/setup.py`

 * *Files identical despite different names*

