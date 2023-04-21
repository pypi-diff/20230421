# Comparing `tmp/squiral-0.4.0.tar.gz` & `tmp/squiral-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squiral-0.4.0.tar", max compression
+gzip compressed data, was "squiral-0.4.1.tar", max compression
```

## Comparing `squiral-0.4.0.tar` & `squiral-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-03-18 10:12:55.657942 squiral-0.4.0/LICENSE
--rw-r--r--   0        0        0     2916 2023-03-18 10:12:55.657942 squiral-0.4.0/README.md
--rw-r--r--   0        0        0      531 2023-03-18 10:12:55.657942 squiral-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      184 2023-03-18 10:12:55.657942 squiral-0.4.0/squiral/__init__.py
--rw-r--r--   0        0        0      151 2023-03-18 10:12:55.657942 squiral-0.4.0/squiral/__main__.py
--rw-r--r--   0        0        0      744 2023-03-18 10:12:55.657942 squiral-0.4.0/squiral/main.py
--rw-r--r--   0        0        0     2464 2023-03-18 10:12:55.657942 squiral-0.4.0/squiral/squiral.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 squiral-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-21 17:22:00.053933 squiral-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3056 2023-04-21 17:22:00.053933 squiral-0.4.1/README.md
+-rw-r--r--   0        0        0      531 2023-04-21 17:22:00.053933 squiral-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/__init__.py
+-rw-r--r--   0        0        0      151 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/__main__.py
+-rw-r--r--   0        0        0      744 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/main.py
+-rw-r--r--   0        0        0     2464 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/squiral.py
+-rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 squiral-0.4.1/PKG-INFO
```

### Comparing `squiral-0.4.0/LICENSE` & `squiral-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squiral-0.4.0/README.md` & `squiral-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![Downloads](https://pepy.tech/badge/squiral)](https://pepy.tech/project/squiral)
 <br/>
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sadikkuzu/squiral/main.svg)](https://results.pre-commit.ci/latest/github/sadikkuzu/squiral/main)
 [![Python lint&test](https://github.com/sadikkuzu/squiral/actions/workflows/python-package.yml/badge.svg)](https://github.com/sadikkuzu/squiral/actions/workflows/python-package.yml)
 [![Publish Python Package](https://github.com/sadikkuzu/squiral/actions/workflows/python-publish.yml/badge.svg)](https://github.com/sadikkuzu/squiral/actions/workflows/python-publish.yml)
 <br/>
 [![Sourcegraph](https://img.shields.io/badge/view%20on-Sourcegraph-brightgreen.svg?style=for-the-badge&logo=sourcegraph)](https://sourcegraph.com/github.com/sadikkuzu/squiral)
+[![codecov](https://codecov.io/gh/sadikkuzu/squiral/branch/main/graph/badge.svg?token=4KLW43HVVY)](https://codecov.io/gh/sadikkuzu/squiral)
 
 **squ**are sp**iral**
 
 ```
 Welcome to Squiral!
 Here is an example:
 21 22 23 24 25
```

### Comparing `squiral-0.4.0/pyproject.toml` & `squiral-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squiral"
-version = "0.4.0"
+version = "0.4.1"
 description = "squiral - square spiral"
 authors = ["SADIK KUZU <sadikkuzu@hotmail.com>"]
 homepage = "https://github.com/sadikkuzu/squiral"
 readme = "README.md"
 license = "MIT"
 packages = [{include = "squiral"}]
```

### Comparing `squiral-0.4.0/squiral/main.py` & `squiral-0.4.1/squiral/main.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.0/squiral/squiral.py` & `squiral-0.4.1/squiral/squiral.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.0/PKG-INFO` & `squiral-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squiral
-Version: 0.4.0
+Version: 0.4.1
 Summary: squiral - square spiral
 Home-page: https://github.com/sadikkuzu/squiral
 License: MIT
 Author: SADIK KUZU
 Author-email: sadikkuzu@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,15 @@
 [![Downloads](https://pepy.tech/badge/squiral)](https://pepy.tech/project/squiral)
 <br/>
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sadikkuzu/squiral/main.svg)](https://results.pre-commit.ci/latest/github/sadikkuzu/squiral/main)
 [![Python lint&test](https://github.com/sadikkuzu/squiral/actions/workflows/python-package.yml/badge.svg)](https://github.com/sadikkuzu/squiral/actions/workflows/python-package.yml)
 [![Publish Python Package](https://github.com/sadikkuzu/squiral/actions/workflows/python-publish.yml/badge.svg)](https://github.com/sadikkuzu/squiral/actions/workflows/python-publish.yml)
 <br/>
 [![Sourcegraph](https://img.shields.io/badge/view%20on-Sourcegraph-brightgreen.svg?style=for-the-badge&logo=sourcegraph)](https://sourcegraph.com/github.com/sadikkuzu/squiral)
+[![codecov](https://codecov.io/gh/sadikkuzu/squiral/branch/main/graph/badge.svg?token=4KLW43HVVY)](https://codecov.io/gh/sadikkuzu/squiral)
 
 **squ**are sp**iral**
 
 ```
 Welcome to Squiral!
 Here is an example:
 21 22 23 24 25
```

