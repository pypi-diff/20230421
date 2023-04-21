# Comparing `tmp/basaran-0.16.2.tar.gz` & `tmp/basaran-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.16.2.tar", last modified: Thu Apr 20 04:37:49 2023, max compression
+gzip compressed data, was "basaran-0.17.0.tar", last modified: Fri Apr 21 04:53:42 2023, max compression
```

## Comparing `basaran-0.16.2.tar` & `basaran-0.17.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-20 04:35:16.000000 basaran-0.16.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 04:35:16.000000 basaran-0.16.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 04:37:49.184005 basaran-0.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-20 04:35:16.000000 basaran-0.16.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.180005 basaran-0.16.2/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.180005 basaran-0.16.2/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 04:37:49.184005 basaran-0.16.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 04:35:16.000000 basaran-0.16.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-20 04:35:17.000000 basaran-0.16.2/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 04:35:17.000000 basaran-0.16.2/utils/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.195028 basaran-0.17.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-21 04:51:10.000000 basaran-0.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-21 04:51:10.000000 basaran-0.17.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-21 04:53:42.195028 basaran-0.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-21 04:51:10.000000 basaran-0.17.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.191028 basaran-0.17.0/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.195028 basaran-0.17.0/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.195028 basaran-0.17.0/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/templates/default.chat.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-21 04:51:10.000000 basaran-0.17.0/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.191028 basaran-0.17.0/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-21 04:53:42.000000 basaran-0.17.0/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-21 04:53:42.000000 basaran-0.17.0/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:53:42.000000 basaran-0.17.0/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 04:53:42.000000 basaran-0.17.0/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 04:53:42.000000 basaran-0.17.0/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:53:42.195028 basaran-0.17.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-21 04:51:10.000000 basaran-0.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.195028 basaran-0.17.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-21 04:51:10.000000 basaran-0.17.0/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-21 04:51:10.000000 basaran-0.17.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-21 04:51:10.000000 basaran-0.17.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:53:42.195028 basaran-0.17.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-21 04:51:10.000000 basaran-0.17.0/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 04:51:10.000000 basaran-0.17.0/utils/render.py
```

### Comparing `basaran-0.16.2/LICENSE` & `basaran-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/PKG-INFO` & `basaran-0.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.16.2
+Version: 0.17.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.16.2/README.md` & `basaran-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/__init__.py` & `basaran-0.17.0/basaran/__init__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/__main__.py` & `basaran-0.17.0/basaran/__main__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/choice.py` & `basaran-0.17.0/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/model.py` & `basaran-0.17.0/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/static/playground.css` & `basaran-0.17.0/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/static/playground.js` & `basaran-0.17.0/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/static/presets.json` & `basaran-0.17.0/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/templates/playground.html` & `basaran-0.17.0/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran/tokenizer.py` & `basaran-0.17.0/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/basaran.egg-info/PKG-INFO` & `basaran-0.17.0/basaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.16.2
+Version: 0.17.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.16.2/setup.py` & `basaran-0.17.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.16.2"
+VERSION = "0.17.0"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
@@ -19,14 +19,15 @@
     scripts=["utils/download.py", "utils/render.py"],
     include_package_data=True,
     python_requires=">=3.8.0",
     install_requires=[
         "flask-cors",
         "flask",
         "jinja2",
+        "safetensors",
         "torch",
         "transformers",
         "waitress",
     ],
     keywords=["api", "huggingface", "nlp", "openai", "transformer"],
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `basaran-0.16.2/tests/test_choice.py` & `basaran-0.17.0/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/tests/test_model.py` & `basaran-0.17.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/tests/test_tokenizer.py` & `basaran-0.17.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.2/utils/download.py` & `basaran-0.17.0/utils/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """
 Use this script to download a model without loading it into memory.
 This allows memory-constrained CI/CD runners to build container images
 with large bundled models. See ../deployments/bundle/ for examples.
 """
+import os
 import sys
 import tempfile
 
 import huggingface_hub
 
 if len(sys.argv) < 3:
     sys.exit("usage: python download.py REPO_ID LOCAL_DIR [REVISION]")
 
+if os.getenv("TENSOR_FORMAT") == "safetensors":
+    tensor_format = "*.safetensors"
+else:
+    tensor_format = "*.bin"
+
 with tempfile.TemporaryDirectory() as cache_dir:
     huggingface_hub.snapshot_download(
         repo_id=sys.argv[1],
         local_dir=sys.argv[2],
         revision=sys.argv[3] if len(sys.argv) > 3 else None,
         cache_dir=cache_dir,
         local_dir_use_symlinks=False,
         resume_download=True,
+        allow_patterns=[tensor_format, "*.json", "*.model", "*.py"],
     )
```

### Comparing `basaran-0.16.2/utils/render.py` & `basaran-0.17.0/utils/render.py`

 * *Files identical despite different names*

