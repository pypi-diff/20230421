# Comparing `tmp/dfsjson-1.0.2.tar.gz` & `tmp/dfsjson-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.0.2.tar", max compression
+gzip compressed data, was "dfsjson-1.0.3.tar", max compression
```

## Comparing `dfsjson-1.0.2.tar` & `dfsjson-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.2/LICENSE
--rw-r--r--   0        0        0      971 2023-04-21 10:50:13.452366 dfsjson-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.2/dfsjson/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.2/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.2/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      442 2023-04-21 11:33:22.198700 dfsjson-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 dfsjson-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.3/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-21 10:50:13.452366 dfsjson-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.3/dfsjson/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.3/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.3/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      446 2023-04-21 11:34:53.240332 dfsjson-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 dfsjson-1.0.3/PKG-INFO
```

### Comparing `dfsjson-1.0.2/LICENSE` & `dfsjson-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.2/README.md` & `dfsjson-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.2/dfsjson/src/dfsjson.py` & `dfsjson-1.0.3/dfsjson/src/dfsjson.py`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.2/PKG-INFO` & `dfsjson-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.0.2
+Version: 1.0.3
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

