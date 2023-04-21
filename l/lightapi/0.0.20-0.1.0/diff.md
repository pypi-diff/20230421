# Comparing `tmp/lightapi-0.0.20.tar.gz` & `tmp/lightapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightapi-0.0.20.tar", max compression
+gzip compressed data, was "lightapi-0.1.0.tar", max compression
```

## Comparing `lightapi-0.0.20.tar` & `lightapi-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2085 2023-04-21 02:20:05.791554 lightapi-0.0.20/README.md
--rw-r--r--   0        0        0      410 2023-04-21 02:25:29.504278 lightapi-0.0.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 02:14:32.567721 lightapi-0.0.20/src/lightapi/__init__.py
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 lightapi-0.0.20/setup.py
--rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 lightapi-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0     2089 2023-04-14 23:36:28.355001 lightapi-0.1.0/README.md
+-rw-r--r--   0        0        0      340 2023-04-21 02:14:32.569717 lightapi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 02:14:32.567721 lightapi-0.1.0/src/lightapi/__init__.py
+-rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 lightapi-0.1.0/setup.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 lightapi-0.1.0/PKG-INFO
```

### Comparing `lightapi-0.0.20/README.md` & `lightapi-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-<h1 align=left><strong>Light API 0.0.19</strong></h1>
+<h1 align=center><strong>Light API 0.0.19</strong></h1>
 
-<div align=left>
+<div align=center>
  <a href="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml">
   <img src="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml/badge.svg"/> 
  </a>
 
  <a href="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template">
   <img src="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/badge.svg?token=1hiVayuLRl"/> 
  </a>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-****** Light API 0.0.19 ******
