# Comparing `tmp/hyfi_template-0.1.7.tar.gz` & `tmp/hyfi_template-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.7.tar", max compression
+gzip compressed data, was "hyfi_template-0.1.8.tar", max compression
```

## Comparing `hyfi_template-0.1.7.tar` & `hyfi_template-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 10:55:02.049782 hyfi_template-0.1.7/LICENSE
--rw-r--r--   0        0        0     6988 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/README.md
--rw-r--r--   0        0        0     3119 2023-04-21 10:55:34.926149 hyfi_template-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      882 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       35 2023-04-21 10:55:34.866149 hyfi_template-0.1.7/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0      224 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 hyfi_template-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 11:09:09.810350 hyfi_template-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6988 2023-04-21 11:09:09.810350 hyfi_template-0.1.8/README.md
+-rw-r--r--   0        0        0     3119 2023-04-21 11:09:42.872184 hyfi_template-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      882 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 11:09:42.808181 hyfi_template-0.1.8/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      224 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 11:09:09.814350 hyfi_template-0.1.8/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 hyfi_template-0.1.8/PKG-INFO
```

### Comparing `hyfi_template-0.1.7/LICENSE` & `hyfi_template-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/README.md` & `hyfi_template-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/pyproject.toml` & `hyfi_template-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.7"
+version = "0.1.8"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
```

### Comparing `hyfi_template-0.1.7/src/hyfi_template/__init__.py` & `hyfi_template-0.1.8/src/hyfi_template/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.1.8/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.1.8/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.1.8/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.1.8/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.1.8/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.7/PKG-INFO` & `hyfi_template-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.1.7
+Version: 0.1.8
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

