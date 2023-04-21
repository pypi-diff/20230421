# Comparing `tmp/chlorophyll-0.3.0.tar.gz` & `tmp/chlorophyll-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlorophyll-0.3.0.tar", last modified: Fri Apr  7 16:04:39 2023, max compression
+gzip compressed data, was "chlorophyll-0.3.1.tar", last modified: Fri Apr 21 14:00:48 2023, max compression
```

## Comparing `chlorophyll-0.3.0.tar` & `chlorophyll-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.523256 chlorophyll-0.3.0/chlorophyll/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/codeview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/chlorophyll/colorschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-dark.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-light.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/dracula.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/mariana.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/colorschemes/monokai.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/chlorophyll/schemeparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/chlorophyll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 16:04:39.000000 chlorophyll-0.3.0/chlorophyll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:04:39.527256 chlorophyll-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-07 16:04:30.000000 chlorophyll-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.670071 chlorophyll-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/codeview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll/colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-dark.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-light.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/dracula.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/mariana.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/monokai.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/schemeparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:00:48.670071 chlorophyll-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/setup.py
```

### Comparing `chlorophyll-0.3.0/LICENSE` & `chlorophyll-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/PKG-INFO` & `chlorophyll-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.3.0
+Version: 0.3.1
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -19,33 +19,44 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Chlorophyll</h1>
 
-A module that fills your code with color - syntax highlighted text box widget for Tkinter.
+> **Note**
+> This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it any more.
+
+## Description
+Chlorophyll provides the `CodeView` widget for tkinter, which is a `Text` widget with syntax highlighting, line numbers, and works as a simple code editor. It is written in Python and uses the [`pygments`](https://pygments.org/) library for syntax highlighting and the [`TkLineNums`](https://www.github.com/Moosems/TkLineNums) module for line numbers.
 
-This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
 
 ## Installation
 
 `pip install chlorophyll`
 
-## Basic usage
-Until there's no documentation
+# Documentation
+
+### `CodeView` Widget
+|Options      |Description                     |Input                                         |
+|-------------|--------------------------------|----------------------------------------------|
+|master       |The parent widget               |Tkinter widget                                |
+|lexer        |The Language lexer              |Pygments lexer                                |
+|color_scheme |A color scheme for the code     |Dict, string, or toml file                    |
+|tab_width    |The width of a tab (`\t`)       |Int                                           |
+|**kwargs      |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
 
+#### Basic Usage:
 ```python
-import tkinter
+from tkinter import Tk
 
 import pygments.lexers
 from chlorophyll import CodeView
 
-root = tkinter.Tk()
+root = Tk()
 
 codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
 codeview.pack(fill="both", expand=True)
 
 root.mainloop()
 ```
 
-
```

### Comparing `chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-dark.toml` & `chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-dark.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll/colorschemes/ayu-light.toml` & `chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-light.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll/colorschemes/dracula.toml` & `chlorophyll-0.3.1/chlorophyll/colorschemes/dracula.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll/colorschemes/mariana.toml` & `chlorophyll-0.3.1/chlorophyll/colorschemes/mariana.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll/colorschemes/monokai.toml` & `chlorophyll-0.3.1/chlorophyll/colorschemes/monokai.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll/schemeparser.py` & `chlorophyll-0.3.1/chlorophyll/schemeparser.py`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.0/chlorophyll.egg-info/PKG-INFO` & `chlorophyll-0.3.1/chlorophyll.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.3.0
+Version: 0.3.1
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -19,33 +19,44 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Chlorophyll</h1>
 
-A module that fills your code with color - syntax highlighted text box widget for Tkinter.
+> **Note**
+> This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it any more.
+
+## Description
+Chlorophyll provides the `CodeView` widget for tkinter, which is a `Text` widget with syntax highlighting, line numbers, and works as a simple code editor. It is written in Python and uses the [`pygments`](https://pygments.org/) library for syntax highlighting and the [`TkLineNums`](https://www.github.com/Moosems/TkLineNums) module for line numbers.
 
-This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it anymore.
 
 ## Installation
 
 `pip install chlorophyll`
 
-## Basic usage
-Until there's no documentation
+# Documentation
+
+### `CodeView` Widget
+|Options      |Description                     |Input                                         |
+|-------------|--------------------------------|----------------------------------------------|
+|master       |The parent widget               |Tkinter widget                                |
+|lexer        |The Language lexer              |Pygments lexer                                |
+|color_scheme |A color scheme for the code     |Dict, string, or toml file                    |
+|tab_width    |The width of a tab (`\t`)       |Int                                           |
+|**kwargs      |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
 
+#### Basic Usage:
 ```python
-import tkinter
+from tkinter import Tk
 
 import pygments.lexers
 from chlorophyll import CodeView
 
-root = tkinter.Tk()
+root = Tk()
 
 codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
 codeview.pack(fill="both", expand=True)
 
 root.mainloop()
 ```
 
-
```

### Comparing `chlorophyll-0.3.0/setup.py` & `chlorophyll-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="chlorophyll",
-    version="0.3.0",
+    version="0.3.1",
     description="A module that fills your code with color - syntax highlighted text box widget for Tkinter.",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://gitlab.com/rdbende/chlorophyll",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["pygments", "toml"],
+    install_requires=["pygments", "toml", "tklinenums", "pyperclip"],
     python_requires=">=3.7",
     license="MIT license",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

