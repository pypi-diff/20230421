# Comparing `tmp/twot-0.0.2.tar.gz` & `tmp/twot-0.0.3.tar.gz`

## Comparing `twot-0.0.2.tar` & `twot-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 twot-0.0.2/example.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 twot-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twot-0.0.2/src/__init__.py
--rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 twot-0.0.2/src/twot.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 twot-0.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 twot-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 twot-0.0.2/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 twot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 twot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 twot-0.0.3/example.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 twot-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twot-0.0.3/twot/__init__.py
+-rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 twot-0.0.3/twot/twot.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 twot-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 twot-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 twot-0.0.3/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 twot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 twot-0.0.3/PKG-INFO
```

### Comparing `twot-0.0.2/example.py` & `twot-0.0.3/example.py`

 * *Files identical despite different names*

### Comparing `twot-0.0.2/src/twot.py` & `twot-0.0.3/twot/twot.py`

 * *Files identical despite different names*

### Comparing `twot-0.0.2/LICENSE.md` & `twot-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `twot-0.0.2/README.md` & `twot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `twot-0.0.2/pyproject.toml` & `twot-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "twot"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="gpl27", email="gpl27.dev@gmail.com" },
 ]
 description = "The Twitter Bot API - Tweet, Follow, Like, Retweet, and more with Python without using Twitter's API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twot-0.0.2/PKG-INFO` & `twot-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twot
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Twitter Bot API - Tweet, Follow, Like, Retweet, and more with Python without using Twitter's API
 Project-URL: Homepage, https://github.com/gpl27/twot
 Project-URL: Bug Tracker, https://github.com/gpl27/twot/issues
 Author-email: gpl27 <gpl27.dev@gmail.com>
 License-File: LICENSE.md
 Keywords: twitter,twitter-api,twitter-bot
 Classifier: License :: OSI Approved :: MIT License
```

