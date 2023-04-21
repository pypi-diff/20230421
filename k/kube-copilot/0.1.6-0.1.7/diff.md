# Comparing `tmp/kube_copilot-0.1.6.tar.gz` & `tmp/kube_copilot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_copilot-0.1.6.tar", max compression
+gzip compressed data, was "kube_copilot-0.1.7.tar", max compression
```

## Comparing `kube_copilot-0.1.6.tar` & `kube_copilot-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.6/LICENSE
--rw-r--r--   0        0        0    13659 2023-03-29 13:15:38.920561 kube_copilot-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.6/kube_copilot/__init__.py
--rw-r--r--   0        0        0     3699 2023-03-30 03:12:54.950641 kube_copilot-0.1.6/kube_copilot/agent.py
--rw-r--r--   0        0        0     2616 2023-03-29 12:41:27.907090 kube_copilot-0.1.6/kube_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 10:47:12.857795 kube_copilot-0.1.6/kube_copilot/llm.py
--rw-r--r--   0        0        0     3164 2023-03-29 13:04:38.734591 kube_copilot-0.1.6/kube_copilot/prompts.py
--rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.6/kube_copilot/shell.py
--rw-r--r--   0        0        0      699 2023-03-30 12:43:45.242841 kube_copilot-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    14393 1970-01-01 00:00:00.000000 kube_copilot-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.7/LICENSE
+-rw-r--r--   0        0        0    13659 2023-03-29 13:15:38.920561 kube_copilot-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.7/kube_copilot/__init__.py
+-rw-r--r--   0        0        0     3699 2023-03-30 03:12:54.950641 kube_copilot-0.1.7/kube_copilot/agent.py
+-rw-r--r--   0        0        0     2616 2023-03-29 12:41:27.907090 kube_copilot-0.1.7/kube_copilot/cli.py
+-rw-r--r--   0        0        0      671 2023-03-25 10:47:12.857795 kube_copilot-0.1.7/kube_copilot/llm.py
+-rw-r--r--   0        0        0     3164 2023-03-29 13:04:38.734591 kube_copilot-0.1.7/kube_copilot/prompts.py
+-rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.7/kube_copilot/shell.py
+-rw-r--r--   0        0        0      701 2023-04-21 04:55:03.325223 kube_copilot-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14395 1970-01-01 00:00:00.000000 kube_copilot-0.1.7/PKG-INFO
```

### Comparing `kube_copilot-0.1.6/LICENSE` & `kube_copilot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/README.md` & `kube_copilot-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/kube_copilot/agent.py` & `kube_copilot-0.1.7/kube_copilot/agent.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/kube_copilot/cli.py` & `kube_copilot-0.1.7/kube_copilot/cli.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/kube_copilot/llm.py` & `kube_copilot-0.1.7/kube_copilot/llm.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/kube_copilot/prompts.py` & `kube_copilot-0.1.7/kube_copilot/prompts.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/kube_copilot/shell.py` & `kube_copilot-0.1.7/kube_copilot/shell.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.6/pyproject.toml` & `kube_copilot-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "kube-copilot"
-version = "0.1.6"
+version = "0.1.7"
 description = "Kubernetes Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kube_copilot"}]
 homepage = "https://github.com/feiskyer/kube-copilot"
 repository = "https://github.com/feiskyer/kube-copilot"
 keywords = ["kubernetes", "copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 kube-copilot = 'kube_copilot.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
-langchain = ">=0.0.120"
+langchain = ">=0.0.141"
 requests = ">=2.28"
-openai = ">=0.27"
+openai = ">=0.27.4"
 tiktoken = ">=0.3.1"
-google-api-python-client = ">=2.80.0"
-click = ">=8.1.0"
+google-api-python-client = ">=2.85.0"
+click = ">=8.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kube_copilot-0.1.6/PKG-INFO` & `kube_copilot-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kube-copilot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Kubernetes Copilot
 Home-page: https://github.com/feiskyer/kube-copilot
 Keywords: kubernetes,copilot,openai,chatgpt
 Author: Pengfei Ni
 Author-email: feiskyer@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.0)
-Requires-Dist: google-api-python-client (>=2.80.0)
-Requires-Dist: langchain (>=0.0.120)
-Requires-Dist: openai (>=0.27)
+Requires-Dist: click (>=8.1.3)
+Requires-Dist: google-api-python-client (>=2.85.0)
+Requires-Dist: langchain (>=0.0.141)
+Requires-Dist: openai (>=0.27.4)
 Requires-Dist: requests (>=2.28)
 Requires-Dist: tiktoken (>=0.3.1)
 Project-URL: Repository, https://github.com/feiskyer/kube-copilot
 Description-Content-Type: text/markdown
 
 # Kubernetes Copilot
```

