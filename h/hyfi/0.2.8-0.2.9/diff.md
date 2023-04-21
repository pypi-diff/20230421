# Comparing `tmp/hyfi-0.2.8.tar.gz` & `tmp/hyfi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.2.8.tar", max compression
+gzip compressed data, was "hyfi-0.2.9.tar", max compression
```

## Comparing `hyfi-0.2.8.tar` & `hyfi-0.2.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-04-21 10:54:10.943315 hyfi-0.2.8/LICENSE
--rw-r--r--   0        0        0     1949 2023-04-21 10:54:10.943315 hyfi-0.2.8/README.md
--rw-r--r--   0        0        0     3942 2023-04-21 10:54:38.507707 hyfi-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1700 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/__init__.py
--rw-r--r--   0        0        0       36 2023-04-21 10:54:38.451707 hyfi-0.2.8/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0       21 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19380 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/env.py
--rw-r--r--   0        0        0    12911 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     5625 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26361 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/main.py
--rw-r--r--   0        0        0     2134 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/pipe.py
--rw-r--r--   0        0        0      221 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     2281 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-04-21 10:54:10.947315 hyfi-0.2.8/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 hyfi-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 11:02:36.885051 hyfi-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1949 2023-04-21 11:02:36.885051 hyfi-0.2.9/README.md
+-rw-r--r--   0        0        0     3946 2023-04-21 11:03:10.591819 hyfi-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1700 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 11:03:10.523814 hyfi-0.2.9/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19380 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/env.py
+-rw-r--r--   0        0        0    12911 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26361 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/main.py
+-rw-r--r--   0        0        0     2134 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/pipe.py
+-rw-r--r--   0        0        0      221 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/project.toml
+-rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     2281 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 hyfi-0.2.9/PKG-INFO
```

### Comparing `hyfi-0.2.8/LICENSE` & `hyfi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/README.md` & `hyfi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/pyproject.toml` & `hyfi-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.2.8"
+version = "0.2.9"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
-hyfi = 'hyfi.cli:hydra_main'
+hyfi = 'hyfi.__cli__:hydra_main'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
 pydantic = "^1.10.7"
 chardet = "<=4.0.0"
```

### Comparing `hyfi-0.2.8/src/hyfi/__cli__.py` & `hyfi-0.2.9/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.2.9/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.2.9/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.2.9/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.2.9/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.2.9/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/config/batch.py` & `hyfi-0.2.9/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/env.py` & `hyfi-0.2.9/src/hyfi/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/hydra.py` & `hyfi-0.2.9/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/image/collage.py` & `hyfi-0.2.9/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/image/motion.py` & `hyfi-0.2.9/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/image/plot.py` & `hyfi-0.2.9/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/image/utils.py` & `hyfi-0.2.9/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/io/cached_path.py` & `hyfi-0.2.9/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/io/file.py` & `hyfi-0.2.9/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/main.py` & `hyfi-0.2.9/src/hyfi/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/pipe.py` & `hyfi-0.2.9/src/hyfi/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/batch/apply.py` & `hyfi-0.2.9/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.2.9/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/batch/batcher.py` & `hyfi-0.2.9/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/env.py` & `hyfi-0.2.9/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/func.py` & `hyfi-0.2.9/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/google.py` & `hyfi-0.2.9/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/gpu.py` & `hyfi-0.2.9/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/lib.py` & `hyfi-0.2.9/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/logging.py` & `hyfi-0.2.9/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/src/hyfi/utils/notebook.py` & `hyfi-0.2.9/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.8/PKG-INFO` & `hyfi-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

