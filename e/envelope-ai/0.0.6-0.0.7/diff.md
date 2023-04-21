# Comparing `tmp/envelope_ai-0.0.6.tar.gz` & `tmp/envelope_ai-0.0.7.tar.gz`

## Comparing `envelope_ai-0.0.6.tar` & `envelope_ai-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/wayfarer/__init__.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/wayfarer/wayfarer.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 envelope_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/wayfarer/__init__.py
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/wayfarer/wayfarer.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 envelope_ai-0.0.7/PKG-INFO
```

### Comparing `envelope_ai-0.0.6/wayfarer/wayfarer.py` & `envelope_ai-0.0.7/wayfarer/wayfarer.py`

 * *Files identical despite different names*

### Comparing `envelope_ai-0.0.6/LICENSE` & `envelope_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `envelope_ai-0.0.6/pyproject.toml` & `envelope_ai-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "envelope-ai"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="envelope.ai", email="support@envelope.ai"},
 ]
 description = "SDK for envelope DB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envelope_ai-0.0.6/PKG-INFO` & `envelope_ai-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envelope-ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: SDK for envelope DB
 Project-URL: Homepage, https://github.com/envelope-ai/wayfarer
 Project-URL: Bug Tracker, https://github.com/envelope-ai/wayfarer/issues
 Author-email: "envelope.ai" <support@envelope.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

