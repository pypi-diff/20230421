# Comparing `tmp/dedomenon-0.1.0.tar.gz` & `tmp/dedomenon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedomenon-0.1.0.tar", max compression
+gzip compressed data, was "dedomenon-0.1.1.tar", max compression
```

## Comparing `dedomenon-0.1.0.tar` & `dedomenon-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 06:06:05.406221 dedomenon-0.1.0/LICENSE
--rw-r--r--   0        0        0     3131 2023-04-21 06:06:05.406221 dedomenon-0.1.0/README.md
--rw-r--r--   0        0        0     2976 2023-04-21 06:06:35.705221 dedomenon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/__cli__.py
--rw-r--r--   0        0        0      878 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/__init__.py
--rw-r--r--   0        0        0       43 2023-04-21 06:06:35.645215 dedomenon-0.1.0/src/dedomenon/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 06:06:05.406221 dedomenon-0.1.0/src/dedomenon/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 06:06:05.410221 dedomenon-0.1.0/src/dedomenon/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 06:06:05.410221 dedomenon-0.1.0/src/dedomenon/conf/task/__init__.yaml
--rw-r--r--   0        0        0      193 2023-04-21 06:06:05.410221 dedomenon-0.1.0/src/dedomenon/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 06:06:05.410221 dedomenon-0.1.0/src/dedomenon/py.typed
--rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 dedomenon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:58:25.414890 dedomenon-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3131 2023-04-21 10:58:25.414890 dedomenon-0.1.1/README.md
+-rw-r--r--   0        0        0     3016 2023-04-21 10:58:51.867106 dedomenon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/__cli__.py
+-rw-r--r--   0        0        0      878 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 10:58:51.815104 dedomenon-0.1.1/src/dedomenon/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      193 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 10:58:25.414890 dedomenon-0.1.1/src/dedomenon/py.typed
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 dedomenon-0.1.1/PKG-INFO
```

### Comparing `dedomenon-0.1.0/LICENSE` & `dedomenon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/README.md` & `dedomenon-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/pyproject.toml` & `dedomenon-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dedomenon"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python Library for Datasets"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://dedomenom.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "dedomenon", from = "src" }]
 
@@ -89,14 +89,15 @@
 version_variable = "src/dedomenon/_version.py:__version__"
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

### Comparing `dedomenon-0.1.0/src/dedomenon/__init__.py` & `dedomenon-0.1.1/src/dedomenon/__init__.py`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/src/dedomenon/conf/dotenv/__init__.yaml` & `dedomenon-0.1.1/src/dedomenon/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/src/dedomenon/conf/hydra/help/help.yaml` & `dedomenon-0.1.1/src/dedomenon/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/src/dedomenon/conf/mode/__init__.yaml` & `dedomenon-0.1.1/src/dedomenon/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/src/dedomenon/conf/path/__default__.yaml` & `dedomenon-0.1.1/src/dedomenon/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/src/dedomenon/conf/path/__init__.yaml` & `dedomenon-0.1.1/src/dedomenon/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.0/PKG-INFO` & `dedomenon-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedomenon
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library for Datasets
 Home-page: https://dedomenom.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

