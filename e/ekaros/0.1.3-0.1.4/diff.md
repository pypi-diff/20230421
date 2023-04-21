# Comparing `tmp/ekaros-0.1.3.tar.gz` & `tmp/ekaros-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.3.tar", max compression
+gzip compressed data, was "ekaros-0.1.4.tar", max compression
```

## Comparing `ekaros-0.1.3.tar` & `ekaros-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 00:46:41.206170 ekaros-0.1.3/LICENSE
--rw-r--r--   0        0        0     3345 2023-04-21 00:46:41.206170 ekaros-0.1.3/README.md
--rw-r--r--   0        0        0     2964 2023-04-21 00:47:15.582287 ekaros-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      875 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/__init__.py
--rw-r--r--   0        0        0       44 2023-04-21 00:47:15.518287 ekaros-0.1.3/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/conf/task/__init__.yaml
--rw-r--r--   0        0        0      191 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 00:46:41.210169 ekaros-0.1.3/src/ekaros/py.typed
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 ekaros-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 00:50:28.647872 ekaros-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3345 2023-04-21 00:50:28.647872 ekaros-0.1.4/README.md
+-rw-r--r--   0        0        0     2964 2023-04-21 00:51:01.404156 ekaros-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      875 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-21 00:51:01.344155 ekaros-0.1.4/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/py.typed
+-rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 ekaros-0.1.4/PKG-INFO
```

### Comparing `ekaros-0.1.3/LICENSE` & `ekaros-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/README.md` & `ekaros-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/pyproject.toml` & `ekaros-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
```

### Comparing `ekaros-0.1.3/src/ekaros/__init__.py` & `ekaros-0.1.4/src/ekaros/__init__.py`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/src/ekaros/conf/dotenv/__init__.yaml` & `ekaros-0.1.4/src/ekaros/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/src/ekaros/conf/hydra/help/help.yaml` & `ekaros-0.1.4/src/ekaros/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/src/ekaros/conf/mode/__init__.yaml` & `ekaros-0.1.4/src/ekaros/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/src/ekaros/conf/path/__default__.yaml` & `ekaros-0.1.4/src/ekaros/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/src/ekaros/conf/path/__init__.yaml` & `ekaros-0.1.4/src/ekaros/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.3/PKG-INFO` & `ekaros-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekaros
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Library for Generative AI Art
 Home-page: https://ekaros.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

