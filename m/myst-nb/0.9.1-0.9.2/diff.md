# Comparing `tmp/myst-nb-0.9.1.tar.gz` & `tmp/myst-nb-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/myst-nb-0.9.1.tar", last modified: Tue Aug 25 03:31:02 2020, max compression
+gzip compressed data, was "dist/myst-nb-0.9.2.tar", last modified: Wed Aug 26 23:40:46 2020, max compression
```

## Comparing `myst-nb-0.9.1.tar` & `myst-nb-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-25 03:31:02.000000 myst-nb-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1529 2020-08-25 03:31:00.000000 myst-nb-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-08-25 03:31:00.000000 myst-nb-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-08-25 03:31:02.000000 myst-nb-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1327 2020-08-25 03:31:00.000000 myst-nb-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb/
--rw-r--r--   0 runner    (1001) docker     (116)    11980 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     3703 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (116)     5233 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/ansi_lexer.py
--rw-r--r--   0 runner    (1001) docker     (116)     9359 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/converter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4411 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/exec_table.py
--rw-r--r--   0 runner    (1001) docker     (116)    12260 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb/nb_glue/
--rw-r--r--   0 runner    (1001) docker     (116)     1111 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/nb_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12155 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/nb_glue/domain.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/nb_glue/transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     4263 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/nb_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1784 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/nodes.py
--rw-r--r--   0 runner    (1001) docker     (116)    11421 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)    19786 2020-08-25 03:31:00.000000 myst-nb-0.9.1/myst_nb/render_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      554 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      132 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      545 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-25 03:31:02.000000 myst-nb-0.9.1/myst_nb.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-25 03:31:02.000000 myst-nb-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3170 2020-08-25 03:31:00.000000 myst-nb-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-26 23:40:46.000000 myst-nb-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1529 2020-08-26 23:40:40.000000 myst-nb-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2020-08-26 23:40:40.000000 myst-nb-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-08-26 23:40:46.000000 myst-nb-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1327 2020-08-26 23:40:40.000000 myst-nb-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb/
+-rw-r--r--   0 runner    (1001) docker     (116)    11980 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     3703 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (116)     5233 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/ansi_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9359 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4411 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/exec_table.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12260 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb/nb_glue/
+-rw-r--r--   0 runner    (1001) docker     (116)     1111 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/nb_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12155 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/nb_glue/domain.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1539 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/nb_glue/transform.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4263 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/nb_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1784 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11421 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19786 2020-08-26 23:40:40.000000 myst-nb-0.9.2/myst_nb/render_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      554 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      132 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      545 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-26 23:40:46.000000 myst-nb-0.9.2/myst_nb.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-26 23:40:46.000000 myst-nb-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3170 2020-08-26 23:40:40.000000 myst-nb-0.9.2/setup.py
```

### Comparing `myst-nb-0.9.1/LICENSE` & `myst-nb-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/PKG-INFO` & `myst-nb-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myst-nb
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Jupyter Notebook Sphinx reader built on top of the MyST markdown parser.
 Home-page: https://github.com/executablebooks/myst_nb
 Author: ExecutableBookProject
 Author-email: choldgraf@berkeley.edu
 License: BSD-3
 Description: # MyST-NB
```

### Comparing `myst-nb-0.9.1/README.md` & `myst-nb-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/__init__.py` & `myst-nb-0.9.2/myst_nb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 from collections.abc import Sequence
 import os
 from pathlib import Path
 
 from docutils import nodes
 from sphinx.application import Sphinx
```

### Comparing `myst-nb-0.9.1/myst_nb/_static/mystnb.css` & `myst-nb-0.9.2/myst_nb/_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/ansi_lexer.py` & `myst-nb-0.9.2/myst_nb/ansi_lexer.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/converter.py` & `myst-nb-0.9.2/myst_nb/converter.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/exec_table.py` & `myst-nb-0.9.2/myst_nb/exec_table.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/execution.py` & `myst-nb-0.9.2/myst_nb/execution.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/nb_glue/__init__.py` & `myst-nb-0.9.2/myst_nb/nb_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/nb_glue/domain.py` & `myst-nb-0.9.2/myst_nb/nb_glue/domain.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/nb_glue/transform.py` & `myst-nb-0.9.2/myst_nb/nb_glue/transform.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/nb_glue/utils.py` & `myst-nb-0.9.2/myst_nb/nb_glue/utils.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/nodes.py` & `myst-nb-0.9.2/myst_nb/nodes.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/parser.py` & `myst-nb-0.9.2/myst_nb/parser.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb/render_outputs.py` & `myst-nb-0.9.2/myst_nb/render_outputs.py`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb.egg-info/PKG-INFO` & `myst-nb-0.9.2/myst_nb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myst-nb
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Jupyter Notebook Sphinx reader built on top of the MyST markdown parser.
 Home-page: https://github.com/executablebooks/myst_nb
 Author: ExecutableBookProject
 Author-email: choldgraf@berkeley.edu
 License: BSD-3
 Description: # MyST-NB
```

### Comparing `myst-nb-0.9.1/myst_nb.egg-info/SOURCES.txt` & `myst-nb-0.9.2/myst_nb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myst-nb-0.9.1/myst_nb.egg-info/requires.txt` & `myst-nb-0.9.2/myst_nb.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-myst-parser~=0.12.1
+myst-parser~=0.12.4
 docutils>=0.15
 sphinx<4,>=2
 jupyter_sphinx~=0.2.4
 jupyter-cache~=0.4.0
 ipython
 nbformat~=5.0
 nbconvert~=5.6
```

### Comparing `myst-nb-0.9.1/setup.py` & `myst-nb-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         "Topic :: Text Processing :: Markup",
         "Framework :: Sphinx :: Extension",
     ],
     keywords="markdown lexer parser development docutils sphinx",
     python_requires=">=3.6",
     package_data={"myst_nb": ["_static/*"]},
     install_requires=[
-        "myst-parser~=0.12.1",
+        "myst-parser~=0.12.4",
         "docutils>=0.15",
         "sphinx>=2,<4",
         "jupyter_sphinx~=0.2.4",
         "jupyter-cache~=0.4.0",
         "ipython",
         "nbformat~=5.0",
         "nbconvert~=5.6",
```

