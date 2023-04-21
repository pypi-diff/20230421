# Comparing `tmp/ancv-1.3.0.tar.gz` & `tmp/ancv-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancv-1.3.0.tar", max compression
+gzip compressed data, was "ancv-1.3.1.tar", max compression
```

## Comparing `ancv-1.3.0.tar` & `ancv-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-04-21 19:53:30.294429 ancv-1.3.0/LICENSE
--rw-r--r--   0        0        0    10301 2023-04-21 19:53:30.294429 ancv-1.3.0/README.md
--rw-r--r--   0        0        0      308 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/__init__.py
--rw-r--r--   0        0        0     8719 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/__main__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/github.py
--rw-r--r--   0        0        0    13506 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/models/resume.py
--rw-r--r--   0        0        0     7803 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/showcase.resume.json
--rw-r--r--   0        0        0      932 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/data/validation.py
--rw-r--r--   0        0        0      250 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/py.typed
--rw-r--r--   0        0        0     3115 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/reflection.py
--rw-r--r--   0        0        0     1639 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/timing.py
--rw-r--r--   0        0        0      172 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/__init__.py
--rw-r--r--   0        0        0    30290 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/templates.py
--rw-r--r--   0        0        0     4199 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/themes.py
--rw-r--r--   0        0        0     2778 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/visualization/translations.py
--rw-r--r--   0        0        0        0 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/__init__.py
--rw-r--r--   0        0        0     4004 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/client.py
--rw-r--r--   0        0        0     8835 2023-04-21 19:53:30.298429 ancv-1.3.0/ancv/web/server.py
--rw-r--r--   0        0        0     2732 2023-04-21 19:53:30.306429 ancv-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    12351 1970-01-01 00:00:00.000000 ancv-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 20:08:22.234434 ancv-1.3.1/LICENSE
+-rw-r--r--   0        0        0    10301 2023-04-21 20:08:22.234434 ancv-1.3.1/README.md
+-rw-r--r--   0        0        0      308 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/__init__.py
+-rw-r--r--   0        0        0     8719 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/github.py
+-rw-r--r--   0        0        0    13506 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/resume.py
+-rw-r--r--   0        0        0     7803 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/showcase.resume.json
+-rw-r--r--   0        0        0      932 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/validation.py
+-rw-r--r--   0        0        0      250 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/py.typed
+-rw-r--r--   0        0        0     3115 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/reflection.py
+-rw-r--r--   0        0        0     1639 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/timing.py
+-rw-r--r--   0        0        0      172 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/__init__.py
+-rw-r--r--   0        0        0    30290 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/templates.py
+-rw-r--r--   0        0        0     4199 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/themes.py
+-rw-r--r--   0        0        0     2778 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/translations.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/__init__.py
+-rw-r--r--   0        0        0     4004 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/client.py
+-rw-r--r--   0        0        0     8835 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/server.py
+-rw-r--r--   0        0        0     2732 2023-04-21 20:08:22.246434 ancv-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12351 1970-01-01 00:00:00.000000 ancv-1.3.1/PKG-INFO
```

### Comparing `ancv-1.3.0/LICENSE` & `ancv-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/README.md` & `ancv-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/__main__.py` & `ancv-1.3.1/ancv/__main__.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/data/models/github.py` & `ancv-1.3.1/ancv/data/models/github.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/data/models/resume.py` & `ancv-1.3.1/ancv/data/models/resume.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/data/showcase.resume.json` & `ancv-1.3.1/ancv/data/showcase.resume.json`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/data/validation.py` & `ancv-1.3.1/ancv/data/validation.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/reflection.py` & `ancv-1.3.1/ancv/reflection.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/timing.py` & `ancv-1.3.1/ancv/timing.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/visualization/templates.py` & `ancv-1.3.1/ancv/visualization/templates.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/visualization/themes.py` & `ancv-1.3.1/ancv/visualization/themes.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/visualization/translations.py` & `ancv-1.3.1/ancv/visualization/translations.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/web/client.py` & `ancv-1.3.1/ancv/web/client.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/ancv/web/server.py` & `ancv-1.3.1/ancv/web/server.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.0/pyproject.toml` & `ancv-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ancv"
-version = "1.3.0"
+version = "1.3.1"
 description = "Renders your (JSON) resume/CV for online & pretty terminal display"
 authors = ["Alex Povel <python@alexpovel.de>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://ancv.io"
 repository = "https://github.com/alexpovel/ancv/"
 classifiers = [
```

### Comparing `ancv-1.3.0/PKG-INFO` & `ancv-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancv
-Version: 1.3.0
+Version: 1.3.1
 Summary: Renders your (JSON) resume/CV for online & pretty terminal display
 Home-page: https://ancv.io
 License: MIT
 Author: Alex Povel
 Author-email: python@alexpovel.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

