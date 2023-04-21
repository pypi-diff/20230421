# Comparing `tmp/windeurope72hours-0.1.2.tar.gz` & `tmp/windeurope72hours-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windeurope72hours-0.1.2.tar", max compression
+gzip compressed data, was "windeurope72hours-0.1.3.tar", max compression
```

## Comparing `windeurope72hours-0.1.2.tar` & `windeurope72hours-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-21 18:58:45.256774 windeurope72hours-0.1.2/LICENSE
--rw-r--r--   0        0        0     6230 2023-04-21 18:58:45.256774 windeurope72hours-0.1.2/README.md
--rw-r--r--   0        0        0      210 2023-04-21 18:58:45.256774 windeurope72hours-0.1.2/elevations_client/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-21 18:58:45.256774 windeurope72hours-0.1.2/elevations_client/client.py
--rw-r--r--   0        0        0      447 2023-04-21 18:58:45.256774 windeurope72hours-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 windeurope72hours-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 19:08:34.713014 windeurope72hours-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6230 2023-04-21 19:08:34.713014 windeurope72hours-0.1.3/README.md
+-rw-r--r--   0        0        0      447 2023-04-21 19:08:34.717014 windeurope72hours-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-04-21 19:08:34.717014 windeurope72hours-0.1.3/windeurope72hours/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-21 19:08:34.717014 windeurope72hours-0.1.3/windeurope72hours/client.py
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 windeurope72hours-0.1.3/PKG-INFO
```

### Comparing `windeurope72hours-0.1.2/LICENSE` & `windeurope72hours-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `windeurope72hours-0.1.2/README.md` & `windeurope72hours-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `windeurope72hours-0.1.2/elevations_client/client.py` & `windeurope72hours-0.1.3/windeurope72hours/client.py`

 * *Files identical despite different names*

### Comparing `windeurope72hours-0.1.2/PKG-INFO` & `windeurope72hours-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windeurope72hours
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Marcus Lugg
 Author-email: marcus@octue.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

