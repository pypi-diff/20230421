# Comparing `tmp/scrubadubdub-0.2.0.tar.gz` & `tmp/scrubadubdub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrubadubdub-0.2.0.tar", max compression
+gzip compressed data, was "scrubadubdub-0.2.1.tar", max compression
```

## Comparing `scrubadubdub-0.2.0.tar` & `scrubadubdub-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/LICENSE
--rw-r--r--   0        0        0     2153 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/README.md
--rw-r--r--   0        0        0      544 2023-04-21 10:02:52.266377 scrubadubdub-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/cli.py
--rw-r--r--   0        0        0     1891 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/scrub.py
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 scrubadubdub-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 10:11:13.603684 scrubadubdub-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2153 2023-04-21 10:11:13.603684 scrubadubdub-0.2.1/README.md
+-rw-r--r--   0        0        0      544 2023-04-21 10:11:25.419827 scrubadubdub-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-21 10:11:13.607684 scrubadubdub-0.2.1/scrubadubdub/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-21 10:11:13.607684 scrubadubdub-0.2.1/scrubadubdub/cli.py
+-rw-r--r--   0        0        0     3757 2023-04-21 10:11:13.607684 scrubadubdub-0.2.1/scrubadubdub/scrub.py
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 scrubadubdub-0.2.1/PKG-INFO
```

### Comparing `scrubadubdub-0.2.0/LICENSE` & `scrubadubdub-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrubadubdub-0.2.0/README.md` & `scrubadubdub-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scrubadubdub-0.2.0/pyproject.toml` & `scrubadubdub-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrubadubdub"
-version = "v0.2.0"
+version = "v0.2.1"
 description = "A Python package to scrub PII"
 repository = "https://github.com/kylemclaren/scrub"
 authors = ["Kyle McLaren <kylemclaren@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `scrubadubdub-0.2.0/scrubadubdub/cli.py` & `scrubadubdub-0.2.1/scrubadubdub/cli.py`

 * *Files identical despite different names*

### Comparing `scrubadubdub-0.2.0/PKG-INFO` & `scrubadubdub-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrubadubdub
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to scrub PII
 Home-page: https://github.com/kylemclaren/scrub
 License: MIT
 Author: Kyle McLaren
 Author-email: kylemclaren@protonmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

