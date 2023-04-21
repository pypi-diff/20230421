# Comparing `tmp/talkwave-0.0.5.tar.gz` & `tmp/talkwave-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkwave-0.0.5.tar", last modified: Wed Apr 12 13:45:39 2023, max compression
+gzip compressed data, was "talkwave-0.0.6.tar", last modified: Fri Apr 21 20:59:58 2023, max compression
```

## Comparing `talkwave-0.0.5.tar` & `talkwave-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-12 13:45:29.000000 talkwave-0.0.5/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-12 13:45:29.000000 talkwave-0.0.5/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 13:45:29.000000 talkwave-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-12 13:45:39.099635 talkwave-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-12 13:45:29.000000 talkwave-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-12 13:45:29.000000 talkwave-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 13:45:39.099635 talkwave-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-12 13:45:29.000000 talkwave-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/talkwave/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/talkwave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:59:58.831947 talkwave-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-21 20:59:49.000000 talkwave-0.0.6/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 20:59:49.000000 talkwave-0.0.6/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 20:59:49.000000 talkwave-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-21 20:59:58.831947 talkwave-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-21 20:59:49.000000 talkwave-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-21 20:59:49.000000 talkwave-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-21 20:59:58.831947 talkwave-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-21 20:59:49.000000 talkwave-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:59:58.831947 talkwave-0.0.6/talkwave/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-21 20:59:49.000000 talkwave-0.0.6/talkwave/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:59:58.831947 talkwave-0.0.6/talkwave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-21 20:59:58.000000 talkwave-0.0.6/talkwave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-21 20:59:58.000000 talkwave-0.0.6/talkwave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:59:58.000000 talkwave-0.0.6/talkwave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-21 20:59:58.000000 talkwave-0.0.6/talkwave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 20:59:58.000000 talkwave-0.0.6/talkwave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:59:58.831947 talkwave-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-21 20:59:49.000000 talkwave-0.0.6/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-21 20:59:49.000000 talkwave-0.0.6/tests/test_curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-21 20:59:49.000000 talkwave-0.0.6/tests/test_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-21 20:59:49.000000 talkwave-0.0.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-21 20:59:49.000000 talkwave-0.0.6/tests/test_main.py
```

### Comparing `talkwave-0.0.5/LICENSE-APACHE` & `talkwave-0.0.6/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/LICENSE-MIT` & `talkwave-0.0.6/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/PKG-INFO` & `talkwave-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.5
+Version: 0.0.6
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
@@ -21,21 +21,21 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 <!-- markdownlint-disable MD033 MD041 -->
 
-<img src="https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/icon/ico-talkwave.svg" alt="talkwave logo" width="261" align="right" />
+<img src="https://kura.pro/talkwave/images/logos/talkwave.svg" alt="talkwave logo" width="261" align="right" />
 
 <!-- markdownlint-enable MD033 MD041 -->
 
 # Python TalkWave
 
-![talkwave banner](https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/title/title-talkwave.svg)
+![talkwave banner](https://kura.pro/talkwave/images/titles/title-talkwave.svg)
 
 ## Overview 📖
 
 TalkWave is an AI chatbot for developers written in Python. It features
 a simple HTML frontend and is designed to be accessible across various
 browsers and devices. TalkWave supports asynchronous operations and can
 handle multiple requests simultaneously.
```

### Comparing `talkwave-0.0.5/README.md` & `talkwave-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!-- markdownlint-disable MD033 MD041 -->
 
-<img src="https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/icon/ico-talkwave.svg" alt="talkwave logo" width="261" align="right" />
+<img src="https://kura.pro/talkwave/images/logos/talkwave.svg" alt="talkwave logo" width="261" align="right" />
 
 <!-- markdownlint-enable MD033 MD041 -->
 
 # Python TalkWave
 
-![talkwave banner](https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/title/title-talkwave.svg)
+![talkwave banner](https://kura.pro/talkwave/images/titles/title-talkwave.svg)
 
 ## Overview 📖
 
 TalkWave is an AI chatbot for developers written in Python. It features
 a simple HTML frontend and is designed to be accessible across various
 browsers and devices. TalkWave supports asynchronous operations and can
 handle multiple requests simultaneously.
```

### Comparing `talkwave-0.0.5/pyproject.toml` & `talkwave-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkwave"
-version = "0.0.5"
+version = "0.0.6"
 description = "TalkWave is an AI chatbot for developers written in Python."
 authors = ["Sebastien Rousseau <sebastian.rousseau at gmail.com>"]
 license = "Apache Software License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `talkwave-0.0.5/setup.cfg` & `talkwave-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = talkwave
-version = 0.0.5
+version = 0.0.6
 author = Sebastian Rousseau
 author_email = sebastian.rousseau@gmail.com
 description = TalkWave is an AI chatbot for developers written in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sebastienrousseau/talkwave
 license = Apache Software License
```

### Comparing `talkwave-0.0.5/setup.py` & `talkwave-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 TEST_DEPENDENCIES = [
     "coverage>=7.2.3",
     "pytest-cov>=4.0.0",
     "pytest>=7.3.0",
 ]
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 URL = 'https://github.com/sebastienrousseau/talkwave'
 
 setup(
     name='talkwave',
     version=VERSION,
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

### Comparing `talkwave-0.0.5/talkwave/__init__.py` & `talkwave-0.0.6/talkwave/__init__.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave/__main__.py` & `talkwave-0.0.6/talkwave/__main__.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave/__version__.py` & `talkwave-0.0.6/talkwave/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 __logo__ = (
     "https://raw.githubusercontent.com/"
     "sebastienrousseau/vault/main/assets/"
     "talkwave/icon/ico-talkwave.svg"
 )
 __title__ = "TalkWave 🐍"
 __url__ = "https://talkwave.co/"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

### Comparing `talkwave-0.0.5/talkwave/core.py` & `talkwave-0.0.6/talkwave/core.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave/curl.py` & `talkwave-0.0.6/talkwave/curl.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave/frontend.py` & `talkwave-0.0.6/talkwave/frontend.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave/parse.py` & `talkwave-0.0.6/talkwave/parse.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/talkwave.egg-info/PKG-INFO` & `talkwave-0.0.6/talkwave.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.5
+Version: 0.0.6
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
@@ -21,21 +21,21 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 <!-- markdownlint-disable MD033 MD041 -->
 
-<img src="https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/icon/ico-talkwave.svg" alt="talkwave logo" width="261" align="right" />
+<img src="https://kura.pro/talkwave/images/logos/talkwave.svg" alt="talkwave logo" width="261" align="right" />
 
 <!-- markdownlint-enable MD033 MD041 -->
 
 # Python TalkWave
 
-![talkwave banner](https://raw.githubusercontent.com/sebastienrousseau/vault/main/assets/talkwave/title/title-talkwave.svg)
+![talkwave banner](https://kura.pro/talkwave/images/titles/title-talkwave.svg)
 
 ## Overview 📖
 
 TalkWave is an AI chatbot for developers written in Python. It features
 a simple HTML frontend and is designed to be accessible across various
 browsers and devices. TalkWave supports asynchronous operations and can
 handle multiple requests simultaneously.
```

### Comparing `talkwave-0.0.5/tests/test_core.py` & `talkwave-0.0.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/tests/test_curl.py` & `talkwave-0.0.6/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/tests/test_dir.py` & `talkwave-0.0.6/tests/test_dir.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/tests/test_init.py` & `talkwave-0.0.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.5/tests/test_main.py` & `talkwave-0.0.6/tests/test_main.py`

 * *Files identical despite different names*

