# Comparing `tmp/sphinx_inline_tabs-2021.8.17b10.tar.gz` & `tmp/sphinx_inline_tabs-2022.1.2b11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_inline_tabs-2021.8.17b10.tar", last modified: Tue Aug 17 08:23:12 2021, max compression
+gzip compressed data, was "sphinx_inline_tabs-2022.1.2b11.tar", last modified: Sun Jan  2 17:35:41 2022, max compression
```

## Comparing `sphinx_inline_tabs-2021.8.17b10.tar` & `sphinx_inline_tabs-2022.1.2b11.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       56 2021-08-17 08:19:55.068040 sphinx_inline_tabs-2021.8.17b10/.flake8
--rw-r--r--   0        0        0       45 2021-08-17 08:19:55.068118 sphinx_inline_tabs-2021.8.17b10/.gitignore
--rw-r--r--   0        0        0       25 2021-08-17 08:19:55.068195 sphinx_inline_tabs-2021.8.17b10/.isort.cfg
--rw-r--r--   0        0        0     1077 2021-08-17 08:19:55.068288 sphinx_inline_tabs-2021.8.17b10/.pre-commit-config.yaml
--rw-r--r--   0        0        0      188 2021-08-17 08:19:55.068378 sphinx_inline_tabs-2021.8.17b10/.readthedocs.yml
--rw-r--r--   0        0        0     5212 2021-08-17 08:19:55.068487 sphinx_inline_tabs-2021.8.17b10/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1078 2021-08-17 08:19:55.068585 sphinx_inline_tabs-2021.8.17b10/LICENSE
--rw-r--r--   0        0        0     1378 2021-08-17 08:19:55.068682 sphinx_inline_tabs-2021.8.17b10/README.md
--rw-r--r--   0        0        0    32650 2021-08-17 08:19:55.069045 sphinx_inline_tabs-2021.8.17b10/docs/_static/demo.png
--rw-r--r--   0        0        0     1618 2021-08-17 08:19:55.069147 sphinx_inline_tabs-2021.8.17b10/docs/conf.py
--rw-r--r--   0        0        0      948 2021-08-17 08:19:55.069230 sphinx_inline_tabs-2021.8.17b10/docs/index.md
--rw-r--r--   0        0        0     3372 2021-08-17 08:19:55.069327 sphinx_inline_tabs-2021.8.17b10/docs/usage.md
--rw-r--r--   0        0        0     4629 2021-08-17 08:19:55.069429 sphinx_inline_tabs-2021.8.17b10/noxfile.py
--rw-r--r--   0        0        0      466 2021-08-17 08:19:55.069514 sphinx_inline_tabs-2021.8.17b10/pyproject.toml
--rw-r--r--   0        0        0      993 2021-08-17 08:23:12.379920 sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/__init__.py
--rw-r--r--   0        0        0     6193 2021-08-17 08:19:55.069837 sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/_impl.py
--rw-r--r--   0        0        0     2148 2021-08-17 08:20:17.405353 sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/static/tabs.css
--rw-r--r--   0        0        0      585 2021-08-17 08:19:55.070054 sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/static/tabs.js
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 sphinx_inline_tabs-2021.8.17b10/setup.py
--rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 sphinx_inline_tabs-2021.8.17b10/PKG-INFO
+-rw-r--r--   0        0        0       56 2021-08-17 08:19:55.068040 sphinx_inline_tabs-2022.1.2b11/.flake8
+-rw-r--r--   0        0        0       45 2021-08-17 08:19:55.068118 sphinx_inline_tabs-2022.1.2b11/.gitignore
+-rw-r--r--   0        0        0       25 2021-08-17 08:19:55.068195 sphinx_inline_tabs-2022.1.2b11/.isort.cfg
+-rw-r--r--   0        0        0     1077 2021-08-17 08:19:55.068288 sphinx_inline_tabs-2022.1.2b11/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      188 2021-08-17 08:19:55.068378 sphinx_inline_tabs-2022.1.2b11/.readthedocs.yml
+-rw-r--r--   0        0        0     5212 2021-08-17 08:19:55.068487 sphinx_inline_tabs-2022.1.2b11/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1078 2021-08-17 08:19:55.068585 sphinx_inline_tabs-2022.1.2b11/LICENSE
+-rw-r--r--   0        0        0     1217 2021-12-22 12:34:33.341438 sphinx_inline_tabs-2022.1.2b11/README.md
+-rw-r--r--   0        0        0    32650 2021-08-17 08:19:55.069045 sphinx_inline_tabs-2022.1.2b11/docs/_static/demo.png
+-rw-r--r--   0        0        0     1618 2021-08-17 08:19:55.069147 sphinx_inline_tabs-2022.1.2b11/docs/conf.py
+-rw-r--r--   0        0        0      948 2021-08-17 08:19:55.069230 sphinx_inline_tabs-2022.1.2b11/docs/index.md
+-rw-r--r--   0        0        0     3715 2021-12-22 12:44:38.571771 sphinx_inline_tabs-2022.1.2b11/docs/usage.md
+-rw-r--r--   0        0        0     4629 2021-08-17 08:19:55.069429 sphinx_inline_tabs-2022.1.2b11/noxfile.py
+-rw-r--r--   0        0        0      466 2021-08-17 08:19:55.069514 sphinx_inline_tabs-2022.1.2b11/pyproject.toml
+-rw-r--r--   0        0        0      993 2022-01-02 17:35:41.086430 sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/__init__.py
+-rw-r--r--   0        0        0     6193 2021-08-17 08:19:55.069837 sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/_impl.py
+-rw-r--r--   0        0        0     2589 2021-12-22 12:43:11.167793 sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/static/tabs.css
+-rw-r--r--   0        0        0      551 2021-12-22 12:20:46.499434 sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/static/tabs.js
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 sphinx_inline_tabs-2022.1.2b11/PKG-INFO
```

### Comparing `sphinx_inline_tabs-2021.8.17b10/.pre-commit-config.yaml` & `sphinx_inline_tabs-2022.1.2b11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/CODE_OF_CONDUCT.md` & `sphinx_inline_tabs-2022.1.2b11/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/LICENSE` & `sphinx_inline_tabs-2022.1.2b11/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/README.md` & `sphinx_inline_tabs-2022.1.2b11/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 - **Synchronisation**: Tabs with the same label all switch with a single click.
 - **Works without JavaScript**: JavaScript is not required for the basics, only for synchronisation.
 
 <!-- end-include-here -->
 
 ## Contributing
 
