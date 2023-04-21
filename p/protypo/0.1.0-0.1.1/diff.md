# Comparing `tmp/protypo-0.1.0.tar.gz` & `tmp/protypo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protypo-0.1.0.tar", max compression
+gzip compressed data, was "protypo-0.1.1.tar", max compression
```

## Comparing `protypo-0.1.0.tar` & `protypo-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 05:48:33.934550 protypo-0.1.0/LICENSE
--rw-r--r--   0        0        0     3455 2023-04-21 05:48:33.934550 protypo-0.1.0/README.md
--rw-r--r--   0        0        0     2969 2023-04-21 05:48:59.807085 protypo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-04-21 05:48:33.934550 protypo-0.1.0/src/protypo/__cli__.py
--rw-r--r--   0        0        0      876 2023-04-21 05:48:33.934550 protypo-0.1.0/src/protypo/__init__.py
--rw-r--r--   0        0        0       43 2023-04-21 05:48:59.751084 protypo-0.1.0/src/protypo/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/conf/task/__init__.yaml
--rw-r--r--   0        0        0      196 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 05:48:33.938550 protypo-0.1.0/src/protypo/py.typed
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 protypo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:56:42.154103 protypo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3455 2023-04-21 10:56:42.154103 protypo-0.1.1/README.md
+-rw-r--r--   0        0        0     3009 2023-04-21 10:57:15.506271 protypo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/__cli__.py
+-rw-r--r--   0        0        0      876 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 10:57:15.442271 protypo-0.1.1/src/protypo/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 10:56:42.154103 protypo-0.1.1/src/protypo/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 10:56:42.158103 protypo-0.1.1/src/protypo/py.typed
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 protypo-0.1.1/PKG-INFO
```

### Comparing `protypo-0.1.0/LICENSE` & `protypo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/README.md` & `protypo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/pyproject.toml` & `protypo-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protypo"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python Library for Language Models"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://protypo.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "protypo", from = "src" }]
 
@@ -89,14 +89,15 @@
 version_variable = "src/protypo/_version.py:__version__"
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
+pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
```

### Comparing `protypo-0.1.0/src/protypo/__init__.py` & `protypo-0.1.1/src/protypo/__init__.py`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/src/protypo/conf/dotenv/__init__.yaml` & `protypo-0.1.1/src/protypo/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/src/protypo/conf/hydra/help/help.yaml` & `protypo-0.1.1/src/protypo/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/src/protypo/conf/mode/__init__.yaml` & `protypo-0.1.1/src/protypo/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/src/protypo/conf/path/__default__.yaml` & `protypo-0.1.1/src/protypo/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/src/protypo/conf/path/__init__.yaml` & `protypo-0.1.1/src/protypo/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `protypo-0.1.0/PKG-INFO` & `protypo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protypo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library for Language Models
 Home-page: https://protypo.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