-[https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
-workflows/ci-backend.yaml/badge.svg] [https://codecov.io/gh/Aeternalis-
-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
-badge.svg?token=1hiVayuLRl] [pre-commit] [https://img.shields.io/badge/
+                        ****** Light API 0.0.19 ******
+   [https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
+    workflows/ci-backend.yaml/badge.svg] [https://codecov.io/gh/Aeternalis-
+             Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
+    badge.svg?token=1hiVayuLRl] [pre-commit] [https://img.shields.io/badge/
 code%20style-black-000000.svg] [https://img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336] [check_with_mypy]
+          %231674b1?style=flat&labelColor=ef8336] [check_with_mypy]
 ## Introduction Light Assistant powered by LightAI is an AI-powered application
-designed to help you streamline your work and free up time for more important
-tasks. It can handle a wide range of tasks, from organizing files to managing
-your email inbox, scheduling meetings, and much more. ## Installation `pip
+ designed to help you streamline your work and free up time for more important
+ tasks. It can handle a wide range of tasks, from organizing files to managing
+  your email inbox, scheduling meetings, and much more. ## Installation `pip
 install lightapi` ## Authentication To use the LightAI Assistant API, you will
 need to create an account and generate an API key. You can do this by visiting
-the [Light API](https://beta.lightapi.com) website. ## Usage ``` import
-lightapi client = lightapi.LightClient("YOUR_API_KEY_HERE") ``` ##
+    the [Light API](https://beta.lightapi.com) website. ## Usage ``` import
+      lightapi client = lightapi.LightClient("YOUR_API_KEY_HERE") ``` ##
 Documentation For a comprehensive understanding of LightAI Assistant's features
-and capabilities, visit our [Documentation](https://docs.lightapi.com).
+   and capabilities, visit our [Documentation](https://docs.lightapi.com).
```

### Comparing `lightapi-0.0.20/setup.py` & `lightapi-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,25 @@
 
 packages = \
 ['lightapi']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['aiohttp>=3.8.4,<4.0.0']
-
 setup_kwargs = {
     'name': 'lightapi',
-    'version': '0.0.20',
-    'description': "Light API turns LLM's into Autonomous, MultiModal, MultiTasking Agents.",
-    'long_description': '<h1 align=left><strong>Light API 0.0.19</strong></h1>\n\n<div align=left>\n <a href="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml">\n  <img src="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml/badge.svg"/> \n </a>\n\n <a href="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template">\n  <img src="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/badge.svg?token=1hiVayuLRl"/> \n </a>\n\n <a href="https://github.com/pre-commit/pre-commit">\n  <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit" alt="pre-commit" style="max-width:100%;">\n </a>\n\n <a href="https://github.com/psf/black">\n  <img src="https://img.shields.io/badge/code%20style-black-000000.svg">\n </a>\n\n <a href="https://pycqa.github.io/isort/">\n  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">\n </a>\n\n <a href="http://www.mypy-lang.org/static/mypy_badge.svg">\n  <img src="https://camo.githubusercontent.com/59eab954a267c6e9ff1d80e8055de43a0ad771f5e1f3779aef99d111f20bee40/687474703a2f2f7777772e6d7970792d6c616e672e6f72672f7374617469632f6d7970795f62616467652e737667" alt="check with mypy" style="max-width:100%;">\n </a>\n<br>\n\n\n## Introduction\n\nLight Assistant powered by LightAI is an AI-powered application designed to help you streamline your work and free up time for more important tasks. It can handle a wide range of tasks, from organizing files to managing your email inbox, scheduling meetings, and much more.\n\n## Installation\n\n`pip install lightapi`\n\n## Authentication\n\nTo use the LightAI Assistant API, you will need to create an account and generate an API key. You can do this by visiting the [Light API](https://beta.lightapi.com) website.\n\n## Usage\n\n```\nimport lightapi\n\nclient = lightapi.LightClient("YOUR_API_KEY_HERE")\n\n```\n## Documentation\n\nFor a comprehensive understanding of LightAI Assistant\'s features and capabilities, visit our [Documentation](https://docs.lightapi.com).\n',
+    'version': '0.1.0',
+    'description': '',
+    'long_description': '<h1 align=center><strong>Light API 0.0.19</strong></h1>\n\n<div align=center>\n <a href="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml">\n  <img src="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml/badge.svg"/> \n </a>\n\n <a href="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template">\n  <img src="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/badge.svg?token=1hiVayuLRl"/> \n </a>\n\n <a href="https://github.com/pre-commit/pre-commit">\n  <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit" alt="pre-commit" style="max-width:100%;">\n </a>\n\n <a href="https://github.com/psf/black">\n  <img src="https://img.shields.io/badge/code%20style-black-000000.svg">\n </a>\n\n <a href="https://pycqa.github.io/isort/">\n  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">\n </a>\n\n <a href="http://www.mypy-lang.org/static/mypy_badge.svg">\n  <img src="https://camo.githubusercontent.com/59eab954a267c6e9ff1d80e8055de43a0ad771f5e1f3779aef99d111f20bee40/687474703a2f2f7777772e6d7970792d6c616e672e6f72672f7374617469632f6d7970795f62616467652e737667" alt="check with mypy" style="max-width:100%;">\n </a>\n<br>\n\n\n## Introduction\n\nLight Assistant powered by LightAI is an AI-powered application designed to help you streamline your work and free up time for more important tasks. It can handle a wide range of tasks, from organizing files to managing your email inbox, scheduling meetings, and much more.\n\n## Installation\n\n`pip install lightapi`\n\n## Authentication\n\nTo use the LightAI Assistant API, you will need to create an account and generate an API key. You can do this by visiting the [Light API](https://beta.lightapi.com) website.\n\n## Usage\n\n```\nimport lightapi\n\nclient = lightapi.LightClient("YOUR_API_KEY_HERE")\n\n```\n## Documentation\n\nFor a comprehensive understanding of LightAI Assistant\'s features and capabilities, visit our [Documentation](https://docs.lightapi.com).\n',
     'author': 'Jordan Plows ',
-    'author_email': 'jordan@lightapi.com',
+    'author_email': '{ID}+{username}@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['lightapi'] package_data = \ {'': ['*']} install_requires
-= \ ['aiohttp>=3.8.4,<4.0.0'] setup_kwargs = { 'name': 'lightapi', 'version':
-'0.0.20', 'description': "Light API turns LLM's into Autonomous, MultiModal,
-MultiTasking Agents.", 'long_description': '
-****** Light API 0.0.19 ******
+'src'} packages = \ ['lightapi'] package_data = \ {'': ['*']} setup_kwargs =
+{ 'name': 'lightapi', 'version': '0.1.0', 'description': '',
+'long_description': '
+                        ****** Light API 0.0.19 ******
 \n\n
 \n \n_[https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
-workflows/ci-backend.yaml/badge.svg]_\n\n\n \n_[https://codecov.io/gh/
-Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
-badge.svg?token=1hiVayuLRl]_\n\n\n \n_[pre-commit]\n\n\n \n_[https://
-img.shields.io/badge/code%20style-black-000000.svg]\n\n\n \n_[https://
-img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336]\n\n\n \n_[check_with_mypy]\n\n
-\n\n\n## Introduction\n\nLight Assistant powered by LightAI is an AI-powered
+    workflows/ci-backend.yaml/badge.svg]_\n\n\n \n_[https://codecov.io/gh/
+       Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
+     badge.svg?token=1hiVayuLRl]_\n\n\n \n_[pre-commit]\n\n\n \n_[https://
+    img.shields.io/badge/code%20style-black-000000.svg]\n\n\n \n_[https://
+                    img.shields.io/badge/%20imports-isort-
+    %231674b1?style=flat&labelColor=ef8336]\n\n\n \n_[check_with_mypy]\n\n
+ \n\n\n## Introduction\n\nLight Assistant powered by LightAI is an AI-powered
 application designed to help you streamline your work and free up time for more
 important tasks. It can handle a wide range of tasks, from organizing files to
-managing your email inbox, scheduling meetings, and much more.\n\n##
-Installation\n\n`pip install lightapi`\n\n## Authentication\n\nTo use the
-LightAI Assistant API, you will need to create an account and generate an API
-key. You can do this by visiting the [Light API](https://beta.lightapi.com)
-website.\n\n## Usage\n\n```\nimport lightapi\n\nclient = lightapi.LightClient
-("YOUR_API_KEY_HERE")\n\n```\n## Documentation\n\nFor a comprehensive
-understanding of LightAI Assistant\'s features and capabilities, visit our
-[Documentation](https://docs.lightapi.com).\n', 'author': 'Jordan Plows ',
-'author_email': 'jordan@lightapi.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'package_dir': package_dir,
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+     managing your email inbox, scheduling meetings, and much more.\n\n##
+   Installation\n\n`pip install lightapi`\n\n## Authentication\n\nTo use the
+ LightAI Assistant API, you will need to create an account and generate an API
+  key. You can do this by visiting the [Light API](https://beta.lightapi.com)
+ website.\n\n## Usage\n\n```\nimport lightapi\n\nclient = lightapi.LightClient
+     ("YOUR_API_KEY_HERE")\n\n```\n## Documentation\n\nFor a comprehensive
+  understanding of LightAI Assistant\'s features and capabilities, visit our
+  [Documentation](https://docs.lightapi.com).\n', 'author': 'Jordan Plows ',
+   'author_email': '{ID}+{username}@users.noreply.github.com', 'maintainer':
+'None', 'maintainer_email': 'None', 'url': 'None', 'package_dir': package_dir,
+    'packages': packages, 'package_data': package_data, 'python_requires':
+                    '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `lightapi-0.0.20/PKG-INFO` & `lightapi-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: lightapi
-Version: 0.0.20
-Summary: Light API turns LLM's into Autonomous, MultiModal, MultiTasking Agents.
+Version: 0.1.0
+Summary: 
 Author: Jordan Plows 
-Author-email: jordan@lightapi.com
+Author-email: {ID}+{username}@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Description-Content-Type: text/markdown
 
-<h1 align=left><strong>Light API 0.0.19</strong></h1>
+<h1 align=center><strong>Light API 0.0.19</strong></h1>
 
-<div align=left>
+<div align=center>
  <a href="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml">
   <img src="https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/workflows/ci-backend.yaml/badge.svg"/> 
  </a>
 
  <a href="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template">
   <img src="https://codecov.io/gh/Aeternalis-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/badge.svg?token=1hiVayuLRl"/> 
  </a>
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: lightapi Version: 0.0.20 Summary: Light API turns
-LLM's into Autonomous, MultiModal, MultiTasking Agents. Author: Jordan Plows
-Author-email: jordan@lightapi.com Requires-Python: >=3.10,<4.0 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
-aiohttp (>=3.8.4,<4.0.0) Description-Content-Type: text/markdown
-****** Light API 0.0.19 ******
-[https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
-workflows/ci-backend.yaml/badge.svg] [https://codecov.io/gh/Aeternalis-
-Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
-badge.svg?token=1hiVayuLRl] [pre-commit] [https://img.shields.io/badge/
+Metadata-Version: 2.1 Name: lightapi Version: 0.1.0 Summary: Author: Jordan
+Plows Author-email: {ID}+{username}@users.noreply.github.com Requires-Python:
+>=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown
+                        ****** Light API 0.0.19 ******
+   [https://github.com/Aeternalis-Ingenium/FastAPI-Backend-Template/actions/
+    workflows/ci-backend.yaml/badge.svg] [https://codecov.io/gh/Aeternalis-
+             Ingenium/FastAPI-Backend-Template/branch/trunk/graph/
+    badge.svg?token=1hiVayuLRl] [pre-commit] [https://img.shields.io/badge/
 code%20style-black-000000.svg] [https://img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336] [check_with_mypy]
+          %231674b1?style=flat&labelColor=ef8336] [check_with_mypy]
 ## Introduction Light Assistant powered by LightAI is an AI-powered application
-designed to help you streamline your work and free up time for more important
-tasks. It can handle a wide range of tasks, from organizing files to managing
-your email inbox, scheduling meetings, and much more. ## Installation `pip
+ designed to help you streamline your work and free up time for more important
+ tasks. It can handle a wide range of tasks, from organizing files to managing
+  your email inbox, scheduling meetings, and much more. ## Installation `pip
 install lightapi` ## Authentication To use the LightAI Assistant API, you will
 need to create an account and generate an API key. You can do this by visiting
-the [Light API](https://beta.lightapi.com) website. ## Usage ``` import
-lightapi client = lightapi.LightClient("YOUR_API_KEY_HERE") ``` ##
+    the [Light API](https://beta.lightapi.com) website. ## Usage ``` import
+      lightapi client = lightapi.LightClient("YOUR_API_KEY_HERE") ``` ##
 Documentation For a comprehensive understanding of LightAI Assistant's features
-and capabilities, visit our [Documentation](https://docs.lightapi.com).
+   and capabilities, visit our [Documentation](https://docs.lightapi.com).
```

