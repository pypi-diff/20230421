# Comparing `tmp/fireorm-repository-1.0.8.tar.gz` & `tmp/fireorm-repository-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireorm-repository-1.0.8.tar", max compression
+gzip compressed data, was "fireorm-repository-1.0.9.tar", max compression
```

## Comparing `fireorm-repository-1.0.8.tar` & `fireorm-repository-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2021-10-23 10:19:04.534203 fireorm-repository-1.0.8/LICENSE
--rw-r--r--   0        0        0      280 2021-11-29 07:01:20.510406 fireorm-repository-1.0.8/README.md
--rw-r--r--   0        0        0       22 2021-10-23 11:01:05.524996 fireorm-repository-1.0.8/fireorm_repository/__init__.py
--rw-r--r--   0        0        0        1 2021-10-23 10:20:16.758893 fireorm-repository-1.0.8/fireorm_repository/repositories/__init__.py
--rw-r--r--   0        0        0     1520 2021-11-10 17:06:53.239548 fireorm-repository-1.0.8/fireorm_repository/repositories/base.py
--rw-r--r--   0        0        0      695 2021-10-26 09:46:56.741506 fireorm-repository-1.0.8/fireorm_repository/repositories/interface.py
--rw-r--r--   0        0        0       45 2021-10-23 10:20:16.758893 fireorm-repository-1.0.8/fireorm_repository/types/__init__.py
--rw-r--r--   0        0        0       45 2021-10-23 10:20:16.758893 fireorm-repository-1.0.8/fireorm_repository/types/types.py
--rw-r--r--   0        0        0      991 2021-11-29 10:38:08.222452 fireorm-repository-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1122 2021-11-29 10:38:08.717555 fireorm-repository-1.0.8/setup.py
--rw-r--r--   0        0        0     1249 2021-11-29 10:38:08.717754 fireorm-repository-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-10-23 10:19:04.534203 fireorm-repository-1.0.9/LICENSE
+-rw-r--r--   0        0        0      280 2021-11-29 07:01:20.510406 fireorm-repository-1.0.9/README.md
+-rw-r--r--   0        0        0       22 2021-10-23 11:01:05.524996 fireorm-repository-1.0.9/fireorm_repository/__init__.py
+-rw-r--r--   0        0        0        1 2021-10-23 10:20:16.758893 fireorm-repository-1.0.9/fireorm_repository/repositories/__init__.py
+-rw-r--r--   0        0        0     1520 2021-11-10 17:06:53.239548 fireorm-repository-1.0.9/fireorm_repository/repositories/base.py
+-rw-r--r--   0        0        0      695 2021-10-26 09:46:56.741506 fireorm-repository-1.0.9/fireorm_repository/repositories/interface.py
+-rw-r--r--   0        0        0       45 2021-10-23 10:20:16.758893 fireorm-repository-1.0.9/fireorm_repository/types/__init__.py
+-rw-r--r--   0        0        0       45 2021-10-23 10:20:16.758893 fireorm-repository-1.0.9/fireorm_repository/types/types.py
+-rw-r--r--   0        0        0     1053 2021-11-29 10:41:54.859499 fireorm-repository-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1184 2021-11-29 10:42:03.692332 fireorm-repository-1.0.9/setup.py
+-rw-r--r--   0        0        0     1311 2021-11-29 10:42:03.692541 fireorm-repository-1.0.9/PKG-INFO
```

### Comparing `fireorm-repository-1.0.8/LICENSE` & `fireorm-repository-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fireorm-repository-1.0.8/fireorm_repository/repositories/base.py` & `fireorm-repository-1.0.9/fireorm_repository/repositories/base.py`

 * *Files identical despite different names*

### Comparing `fireorm-repository-1.0.8/fireorm_repository/repositories/interface.py` & `fireorm-repository-1.0.9/fireorm_repository/repositories/interface.py`

 * *Files identical despite different names*

### Comparing `fireorm-repository-1.0.8/pyproject.toml` & `fireorm-repository-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fireorm-repository"
-version = "1.0.8"
-description = "Layer base repository for fireorm"
+version = "1.0.9"
+description = "Базовый репозиторий для выполнения запросов к Firestore"
 authors = ["sergey <alekseyserzh88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Sergey199408081/fireorm-repository"
 repository = "https://github.com/Sergey199408081/fireorm-repository"
 keywords = ["firebase", "firestore", "fireorm", "repository"]
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fireorm-repository-1.0.8/setup.py` & `fireorm-repository-1.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 modules = \
 ['README', 'LICENSE']
 install_requires = \
 ['fireorm==0.0.14', 'python-interface==1.6.0']
 
 setup_kwargs = {
     'name': 'fireorm-repository',
-    'version': '1.0.8',
-    'description': 'Layer base repository for fireorm',
+    'version': '1.0.9',
+    'description': 'Базовый репозиторий для выполнения запросов к Firestore',
     'long_description': '# fireorm-repository\n\n# Описание\n    Базовый репозиторий для выполнения запросов к Firestore\n\n# Зависимости\n    Python, Pip\n    Файл доступа к Firestore\n\n# Установка\n    pip install fireorm-repository',
     'author': 'sergey',
     'author_email': 'alekseyserzh88@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Sergey199408081/fireorm-repository',
     'packages': packages,
```

### Comparing `fireorm-repository-1.0.8/PKG-INFO` & `fireorm-repository-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fireorm-repository
-Version: 1.0.8
-Summary: Layer base repository for fireorm
+Version: 1.0.9
+Summary: Базовый репозиторий для выполнения запросов к Firestore
 Home-page: https://github.com/Sergey199408081/fireorm-repository
 License: MIT
 Keywords: firebase,firestore,fireorm,repository
 Author: sergey
 Author-email: alekseyserzh88@gmail.com
 Requires-Python: ==3.10.0
 Classifier: Environment :: Console
```

