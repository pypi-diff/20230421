# Comparing `tmp/hyfi_template-0.1.6.tar.gz` & `tmp/hyfi_template-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.6.tar", max compression
+gzip compressed data, was "hyfi_template-0.1.7.tar", max compression
```

## Comparing `hyfi_template-0.1.6.tar` & `hyfi_template-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 00:42:47.602675 hyfi_template-0.1.6/LICENSE
--rw-r--r--   0        0        0     6981 2023-04-21 00:42:47.602675 hyfi_template-0.1.6/README.md
--rw-r--r--   0        0        0     3079 2023-04-21 00:43:16.566424 hyfi_template-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      882 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 00:43:16.514425 hyfi_template-0.1.6/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0      224 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7627 1970-01-01 00:00:00.000000 hyfi_template-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:55:02.049782 hyfi_template-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6988 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/README.md
+-rw-r--r--   0        0        0     3119 2023-04-21 10:55:34.926149 hyfi_template-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      882 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 10:55:34.866149 hyfi_template-0.1.7/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      224 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 10:55:02.053782 hyfi_template-0.1.7/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 hyfi_template-0.1.7/PKG-INFO
```

### Comparing `hyfi_template-0.1.6/LICENSE` & `hyfi_template-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/README.md` & `hyfi_template-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 - **Documentation**: The template repository includes clear instructions and guidelines for getting started with a HyFI-based project, helping developers quickly familiarize themselves with the framework and its features.
 
 ## Getting Started
 
 To begin using HyFI-Template for your project, simply follow these steps:
 
-1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/hyfi/hyfi-template) to create a new repository based on the template.
+1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/entelecheia/hyfi-template) to create a new repository based on the template.
 2. Clone the newly created repository to your local machine.
 3. Run `make init-project` to initialize the project with the necessary files and configurations.
 4. Follow the provided documentation and guidelines to start building your HyFI-based application.
 
 Or you can inject the template into an existing repository:
 
 1. From the root of your repository, run the following command:
```

### Comparing `hyfi_template-0.1.6/pyproject.toml` & `hyfi_template-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.6"
+version = "0.1.7"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
@@ -90,14 +90,15 @@
 version_variable = "src/hyfi_template/_version.py:__version__"
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

### Comparing `hyfi_template-0.1.6/src/hyfi_template/__init__.py` & `hyfi_template-0.1.7/src/hyfi_template/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.1.7/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.1.7/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.1.7/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.1.7/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.1.7/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.6/PKG-INFO` & `hyfi_template-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.1.6
+Version: 0.1.7
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -67,15 +67,15 @@
 
 - **Documentation**: The template repository includes clear instructions and guidelines for getting started with a HyFI-based project, helping developers quickly familiarize themselves with the framework and its features.
 
 ## Getting Started
 
 To begin using HyFI-Template for your project, simply follow these steps:
 
-1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/hyfi/hyfi-template) to create a new repository based on the template.
+1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/entelecheia/hyfi-template) to create a new repository based on the template.
 2. Clone the newly created repository to your local machine.
 3. Run `make init-project` to initialize the project with the necessary files and configurations.
 4. Follow the provided documentation and guidelines to start building your HyFI-based application.
 
 Or you can inject the template into an existing repository:
 
 1. From the root of your repository, run the following command:
```

