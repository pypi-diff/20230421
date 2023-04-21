# Comparing `tmp/elefantolib_fastapi-0.1.0.tar.gz` & `tmp/elefantolib_fastapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.1.0.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.1.1.tar", max compression
```

## Comparing `elefantolib_fastapi-0.1.0.tar` & `elefantolib_fastapi-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-20 13:15:24.779246 elefantolib_fastapi-0.1.0/README.md
--rw-r--r--   0        0        0       22 2023-04-20 13:09:46.994816 elefantolib_fastapi-0.1.0/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0      471 2023-04-21 09:54:08.588096 elefantolib_fastapi-0.1.0/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      821 2023-04-21 09:55:03.090879 elefantolib_fastapi-0.1.0/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      895 2023-04-21 09:37:37.454903 elefantolib_fastapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-20 13:15:24.779246 elefantolib_fastapi-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-21 10:05:57.012413 elefantolib_fastapi-0.1.1/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0      471 2023-04-21 09:54:08.588096 elefantolib_fastapi-0.1.1/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      821 2023-04-21 09:55:03.090879 elefantolib_fastapi-0.1.1/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      872 2023-04-21 10:05:53.004501 elefantolib_fastapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.1.1/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.1.0/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.1.1/elefantolib_fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.1.0/pyproject.toml` & `elefantolib_fastapi-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.95.1"
 elefantolib = "^0.8.0"
-setuptools = "^67.7.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-flake8 = "^1.1.1"
```

