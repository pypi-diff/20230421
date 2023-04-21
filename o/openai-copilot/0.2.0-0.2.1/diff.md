# Comparing `tmp/openai_copilot-0.2.0.tar.gz` & `tmp/openai_copilot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_copilot-0.2.0.tar", max compression
+gzip compressed data, was "openai_copilot-0.2.1.tar", max compression
```

## Comparing `openai_copilot-0.2.0.tar` & `openai_copilot-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.0/LICENSE
--rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.0/openai_copilot/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-10 14:19:03.562584 openai_copilot-0.2.0/openai_copilot/agent.py
--rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.0/openai_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.0/openai_copilot/llm.py
--rw-r--r--   0        0        0      672 2023-04-10 14:41:11.434065 openai_copilot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 openai_copilot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.1/openai_copilot/__init__.py
+-rw-r--r--   0        0        0     2857 2023-04-10 14:19:03.562584 openai_copilot-0.2.1/openai_copilot/agent.py
+-rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.1/openai_copilot/cli.py
+-rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.1/openai_copilot/llm.py
+-rw-r--r--   0        0        0      674 2023-04-21 04:52:05.236119 openai_copilot-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 openai_copilot-0.2.1/PKG-INFO
```

### Comparing `openai_copilot-0.2.0/LICENSE` & `openai_copilot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.0/README.md` & `openai_copilot-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.0/openai_copilot/agent.py` & `openai_copilot-0.2.1/openai_copilot/agent.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.0/openai_copilot/cli.py` & `openai_copilot-0.2.1/openai_copilot/cli.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.0/openai_copilot/llm.py` & `openai_copilot-0.2.1/openai_copilot/llm.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.0/pyproject.toml` & `openai_copilot-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "openai-copilot"
-version = "0.2.0"
+version = "0.2.1"
 description = "OpenAI Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_copilot"}]
 homepage = "https://github.com/feiskyer/openai-copilot"
 repository = "https://github.com/feiskyer/openai-copilot"
 keywords = ["copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 openai-copilot = 'openai_copilot.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
-langchain = ">=0.0.120"
+langchain = ">=0.0.141"
 requests = ">=2.28"
-openai = ">=0.27"
-google-api-python-client = ">=2.80.0"
-click = ">=8.1.0"
+openai = ">=0.27.4"
+google-api-python-client = ">=2.85.0"
+click = ">=8.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openai_copilot-0.2.0/PKG-INFO` & `openai_copilot-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openai-copilot
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenAI Copilot
 Home-page: https://github.com/feiskyer/openai-copilot
 Keywords: copilot,openai,chatgpt
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
 Project-URL: Repository, https://github.com/feiskyer/openai-copilot
 Description-Content-Type: text/markdown
 
 # OpenAI Copilot
 
 Your life Copilot powered by OpenAI (CLI interface for OpenAI with searching).
```

