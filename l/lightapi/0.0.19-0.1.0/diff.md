# Comparing `tmp/lightapi-0.0.19.tar.gz` & `tmp/lightapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightapi-0.0.19.tar", max compression
+gzip compressed data, was "lightapi-0.1.0.tar", max compression
```

## Comparing `lightapi-0.0.19.tar` & `lightapi-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2089 2023-04-14 23:36:28.355001 lightapi-0.0.19/README.md
--rw-r--r--   0        0        0      341 2023-04-21 02:19:34.564411 lightapi-0.0.19/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 02:14:32.567721 lightapi-0.0.19/src/lightapi/__init__.py
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 lightapi-0.0.19/setup.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 lightapi-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0     2089 2023-04-14 23:36:28.355001 lightapi-0.1.0/README.md
+-rw-r--r--   0        0        0      340 2023-04-21 02:14:32.569717 lightapi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 02:14:32.567721 lightapi-0.1.0/src/lightapi/__init__.py
+-rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 lightapi-0.1.0/setup.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 lightapi-0.1.0/PKG-INFO
```

### Comparing `lightapi-0.0.19/README.md` & `lightapi-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lightapi-0.0.19/setup.py` & `lightapi-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['lightapi']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lightapi',
-    'version': '0.0.19',
+    'version': '0.1.0',
     'description': '',
     'long_description': '<h1 align=center><strong>Light API 0.0.19</strong></h1>\n\n<div align=center>\n <a href="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml">\n  <img src="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml/badge.svg"/> \n </a>\n\n <a href="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template">\n  <img src="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/badge.svg?token=1hiVayuLRl"/> \n </a>\n\n <a href="https://github.com/pre-commit/pre-commit">\n  <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit" alt="pre-commit" style="max-width:100%;">\n </a>\n\n <a href="https://github.com/psf/black">\n  <img src="https://img.shields.io/badge/code%20style-black-000000.svg">\n </a>\n\n <a href="https://pycqa.github.io/isort/">\n  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">\n </a>\n\n <a href="http://www.mypy-lang.org/static/mypy_badge.svg">\n  <img src="https://camo.githubusercontent.com/59eab954a267c6e9ff1d80e8055de43a0ad771f5e1f3779aef99d111f20bee40/687474703a2f2f7777772e6d7970792d6c616e672e6f72672f7374617469632f6d7970795f62616467652e737667" alt="check with mypy" style="max-width:100%;">\n </a>\n<br>\n\n\n## Introduction\n\nLight Assistant powered by LightAI is an AI-powered application designed to help you streamline your work and free up time for more important tasks. It can handle a wide range of tasks, from organizing files to managing your email inbox, scheduling meetings, and much more.\n\n## Installation\n\n`pip install lightapi`\n\n## Authentication\n\nTo use the LightAI Assistant API, you will need to create an account and generate an API key. You can do this by visiting the [Light API](https://beta.lightapi.com) website.\n\n## Usage\n\n```\nimport lightapi\n\nclient = lightapi.LightClient("YOUR_API_KEY_HERE")\n\n```\n## Documentation\n\nFor a comprehensive understanding of LightAI Assistant\'s features and capabilities, visit our [Documentation](https://docs.lightapi.com).\n',
     'author': 'Jordan Plows ',
     'author_email': '{ID}+{username}@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['lightapi'] package_data = \ {'': ['*']} setup_kwargs =
-{ 'name': 'lightapi', 'version': '0.0.19', 'description': '',
+{ 'name': 'lightapi', 'version': '0.1.0', 'description': '',
 'long_description': '
                         ****** Light API 0.0.19 ******
 \n\n
 \n \n_[https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
     workflows/ci-backend.yaml/badge.svg]_\n\n\n \n_[https://codecov.io/gh/
        Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
      badge.svg?token=1hiVayuLRl]_\n\n\n \n_[pre-commit]\n\n\n \n_[https://
```

### Comparing `lightapi-0.0.19/PKG-INFO` & `lightapi-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightapi
-Version: 0.0.19
+Version: 0.1.0
 Summary: 
 Author: Jordan Plows 
 Author-email: {ID}+{username}@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightapi Version: 0.0.19 Summary: Author: Jordan
+Metadata-Version: 2.1 Name: lightapi Version: 0.1.0 Summary: Author: Jordan
 Plows Author-email: {ID}+{username}@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown
                         ****** Light API 0.0.19 ******
    [https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
     workflows/ci-backend.yaml/badge.svg] [https://codecov.io/gh/Aeternalis-
```

