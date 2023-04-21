# Comparing `tmp/wikitext_asymptote-0.0.3.tar.gz` & `tmp/wikitext_asymptote-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikitext_asymptote-0.0.3.tar", last modified: Mon Mar 27 14:24:11 2023, max compression
+gzip compressed data, was "wikitext_asymptote-0.0.4.tar", last modified: Fri Apr 21 12:37:43 2023, max compression
```

## Comparing `wikitext_asymptote-0.0.3.tar` & `wikitext_asymptote-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-03-27 14:24:11.495675 wikitext_asymptote-0.0.3/
--rw-r--r--   0 hera       (501) staff       (20)     1067 2023-03-27 08:06:51.000000 wikitext_asymptote-0.0.3/LICENSE
--rw-r--r--   0 hera       (501) staff       (20)     2635 2023-03-27 14:24:11.495548 wikitext_asymptote-0.0.3/PKG-INFO
--rw-r--r--   0 hera       (501) staff       (20)     1976 2023-03-27 09:48:29.000000 wikitext_asymptote-0.0.3/README.md
--rw-r--r--   0 hera       (501) staff       (20)      792 2023-03-27 11:42:16.000000 wikitext_asymptote-0.0.3/pyproject.toml
--rw-r--r--   0 hera       (501) staff       (20)       38 2023-03-27 14:24:11.495717 wikitext_asymptote-0.0.3/setup.cfg
-drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-03-27 14:24:11.494088 wikitext_asymptote-0.0.3/src/
-drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-03-27 14:24:11.494749 wikitext_asymptote-0.0.3/src/wikitext_asymptote/
--rw-r--r--   0 hera       (501) staff       (20)       56 2023-03-27 11:42:06.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote/__init__.py
--rw-r--r--   0 hera       (501) staff       (20)    27956 2023-03-27 08:13:49.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote/parse.py
-drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-03-27 14:24:11.495388 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/
--rw-r--r--   0 hera       (501) staff       (20)     2635 2023-03-27 14:24:11.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/PKG-INFO
--rw-r--r--   0 hera       (501) staff       (20)      328 2023-03-27 14:24:11.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/SOURCES.txt
--rw-r--r--   0 hera       (501) staff       (20)        1 2023-03-27 14:24:11.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/dependency_links.txt
--rw-r--r--   0 hera       (501) staff       (20)       17 2023-03-27 14:24:11.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/requires.txt
--rw-r--r--   0 hera       (501) staff       (20)       19 2023-03-27 14:24:11.000000 wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/top_level.txt
+drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-04-21 12:37:43.158720 wikitext_asymptote-0.0.4/
+-rw-r--r--   0 hera       (501) staff       (20)     1067 2023-03-27 08:06:51.000000 wikitext_asymptote-0.0.4/LICENSE
+-rw-r--r--   0 hera       (501) staff       (20)     2635 2023-04-21 12:37:43.158605 wikitext_asymptote-0.0.4/PKG-INFO
+-rw-r--r--   0 hera       (501) staff       (20)     1976 2023-03-27 09:48:29.000000 wikitext_asymptote-0.0.4/README.md
+-rw-r--r--   0 hera       (501) staff       (20)      792 2023-04-21 12:34:53.000000 wikitext_asymptote-0.0.4/pyproject.toml
+-rw-r--r--   0 hera       (501) staff       (20)       38 2023-04-21 12:37:43.158758 wikitext_asymptote-0.0.4/setup.cfg
+drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-04-21 12:37:43.156847 wikitext_asymptote-0.0.4/src/
+drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-04-21 12:37:43.157863 wikitext_asymptote-0.0.4/src/wikitext_asymptote/
+-rw-r--r--   0 hera       (501) staff       (20)       56 2023-03-27 11:42:06.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote/__init__.py
+-rw-r--r--   0 hera       (501) staff       (20)    29150 2023-04-21 11:22:45.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote/parse.py
+drwxr-xr-x   0 hera       (501) staff       (20)        0 2023-04-21 12:37:43.158460 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/
+-rw-r--r--   0 hera       (501) staff       (20)     2635 2023-04-21 12:37:43.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/PKG-INFO
+-rw-r--r--   0 hera       (501) staff       (20)      328 2023-04-21 12:37:43.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/SOURCES.txt
+-rw-r--r--   0 hera       (501) staff       (20)        1 2023-04-21 12:37:43.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/dependency_links.txt
+-rw-r--r--   0 hera       (501) staff       (20)       17 2023-04-21 12:37:43.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/requires.txt
+-rw-r--r--   0 hera       (501) staff       (20)       19 2023-04-21 12:37:43.000000 wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/top_level.txt
```

### Comparing `wikitext_asymptote-0.0.3/LICENSE` & `wikitext_asymptote-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wikitext_asymptote-0.0.3/PKG-INFO` & `wikitext_asymptote-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitext_asymptote
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom wikitext parser to produce html, plain text fields and relevant links from wikipedia page source code.
 Author-email: Aitor Pérez <aitor.perez@epfl.ch>, Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/wikitext-asymptote
 Project-URL: Bug Tracker, https://github.com/epflgraph/wikitext-asymptote/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wikitext_asymptote-0.0.3/README.md` & `wikitext_asymptote-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wikitext_asymptote-0.0.3/pyproject.toml` & `wikitext_asymptote-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wikitext_asymptote"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Aitor Pérez", email="aitor.perez@epfl.ch" },
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Custom wikitext parser to produce html, plain text fields and relevant links from wikipedia page source code."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `wikitext_asymptote-0.0.3/src/wikitext_asymptote/parse.py` & `wikitext_asymptote-0.0.4/src/wikitext_asymptote/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,43 @@
     text = re.sub(' +', ' ', text)
 
     # Normalize unicode characters
     text = unicodedata.normalize('NFKC', text)
 
     return text
 
