# Comparing `tmp/visual_novel_toolkit-1.8.3.tar.gz` & `tmp/visual_novel_toolkit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual_novel_toolkit-1.8.3.tar", max compression
+gzip compressed data, was "visual_novel_toolkit-1.9.0.tar", max compression
```

## Comparing `visual_novel_toolkit-1.8.3.tar` & `visual_novel_toolkit-1.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1279 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/LICENSE
--rw-r--r--   0        0        0     1542 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/docs/index.md
--rw-r--r--   0        0        0     1085 2023-01-15 01:29:14.930724 visual_novel_toolkit-1.8.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/__init__.py
--rw-r--r--   0        0        0      250 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/cli.py
--rw-r--r--   0        0        0        0 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/drafts/__init__.py
--rw-r--r--   0        0        0      322 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/drafts/cli.py
--rw-r--r--   0        0        0      237 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/drafts/missed.py
--rw-r--r--   0        0        0      421 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/drafts/new.py
--rw-r--r--   0        0        0        0 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/events/__init__.py
--rw-r--r--   0        0        0      166 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/events/cli.py
--rw-r--r--   0        0        0     1211 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/events/plot.py
--rw-r--r--   0        0        0       72 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/events/types.py
--rw-r--r--   0        0        0        0 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/__init__.py
--rw-r--r--   0        0        0      623 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/cli.py
--rw-r--r--   0        0        0      185 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/interfaces.py
--rw-r--r--   0        0        0     3152 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/proofread.py
--rw-r--r--   0        0        0      525 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/sort.py
--rw-r--r--   0        0        0      286 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/types.py
--rw-r--r--   0        0        0      964 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/unused.py
--rw-r--r--   0        0        0      141 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/words/__init__.py
--rw-r--r--   0        0        0      728 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/words/config_words.py
--rw-r--r--   0        0        0      602 2023-01-15 01:27:14.791257 visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/words/file_words.py
--rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 visual_novel_toolkit-1.8.3/setup.py
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 visual_novel_toolkit-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1279 2023-01-16 12:33:06.410113 visual_novel_toolkit-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1542 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/docs/index.md
+-rw-r--r--   0        0        0     1085 2023-01-16 12:34:58.638367 visual_novel_toolkit-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/__init__.py
+-rw-r--r--   0        0        0      250 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/cli.py
+-rw-r--r--   0        0        0        0 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/drafts/__init__.py
+-rw-r--r--   0        0        0      322 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/drafts/cli.py
+-rw-r--r--   0        0        0      237 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/drafts/missed.py
+-rw-r--r--   0        0        0      421 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/drafts/new.py
+-rw-r--r--   0        0        0        0 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/events/__init__.py
+-rw-r--r--   0        0        0      166 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/events/cli.py
+-rw-r--r--   0        0        0     2072 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/events/plot.py
+-rw-r--r--   0        0        0      467 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/events/types.py
+-rw-r--r--   0        0        0        0 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/__init__.py
+-rw-r--r--   0        0        0      623 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/cli.py
+-rw-r--r--   0        0        0      185 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/interfaces.py
+-rw-r--r--   0        0        0     3152 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/proofread.py
+-rw-r--r--   0        0        0      525 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/sort.py
+-rw-r--r--   0        0        0      286 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/types.py
+-rw-r--r--   0        0        0      964 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/unused.py
+-rw-r--r--   0        0        0      141 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/words/__init__.py
+-rw-r--r--   0        0        0      728 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/words/config_words.py
+-rw-r--r--   0        0        0      602 2023-01-16 12:33:06.414113 visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/words/file_words.py
+-rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 visual_novel_toolkit-1.9.0/setup.py
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 visual_novel_toolkit-1.9.0/PKG-INFO
```

### Comparing `visual_novel_toolkit-1.8.3/LICENSE` & `visual_novel_toolkit-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/docs/index.md` & `visual_novel_toolkit-1.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/pyproject.toml` & `visual_novel_toolkit-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "BSD-2-Clause"
 name = "visual-novel-toolkit"
 packages = [
   {from = "src", include = "visual_novel_toolkit"}
 ]
 readme = "docs/index.md"
 repository = "https://github.com/proofit404/visual-novel-toolkit"
-version = "1.8.3"
+version = "1.9.0"
 
 [tool.poetry.dependencies]
 beautifulsoup4 = "*"
 httpx = "*"
 python = "3.11.1"
 typer = "*"
```

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/cli.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/cli.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/proofread.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/proofread.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/sort.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/sort.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/unused.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/unused.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/words/config_words.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/words/config_words.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/src/visual_novel_toolkit/speller/words/file_words.py` & `visual_novel_toolkit-1.9.0/src/visual_novel_toolkit/speller/words/file_words.py`

 * *Files identical despite different names*

### Comparing `visual_novel_toolkit-1.8.3/setup.py` & `visual_novel_toolkit-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['beautifulsoup4', 'httpx', 'typer']
 
 entry_points = \
 {'console_scripts': ['vntk = visual_novel_toolkit.cli:cli']}
 
 setup_kwargs = {
     'name': 'visual-novel-toolkit',
-    'version': '1.8.3',
+    'version': '1.9.0',
     'description': 'A set of useful tools to improve DX of visual novel games.',
     'long_description': '# Visual novel toolkit [![build](https://img.shields.io/github/workflow/status/proofit404/visual-novel-toolkit/release?style=flat-square)](https://github.com/proofit404/visual-novel-toolkit/actions/workflows/release.yml?query=branch%3Arelease) [![pypi](https://img.shields.io/pypi/v/visual-novel-toolkit?style=flat-square)](https://pypi.org/project/visual-novel-toolkit)\n\nA set of useful tools to improve DX of visual novel games.\n\n**[Documentation](https://proofit404.github.io/visual-novel-toolkit) |\n[Source Code](https://github.com/proofit404/visual-novel-toolkit) |\n[Task Tracker](https://github.com/proofit404/visual-novel-toolkit/issues)**\n\n![](index.jpg)\n\n## Questions\n\nIf you have any questions, feel free to create an issue in our\n[Task Tracker](https://github.com/proofit404/visual-novel-toolkit/issues). We\nhave the\n[question label](https://github.com/proofit404/visual-novel-toolkit/issues?q=is%3Aopen+is%3Aissue+label%3Aquestion)\nexactly for this purpose.\n\n## Enterprise support\n\nIf you have an issue with any version of the library, you can apply for a paid\nenterprise support contract. This will guarantee you that no breaking changes\nwill happen to you. No matter how old version you\'re using at the moment. All\nnecessary features and bug fixes will be backported in a way that serves your\nneeds.\n\nPlease contact [proofit404@gmail.com](mailto:proofit404@gmail.com) if you\'re\ninterested in it.\n\n## License\n\n`visual-novel-toolkit` library is offered under the two clause BSD license.\n\n<p align="center">&mdash; ⭐ &mdash;</p>\n',
     'author': 'Josiah Kaviani',
     'author_email': 'proofit404@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/visual-novel-toolkit',
```

### Comparing `visual_novel_toolkit-1.8.3/PKG-INFO` & `visual_novel_toolkit-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-novel-toolkit
-Version: 1.8.3
+Version: 1.9.0
 Summary: A set of useful tools to improve DX of visual novel games.
 Home-page: https://pypi.org/project/visual-novel-toolkit
 License: BSD-2-Clause
 Author: Josiah Kaviani
 Author-email: proofit404@gmail.com
 Requires-Python: ==3.11.1
 Classifier: License :: OSI Approved :: BSD License
```

