# Comparing `tmp/gentrace_py-0.4.1.tar.gz` & `tmp/gentrace_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.4.1.tar", max compression
+gzip compressed data, was "gentrace_py-0.5.0.tar", max compression
```

## Comparing `gentrace_py-0.4.1.tar` & `gentrace_py-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      980 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      202 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    22973 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6318 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      980 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-20 15:35:31.486062 gentrace_py-0.5.0/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      202 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     3043 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    23469 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6318 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/gentrace/schemas.py
+-rw-r--r--   0        0        0     1298 2023-04-20 15:35:31.490062 gentrace_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.5.0/PKG-INFO
```

### Comparing `gentrace_py-0.4.1/gentrace/__init__.py` & `gentrace_py-0.5.0/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/api_client.py` & `gentrace_py-0.5.0/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/configuration.py` & `gentrace_py-0.5.0/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/exceptions.py` & `gentrace_py-0.5.0/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/feedback_request.py` & `gentrace_py-0.5.0/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/feedback_request.pyi` & `gentrace_py-0.5.0/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/feedback_response.py` & `gentrace_py-0.5.0/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/feedback_response.pyi` & `gentrace_py-0.5.0/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.5.0/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.5.0/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.5.0/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.5.0/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/models/__init__.py` & `gentrace_py-0.5.0/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.5.0/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.5.0/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/providers/getters.py` & `gentrace_py-0.5.0/gentrace/providers/getters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from typing import Any, Dict, Optional, cast
 
 from gentrace.configuration import Configuration as GentraceConfiguration
 
 
 class ProvidersGetter:
-    openai_config: Dict = {}
-
     openai_handle: Any = None
 
     def get_openai(self):
         if self.openai_handle:
             return self.openai_handle
 
         try:
             from gentrace import api_key, host
 
             from .llms.openai import OpenAIPipelineHandler
 
             gentrace_config = GentraceConfiguration(host=host)
             gentrace_config.access_token = api_key
 
-            OpenAIPipelineHandler.setup(self.openai_config)
             openai_handler = OpenAIPipelineHandler(
                 gentrace_config=gentrace_config,
-                config=self.openai_config,
             )
 
             from .llms.openai import annotate_pipeline_handler
 
             annotated_handler = annotate_pipeline_handler(
                 openai_handler, gentrace_config
             )
@@ -36,28 +32,23 @@
 
             # TODO: Could not find an easy way to create a union type with openai and
             # OpenAIPipelineHandler, so we just use openai.
             typed_cloned_handler = cast(openai, annotated_handler)
             self.openai_handle = typed_cloned_handler
             return typed_cloned_handler
         except Exception as e:
+            print(e)
             raise ImportError(
                 "Please install OpenAI as a dependency with, e.g. `pip install openai`"
             )
 
     def __getattr__(self, name):
         if name == "openai":
             return self.get_openai()
 
-    def __setattr__(self, name, value):
-        if name.startswith("openai_"):
-            self.openai_config[name[7:]] = value
-        else:
-            raise AttributeError("Invalid attribute")
-
 
 providers = ProvidersGetter()
 
 __all__ = ["providers"]
 
 # def openai(
 #     gentrace_api_key: str,
```

### Comparing `gentrace_py-0.4.1/gentrace/providers/llms/openai.py` & `gentrace_py-0.5.0/gentrace/providers/llms/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,47 @@
 from gentrace.providers.utils import to_date_string
 
 
 class OpenAIPipelineHandler:
     pipeline_run: Optional[PipelineRun] = None
     pipeline: Optional[Pipeline] = None
     gentrace_config: Dict
-    config: Dict
+    config: Dict = {}
 
-    def __init__(self, gentrace_config, config, pipeline=None, pipeline_run=None):
+    def __init__(self, gentrace_config, config=None, pipeline=None, pipeline_run=None):
         self.pipeline = pipeline
         self.pipeline_run = pipeline_run
         self.gentrace_config = gentrace_config
-        self.config = config
+        if config:
+            self.config = config
 
     @classmethod
     def setup(cls, config):
         if config:
             for key, value in config.items():
                 setattr(openai, key, value)
 
+    @property
+    def api_key(self):
+        return self.config.get("api_key")
+
+    @api_key.setter
+    def api_key(self, value):
+        self.config["api_key"] = value
+        OpenAIPipelineHandler.setup(self.config)
+
+    @property
+    def organization(self):
+        return self.config.get("organization")
+
+    @organization.setter
+    def organization(self, value):
+        self.config["organization"] = value
+        OpenAIPipelineHandler.setup(self.config)
+
     def set_pipeline_run(self, pipeline_run):
         self.pipeline_run = pipeline_run
 
 
 def create_completion_step_run(
     cls,
     pipeline_id: str,
```

### Comparing `gentrace_py-0.4.1/gentrace/providers/pipeline.py` & `gentrace_py-0.5.0/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/providers/pipeline_run.py` & `gentrace_py-0.5.0/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/providers/step_run.py` & `gentrace_py-0.5.0/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/providers/utils.py` & `gentrace_py-0.5.0/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.5.0/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/rest.py` & `gentrace_py-0.5.0/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/gentrace/schemas.py` & `gentrace_py-0.5.0/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.1/pyproject.toml` & `gentrace_py-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.4.1"
+version = "0.5.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 pydantic = ">=1.10.2"
 pystache = "^0.6.0"
 python = ">=3.8.1,<4.0"
```

### Comparing `gentrace_py-0.4.1/PKG-INFO` & `gentrace_py-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

