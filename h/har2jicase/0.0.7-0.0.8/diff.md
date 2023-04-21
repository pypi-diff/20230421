# Comparing `tmp/har2jicase-0.0.7.tar.gz` & `tmp/har2jicase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.0.7.tar", last modified: Fri Apr 21 05:30:25 2023, max compression
+gzip compressed data, was "har2jicase-0.0.8.tar", last modified: Fri Apr 21 05:42:13 2023, max compression
```

## Comparing `har2jicase-0.0.7.tar` & `har2jicase-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.787051 har2jicase-0.0.7/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:30:25.785979 har2jicase-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.775653 har2jicase-0.0.7/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      484 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 05:30:25.000000 har2jicase-0.0.7/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.7/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.782203 har2jicase-0.0.7/har_to_case/
--rw-rw-rw-   0        0        0      493 2023-04-21 05:30:17.000000 har2jicase-0.0.7/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:30:25.784974 har2jicase-0.0.7/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.7/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.7/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.7/har_to_case/main.py
--rw-rw-rw-   0        0        0     8568 2023-04-21 05:30:17.000000 har2jicase-0.0.7/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 05:30:25.787051 har2jicase-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.310704 har2jicase-0.0.8/
+-rw-rw-rw-   0        0        0      484 2023-04-21 05:42:13.310704 har2jicase-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.303709 har2jicase-0.0.8/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      484 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 05:42:13.000000 har2jicase-0.0.8/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.0.8/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.307704 har2jicase-0.0.8/har_to_case/
+-rw-rw-rw-   0        0        0      493 2023-04-21 05:42:05.000000 har2jicase-0.0.8/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:42:13.308704 har2jicase-0.0.8/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.0.8/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.0.8/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1388 2023-04-21 04:57:33.000000 har2jicase-0.0.8/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8608 2023-04-21 05:42:05.000000 har2jicase-0.0.8/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:42:13.310704 har2jicase-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2082 2023-04-21 04:28:24.000000 har2jicase-0.0.8/setup.py
```

### Comparing `har2jicase-0.0.7/har_to_case/common/tools.py` & `har2jicase-0.0.8/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.7/har_to_case/main.py` & `har2jicase-0.0.8/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.0.7/har_to_case/parse_har.py` & `har2jicase-0.0.8/har_to_case/parse_har.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class ParseHar:
     regex_resource = re.compile(r"\/[^\/?\/]*\.(css|ico|jpg|png|gif|bmp|wav|js|jpeg|woff2)(\?.*)?")
     regex_name = re.compile(r"(?<=/api\/)(.*)(?=\?)|(?<=/api\/)(.*)")
     regex_api = re.compile(r"(\/api\/.*)")
 
-    def __init__(self, har_file_path, output_file_path=None):
+    def __init__(self, har_file_path, output_file_path):
         '''
         ParseHar初始化，传入har文件路径，与输出文件路径
         :param har_file_path: har文件路径
         :param output_file_path: 输出文件路径
         '''
         with open(har_file_path, "r", encoding="utf-8") as f:
             self.har_parser = HarParser(yaml.safe_load(f))
@@ -192,18 +192,20 @@
                         pass
                     else:
                         test_case_list.append(test_case_dict)
             return test_case_list
 
     def generate_yaml_case(self):
         now = time.strftime("%Y-%m-%d-%H_%M_%S", time.localtime(time.time()))
-        if '.yaml' or '.yml' not in self.output_file_path:
-            file = self.output_file_path + f"test_record_{now}.yaml"
-        else:
+        if '.yaml' in self.output_file_path or '.yml' in self.output_file_path:
             file = self.output_file_path
+
+        else:
+            file = self.output_file_path + f"/test_record_{now}.yaml"
+        print(file)
         test_case = self._generate_case_list()
         dump_yaml(test_case, file)
 
 
 if __name__ == '__main__':
-    case = ParseHar('../192.168.1.117.har', '123.yaml')
+    case = ParseHar('../192.168.1.117.har', './common')
     case.generate_yaml_case()
```

### Comparing `har2jicase-0.0.7/setup.py` & `har2jicase-0.0.8/setup.py`

 * *Files identical despite different names*

