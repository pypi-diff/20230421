# Comparing `tmp/hyfi_template-0.1.5.tar.gz` & `tmp/hyfi_template-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.5.tar", max compression
+gzip compressed data, was "hyfi_template-0.1.6.tar", max compression
```

## Comparing `hyfi_template-0.1.5.tar` & `hyfi_template-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-20 11:54:54.607942 hyfi_template-0.1.5/LICENSE
--rw-r--r--   0        0        0     6602 2023-04-20 11:54:54.607942 hyfi_template-0.1.5/README.md
--rw-r--r--   0        0        0     3086 2023-04-20 11:55:24.780315 hyfi_template-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      882 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-20 11:55:24.728315 hyfi_template-0.1.5/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/project.toml
--rw-r--r--   0        0        0        0 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 hyfi_template-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 00:42:47.602675 hyfi_template-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6981 2023-04-21 00:42:47.602675 hyfi_template-0.1.6/README.md
+-rw-r--r--   0        0        0     3079 2023-04-21 00:43:16.566424 hyfi_template-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      882 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-21 00:43:16.514425 hyfi_template-0.1.6/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      224 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 00:42:47.606675 hyfi_template-0.1.6/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     7627 1970-01-01 00:00:00.000000 hyfi_template-0.1.6/PKG-INFO
```

### Comparing `hyfi_template-0.1.5/LICENSE` & `hyfi_template-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/README.md` & `hyfi_template-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 [![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
 
-[pypi-image]: https://badge.fury.io/py/hyfi-template.svg
+[pypi-image]: https://img.shields.io/pypi/v/hyfi-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-template
 [license-url]: https://github.com/entelecheia/hyfi-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-template
 [release-url]: https://github.com/entelecheia/hyfi-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 [repo-url]: https://github.com/entelecheia/hyfi-template
 [pypi-url]: https://pypi.org/project/hyfi-template
-[docs-url]: https://entelecheia.github.io/hyfi-template
+[docs-url]: https://hyfi-template.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi-template/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
 A GitHub Template Repository for HyFI-based Projects
 
-- Documentation: [https://entelecheia.github.io/hyfi-template][docs-url]
+- Documentation: [https://hyfi-template.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi-template][repo-url]
 - PyPI: [https://pypi.org/project/hyfi-template][pypi-url]
 
 HyFI-Template is a ready-to-use GitHub template repository designed to streamline the process of initializing new projects based on HyFI, a robust framework for building interfaces for Python applications. HyFI leverages the power of the Hydra configuration system and the Pydantic data validation library, offering a comprehensive set of tools to create flexible and adaptable interfaces for various Python projects.
 
 ## Features
 
@@ -54,14 +54,24 @@
 To begin using HyFI-Template for your project, simply follow these steps:
 
 1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/hyfi/hyfi-template) to create a new repository based on the template.
 2. Clone the newly created repository to your local machine.
 3. Run `make init-project` to initialize the project with the necessary files and configurations.
 4. Follow the provided documentation and guidelines to start building your HyFI-based application.
 
+Or you can inject the template into an existing repository:
+
+1. From the root of your repository, run the following command:
+
+   ```bash
+   copier --data 'code_template_source=gh:entelecheia/hyfi-template' --answers-file .copier-config.yaml gh:entelecheia/hyperfast-python-template .
+   ```
+
+2. Follow the provided documentation and guidelines to start building your HyFI-based application.
+
 By using HyFI-Template as the foundation for your project, you'll be well on your way to creating powerful and adaptable interfaces for your Python applications.
 
 ## Managing Actions Secrets and Variables in Your Project
 
 When using the HyFI-Template for your project, there are several GitHub Actions secrets and variables that you need to add to ensure proper functioning of the release action and optional JupyterBook deployment.
 
 ### Adding PYPI_API_TOKEN and TEST_PYPI_API_TOKEN
```

### Comparing `hyfi_template-0.1.5/pyproject.toml` & `hyfi_template-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.5"
+version = "0.1.6"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
-homepage = "https://entelecheia.github.io/hyfi-template"
+homepage = "https://hyfi-template.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
```

### Comparing `hyfi_template-0.1.5/src/hyfi_template/__init__.py` & `hyfi_template-0.1.6/src/hyfi_template/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.1.6/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.1.6/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.1.6/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.1.6/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.1.6/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.5/PKG-INFO` & `hyfi_template-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.1.5
+Version: 0.1.6
 Summary: A GitHub Template Repository for HyFI-based Projects
-Home-page: https://entelecheia.github.io/hyfi-template
+Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,32 +22,32 @@
 [![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
 
-[pypi-image]: https://badge.fury.io/py/hyfi-template.svg
+[pypi-image]: https://img.shields.io/pypi/v/hyfi-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-template
 [license-url]: https://github.com/entelecheia/hyfi-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-template
 [release-url]: https://github.com/entelecheia/hyfi-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 [repo-url]: https://github.com/entelecheia/hyfi-template
 [pypi-url]: https://pypi.org/project/hyfi-template
-[docs-url]: https://entelecheia.github.io/hyfi-template
+[docs-url]: https://hyfi-template.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi-template/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
 A GitHub Template Repository for HyFI-based Projects
 
-- Documentation: [https://entelecheia.github.io/hyfi-template][docs-url]
+- Documentation: [https://hyfi-template.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi-template][repo-url]
 - PyPI: [https://pypi.org/project/hyfi-template][pypi-url]
 
 HyFI-Template is a ready-to-use GitHub template repository designed to streamline the process of initializing new projects based on HyFI, a robust framework for building interfaces for Python applications. HyFI leverages the power of the Hydra configuration system and the Pydantic data validation library, offering a comprehensive set of tools to create flexible and adaptable interfaces for various Python projects.
 
 ## Features
 
@@ -72,14 +72,24 @@
 To begin using HyFI-Template for your project, simply follow these steps:
 
 1. Click the "Use this template" button on the [HyFI-Template GitHub repository](https://github.com/hyfi/hyfi-template) to create a new repository based on the template.
 2. Clone the newly created repository to your local machine.
 3. Run `make init-project` to initialize the project with the necessary files and configurations.
 4. Follow the provided documentation and guidelines to start building your HyFI-based application.
 
+Or you can inject the template into an existing repository:
+
+1. From the root of your repository, run the following command:
+
+   ```bash
+   copier --data 'code_template_source=gh:entelecheia/hyfi-template' --answers-file .copier-config.yaml gh:entelecheia/hyperfast-python-template .
+   ```
+
+2. Follow the provided documentation and guidelines to start building your HyFI-based application.
+
 By using HyFI-Template as the foundation for your project, you'll be well on your way to creating powerful and adaptable interfaces for your Python applications.
 
 ## Managing Actions Secrets and Variables in Your Project
 
 When using the HyFI-Template for your project, there are several GitHub Actions secrets and variables that you need to add to ensure proper functioning of the release action and optional JupyterBook deployment.
 
 ### Adding PYPI_API_TOKEN and TEST_PYPI_API_TOKEN
```

