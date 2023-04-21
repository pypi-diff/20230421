# Comparing `tmp/smartonnx-0.1.5.tar.gz` & `tmp/smartonnx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartonnx-0.1.5.tar", max compression
+gzip compressed data, was "smartonnx-0.1.6.tar", max compression
```

## Comparing `smartonnx-0.1.5.tar` & `smartonnx-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0       66 2022-04-26 06:12:40.663844 smartonnx-0.1.5/README.md
--rw-r--r--   0        0        0     1204 2022-04-26 06:12:40.663844 smartonnx-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/.DS_Store
--rw-r--r--   0        0        0        0 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/__init__.py
--rw-r--r--   0        0        0      135 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/entities/inputs.py
--rw-r--r--   0        0        0      248 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/entities/operators.py
--rw-r--r--   0        0        0      283 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/entities/tensors.py
--rw-r--r--   0        0        0     2173 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/main.py
--rw-r--r--   0        0        0     1972 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/templates/contract.cairo.tmpl
--rw-r--r--   0        0        0     1280 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/templates/tensor_loader.cairo.tmpl
--rw-r--r--   0        0        0     3147 2022-04-26 06:12:40.663844 smartonnx-0.1.5/smartonnx/utils.py
--rw-r--r--   0        0        0     1100 2022-04-26 06:13:06.840421 smartonnx-0.1.5/setup.py
--rw-r--r--   0        0        0     1035 2022-04-26 06:13:06.840770 smartonnx-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      884 2023-04-21 10:38:08.531175 smartonnx-0.1.6/README.md
+-rw-r--r--   0        0        0     1208 2023-04-21 10:38:08.531175 smartonnx-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/entities/inputs.py
+-rw-r--r--   0        0        0      248 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/entities/operators.py
+-rw-r--r--   0        0        0      283 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/entities/tensors.py
+-rw-r--r--   0        0        0     2173 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/main.py
+-rw-r--r--   0        0        0     1972 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/templates/contract.cairo.tmpl
+-rw-r--r--   0        0        0     1280 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/templates/tensor_loader.cairo.tmpl
+-rw-r--r--   0        0        0     3147 2023-04-21 10:38:08.531175 smartonnx-0.1.6/smartonnx/utils.py
+-rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 smartonnx-0.1.6/PKG-INFO
```

### Comparing `smartonnx-0.1.5/pyproject.toml` & `smartonnx-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "smartonnx"
-version = "0.1.5"
+version = "0.1.6"
 description = "Tool to convert a ONNX model to Cairo smart contract."
 readme = "README.md"
 authors = [
   "Fran Algaba <f.algaba.work@gmail.com>"
 ]
 license = "MIT"
 keywords = ["packaging", "dependency", "poetry"]
@@ -19,34 +19,34 @@
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 include = ["smartonnx/templates/*.tmpl"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.11,<3.9"
-typer = "^0.4.1"
-rich = "^12.0.1"
+typer = "^0.4.2"
+rich = "^12.6.0"
 click = "8.0.4"
 toml = "^0.10.2"
-requests = "^2.27.1"
+requests = "^2.28.2"
 cookiecutter = "^1.7.3"
-onnx = "^1.11.0"
-protobuf = "^3.20.1"
+onnx = "^1.13.1"
+protobuf = "^3.20.3"
 cogapp = "^3.3.0"
-Jinja2 = "^3.1.1"
+Jinja2 = "^3.1.2"
 
 [tool.poetry.dev-dependencies]
-darglint = "^1.5.8"
-isort = "^5.7.0"
-pyupgrade = "^2.7.4"
+darglint = "^1.8.1"
+isort = "^5.11.5"
+pyupgrade = "^2.38.4"
 black = "^20.8b1"
 mypy = "^0.790"
-bandit = "^1.7.0"
+bandit = "^1.7.5"
 safety = "^1.10.3"
-pytest = "^6.2.1"
-pylint = "^2.6.0"
+pytest = "^6.2.5"
+pylint = "^2.17.2"
 pydocstyle = "^5.1.1"
-pre-commit = "^2.9.3"
+pre-commit = "^2.21.0"
 flake8 = "^3.9.2"
 
 [tool.poetry.scripts]
 smartonnx = "smartonnx.main:app"
```

### Comparing `smartonnx-0.1.5/smartonnx/.DS_Store` & `smartonnx-0.1.6/smartonnx/.DS_Store`

 * *Files identical despite different names*

### Comparing `smartonnx-0.1.5/smartonnx/main.py` & `smartonnx-0.1.6/smartonnx/main.py`

 * *Files identical despite different names*

### Comparing `smartonnx-0.1.5/smartonnx/templates/contract.cairo.tmpl` & `smartonnx-0.1.6/smartonnx/templates/contract.cairo.tmpl`

 * *Files identical despite different names*

### Comparing `smartonnx-0.1.5/smartonnx/templates/tensor_loader.cairo.tmpl` & `smartonnx-0.1.6/smartonnx/templates/tensor_loader.cairo.tmpl`

 * *Files identical despite different names*

### Comparing `smartonnx-0.1.5/smartonnx/utils.py` & `smartonnx-0.1.6/smartonnx/utils.py`

 * *Files identical despite different names*