+
+def preprocess_text(text):
+    # PROBLEM:
+    #   Headings like ===''The Times They Are A-Changin''' sessions, part 1=== are not correctly parsed
+    # WORKAROUND:
+    #   1. Check if there are headings with an odd number of single quotes (').
+    #   2. If so, replace all occurrences of ''[...]in''' with HTML tags <i>[...]in'</i>.
+    #      For instance, ''The Times They Are A-Changin''' becomes <i>The Times They Are A-Changin'</i>.
+
+    # Check for lines that start and end with the same number of = characters and contain at least one single quote (')
+    matches = re.findall(r"^(=+)(.*'.*)\1$", text, re.MULTILINE)
+
+    # For all matches, check if they contain an odd number of single quotes (')
+    ok = True
+    for _, match in matches:
+        if match.count("'") % 2 != 0:
+            ok = False
+            break
+
+    # If all headings are ok (contain an even number of single quotes (')), return the text unchanged
+    if ok:
+        return text
+
+    # Replace all occurrences of ''[...]in''' with HTML tags <i>[...]in'</i>
+    text = re.sub(r"''(.*in')''", r"<i>\1</i>", text)
+
+    return text
+
+
 ############################################################
 
 
 def parse_template(node):
     """
     Parse template node.
 
@@ -760,14 +789,17 @@
     title = title.split('#')[0]
 
     # Return title with capital first letter and replacing spaces with underscores
     return title.capitalize().replace(' ', '_')
 
 
 def parse_page(page_content):
+    # Preprocess page content
+    page_content = preprocess_text(page_content)
+
     # Produce wikicode object from page content
     wikicode = mwparserfromhell.parse(page_content)
 
     # Split into sections
     sections = wikicode.get_sections(levels=[2], include_lead=True, matches=section_is_wanted)
 
     # Initialise object to return
```

### Comparing `wikitext_asymptote-0.0.3/src/wikitext_asymptote.egg-info/PKG-INFO` & `wikitext_asymptote-0.0.4/src/wikitext_asymptote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitext-asymptote
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom wikitext parser to produce html, plain text fields and relevant links from wikipedia page source code.
 Author-email: Aitor Pérez <aitor.perez@epfl.ch>, Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/wikitext-asymptote
 Project-URL: Bug Tracker, https://github.com/epflgraph/wikitext-asymptote/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

