# Comparing `tmp/lexikanon-0.1.0.tar.gz` & `tmp/lexikanon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.1.0.tar", max compression
+gzip compressed data, was "lexikanon-0.1.1.tar", max compression
```

## Comparing `lexikanon-0.1.0.tar` & `lexikanon-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 05:59:27.692201 lexikanon-0.1.0/LICENSE
--rw-r--r--   0        0        0     3572 2023-04-21 05:59:27.692201 lexikanon-0.1.0/README.md
--rw-r--r--   0        0        0     2978 2023-04-21 05:59:52.436465 lexikanon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-21 05:59:27.692201 lexikanon-0.1.0/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      878 2023-04-21 05:59:27.692201 lexikanon-0.1.0/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       43 2023-04-21 05:59:52.384465 lexikanon-0.1.0/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 05:59:27.692201 lexikanon-0.1.0/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 05:59:27.692201 lexikanon-0.1.0/src/lexikanon/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 05:59:27.692201 lexikanon-0.1.0/src/lexikanon/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/conf/task/__init__.yaml
--rw-r--r--   0        0        0      195 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 05:59:27.696201 lexikanon-0.1.0/src/lexikanon/py.typed
--rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 lexikanon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:56:15.486513 lexikanon-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3572 2023-04-21 10:56:15.486513 lexikanon-0.1.1/README.md
+-rw-r--r--   0        0        0     3018 2023-04-21 10:56:43.334334 lexikanon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      878 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 10:56:43.282334 lexikanon-0.1.1/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      195 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 10:56:15.486513 lexikanon-0.1.1/src/lexikanon/py.typed
+-rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 lexikanon-0.1.1/PKG-INFO
```

### Comparing `lexikanon-0.1.0/LICENSE` & `lexikanon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/README.md` & `lexikanon-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/pyproject.toml` & `lexikanon-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
@@ -89,14 +89,15 @@
 version_variable = "src/lexikanon/_version.py:__version__"
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

### Comparing `lexikanon-0.1.0/src/lexikanon/__init__.py` & `lexikanon-0.1.1/src/lexikanon/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/src/lexikanon/conf/dotenv/__init__.yaml` & `lexikanon-0.1.1/src/lexikanon/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/src/lexikanon/conf/hydra/help/help.yaml` & `lexikanon-0.1.1/src/lexikanon/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/src/lexikanon/conf/mode/__init__.yaml` & `lexikanon-0.1.1/src/lexikanon/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/src/lexikanon/conf/path/__default__.yaml` & `lexikanon-0.1.1/src/lexikanon/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/src/lexikanon/conf/path/__init__.yaml` & `lexikanon-0.1.1/src/lexikanon/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.0/PKG-INFO` & `lexikanon-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

