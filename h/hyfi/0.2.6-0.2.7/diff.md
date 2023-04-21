# Comparing `tmp/hyfi-0.2.6.tar.gz` & `tmp/hyfi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.2.6.tar", max compression
+gzip compressed data, was "hyfi-0.2.7.tar", max compression
```

## Comparing `hyfi-0.2.6.tar` & `hyfi-0.2.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-04-20 10:50:30.121958 hyfi-0.2.6/LICENSE
--rw-r--r--   0        0        0     1949 2023-04-20 10:50:30.121958 hyfi-0.2.6/README.md
--rw-r--r--   0        0        0     3902 2023-04-20 10:50:54.738227 hyfi-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/__init__.py
--rw-r--r--   0        0        0       49 2023-04-20 10:50:54.674226 hyfi-0.2.6/src/hyfi/_version.py
--rw-r--r--   0        0        0     1700 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/cli.py
--rw-r--r--   0        0        0        0 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-20 10:50:30.121958 hyfi-0.2.6/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0       21 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19380 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/env.py
--rw-r--r--   0        0        0    12911 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     5625 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26361 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/main.py
--rw-r--r--   0        0        0     2134 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/pipe.py
--rw-r--r--   0        0        0        0 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     2281 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-04-20 10:50:30.125958 hyfi-0.2.6/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 hyfi-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:13:14.628685 hyfi-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1949 2023-04-21 10:13:14.628685 hyfi-0.2.7/README.md
+-rw-r--r--   0        0        0     3902 2023-04-21 10:13:47.534383 hyfi-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1700 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      297 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-21 10:13:47.462379 hyfi-0.2.7/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19380 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/env.py
+-rw-r--r--   0        0        0    12911 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26361 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/main.py
+-rw-r--r--   0        0        0     2134 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/pipe.py
+-rw-r--r--   0        0        0      221 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-21 10:13:14.632685 hyfi-0.2.7/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     2281 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-04-21 10:13:14.636685 hyfi-0.2.7/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 hyfi-0.2.7/PKG-INFO
```

### Comparing `hyfi-0.2.6/LICENSE` & `hyfi-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/README.md` & `hyfi-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://conventionalcommits.org
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-[jupyter book]: https://hyfi.entelecheia.cc
+[jupyter book]: https://hyfi.entelecheia.ai
 
 [repo-url]: https://github.com/entelecheia/hyfi
 [pypi-url]: https://pypi.org/project/hyfi
-[docs-url]: https://hyfi.entelecheia.cc
+[docs-url]: https://hyfi.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi/blob/main/CONTRIBUTING.md
 <!-- Links: -->
 
 Hydra Fast Interface (Hydra and Pydantic based interface framework)
 
-- Documentation: [https://hyfi.entelecheia.cc][docs-url]
+- Documentation: [https://hyfi.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi][repo-url]
 - PyPI: [https://pypi.org/project/hyfi][pypi-url]
 
 HyFI is a framework for building interfaces for Python applications. It is based on [Hydra] and [Pydantic] and provides a set of tools to build interfaces for Python applications.
 
 ## Changelog
```

### Comparing `hyfi-0.2.6/pyproject.toml` & `hyfi-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.2.6"
+version = "0.2.7"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `hyfi-0.2.6/src/hyfi/cli.py` & `hyfi-0.2.7/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.2.7/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.2.7/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.2.7/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.2.7/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.2.7/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/config/batch.py` & `hyfi-0.2.7/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/env.py` & `hyfi-0.2.7/src/hyfi/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """About Configuration"""
 
     name: str = "HyFI"
     author: str = "Young Joon Lee"
     description: str = (
         "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
     )
-    homepage: str = "https://hyfi.entelecheia.cc"
+    homepage: str = "https://hyfi.entelecheia.ai"
     version: str = __version__()
 
 
 __about__ = AboutConfig()
 
 
 class DistFramwork(BaseModel):
```

### Comparing `hyfi-0.2.6/src/hyfi/hydra.py` & `hyfi-0.2.7/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/image/collage.py` & `hyfi-0.2.7/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/image/motion.py` & `hyfi-0.2.7/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/image/plot.py` & `hyfi-0.2.7/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/image/utils.py` & `hyfi-0.2.7/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/io/cached_path.py` & `hyfi-0.2.7/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/io/file.py` & `hyfi-0.2.7/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/main.py` & `hyfi-0.2.7/src/hyfi/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/pipe.py` & `hyfi-0.2.7/src/hyfi/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/batch/apply.py` & `hyfi-0.2.7/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.2.7/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/batch/batcher.py` & `hyfi-0.2.7/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/env.py` & `hyfi-0.2.7/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/func.py` & `hyfi-0.2.7/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/google.py` & `hyfi-0.2.7/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/gpu.py` & `hyfi-0.2.7/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/lib.py` & `hyfi-0.2.7/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/logging.py` & `hyfi-0.2.7/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/src/hyfi/utils/notebook.py` & `hyfi-0.2.7/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.6/PKG-INFO` & `hyfi-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.2.6
+Version: 0.2.7
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -46,26 +46,26 @@
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://conventionalcommits.org
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-[jupyter book]: https://hyfi.entelecheia.cc
+[jupyter book]: https://hyfi.entelecheia.ai
 
 [repo-url]: https://github.com/entelecheia/hyfi
 [pypi-url]: https://pypi.org/project/hyfi
-[docs-url]: https://hyfi.entelecheia.cc
+[docs-url]: https://hyfi.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi/blob/main/CONTRIBUTING.md
 <!-- Links: -->
 
 Hydra Fast Interface (Hydra and Pydantic based interface framework)
 
-- Documentation: [https://hyfi.entelecheia.cc][docs-url]
+- Documentation: [https://hyfi.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi][repo-url]
 - PyPI: [https://pypi.org/project/hyfi][pypi-url]
 
 HyFI is a framework for building interfaces for Python applications. It is based on [Hydra] and [Pydantic] and provides a set of tools to build interfaces for Python applications.
 
 ## Changelog
```

