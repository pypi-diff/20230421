# Comparing `tmp/griptape-0.4.0.tar.gz` & `tmp/griptape-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.4.0.tar", max compression
+gzip compressed data, was "griptape-0.5.0.tar", max compression
```

## Comparing `griptape-0.4.0.tar` & `griptape-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.4.0/LICENSE
--rw-r--r--   0        0        0     4198 2023-04-20 17:21:29.660292 griptape-0.4.0/README.md
--rw-r--r--   0        0        0       65 2023-04-18 23:10:38.312719 griptape-0.4.0/griptape/__init__.py
--rw-r--r--   0        0        0      529 2023-04-20 17:31:51.860438 griptape-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4951 1970-01-01 00:00:00.000000 griptape-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4198 2023-04-20 17:21:29.660292 griptape-0.5.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-18 23:10:38.312719 griptape-0.5.0/griptape/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-20 21:07:17.078072 griptape-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4951 1970-01-01 00:00:00.000000 griptape-0.5.0/PKG-INFO
```

### Comparing `griptape-0.4.0/LICENSE` & `griptape-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.4.0/README.md` & `griptape-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape-0.4.0/pyproject.toml` & `griptape-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "griptape"
-version = "0.4.0"
+version = "0.5.0"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 griptape-core = "==0.9.3"
-griptape-flow = "==0.11.0"
+griptape-flow = "==0.12.0"
 griptape-tools = "==0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `griptape-0.4.0/PKG-INFO` & `griptape-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.4.0
+Version: 0.5.0
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: griptape-core (==0.9.3)
-Requires-Dist: griptape-flow (==0.11.0)
+Requires-Dist: griptape-flow (==0.12.0)
 Requires-Dist: griptape-tools (==0.7.0)
 Project-URL: Repository, https://github.com/griptape-ai/griptape
 Description-Content-Type: text/markdown
 
 # griptape
 
 [![PyPI Version](https://img.shields.io/pypi/v/griptape.svg)](https://pypi.python.org/pypi/griptape)
```

