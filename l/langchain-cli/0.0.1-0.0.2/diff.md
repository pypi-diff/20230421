# Comparing `tmp/langchain_cli-0.0.1.tar.gz` & `tmp/langchain_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cli-0.0.1.tar", max compression
+gzip compressed data, was "langchain_cli-0.0.2.tar", max compression
```

## Comparing `langchain_cli-0.0.1.tar` & `langchain_cli-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-14 14:15:06.293533 langchain_cli-0.0.1/langchain_cli/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-14 14:30:23.227665 langchain_cli-0.0.1/langchain_cli/main.py
--rw-r--r--   0        0        0     1100 2023-04-14 14:26:05.433704 langchain_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0      541 2023-04-14 14:31:43.522412 langchain_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      178 2023-04-14 14:26:05.433704 langchain_cli-0.0.1/README.md
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 langchain_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 14:15:06.293533 langchain_cli-0.0.2/langchain_cli/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-14 14:30:23.227665 langchain_cli-0.0.2/langchain_cli/main.py
+-rw-r--r--   0        0        0     1100 2023-04-14 14:26:05.433704 langchain_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0      548 2023-04-21 04:35:22.347874 langchain_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1407 2023-04-21 04:16:54.994986 langchain_cli-0.0.2/README.md
+-rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 langchain_cli-0.0.2/PKG-INFO
```

### Comparing `langchain_cli-0.0.1/langchain_cli/main.py` & `langchain_cli-0.0.2/langchain_cli/main.py`

 * *Files identical despite different names*

### Comparing `langchain_cli-0.0.1/LICENSE` & `langchain_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cli-0.0.1/pyproject.toml` & `langchain_cli-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "langchain-cli"
-version = "0.0.1"
+version = "0.0.2"
 description = "A command line interface for LangChain."
 authors = ["Rajtilak Bhattacharjee <rajtilak.blog@gmail.com>"]
 readme = "README.md"
 packages = [{include = "langchain_cli"}]
 
 [tool.poetry.scripts]
 langchain-cli = "langchain_cli.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8.1,<4.0"
 typer = {extras = ["all"], version = "^0.7.0"}
 langchain = "^0.0.139"
 openai = "^0.27.4"
 
 
 [build-system]
 requires = ["poetry-core"]
```

