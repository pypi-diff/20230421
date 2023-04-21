# Comparing `tmp/pdm_conda-0.9.2b0.tar.gz` & `tmp/pdm_conda-0.9.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.2b0.tar", last modified: Fri Apr 21 18:22:20 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.2b1.tar", last modified: Fri Apr 21 18:27:35 2023, max compression
```

## Comparing `pdm_conda-0.9.2b0.tar` & `pdm_conda-0.9.2b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.2b0/LICENSE
--rw-r--r--   0        0        0     5649 2023-04-19 19:04:02.148249 pdm_conda-0.9.2b0/README.md
--rw-r--r--   0        0        0     1960 2023-04-21 18:22:20.376185 pdm_conda-0.9.2b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-21 18:22:08.358283 pdm_conda-0.9.2b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.2b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.2b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.2b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.2b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.2b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    15662 2023-04-21 18:19:33.532039 pdm_conda-0.9.2b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.2b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2613 2023-04-21 15:54:37.431271 pdm_conda-0.9.2b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2307 2023-04-19 19:04:02.152461 pdm_conda-0.9.2b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3043 2023-04-19 19:04:02.153381 pdm_conda-0.9.2b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.2b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.2b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.2b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.2b0/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8612 2023-04-19 19:04:02.155447 pdm_conda-0.9.2b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3095 2023-04-19 19:04:02.155978 pdm_conda-0.9.2b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.2b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.2b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.2b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.2b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.2b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.2b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.2b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.2b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7532 1970-01-01 00:00:00.000000 pdm_conda-0.9.2b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.2b1/LICENSE
+-rw-r--r--   0        0        0     5649 2023-04-19 19:04:02.148249 pdm_conda-0.9.2b1/README.md
+-rw-r--r--   0        0        0     1979 2023-04-21 18:27:35.124240 pdm_conda-0.9.2b1/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-21 18:27:32.161644 pdm_conda-0.9.2b1/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.2b1/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.2b1/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    15662 2023-04-21 18:19:33.532039 pdm_conda-0.9.2b1/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.2b1/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-21 15:54:37.431271 pdm_conda-0.9.2b1/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2307 2023-04-19 19:04:02.152461 pdm_conda-0.9.2b1/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3043 2023-04-19 19:04:02.153381 pdm_conda-0.9.2b1/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.2b1/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.2b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.2b1/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.2b1/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8612 2023-04-19 19:04:02.155447 pdm_conda-0.9.2b1/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3095 2023-04-19 19:04:02.155978 pdm_conda-0.9.2b1/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.2b1/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.2b1/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.2b1/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.2b1/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.2b1/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.2b1/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.2b1/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.2b1/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.2b1/PKG-INFO
```

### Comparing `pdm_conda-0.9.2b0/LICENSE` & `pdm_conda-0.9.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/README.md` & `pdm_conda-0.9.2b1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/pyproject.toml` & `pdm_conda-0.9.2b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 dynamic = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "jupyterlab>=3.6.3",
-    "pandas>=2.0.0",
-    "openpyxl>=3.1.1",
+    "pdm~=2.4.0",
+    "requests>=2.28.1",
 ]
-version = "0.9.2b0"
+version = "0.9.2b1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
 
 [project.entry-points.pdm]
 conda = "pdm_conda:main"
 
-[tool.pdm.conda]
-runner = "micromamba"
-channels = [
-    "conda-forge",
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest>=7.2.0",
+    "pytest-mock>=3.10.0",
+    "pytest-cov>=4.0.0",
+    "pytest-random-num>=1.0.13",
+    "responses>=0.22.0",
 ]
-as-default-manager = true
-batched-commands = true
 
 [tool.pdm.version]
 source = "file"
 path = "src/pdm_conda/__init__.py"
 
 [tool.pdm.build]
 package-dir = "src"
```

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/__init__.py` & `pdm_conda-0.9.2b1/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.2b0"
+__version__ = "0.9.2b1"
```

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.2b1/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/conda.py` & `pdm_conda-0.9.2b1/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.2b1/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.2b1/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/mapping.py` & `pdm_conda-0.9.2b1/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/config.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.2b1/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/project.py` & `pdm_conda-0.9.2b1/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.2b1/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.2b1/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/src/pdm_conda/utils.py` & `pdm_conda-0.9.2b1/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b0/PKG-INFO` & `pdm_conda-0.9.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.2b0
+Version: 0.9.2b1
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -27,17 +27,16 @@
         SOFTWARE.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/macro128/pdm-conda
 Project-URL: Changelog, https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md
 Requires-Python: >=3.10
-Requires-Dist: jupyterlab>=3.6.3
-Requires-Dist: pandas>=2.0.0
-Requires-Dist: openpyxl>=3.1.1
+Requires-Dist: pdm~=2.4.0
+Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 # pdm-conda
 
 A PDM plugin to resolve/install/uninstall project dependencies with Conda.
 
 ## Configuration
```

