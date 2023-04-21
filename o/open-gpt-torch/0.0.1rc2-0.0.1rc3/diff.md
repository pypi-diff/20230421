# Comparing `tmp/open_gpt_torch-0.0.1rc2.tar.gz` & `tmp/open_gpt_torch-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc2.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc3.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc2.tar` & `open_gpt_torch-0.0.1rc3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10825 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/LICENSE
--rw-r--r--   0        0        0     7513 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/README.md
--rw-r--r--   0        0        0      442 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/__init__.py
--rw-r--r--   0        0        0      474 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/adapter.py
--rw-r--r--   0        0        0      503 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/executor.py
--rw-r--r--   0        0        0     2544 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/factory.py
--rw-r--r--   0        0        0      844 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/hub.py
--rw-r--r--   0        0        0      349 2023-04-21 08:38:06.166645 open_gpt_torch-0.0.1rc2/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     4994 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     5878 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     8828 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0      863 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0      445 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/hf_model.py
--rw-r--r--   0        0        0        0 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0        0 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     1077 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0     2862 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/profile.py
--rw-r--r--   0        0        0      931 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/open_gpt/serve.py
--rw-r--r--   0        0        0     1894 2023-04-21 08:38:06.170645 open_gpt_torch-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0    19730 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/LICENSE
+-rw-r--r--   0        0        0     7513 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      453 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/__init__.py
+-rw-r--r--   0        0        0      474 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/adapter.py
+-rw-r--r--   0        0        0      503 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/executor.py
+-rw-r--r--   0        0        0     2544 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/factory.py
+-rw-r--r--   0        0        0      844 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/hub.py
+-rw-r--r--   0        0        0      349 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     4994 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     5878 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     8828 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0      863 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0      445 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/hf_model.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     1077 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0     2862 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/profile.py
+-rw-r--r--   0        0        0      931 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/open_gpt/serve.py
+-rw-r--r--   0        0        0     1894 2023-04-21 08:44:23.206074 open_gpt_torch-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0    19730 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc3/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc2/LICENSE` & `open_gpt_torch-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/README.md` & `open_gpt_torch-0.0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc3/open_gpt/factory.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/helper.py` & `open_gpt_torch-0.0.1rc3/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/flan/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/models/pythia/loading.py` & `open_gpt_torch-0.0.1rc3/open_gpt/models/pythia/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc3/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/open_gpt/serve.py` & `open_gpt_torch-0.0.1rc3/open_gpt/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc2/pyproject.toml` & `open_gpt_torch-0.0.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc2"
+version = "0.0.1rc3"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
```

### Comparing `open_gpt_torch-0.0.1rc2/PKG-INFO` & `open_gpt_torch-0.0.1rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
 Requires-Python: >=3.8
```

