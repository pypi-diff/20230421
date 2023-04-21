# Comparing `tmp/coso-1.0.2.tar.gz` & `tmp/coso-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.0.2.tar", last modified: Wed Apr 12 12:21:07 2023, max compression
+gzip compressed data, was "coso-1.0.3.tar", last modified: Wed Apr 19 14:00:04 2023, max compression
```

## Comparing `coso-1.0.2.tar` & `coso-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.188989 coso-1.0.2/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-12 12:21:07.188629 coso-1.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.173005 coso-1.0.2/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-12 12:21:07.189118 coso-1.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      989 2023-04-12 12:07:28.000000 coso-1.0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.187959 coso-1.0.2/src/
--rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.2/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.2/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.2/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.2/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15930 2023-04-12 10:50:48.000000 coso-1.0.2/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)     1739 2023-04-12 12:19:19.000000 coso-1.0.2/src/launcher.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.2/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.2/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8708 2023-04-12 10:37:47.000000 coso-1.0.2/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.2/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.2/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.2/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.2/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.2/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14266 2023-01-13 13:24:30.000000 coso-1.0.2/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.2/src/venn.py
--rwxrwxrwx   0 root         (0) root         (0)    20083 2023-02-03 09:38:17.000000 coso-1.0.2/src/viscoso.py
--rwxrwxrwx   0 root         (0) root         (0)     3477 2023-02-03 09:38:26.000000 coso-1.0.2/src/viscoso_widget.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.718850 coso-1.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-19 14:00:04.718500 coso-1.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.710328 coso-1.0.3/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      559 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-19 14:00:04.719054 coso-1.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1078 2023-04-19 13:58:42.000000 coso-1.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.716443 coso-1.0.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.717553 coso-1.0.3/src/VisCoSo/
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.3/src/VisCoSo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.0.3/src/VisCoSo/header.html
+-rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.0.3/src/VisCoSo/viscoso.css
+-rwxrwxrwx   0 root         (0) root         (0)   113187 2023-04-19 13:32:47.000000 coso-1.0.3/src/VisCoSo/viscoso.html
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.3/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.3/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.3/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.3/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15930 2023-04-12 10:50:48.000000 coso-1.0.3/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)     2003 2023-04-19 13:48:19.000000 coso-1.0.3/src/launcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.3/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.3/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8708 2023-04-12 10:37:47.000000 coso-1.0.3/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.3/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.3/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.3/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.3/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.3/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14336 2023-04-19 12:40:45.000000 coso-1.0.3/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.3/src/venn.py
+-rwxrwxrwx   0 root         (0) root         (0)    20228 2023-04-19 13:59:50.000000 coso-1.0.3/src/viscoso.py
+-rwxrwxrwx   0 root         (0) root         (0)     3394 2023-04-19 12:40:33.000000 coso-1.0.3/src/viscoso_widget.py
```

### Comparing `coso-1.0.2/LICENSE` & `coso-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/PKG-INFO` & `coso-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.2
+Version: 1.0.3
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.2/README.md` & `coso-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/coso.egg-info/PKG-INFO` & `coso-1.0.3/coso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.2
+Version: 1.0.3
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.2/src/__init__.py` & `coso-1.0.3/src/VisCoSo/__init__.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/cola_parser.py` & `coso-1.0.3/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/configuration.py` & `coso-1.0.3/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/count.py` & `coso-1.0.3/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/gen_plots.py` & `coso-1.0.3/src/gen_plots.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/launcher.py` & `coso-1.0.3/src/launcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import os
 import argparse
 import webbrowser
+import tempfile
+import shutil
 
 from .cola_parser import Parser
 from .problem import EmptyException
+from .util import *
 
-
-def run(file=None, cola=None, debug=False):
+def run_coso(file=None, cola=None, debug=False):
     """
 
     """
     parser = Parser(file, cola)
     try:
         parser.parse()
         sol = parser.problem.solve(debug=debug)
