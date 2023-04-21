# Comparing `tmp/dfsjson-1.0.4.tar.gz` & `tmp/dfsjson-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.0.4.tar", max compression
+gzip compressed data, was "dfsjson-1.0.5.tar", max compression
```

## Comparing `dfsjson-1.0.4.tar` & `dfsjson-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.4/LICENSE
--rw-r--r--   0        0        0      971 2023-04-21 10:50:13.452366 dfsjson-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.4/dfsjson/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.4/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.4/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      526 2023-04-21 11:37:57.289500 dfsjson-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 dfsjson-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.5/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.5/dfsjson/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.5/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.5/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      526 2023-04-21 11:40:25.986235 dfsjson-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 dfsjson-1.0.5/PKG-INFO
```

### Comparing `dfsjson-1.0.4/LICENSE` & `dfsjson-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.4/README.md` & `dfsjson-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     "key2": [1 2, 3]
     "key3":  {
         "subkey1": "subvalue1"
         "subkey2": "subvalue2"
     ,
 }"""
 
-rj = DFSJson(max_depth = 100, max_diff = 10)
-rj.loads(example_json)
+dj = DFSJson(max_depth = 100, max_diff = 10)
+dj.loads(example_json)
 
 ```
 
 # Discussion
 ### Hey I know this. Why not have you used Breadth First Search?
 Technically you are correct but keep in mind that Breadth First Search keeps the previous states in its list which 
 scales with number of iterations you are making and it can be a huge strain on the memory.
```

### Comparing `dfsjson-1.0.4/dfsjson/src/dfsjson.py` & `dfsjson-1.0.5/dfsjson/src/dfsjson.py`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.4/pyproject.toml` & `dfsjson-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfsjson"
-version = "1.0.4"
+version = "1.0.5"
 description = "A robust JSON encoder that fixes errors by utilizing DFS algorithm."
 authors = ["Unsal Gokdag <unsal.gokdag@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dfsjson"}]
 
 [project]
 keywords = ["JSON","JSON Serialize", "DFS", "Error correcting JSON"]
```

### Comparing `dfsjson-1.0.4/PKG-INFO` & `dfsjson-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.0.4
+Version: 1.0.5
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -31,16 +31,16 @@
     "key2": [1 2, 3]
     "key3":  {
         "subkey1": "subvalue1"
         "subkey2": "subvalue2"
     ,
 }"""
 
-rj = DFSJson(max_depth = 100, max_diff = 10)
-rj.loads(example_json)
+dj = DFSJson(max_depth = 100, max_diff = 10)
+dj.loads(example_json)
 
 ```
 
 # Discussion
 ### Hey I know this. Why not have you used Breadth First Search?
 Technically you are correct but keep in mind that Breadth First Search keeps the previous states in its list which 
 scales with number of iterations you are making and it can be a huge strain on the memory.
```

