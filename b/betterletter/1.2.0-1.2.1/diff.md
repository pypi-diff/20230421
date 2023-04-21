# Comparing `tmp/betterletter-1.2.0.tar.gz` & `tmp/betterletter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterletter-1.2.0.tar", max compression
+gzip compressed data, was "betterletter-1.2.1.tar", max compression
```

## Comparing `betterletter-1.2.0.tar` & `betterletter-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-03-18 14:16:45.172134 betterletter-1.2.0/LICENSE
--rw-r--r--   0        0        0     9466 2023-03-18 14:16:45.172134 betterletter-1.2.0/README.md
--rw-r--r--   0        0        0     3093 2023-03-18 14:16:45.172134 betterletter-1.2.0/betterletter/__init__.py
--rw-r--r--   0        0        0     6435 2023-03-18 14:16:45.172134 betterletter-1.2.0/betterletter/__main__.py
--rw-r--r--   0        0        0     1721 2023-03-18 14:16:45.172134 betterletter-1.2.0/betterletter/io.py
--rw-r--r--   0        0        0     3111 2023-03-18 14:16:45.172134 betterletter-1.2.0/betterletter/iteration.py
--rw-r--r--   0        0        0      839 2023-03-18 14:16:45.172134 betterletter-1.2.0/betterletter/resources/dicts/README.md
--rw-r--r--   0        0        0 34187973 2023-03-18 14:16:45.376146 betterletter-1.2.0/betterletter/resources/dicts/de.txt
--rw-r--r--   0        0        0      101 2023-03-18 14:16:45.376146 betterletter-1.2.0/betterletter/resources/languages.json
--rw-r--r--   0        0        0      469 2023-03-18 14:16:45.376146 betterletter-1.2.0/betterletter/strings.py
--rw-r--r--   0        0        0     9828 2023-03-18 14:16:45.376146 betterletter-1.2.0/betterletter/substituters.py
--rw-r--r--   0        0        0     1757 2023-03-18 14:16:45.380146 betterletter-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    10738 1970-01-01 00:00:00.000000 betterletter-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 20:13:05.522271 betterletter-1.2.1/LICENSE
+-rw-r--r--   0        0        0     9466 2023-04-21 20:13:05.522271 betterletter-1.2.1/README.md
+-rw-r--r--   0        0        0     3093 2023-04-21 20:13:05.522271 betterletter-1.2.1/betterletter/__init__.py
+-rw-r--r--   0        0        0     6435 2023-04-21 20:13:05.522271 betterletter-1.2.1/betterletter/__main__.py
+-rw-r--r--   0        0        0     1721 2023-04-21 20:13:05.522271 betterletter-1.2.1/betterletter/io.py
+-rw-r--r--   0        0        0     3111 2023-04-21 20:13:05.522271 betterletter-1.2.1/betterletter/iteration.py
+-rw-r--r--   0        0        0      839 2023-04-21 20:13:05.522271 betterletter-1.2.1/betterletter/resources/dicts/README.md
+-rw-r--r--   0        0        0 34187973 2023-04-21 20:13:05.690275 betterletter-1.2.1/betterletter/resources/dicts/de.txt
+-rw-r--r--   0        0        0      101 2023-04-21 20:13:05.694275 betterletter-1.2.1/betterletter/resources/languages.json
+-rw-r--r--   0        0        0      469 2023-04-21 20:13:05.694275 betterletter-1.2.1/betterletter/strings.py
+-rw-r--r--   0        0        0     9828 2023-04-21 20:13:05.694275 betterletter-1.2.1/betterletter/substituters.py
+-rw-r--r--   0        0        0     1757 2023-04-21 20:13:05.698275 betterletter-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10738 1970-01-01 00:00:00.000000 betterletter-1.2.1/PKG-INFO
```

### Comparing `betterletter-1.2.0/LICENSE` & `betterletter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/README.md` & `betterletter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/__init__.py` & `betterletter-1.2.1/betterletter/__init__.py`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/__main__.py` & `betterletter-1.2.1/betterletter/__main__.py`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/io.py` & `betterletter-1.2.1/betterletter/io.py`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/iteration.py` & `betterletter-1.2.1/betterletter/iteration.py`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/resources/dicts/README.md` & `betterletter-1.2.1/betterletter/resources/dicts/README.md`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/resources/dicts/de.txt` & `betterletter-1.2.1/betterletter/resources/dicts/de.txt`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/betterletter/substituters.py` & `betterletter-1.2.1/betterletter/substituters.py`

 * *Files identical despite different names*

### Comparing `betterletter-1.2.0/pyproject.toml` & `betterletter-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Alex Povel <python@alexpovel.de>"]
 description = "Substitute alternative spellings of native characters (e.g. German umlauts [ae, oe, ue] etc. [ss]) with their correct versions (ä, ö, ü, ß)."
 license = "MIT"
 name = "betterletter"
 readme = "README.md"
 repository = "https://github.com/alexpovel/betterletter/"
-version = "1.2.0"
+version = "1.2.1"
 keywords = ["spelling", "umlaut", "substitute", "letter", "alternative"]
 classifiers = [
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Natural Language :: German",
     "Operating System :: OS Independent",
     "Topic :: Communications",
@@ -32,15 +32,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.12,<24.0"
 mypy = ">=0.991,<1.2"
 pytest = "^7.2.0"
 snakeviz = "^2.1.1"
 pytest-cov = "^4.0.0"
-ruff = ">=0.0.224,<0.0.255"
+ruff = ">=0.0.224,<0.0.258"
 pre-commit = "^3.0.0"
 
 [tool.mypy]
 exclude = "tests/*"
 mypy_path = "stubs/"
 show_error_codes = true
 strict = true
```

### Comparing `betterletter-1.2.0/PKG-INFO` & `betterletter-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterletter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Substitute alternative spellings of native characters (e.g. German umlauts [ae, oe, ue] etc. [ss]) with their correct versions (ä, ö, ü, ß).
 Home-page: https://github.com/alexpovel/betterletter/
 License: MIT
 Keywords: spelling,umlaut,substitute,letter,alternative
 Author: Alex Povel
 Author-email: python@alexpovel.de
 Requires-Python: >=3.9,<4.0
```