-sphinx-inline-tabs is a volunteer maintained open source project, and we welcome contributions of all forms. This is a fairly small package, and the development workflow is very similar to [Furo's development workflow](https://pradyunsg.me/furo/contributing/workflow/).
+sphinx-inline-tabs is a volunteer maintained open source project, and we welcome contributions of all forms.
 
 The [Code of Conduct](CODE_OF_CONDUCT.md) applies within all community spaces. If you are not familiar with our Code of Conduct policy, take a minute to read the policy before starting with your first contribution.
```

### Comparing `sphinx_inline_tabs-2021.8.17b10/docs/_static/demo.png` & `sphinx_inline_tabs-2022.1.2b11/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/docs/conf.py` & `sphinx_inline_tabs-2022.1.2b11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/docs/index.md` & `sphinx_inline_tabs-2022.1.2b11/docs/index.md`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/docs/usage.md` & `sphinx_inline_tabs-2022.1.2b11/docs/usage.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 Two is the even prime.
 ```
 
 ```{tab} Three
 Three is an odd prime.
 ```
 
-```{tab} Four (equal to $2^2$)
+```{tab} Four
 Four is not a perfect number.
 ```
 
 This is text after the tabs, which seems to flow right through. There is no visual difference for content that's within a tab vs outside it -- adding tabs doesn't disrupt the flow of the document.
 
 ## Multiple Tab Sets
 
@@ -104,14 +104,36 @@
    Five is a nice number.
 
 .. tab:: Six
 
    Six is also nice.
 ```
 
+## Rich tab labels
+
+This is only possible with Markdown, as far as I know.
+
+````
+```{tab} Three
+Three is an odd prime.
+```
+
+```{tab} Four (equal to $2^2$)
+Four is not a perfect number.
+```
+````
+
+```{tab} Three
+Three is an odd prime.
+```
+
+```{tab} Four (equal to $2^2$)
+Four is not a perfect number.
+```
+
 ## Code Tabs
 
 The first code block in a tab content will "join" with the tabs, making things fairly clean for language snippets and OS-based command suggestions.
 
 ````{tab} Python
 ```python
 print("Hello World!")
@@ -128,14 +150,22 @@
   std::cout << "Hello World!" << std::endl;
 }
 ```
 
 More code, but it works too!
 ````
 
+````{tab} Text
+```none
+Hello World!
+```
+
+Why not.
+````
+
 ## Synchronisation
 
 Tabs across multiple sets are synchronised according to the label, unconditionally. This requires JavaScript to be enabled on the end user's browser and, thus, should be considered a progressive enhancement.
 
 ```{hint}
 Nearly all usage of tabbed content in documentation is based on something about the user which stays consistent throughout the reading (like their OS, or preferred language etc). That's why this behaviour is unconditional.
 ```
```

### Comparing `sphinx_inline_tabs-2021.8.17b10/noxfile.py` & `sphinx_inline_tabs-2022.1.2b11/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/__init__.py` & `sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Add inline tabbed content to your Sphinx documentation."""
 
 import os
 
-__version__ = "2021.08.17.beta10"
+__version__ = "2022.01.02.beta11"
 __all__ = ["setup"]
 
 
 def setup(app):
     """Entry point for sphinx theming."""
     app.require_sphinx("3.0")
```

### Comparing `sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/_impl.py` & `sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/_impl.py`

 * *Files identical despite different names*

### Comparing `sphinx_inline_tabs-2021.8.17b10/src/sphinx_inline_tabs/static/tabs.js` & `sphinx_inline_tabs-2022.1.2b11/src/sphinx_inline_tabs/static/tabs.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -11,12 +11,11 @@
         labels_by_text[text].push(label);
     }
 }
 
 function onLabelClick() {
     // Activate other labels with the same text.
     for (label of labels_by_text[this.textContent]) {
-        if (label === this) continue;
         label.previousSibling.checked = true;
     }
 }
 document.addEventListener("DOMContentLoaded", ready, false);
```

### Comparing `sphinx_inline_tabs-2021.8.17b10/PKG-INFO` & `sphinx_inline_tabs-2022.1.2b11/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_inline_tabs
-Version: 2021.8.17b10
+Version: 2022.1.2b11
 Summary: Add inline tabbed content to your Sphinx documentation.
 Home-page: https://github.com/pradyunsg/sphinx-inline-tabs
 Author: Pradyun Gedam
 Author-email: mail@pradyunsg.me
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx >= 3
@@ -49,11 +49,11 @@
 - **Synchronisation**: Tabs with the same label all switch with a single click.
 - **Works without JavaScript**: JavaScript is not required for the basics, only for synchronisation.
 
 <!-- end-include-here -->
 
 ## Contributing
 
-sphinx-inline-tabs is a volunteer maintained open source project, and we welcome contributions of all forms. This is a fairly small package, and the development workflow is very similar to [Furo's development workflow](https://pradyunsg.me/furo/contributing/workflow/).
+sphinx-inline-tabs is a volunteer maintained open source project, and we welcome contributions of all forms.
 
 The [Code of Conduct](CODE_OF_CONDUCT.md) applies within all community spaces. If you are not familiar with our Code of Conduct policy, take a minute to read the policy before starting with your first contribution.
```

