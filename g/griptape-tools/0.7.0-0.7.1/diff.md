# Comparing `tmp/griptape_tools-0.7.0.tar.gz` & `tmp/griptape_tools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.7.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.7.1.tar", max compression
```

## Comparing `griptape_tools-0.7.0.tar` & `griptape_tools-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.7.0/LICENSE
--rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.7.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.7.0/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.7.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.0/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.7.0/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-18 22:49:15.710526 griptape_tools-0.7.0/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1447 2023-04-16 19:44:48.773728 griptape_tools-0.7.0/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.7.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-18 22:49:15.709272 griptape_tools-0.7.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      652 2023-04-16 19:44:48.772145 griptape_tools-0.7.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.0/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.7.0/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-18 22:49:15.704485 griptape_tools-0.7.0/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     6083 2023-04-18 18:57:03.832587 griptape_tools-0.7.0/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.0/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.7.0/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-18 22:49:15.707814 griptape_tools-0.7.0/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1259 2023-04-16 19:44:48.779356 griptape_tools-0.7.0/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.0/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.7.0/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-18 22:49:15.706181 griptape_tools-0.7.0/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4437 2023-04-18 22:36:34.063641 griptape_tools-0.7.0/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.0/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.7.0/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-18 22:49:15.701853 griptape_tools-0.7.0/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2272 2023-04-16 19:44:48.776769 griptape_tools-0.7.0/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-18 22:51:48.429988 griptape_tools-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1284 2023-04-21 17:41:39.072846 griptape_tools-0.7.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.7.1/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.7.1/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.7.1/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-18 22:49:15.710526 griptape_tools-0.7.1/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1447 2023-04-16 19:44:48.773728 griptape_tools-0.7.1/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.7.1/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-18 22:49:15.709272 griptape_tools-0.7.1/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      652 2023-04-16 19:44:48.772145 griptape_tools-0.7.1/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.7.1/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-18 22:49:15.704485 griptape_tools-0.7.1/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     6073 2023-04-21 17:41:59.159404 griptape_tools-0.7.1/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.7.1/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-18 22:49:15.707814 griptape_tools-0.7.1/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1259 2023-04-16 19:44:48.779356 griptape_tools-0.7.1/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.1/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.7.1/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-18 22:49:15.706181 griptape_tools-0.7.1/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4437 2023-04-18 22:36:34.063641 griptape_tools-0.7.1/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.1/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.7.1/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-18 22:49:15.701853 griptape_tools-0.7.1/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2272 2023-04-16 19:44:48.776769 griptape_tools-0.7.1/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-21 20:55:35.986257 griptape_tools-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 griptape_tools-0.7.1/PKG-INFO
```

### Comparing `griptape_tools-0.7.0/LICENSE` & `griptape_tools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/README.md` & `griptape_tools-0.7.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Griptape Tools
+# griptape-tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_tools/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
-This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core). You can run Griptape tools in [Skatepark](https://github.com/griptape-ai/skatepark), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
+This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape). You can run Griptape tools in [griptape-flow](https://github.com/griptape-ai/griptape-flow), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
 
-- [Learn more](https://github.com/griptape-ai/griptape-core) about Griptape.
-- [Full list](https://github.com/griptape-ai/griptape-tools/tree/main/griptape/tools) of official Griptape tools.
-- [Tool details and docs](https://griptape.readthedocs.io).
+## Documentation
 
-## Contributing
+Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
-Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
+- Getting started guides. 
+- Core concepts and design overviews.
+- Examples.
+- Contribution guidelines.
 
 ## License
 
-Griptape Tools are available under the Apache 2.0 License.
+Griptape Tools are available under the Apache 2.0 License.
```

### Comparing `griptape_tools-0.7.0/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.7.1/griptape/tools/aws_cli/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/griptape/tools/calculator/tool.py` & `griptape_tools-0.7.1/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/griptape/tools/email_client/tool.py` & `griptape_tools-0.7.1/griptape/tools/email_client/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         smtp_from_email = self.env_value("SMTP_FROM_EMAIL")
 
         to_email = params["to"]
         subject = params["subject"]
         msg = MIMEText(params["body"])
 
         try:
-            if self.env_value("SMTP_USE_SSL") == "True":
+            if self.env_value("SMTP_USE_SSL"):
                 server = smtplib.SMTP_SSL(smtp_host, smtp_port)
             else:
                 server = smtplib.SMTP(smtp_host, smtp_port)
 
             msg["Subject"] = subject
             msg["From"] = smtp_from_email
             msg["To"] = to_email
```

### Comparing `griptape_tools-0.7.0/griptape/tools/sql_client/tool.py` & `griptape_tools-0.7.1/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.7.1/griptape/tools/web_scraper/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/griptape/tools/web_search/tool.py` & `griptape_tools-0.7.1/griptape/tools/web_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.0/pyproject.toml` & `griptape_tools-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.7.0"
+version = "0.7.1"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
```

### Comparing `griptape_tools-0.7.0/PKG-INFO` & `griptape_tools-0.7.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,27 +12,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: griptape-core (>=0.9.2)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
-# Griptape Tools
+# griptape-tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_tools/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
-This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core). You can run Griptape tools in [Skatepark](https://github.com/griptape-ai/skatepark), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
+This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape). You can run Griptape tools in [griptape-flow](https://github.com/griptape-ai/griptape-flow), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
 
-- [Learn more](https://github.com/griptape-ai/griptape-core) about Griptape.
-- [Full list](https://github.com/griptape-ai/griptape-tools/tree/main/griptape/tools) of official Griptape tools.
-- [Tool details and docs](https://griptape.readthedocs.io).
+## Documentation
 
-## Contributing
+Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
-Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
+- Getting started guides. 
+- Core concepts and design overviews.
+- Examples.
+- Contribution guidelines.
 
 ## License
 
 Griptape Tools are available under the Apache 2.0 License.
+
```

