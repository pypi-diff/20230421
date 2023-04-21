# Comparing `tmp/pybites_search-0.0.8.tar.gz` & `tmp/pybites_search-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pybites_search-0.0.9.tar", last modified: Wed Apr 19 08:44:10 2023, from Unix
```

## Comparing `pybites_search-0.0.8.tar` & `pybites_search-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pybites_search-0.0.8/.flake8
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pybites_search-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pybites_search-0.0.8/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/__main__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/article.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/base.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/bite.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/cli.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/podcast.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/tip.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pybites_search-0.0.8/src/pybites_search/youtube.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pybites_search-0.0.8/.gitignore
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pybites_search-0.0.8/LICENSE
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 pybites_search-0.0.8/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pybites_search-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 pybites_search-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/__main__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/article.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/base.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/bite.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/cli.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/podcast.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/tip.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/youtube.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pybites_search-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pybites_search-0.0.9/LICENSE
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 pybites_search-0.0.9/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pybites_search-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12133 2020-02-02 00:00:00.000000 pybites_search-0.0.9/PKG-INFO
```

### Comparing `pybites_search-0.0.8/src/pybites_search/article.py` & `pybites_search-0.0.9/src/pybites_search/article.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/base.py` & `pybites_search-0.0.9/src/pybites_search/base.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/bite.py` & `pybites_search-0.0.9/src/pybites_search/bite.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/cli.py` & `pybites_search-0.0.9/src/pybites_search/cli.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/podcast.py` & `pybites_search-0.0.9/src/pybites_search/podcast.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/tip.py` & `pybites_search-0.0.9/src/pybites_search/tip.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/src/pybites_search/youtube.py` & `pybites_search-0.0.9/src/pybites_search/youtube.py`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/.gitignore` & `pybites_search-0.0.9/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .nox/
+coverage
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
```

### Comparing `pybites_search-0.0.8/LICENSE` & `pybites_search-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.8/README.md` & `pybites_search-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,7 +85,8 @@
 | 0.0.2   | ditto                                       |
 | 0.0.3   | ditto                                       |
 | 0.0.4   | Add Pybites Youtube search                  |
 | 0.0.5   | Add platform Bite (exercise) search         |
 | 0.0.6   | Add Pybites Podcast search                  |
 | 0.0.7   | Add Pybites tips search                     |
 | 0.0.8   | Move podcast feed parsing to our platform   |
+| 0.0.9   | Add tox + testing to support 3.9 + 3.10     |
```

### Comparing `pybites_search-0.0.8/pyproject.toml` & `pybites_search-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pybites_search"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Pybites", email="info@pybit.es" },
 ]
 description = "A search engine for Pybites content"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "requests",
   "typer[all]",
 ]
 
 [project.optional-dependencies]
 test = [
+  "tox",
   "pytest",
   "pytest-cov",
+  "strip_ansi",
 ]
 lint = [
   "flake8",
   "black",
   "isort",
   "pyupgrade",
   "mypy",
@@ -36,7 +38,10 @@
 
 [project.urls]
 "Homepage" = "https://github.com/pybites/search"
 "Bug Tracker" = "https://github.com/pybites/search/issues"
 
 [project.scripts]
 search = "pybites_search.cli:app"
+
+[tool.hatch.build]
+only-packages = true
```

### Comparing `pybites_search-0.0.8/PKG-INFO` & `pybites_search-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pybites_search
-Version: 0.0.8
+Version: 0.0.9
 Summary: A search engine for Pybites content
 Project-URL: Homepage, https://github.com/pybites/search
 Project-URL: Bug Tracker, https://github.com/pybites/search/issues
 Author-email: Pybites <info@pybit.es>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: requests
 Requires-Dist: typer[all]
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Requires-Dist: flake8; extra == 'lint'
 Requires-Dist: isort; extra == 'lint'
 Requires-Dist: mypy; extra == 'lint'
 Requires-Dist: pyupgrade; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: strip-ansi; extra == 'test'
+Requires-Dist: tox; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Pybites Search
 
 A command line tool to easily search across Pybites content.
 
 ## Installation
@@ -110,7 +112,8 @@
 | 0.0.2   | ditto                                       |
 | 0.0.3   | ditto                                       |
 | 0.0.4   | Add Pybites Youtube search                  |
 | 0.0.5   | Add platform Bite (exercise) search         |
 | 0.0.6   | Add Pybites Podcast search                  |
 | 0.0.7   | Add Pybites tips search                     |
 | 0.0.8   | Move podcast feed parsing to our platform   |
+| 0.0.9   | Add tox + testing to support 3.9 + 3.10     |
```