-        return sol
+        return str(sol)
     except EmptyException:
         print("Could not find a problem :(")
 
 
-def viscoso(file=None, cola=None, visual=None):
+def run_viscoso(
+    file=None, 
+    cola=None, 
+    visual=tempfile.NamedTemporaryFile(delete=False, suffix='.html').name):
     """
 
     Args:
         file (str, optional): a path to a file containing a CoLa program. Defaults to None.
         cola (str, optional): a CoLa program. Defaults to None.
-
+        visual (str, optional): a path where the html representation should be saved. Defaults to a temporary file
     Returns:
         str: the html string generated by VisCoSo
     """
     parser = Parser(file, cola)
     try:
         parser.parse()
         sol = parser.problem.solve(debug=False)
-        with open(visual, "w") as out:
+        with open(visual, "w+") as out:
             out.write(sol.log.to_viscoso())
             webbrowser.open(visual, new=2)
-        return sol
+        return str(sol)
     except EmptyException:
         print("Could not find a problem :(")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("filename", help="Run solver on CoLa file")
@@ -51,13 +56,13 @@
         help="Generate a visual representation of CoSo reasoning to an html file",
     )
     parser.add_argument("--debug", action="store_true", help="Print log")
     args = parser.parse_args()
     if args.filename:
         print("Running solver...")
         if args.v:
-            sol = viscoso(file=args.filename, visual=args.v)
+            sol = run_viscoso(file=args.filename, visual=args.v)
         else:
-            sol = coso(file=args.filename, debug=args.debug)
+            sol = run_coso(file=args.filename, debug=args.debug)
         print(f"Solution: {sol}")
     else:
         parser.print_help()
```

### Comparing `coso-1.0.2/src/level_1.py` & `coso-1.0.3/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/level_2.py` & `coso-1.0.3/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/logger.py` & `coso-1.0.3/src/logger.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/parsetab.py` & `coso-1.0.3/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/problem.py` & `coso-1.0.3/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/sharpCSP.py` & `coso-1.0.3/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/solver.py` & `coso-1.0.3/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/tester.py` & `coso-1.0.3/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/util.py` & `coso-1.0.3/src/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import portion as P
 import os
 import sys
 from portion.dict import IntervalDict
 from typing import Counter
 
 ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), ".."))
+CSS_VISCOSO = os.path.join(ROOT_DIR, "src", "VisCoSo", "viscoso.css")
 
 
 ######################
 ## Interval methods ##
 ######################
```

### Comparing `coso-1.0.2/src/venn.py` & `coso-1.0.3/src/venn.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.2/src/viscoso.py` & `coso-1.0.3/src/viscoso.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,19 +504,23 @@
         return cola_sets
 
     def generate(self, log):
         h = open(HEADER, "r")
         h_content = h.read()
         h_content = html.unescape(h_content)
 
+        css = open(CSS_VISCOSO, "r")
+        css_content = css.read()
         self.reserve_colours(log)
 
         self.doc.asis("<!DOCTYPE html>")
         with self.tag("html"):
             self.doc.asis(h_content)
+            with self.tag("style"):
+                self.text(css_content)
             with self.tag("body"):
                 self.add_problem(log)
 
         return indent(self.doc.getvalue())
 
     def generate_widget(self, log):
         self.reserve_colours(log)
```

### Comparing `coso-1.0.2/src/viscoso_widget.py` & `coso-1.0.3/src/viscoso_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,13 +103,12 @@
             }
 
             export function render(view) {
                 let widget = () => view.model.get("value");
                 appendHtml(view.el, widget());
             }
             """
-            css_path = os.path.join(ROOT_DIR, "src", "VisCoSo", "css", "viscoso.css")
-            _css = open(css_path, "r").read()
+            _css = open(CSS_VISCOSO, "r").read()
             value = traitlets.Unicode(html).tag(sync=True)
 
         vscw = VisCoSoWidget()
         display(vscw, display_id="viscoso")
```

