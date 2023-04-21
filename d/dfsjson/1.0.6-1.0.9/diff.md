# Comparing `tmp/dfsjson-1.0.6.tar.gz` & `tmp/dfsjson-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.0.6.tar", max compression
+gzip compressed data, was "dfsjson-1.0.9.tar", max compression
```

## Comparing `dfsjson-1.0.6.tar` & `dfsjson-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.6/LICENSE
--rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.6/dfsjson/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.6/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.6/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      499 2023-04-21 11:46:15.381272 dfsjson-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 dfsjson-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.9/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.9/dfsjson/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.9/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.9/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      499 2023-04-21 13:02:41.664411 dfsjson-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 dfsjson-1.0.9/PKG-INFO
```

### Comparing `dfsjson-1.0.6/LICENSE` & `dfsjson-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.6/README.md` & `dfsjson-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.6/dfsjson/src/dfsjson.py` & `dfsjson-1.0.9/dfsjson/src/dfsjson.py`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.6/PKG-INFO` & `dfsjson-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.0.6
+Version: 1.0.9
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Home-page: https://github.com/AutomaticHourglass/dfsjson
 Keywords: JSON,JSON Serialize,DFS,Error correcting JSON
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
```

