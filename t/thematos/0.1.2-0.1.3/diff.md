# Comparing `tmp/thematos-0.1.2.tar.gz` & `tmp/thematos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thematos-0.1.2.tar", max compression
+gzip compressed data, was "thematos-0.1.3.tar", max compression
```

## Comparing `thematos-0.1.2.tar` & `thematos-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 10:57:16.873641 thematos-0.1.2/LICENSE
--rw-r--r--   0        0        0     3479 2023-04-21 10:57:16.873641 thematos-0.1.2/README.md
--rw-r--r--   0        0        0     3015 2023-04-21 10:57:44.633661 thematos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      176 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/__cli__.py
--rw-r--r--   0        0        0      877 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/__init__.py
--rw-r--r--   0        0        0       35 2023-04-21 10:57:44.581661 thematos-0.1.2/src/thematos/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/conf/task/__init__.yaml
--rw-r--r--   0        0        0      197 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 10:57:16.873641 thematos-0.1.2/src/thematos/py.typed
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 thematos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 11:37:07.054945 thematos-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3479 2023-04-21 11:37:07.054945 thematos-0.1.3/README.md
+-rw-r--r--   0        0        0     2977 2023-04-21 11:37:42.020224 thematos-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/__cli__.py
+-rw-r--r--   0        0        0      877 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-21 11:37:41.964222 thematos-0.1.3/src/thematos/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      197 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/py.typed
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 thematos-0.1.3/PKG-INFO
```

### Comparing `thematos-0.1.2/LICENSE` & `thematos-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/README.md` & `thematos-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/pyproject.toml` & `thematos-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thematos"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python Library for Topic Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://thematos.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "thematos", from = "src" }]
 
@@ -75,15 +75,14 @@
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "1.0.1"
 tag_format = "v$version"
 
 [tool.setuptools_scm]
-write_to = "src/thematos/_version.py"
 write_to_template = '__version__ = "{version}"'
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/thematos/_version.py:__version__"
```

### Comparing `thematos-0.1.2/src/thematos/__init__.py` & `thematos-0.1.3/src/thematos/__init__.py`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/src/thematos/conf/dotenv/__init__.yaml` & `thematos-0.1.3/src/thematos/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/src/thematos/conf/hydra/help/help.yaml` & `thematos-0.1.3/src/thematos/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/src/thematos/conf/mode/__init__.yaml` & `thematos-0.1.3/src/thematos/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/src/thematos/conf/path/__default__.yaml` & `thematos-0.1.3/src/thematos/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/src/thematos/conf/path/__init__.yaml` & `thematos-0.1.3/src/thematos/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.2/PKG-INFO` & `thematos-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thematos
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python Library for Topic Modeling
 Home-page: https://thematos.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

