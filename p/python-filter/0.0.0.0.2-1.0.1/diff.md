# Comparing `tmp/python-filter-0.0.0.0.2.tar.gz` & `tmp/python-filter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-filter-0.0.0.0.2.tar", last modified: Fri Mar 10 18:06:52 2023, max compression
+gzip compressed data, was "python-filter-1.0.1.tar", last modified: Fri Apr 21 00:56:49 2023, max compression
```

## Comparing `python-filter-0.0.0.0.2.tar` & `python-filter-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 18:06:52.748413 python-filter-0.0.0.0.2/
--rw-rw-rw-   0        0        0      243 2023-03-10 18:06:52.746415 python-filter-0.0.0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-10 18:06:52.725418 python-filter-0.0.0.0.2/pyfilter/
--rw-rw-rw-   0        0        0       65 2023-03-10 17:31:34.000000 python-filter-0.0.0.0.2/pyfilter/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-03-10 18:00:15.000000 python-filter-0.0.0.0.2/pyfilter/dict_list.py
-drwxrwxrwx   0        0        0        0 2023-03-10 18:06:52.744417 python-filter-0.0.0.0.2/python_filter.egg-info/
--rw-rw-rw-   0        0        0      243 2023-03-10 18:06:52.000000 python-filter-0.0.0.0.2/python_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-03-10 18:06:52.000000 python-filter-0.0.0.0.2/python_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 18:06:52.000000 python-filter-0.0.0.0.2/python_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-10 18:06:52.000000 python-filter-0.0.0.0.2/python_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-10 18:06:52.000000 python-filter-0.0.0.0.2/python_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 18:06:52.748413 python-filter-0.0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      460 2023-03-10 18:00:43.000000 python-filter-0.0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.835456 python-filter-1.0.1/
+-rw-rw-rw-   0        0        0      239 2023-04-21 00:56:49.832449 python-filter-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.800450 python-filter-1.0.1/pyfilter/
+-rw-rw-rw-   0        0        0       93 2023-04-21 00:53:22.000000 python-filter-1.0.1/pyfilter/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-04-21 00:46:51.000000 python-filter-1.0.1/pyfilter/dict_list.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:49.829451 python-filter-1.0.1/python_filter.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 00:56:49.000000 python-filter-1.0.1/python_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 00:56:49.835456 python-filter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-21 00:56:32.000000 python-filter-1.0.1/setup.py
```

### Comparing `python-filter-0.0.0.0.2/pyfilter/dict_list.py` & `python-filter-1.0.1/pyfilter/dict_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,97 @@
 from pydantic import validate_arguments
+from typing import Optional
 
 class FromDictList:
     @validate_arguments
     def __init__(self, list_: list[dict]):
         self.__list = list_
 
     @validate_arguments
-    def get_dict_if_content_key_value(self, key, value) -> dict | None:
+    def get_with_key_value(self, key, value) -> Optional[dict]:
         for x in  self.__list:
 
             if x[key] == value:
                 return x
 
     @validate_arguments
-    def get_dict_if_content_key(self, key) -> dict | None:
+    def get_with_key(self, key) -> Optional[dict]:
         for x in  self.__list:
 
             if key in x.keys():
                 return x
     
     @validate_arguments
-    def get_dicts_if_contents_key_values(self, key, values: list) -> list[dict] | list:
+    def filter_with_key_values(self, key, values: list) -> list[dict]:
         dicts = []
 
         for value in values:
             for x in self.__list:
                 if x[key] == value:
                     dicts.append(x)
 
         return dicts
 
     @validate_arguments
-    def get_dicts_if_contents_keys(self, keys: list) -> list[dict] | list:
+    def filter_with_keys(self, keys: list) -> list[dict]:
         dicts = []
 
         for key in keys:
-            for x in  self.__list:
+            for x in self.__list:
                 if key in x.keys():
                     dicts.append(x)
 
         return dicts
 
     @validate_arguments
-    def get_dicts_if_content_key_value(self, key, value) -> list[dict] | list:
-        dicts = []
-
-        for x in  self.__list:
-            if x[key] == value:
-                dicts.append(x)
-
+    def filter_with_key_value(self, key, value) -> list[dict]:
+        dicts = [ x for x in  self.__list if x[key] == value ]
         return dicts
 
     @validate_arguments
-    def get_dicts_if_content_key(self, key) -> list[dict] | list:
-        dicts = []
-
-        for x in  self.__list:
-            if key in x.keys():
-                dicts.append(x)
-
+    def filter_with_key(self, key) -> list[dict]:
+        dicts = [ x for x in  self.__list if key in x.keys() ]
         return dicts
     
     @validate_arguments
-    def for_each_dict_pop_keys(self, keys: list) -> list[dict] | list:
+    def for_each_dict_pop_keys(self, keys: list) -> list[dict]:
         new_list = []
 
-        for x in  self.__list:
+        for x in self.__list:
             for key in keys:
                 x.pop(key)
+
             new_list.append(x)
 
         return new_list
 
     @validate_arguments
-    def join_keys_of_child_dicts_in_a_new_dict(self) -> dict:
+    def merge_dicts(self) -> dict:
         new_dict = {}
 
-        for x in  self.__list:
+        for x in self.__list:
             for key in x.keys():
                 if not key in new_dict.keys():
                     new_dict[key] = x[key]
+
                 else:
                     raise Exception(f"Duplicate key: {key}")
 
         return new_dict
 
     @validate_arguments
-    def separate_dict_list_items_by_value_from_key(self, key) -> dict:
+    def categorize_dicts_by_key_value(self, key) -> dict[str, list]:
         dict_: dict[str, list] = {}
 
         for x in self.__list:
             new_key = x[key]
             
             if new_key in dict_:
                 dict_[new_key].append(x)
 
             else:
                 dict_[new_key] = []
                 dict_[new_key].append(x)
 
         return dict_
 
-__all__ = [ FromDictList ]
+__all__ = [ "FromDictList" ]
```

